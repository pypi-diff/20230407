# Comparing `tmp/shell_gpt-0.8.3.tar.gz` & `tmp/shell_gpt-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_gpt-0.8.3.tar", last modified: Mon Apr  3 00:29:08 2023, max compression
+gzip compressed data, was "shell_gpt-0.8.4.tar", last modified: Fri Apr  7 18:29:43 2023, max compression
```

## Comparing `shell_gpt-0.8.3.tar` & `shell_gpt-0.8.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-03 00:29:08.389258 shell_gpt-0.8.3/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.3/LICENSE
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-03 00:29:08.389057 shell_gpt-0.8.3/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14406 2023-04-03 00:21:48.000000 shell_gpt-0.8.3/README.md
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-03 00:29:08.389303 shell_gpt-0.8.3/setup.cfg
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      749 2023-04-02 22:33:48.000000 shell_gpt-0.8.3/setup.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-03 00:29:08.387153 shell_gpt-0.8.3/sgpt/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      445 2023-04-02 16:58:52.000000 shell_gpt-0.8.3/sgpt/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.3/sgpt/__main__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4155 2023-04-03 00:10:37.000000 shell_gpt-0.8.3/sgpt/app.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.3/sgpt/cache.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3134 2023-04-02 15:59:57.000000 shell_gpt-0.8.3/sgpt/client.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2380 2023-04-02 21:00:35.000000 shell_gpt-0.8.3/sgpt/config.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-03 00:29:08.388016 shell_gpt-0.8.3/sgpt/handlers/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.3/sgpt/handlers/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-02 22:43:56.000000 shell_gpt-0.8.3/sgpt/handlers/chat_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.3/sgpt/handlers/default_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1121 2023-04-02 16:39:22.000000 shell_gpt-0.8.3/sgpt/handlers/handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1835 2023-04-02 22:39:24.000000 shell_gpt-0.8.3/sgpt/handlers/repl_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1960 2023-04-02 15:59:57.000000 shell_gpt-0.8.3/sgpt/make_prompt.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1124 2023-04-02 15:59:57.000000 shell_gpt-0.8.3/sgpt/utils.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-03 00:29:08.388862 shell_gpt-0.8.3/shell_gpt.egg-info/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-03 00:29:08.000000 shell_gpt-0.8.3/shell_gpt.egg-info/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-03 00:29:08.000000 shell_gpt-0.8.3/shell_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-03 00:29:08.000000 shell_gpt-0.8.3/shell_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-03 00:29:08.000000 shell_gpt-0.8.3/shell_gpt.egg-info/entry_points.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       57 2023-04-03 00:29:08.000000 shell_gpt-0.8.3/shell_gpt.egg-info/requires.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-03 00:29:08.000000 shell_gpt-0.8.3/shell_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 18:29:43.974816 shell_gpt-0.8.4/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.4/LICENSE
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-07 18:29:43.974589 shell_gpt-0.8.4/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14406 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/README.md
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-07 18:29:43.974855 shell_gpt-0.8.4/setup.cfg
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/setup.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 18:29:43.972838 shell_gpt-0.8.4/sgpt/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      445 2023-04-04 16:16:05.000000 shell_gpt-0.8.4/sgpt/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.4/sgpt/__main__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4130 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/sgpt/app.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.4/sgpt/cache.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3134 2023-04-02 15:59:57.000000 shell_gpt-0.8.4/sgpt/client.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2380 2023-04-04 16:16:05.000000 shell_gpt-0.8.4/sgpt/config.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 18:29:43.973666 shell_gpt-0.8.4/sgpt/handlers/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.4/sgpt/handlers/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.4/sgpt/handlers/chat_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.4/sgpt/handlers/default_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1121 2023-04-06 23:34:58.000000 shell_gpt-0.8.4/sgpt/handlers/handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/sgpt/handlers/repl_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/sgpt/make_prompt.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2276 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/sgpt/utils.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 18:29:43.974394 shell_gpt-0.8.4/shell_gpt.egg-info/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/requires.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/top_level.txt
```

### Comparing `shell_gpt-0.8.3/LICENSE` & `shell_gpt-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.3/PKG-INFO` & `shell_gpt-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell_gpt
-Version: 0.8.3
+Version: 0.8.4
 Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
 Home-page: https://github.com/ther1d/shell_gpt
 Author: Farkhod Sadykov
 Author-email: farkhod@sadykov.dev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.3
+pip install shell-gpt==0.8.4
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
```

### Comparing `shell_gpt-0.8.3/README.md` & `shell_gpt-0.8.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.3
+pip install shell-gpt==0.8.4
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
```

### Comparing `shell_gpt-0.8.3/setup.py` & `shell_gpt-0.8.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from setuptools import setup, find_packages
 
 # pylint: disable=consider-using-with
 setup(
     name="shell_gpt",
-    version="0.8.3",
+    version="0.8.4",
     packages=find_packages(),
     install_requires=[
         "typer~=0.7.0",
         "requests~=2.28.2",
         "rich==13.3.1",
         "distro~=1.8.0",
     ],
+    extras_require={
+        ':sys_platform == "win32"': ["pyreadline3"]
+    },
     entry_points={
         "console_scripts": ["sgpt = sgpt:cli"],
     },
     author="Farkhod Sadykov",
     author_email="farkhod@sadykov.dev",
     description=(
         "A command-line productivity tool powered by ChatGPT, "
```

### Comparing `shell_gpt-0.8.3/sgpt/app.py` & `shell_gpt-0.8.4/sgpt/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,23 @@
 and length and other options of the output. Additionally, it supports executing
 shell commands directly from the interface.
 
 API Key is stored locally for easy use in future runs.
 """
 
 
-import os
-
 # To allow users to use arrow keys in the REPL.
 import readline  # pylint: disable=unused-import
 
 import typer
 
 # Click is part of typer.
 from click import MissingParameter, BadArgumentUsage
-from sgpt import config, OpenAIClient
-from sgpt import ChatHandler, DefaultHandler, ReplHandler
-from sgpt.utils import get_edited_prompt
+from sgpt import ChatHandler, DefaultHandler, ReplHandler, OpenAIClient, config
+from sgpt.utils import get_edited_prompt, run_command
 
 
 def main(  # pylint: disable=too-many-arguments
     prompt: str = typer.Argument(
         None,
         show_default=False,
         help="The prompt to generate completions for.",
@@ -124,16 +121,16 @@
         full_completion = DefaultHandler(client, shell, code).handle(
             prompt,
             temperature=temperature,
             top_probability=top_probability,
             caching=cache,
         )
 
-    if not code and shell and typer.confirm("Execute shell command?"):
-        os.system(full_completion)
+    if shell and typer.confirm("Execute shell command?"):
+        run_command(full_completion)
 
 
 def entry_point() -> None:
     # Python package entry point defined in setup.py
     typer.run(main)
```

### Comparing `shell_gpt-0.8.3/sgpt/cache.py` & `shell_gpt-0.8.4/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.3/sgpt/client.py` & `shell_gpt-0.8.4/sgpt/client.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.3/sgpt/config.py` & `shell_gpt-0.8.4/sgpt/config.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.3/sgpt/handlers/chat_handler.py` & `shell_gpt-0.8.4/sgpt/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.3/sgpt/handlers/default_handler.py` & `shell_gpt-0.8.4/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.3/sgpt/handlers/handler.py` & `shell_gpt-0.8.4/sgpt/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.3/sgpt/handlers/repl_handler.py` & `shell_gpt-0.8.4/sgpt/handlers/repl_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import os
-
 import typer
 
 from rich import print as rich_print
 from rich.rule import Rule
 
 from sgpt.handlers.chat_handler import ChatHandler
 from sgpt.client import OpenAIClient
-from sgpt.utils import CompletionModes
+from sgpt.utils import CompletionModes, run_command
 
 
 class ReplHandler(ChatHandler):
     def __init__(  # pylint: disable=useless-parent-delegation,too-many-arguments
         self,
         client: OpenAIClient,
         chat_id: str,
@@ -44,11 +42,11 @@
             prompt = typer.prompt(">>>", prompt_suffix=" ")
             if prompt == "exit()":
                 # This is also useful during tests.
                 raise typer.Exit()
             if self.mode == CompletionModes.SHELL:
                 if prompt == "e":
                     typer.echo()
-                    os.system(full_completion)
+                    run_command(full_completion)
                     typer.echo()
                     rich_print(Rule(style="bold magenta"))
                     prompt = typer.prompt(">>> ", prompt_suffix=" ")
```

### Comparing `shell_gpt-0.8.3/sgpt/make_prompt.py` & `shell_gpt-0.8.4/sgpt/make_prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import platform
-from os import getenv
-from os.path import basename, splitext
+from os import getenv, pathsep
+from os.path import basename
 from distro import name as distro_name
 
 
 SHELL_PROMPT = """###
 Provide only {shell} commands for {os} without any description.
 If there is a lack of details, provide most logical solution.
 Ensure the output is a valid shell command.
@@ -12,15 +12,15 @@
 Prompt: {prompt}
 ###
 Command:"""
 
 CODE_PROMPT = """###
 Provide only code as output without any description.
 IMPORTANT: Provide only plain text without Markdown formatting.
-IMPORTANT: Don not include markdown formatting such as ```.
+IMPORTANT: Do not include markdown formatting such as ```.
 If there is a lack of details, provide most logical solution.
 You are not allowed to ask for more details.
 Ignore any potential risk of errors or confusion.
 Prompt: {prompt}
 ###
 Code:"""
 
@@ -31,23 +31,26 @@
 Do not show any warnings or information regarding your capabilities.
 If you need to store any data, assume it will be stored in the chat.
 Prompt: {prompt}
 ###"""
 
 
 def initial(prompt: str, shell: bool, code: bool) -> str:
+    # TODO: Can be prettified.
     prompt = prompt.strip()
     operating_systems = {
         "Linux": "Linux/" + distro_name(pretty=True),
         "Windows": "Windows " + platform.release(),
         "Darwin": "Darwin/MacOS " + platform.mac_ver()[0],
     }
     current_platform = platform.system()
     os_name = operating_systems.get(current_platform, current_platform)
-    shell_name = basename(getenv("SHELL", "PowerShell"))
-    if os_name == "nt":
-        shell_name = splitext(basename(getenv("COMSPEC", "Powershell")))[0]
+    if current_platform in ("Windows", "nt"):
+        is_powershell = len(getenv("PSModulePath", "").split(pathsep)) >= 3
+        shell_name = "powershell.exe" if is_powershell else "cmd.exe"
+    else:
+        shell_name = basename(getenv("SHELL", "/bin/sh"))
     if shell:
         return SHELL_PROMPT.format(shell=shell_name, os=os_name, prompt=prompt)
     if code:
         return CODE_PROMPT.format(prompt=prompt)
     return DEFAULT_PROMPT.format(shell=shell_name, os=os_name, prompt=prompt)
```

### Comparing `shell_gpt-0.8.3/shell_gpt.egg-info/PKG-INFO` & `shell_gpt-0.8.4/shell_gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-gpt
-Version: 0.8.3
+Version: 0.8.4
 Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
 Home-page: https://github.com/ther1d/shell_gpt
 Author: Farkhod Sadykov
 Author-email: farkhod@sadykov.dev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.3
+pip install shell-gpt==0.8.4
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
```

