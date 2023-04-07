# Comparing `tmp/tdbug-1.0.0.tar.gz` & `tmp/tdbug-1.0.1.tar.gz`

## Comparing `tdbug-1.0.0.tar` & `tdbug-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tdbug-1.0.0/MANIFEST.in
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tdbug-1.0.0/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.0/src/tdbug/__init__.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tdbug-1.0.0/src/tdbug/tdbug.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tdbug-1.0.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tdbug-1.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.0/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tdbug-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 tdbug-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tdbug-1.0.1/MANIFEST.in
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tdbug-1.0.1/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.1/src/tdbug/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tdbug-1.0.1/src/tdbug/tdbug.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tdbug-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tdbug-1.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.1/README.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tdbug-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 tdbug-1.0.1/PKG-INFO
```

### Comparing `tdbug-1.0.0/setup.cfg` & `tdbug-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tdbug
-version = 1.0.0
+version = 1.0.1
 author = Damon Pickett
 author_email = damon.pickett@gmail.com
 description = tdbug is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/damonpickett/tdbug
 classifiers =
```

### Comparing `tdbug-1.0.0/src/tdbug/tdbug.py` & `tdbug-1.0.1/src/tdbug/tdbug.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 import sys
 import openai
 from dotenv import load_dotenv
 import os
 from rich.console import Console
 
-load_dotenv()
+def main():
 
-# Check if OPENAI_API_KEY is set in the environment
-if not os.getenv("OPENAI_API_KEY"):
-
-    # Prompt user for OPENAI_API_KEY value
-    openai_api_key = input("Please enter your OpenAI API key: ")
-
-    # Write value to .env file
-    with open(".env", "w") as f:
-        f.write(f"OPENAI_API_KEY={openai_api_key}")
-    
     load_dotenv()
 
-openai.api_key = os.getenv("OPENAI_API_KEY")
+    # Check if OPENAI_API_KEY is set in the environment
+    if not os.getenv("OPENAI_API_KEY"):
 
-error_message = input("Please paste your error code here: ")
+        # Prompt user for OPENAI_API_KEY value
+        openai_api_key = input("Please enter your OpenAI API key: ")
 
-console = Console()
+        # Write value to .env file
+        with open(".env", "w") as f:
+            f.write(f"OPENAI_API_KEY={openai_api_key}")
+        
+        load_dotenv()
+
+    openai.api_key = os.getenv("OPENAI_API_KEY")
+
+    error_message = input("Please paste your error code here: ")
+
+    console = Console()
+
+    if sys.version_info < (3, 7):
+        console.print("[bold red]Error:[/bold red] DBUG requires Python 3.7 or higher to run.")
+        console.print("Please update to a newer version of Python.\n")
+        console.print("[bold]Suggestions:[/bold]")
+        console.print("- Install the latest version of Python 3 from the official Python website (https://www.python.org/downloads/).")
+        console.print("- Use a Python version manager like pyenv to easily switch between multiple versions of Python.\n")
+        sys.exit(1)
+
+    def get_error_explanation(error_message):
+        prompt = (f'''Generate an explanation and solution for the following error message: `{error_message}`. Preface the explanation with "Explanation: " and the solution with "Solution: " and put Explanation and Solution on separate lines.''')
+        response = openai.Completion.create(
+            engine="text-davinci-003",
+            prompt=prompt,
+            max_tokens=1024,
+            n=1,
+            stop=None,
+            temperature=0.7,
+        )
+        response_text = response.choices[0].text.strip()
+        print(response_text)
 
-if sys.version_info < (3, 7):
-    console.print("[bold red]Error:[/bold red] DBUG requires Python 3.7 or higher to run.")
-    console.print("Please update to a newer version of Python.\n")
-    console.print("[bold]Suggestions:[/bold]")
-    console.print("- Install the latest version of Python 3 from the official Python website (https://www.python.org/downloads/).")
-    console.print("- Use a Python version manager like pyenv to easily switch between multiple versions of Python.\n")
-    sys.exit(1)
-
-def get_error_explanation(error_message):
-    prompt = (f'''Generate an explanation and solution for the following error message: `{error_message}`. Preface the explanation with "Explanation: " and the solution with "Solution: " and put Explanation and Solution on separate lines.''')
-    response = openai.Completion.create(
-        engine="text-davinci-003",
-        prompt=prompt,
-        max_tokens=1024,
-        n=1,
-        stop=None,
-        temperature=0.7,
-    )
-    response_text = response.choices[0].text.strip()
-    print(response_text)
+    get_error_explanation(error_message)
 
-get_error_explanation(error_message)
+if __name__ == '__main__':
+    main()
```

### Comparing `tdbug-1.0.0/LICENSE` & `tdbug-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tdbug-1.0.0/pyproject.toml` & `tdbug-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tdbug"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Damon Pickett", email="damon.pickett@gmail.com" },
 ]
 description = "tdbug is a command-line application that uses the OpenAI API to diagnose bugs when programming."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tdbug-1.0.0/PKG-INFO` & `tdbug-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdbug
-Version: 1.0.0
+Version: 1.0.1
 Summary: tdbug is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 Project-URL: Homepage, https://github.com/damonpickett/tdbug
 Project-URL: Bug Tracker, https://github.com/damonpickett/tdbug/issues
 Author-email: Damon Pickett <damon.pickett@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

