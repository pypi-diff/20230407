# Comparing `tmp/yaml_scripts-0.1.1.post0.tar.gz` & `tmp/yaml_scripts-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_scripts-0.1.1.post0.tar", max compression
+gzip compressed data, was "yaml_scripts-0.1.1.post1.tar", max compression
```

## Comparing `yaml_scripts-0.1.1.post0.tar` & `yaml_scripts-0.1.1.post1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      578 2023-04-07 20:59:19.779010 yaml_scripts-0.1.1.post0/pyproject.toml
--rw-r--r--   0        0        0     2988 2023-04-07 20:58:15.005810 yaml_scripts-0.1.1.post0/README.md
--rw-r--r--   0        0        0       67 2023-04-07 20:13:47.302236 yaml_scripts-0.1.1.post0/yaml_scripts/__init__.py
--rw-r--r--   0        0        0       48 2023-04-07 20:14:13.517705 yaml_scripts-0.1.1.post0/yaml_scripts/__main__.py
--rw-r--r--   0        0        0     7165 2023-04-07 19:36:45.405425 yaml_scripts-0.1.1.post0/yaml_scripts/build.py
--rw-r--r--   0        0        0    10054 2023-04-07 20:11:40.409409 yaml_scripts-0.1.1.post0/yaml_scripts/cli.py
--rw-r--r--   0        0        0      593 2023-04-07 02:17:46.653285 yaml_scripts-0.1.1.post0/yaml_scripts/display.py
--rw-r--r--   0        0        0     3876 1970-01-01 00:00:00.000000 yaml_scripts-0.1.1.post0/setup.py
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 yaml_scripts-0.1.1.post0/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-04-07 21:01:48.264928 yaml_scripts-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     2954 2023-04-07 21:01:24.842113 yaml_scripts-0.1.1.post1/README.md
+-rw-r--r--   0        0        0       67 2023-04-07 20:13:47.302236 yaml_scripts-0.1.1.post1/yaml_scripts/__init__.py
+-rw-r--r--   0        0        0       48 2023-04-07 20:14:13.517705 yaml_scripts-0.1.1.post1/yaml_scripts/__main__.py
+-rw-r--r--   0        0        0     7165 2023-04-07 19:36:45.405425 yaml_scripts-0.1.1.post1/yaml_scripts/build.py
+-rw-r--r--   0        0        0    10054 2023-04-07 20:11:40.409409 yaml_scripts-0.1.1.post1/yaml_scripts/cli.py
+-rw-r--r--   0        0        0      593 2023-04-07 02:17:46.653285 yaml_scripts-0.1.1.post1/yaml_scripts/display.py
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 yaml_scripts-0.1.1.post1/setup.py
+-rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 yaml_scripts-0.1.1.post1/PKG-INFO
```

### Comparing `yaml_scripts-0.1.1.post0/pyproject.toml` & `yaml_scripts-0.1.1.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yaml-scripts"
-version = "0.1.1-post0"
+version = "0.1.1-post1"
 description = "Creating windows auto install scripts from YAML config files"
 authors = ["arnos-stuff <bcda0276@gmail.com>"]
 readme = "README.md"
 packages = [{include = "yaml_scripts"}]
 homepage = "https://github.com/arnos-stuff/yaml-scripts"
 
 [tool.poetry.dependencies]
```

### Comparing `yaml_scripts-0.1.1.post0/README.md` & `yaml_scripts-0.1.1.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Creating auto install scripts from YAML config files
 
 ## Features
 
-- [Pydantic-like Schema validation](#schema-valid): the YAML schema has precise syntax and the build pipeline will yield warnings or stop if your file has errors in it
+- [Pydantic-like Schema validation](https://www.andrewvillazon.com/validate-yaml-python-schema/): the YAML schema has precise syntax and the build pipeline will yield warnings or stop if your file has errors in it
 - A **set of CLIs** to interact with config files:
     - `yamlrun` shows the commands
     - `yamlrun script` is the script building subcommand
     - `yamlrun upload` is the script temp hosting subcommand
     - `yamlrun pack` locates a `setup.yml` file within the current directory and runs all the commands.
 
 
@@ -89,11 +89,8 @@
 
 # Installation
 
 Just `pip install` it if you have it, but an executable is underway 😎
 
 ```powershell
 pip install yaml-scripts
-```
-
-
-[schema-valid]:https://www.andrewvillazon.com/validate-yaml-python-schema/
+```
```

### Comparing `yaml_scripts-0.1.1.post0/yaml_scripts/build.py` & `yaml_scripts-0.1.1.post1/yaml_scripts/build.py`

 * *Files identical despite different names*

### Comparing `yaml_scripts-0.1.1.post0/yaml_scripts/cli.py` & `yaml_scripts-0.1.1.post1/yaml_scripts/cli.py`

 * *Files identical despite different names*

### Comparing `yaml_scripts-0.1.1.post0/yaml_scripts/display.py` & `yaml_scripts-0.1.1.post1/yaml_scripts/display.py`

 * *Files identical despite different names*

### Comparing `yaml_scripts-0.1.1.post0/setup.py` & `yaml_scripts-0.1.1.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['yamlrun = yaml_scripts.cli:app',
                      'ymlr = yaml_scripts.cli:app']}
 
 setup_kwargs = {
     'name': 'yaml-scripts',
-    'version': '0.1.1.post0',
+    'version': '0.1.1.post1',
     'description': 'Creating windows auto install scripts from YAML config files',
-    'long_description': "# Creating auto install scripts from YAML config files\n\n## Features\n\n- [Pydantic-like Schema validation](#schema-valid): the YAML schema has precise syntax and the build pipeline will yield warnings or stop if your file has errors in it\n- A **set of CLIs** to interact with config files:\n    - `yamlrun` shows the commands\n    - `yamlrun script` is the script building subcommand\n    - `yamlrun upload` is the script temp hosting subcommand\n    - `yamlrun pack` locates a `setup.yml` file within the current directory and runs all the commands.\n\n\n## An explanation\n\nRunning the command\n\n```powershell\nyamlrun ?\n```\n\nOr equivalently `yamlrun explain` will output this explanation in the terminal:\n\n---\n### The setup file\n---\n\nThe YAML setup file (which can also be JSON), is a way for you to describle exactly what type of package/program you\nwant to auto-install using a single installer.\n\n---\n### File structure \n---\nThe file is structured in the following way:\n```yaml\n<task name 1>:\n    description: <textual description if you wish, OPTIONAL>\n    items:\n        <item name 1>:\n            description: <textual description if you wish, OPTIONAL>\n            type: <type description, if it's a CLI, GUI, what purpose, REQUIRED>\n            priority: <how important it is to install it within the setup REQUIRED>\n            commands:\n                - <powershell line 1>\n                - <powershell line 2>\n        <item name 2>:\n            ...\n        <item name 3>:\n            ...\n    run:\n        # order in which the items are going to be installed\n        steps:\n            - <item name 1>\n            - <item name 3> # look you just swapped the order !\n            - <item name 2>\n<task name 2>:\n    ...\n<task name 3>:\n    ...\n```\n\n---\n### Script & Executable Builder \n---\n\nTwo options:\n\n(1) One-liner script install. This script is equivalent to:\n\n- Building the PS1 core script `yamlrun script build <task> <path/to/setup.yml>`\n- Uploading the PS1 core script `yamlrun upload f <path/to/setup.ps1>`\n- The previous step should give you an URL of the kind http://ix.io/<letters or numbers>\n- Your resulting one liner is just:\n\n```powershell\nSet-ExecutionPolicy RemoteSigned -Scope CurrentUser -Force ; irm <url> | iex\n```\n\nthis is the `yamlrun script BOL` or `yamlrun script build-one-liner` command.\n\n(2) Doing any of the steps above on its own.\n\n# Sample setup file\n\nYou can peek at the contents of this [setup.yml file](setup.yml).\n\nThe resulting script from calling `yamlrun script build` is [the setup.ps1 file](setup.ps1).\n\nFinally, calling `yamlrun setup render <name>` will generate a [markdown formatted version of your setup file like setup.md](setup.md)\n\n# Installation\n\nJust `pip install` it if you have it, but an executable is underway 😎\n\n```powershell\npip install yaml-scripts\n```\n\n\n[schema-valid]:https://www.andrewvillazon.com/validate-yaml-python-schema/",
+    'long_description': "# Creating auto install scripts from YAML config files\n\n## Features\n\n- [Pydantic-like Schema validation](https://www.andrewvillazon.com/validate-yaml-python-schema/): the YAML schema has precise syntax and the build pipeline will yield warnings or stop if your file has errors in it\n- A **set of CLIs** to interact with config files:\n    - `yamlrun` shows the commands\n    - `yamlrun script` is the script building subcommand\n    - `yamlrun upload` is the script temp hosting subcommand\n    - `yamlrun pack` locates a `setup.yml` file within the current directory and runs all the commands.\n\n\n## An explanation\n\nRunning the command\n\n```powershell\nyamlrun ?\n```\n\nOr equivalently `yamlrun explain` will output this explanation in the terminal:\n\n---\n### The setup file\n---\n\nThe YAML setup file (which can also be JSON), is a way for you to describle exactly what type of package/program you\nwant to auto-install using a single installer.\n\n---\n### File structure \n---\nThe file is structured in the following way:\n```yaml\n<task name 1>:\n    description: <textual description if you wish, OPTIONAL>\n    items:\n        <item name 1>:\n            description: <textual description if you wish, OPTIONAL>\n            type: <type description, if it's a CLI, GUI, what purpose, REQUIRED>\n            priority: <how important it is to install it within the setup REQUIRED>\n            commands:\n                - <powershell line 1>\n                - <powershell line 2>\n        <item name 2>:\n            ...\n        <item name 3>:\n            ...\n    run:\n        # order in which the items are going to be installed\n        steps:\n            - <item name 1>\n            - <item name 3> # look you just swapped the order !\n            - <item name 2>\n<task name 2>:\n    ...\n<task name 3>:\n    ...\n```\n\n---\n### Script & Executable Builder \n---\n\nTwo options:\n\n(1) One-liner script install. This script is equivalent to:\n\n- Building the PS1 core script `yamlrun script build <task> <path/to/setup.yml>`\n- Uploading the PS1 core script `yamlrun upload f <path/to/setup.ps1>`\n- The previous step should give you an URL of the kind http://ix.io/<letters or numbers>\n- Your resulting one liner is just:\n\n```powershell\nSet-ExecutionPolicy RemoteSigned -Scope CurrentUser -Force ; irm <url> | iex\n```\n\nthis is the `yamlrun script BOL` or `yamlrun script build-one-liner` command.\n\n(2) Doing any of the steps above on its own.\n\n# Sample setup file\n\nYou can peek at the contents of this [setup.yml file](setup.yml).\n\nThe resulting script from calling `yamlrun script build` is [the setup.ps1 file](setup.ps1).\n\nFinally, calling `yamlrun setup render <name>` will generate a [markdown formatted version of your setup file like setup.md](setup.md)\n\n# Installation\n\nJust `pip install` it if you have it, but an executable is underway 😎\n\n```powershell\npip install yaml-scripts\n```",
     'author': 'arnos-stuff',
     'author_email': 'bcda0276@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/arnos-stuff/yaml-scripts',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `yaml_scripts-0.1.1.post0/PKG-INFO` & `yaml_scripts-0.1.1.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-scripts
-Version: 0.1.1.post0
+Version: 0.1.1.post1
 Summary: Creating windows auto install scripts from YAML config files
 Home-page: https://github.com/arnos-stuff/yaml-scripts
 Author: arnos-stuff
 Author-email: bcda0276@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,15 +14,15 @@
 Requires-Dist: yaml-setup (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Creating auto install scripts from YAML config files
 
 ## Features
 
-- [Pydantic-like Schema validation](#schema-valid): the YAML schema has precise syntax and the build pipeline will yield warnings or stop if your file has errors in it
+- [Pydantic-like Schema validation](https://www.andrewvillazon.com/validate-yaml-python-schema/): the YAML schema has precise syntax and the build pipeline will yield warnings or stop if your file has errors in it
 - A **set of CLIs** to interact with config files:
     - `yamlrun` shows the commands
     - `yamlrun script` is the script building subcommand
     - `yamlrun upload` is the script temp hosting subcommand
     - `yamlrun pack` locates a `setup.yml` file within the current directory and runs all the commands.
 
 
@@ -106,10 +106,7 @@
 # Installation
 
 Just `pip install` it if you have it, but an executable is underway 😎
 
 ```powershell
 pip install yaml-scripts
 ```
-
-
-[schema-valid]:https://www.andrewvillazon.com/validate-yaml-python-schema/
```

