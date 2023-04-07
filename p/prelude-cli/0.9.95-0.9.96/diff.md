# Comparing `tmp/prelude-cli-0.9.95.tar.gz` & `tmp/prelude-cli-0.9.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-0.9.95.tar", last modified: Wed Mar 29 17:30:30 2023, max compression
+gzip compressed data, was "prelude-cli-0.9.96.tar", last modified: Fri Apr  7 19:52:22 2023, max compression
```

## Comparing `prelude-cli-0.9.95.tar` & `prelude-cli-0.9.96.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:30:30.250966 prelude-cli-0.9.95/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-0.9.95/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-0.9.95/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      833 2023-03-29 17:30:30.251023 prelude-cli-0.9.95/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-0.9.95/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:30:30.247957 prelude-cli-0.9.95/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.95/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1007 2023-02-28 15:28:14.000000 prelude-cli-0.9.95/prelude_cli/cli.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:30:30.249060 prelude-cli-0.9.95/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.95/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-0.9.95/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:30:30.250719 prelude-cli-0.9.95/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.95/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-0.9.95/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-0.9.95/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     5805 2023-03-28 21:39:17.000000 prelude-cli-0.9.95/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3353 2023-03-28 21:39:17.000000 prelude-cli-0.9.95/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)    30857 2023-03-23 14:22:31.000000 prelude-cli-0.9.95/prelude_cli/views/interactive.py
--rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-0.9.95/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-03-29 17:30:30.248869 prelude-cli-0.9.95/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      833 2023-03-29 17:30:30.000000 prelude-cli-0.9.95/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      579 2023-03-29 17:30:30.000000 prelude-cli-0.9.95/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-03-29 17:30:30.000000 prelude-cli-0.9.95/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-03-29 17:30:30.000000 prelude-cli-0.9.95/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-03-29 17:30:30.000000 prelude-cli-0.9.95/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-03-29 17:30:30.000000 prelude-cli-0.9.95/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-0.9.95/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      679 2023-03-29 17:30:30.251268 prelude-cli-0.9.95/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.814551 prelude-cli-0.9.96/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      833 2023-04-07 19:52:22.814601 prelude-cli-0.9.96/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-0.9.96/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.810638 prelude-cli-0.9.96/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1007 2023-02-28 15:28:14.000000 prelude-cli-0.9.96/prelude_cli/cli.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.811769 prelude-cli-0.9.96/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-0.9.96/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.814359 prelude-cli-0.9.96/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-0.9.96/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-0.9.96/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     5805 2023-03-28 21:39:17.000000 prelude-cli-0.9.96/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3355 2023-04-07 19:23:14.000000 prelude-cli-0.9.96/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)    31024 2023-04-07 19:23:14.000000 prelude-cli-0.9.96/prelude_cli/views/interactive.py
+-rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-0.9.96/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-07 19:52:22.811573 prelude-cli-0.9.96/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      833 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      579 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-07 19:52:22.000000 prelude-cli-0.9.96/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-0.9.96/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      679 2023-04-07 19:52:22.814817 prelude-cli-0.9.96/setup.cfg
```

### Comparing `prelude-cli-0.9.95/LICENSE` & `prelude-cli-0.9.96/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.95/PKG-INFO` & `prelude-cli-0.9.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 0.9.95
+Version: 0.9.96
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-0.9.95/prelude_cli/cli.py` & `prelude-cli-0.9.96/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.95/prelude_cli/views/build.py` & `prelude-cli-0.9.96/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.95/prelude_cli/views/configure.py` & `prelude-cli-0.9.96/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.95/prelude_cli/views/detect.py` & `prelude-cli-0.9.96/prelude_cli/views/detect.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.95/prelude_cli/views/iam.py` & `prelude-cli-0.9.96/prelude_cli/views/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 @iam.command('create-account')
 @click.pass_obj
 @handle_api_error
 @click.confirmation_option(prompt='Overwrite local account credentials for selected profile?')
 def register_account(controller):
     """ Register a new account """
     creds = controller.new_account(handle=click.prompt('Enter a handle'))
-    print("Check your email to verifiy your account.\n")
     print_json(data=creds)
+    print("\nCheck your email to verify your account.\n")
 
 
 @iam.command('update-account')
 @click.option('-m', '--mode',
               help='provide a mode',
               default=Mode.MANUAL.name, show_default=True,
               type=click.Choice([m.name for m in Mode], case_sensitive=False))
@@ -57,17 +57,16 @@
     """ Create a new user in your account """
     expires = datetime.utcnow() + timedelta(days=days)
     resp = controller.create_user(
         handle=handle, 
         permission=Permission[permission.upper()].value, 
         expires=expires
     )
-    print("Check your email to verifiy your account.\n")
     print_json(data=resp)
-
+    print("\nCheck your email to verifiy your account.\n")
 
 @iam.command('delete-user')
 @click.confirmation_option(prompt='Are you sure?')
 @click.argument('handle')
 @click.pass_obj
 @handle_api_error
 def delete_user(controller, handle):
@@ -88,15 +87,15 @@
 
 
 @iam.command('detach-control')
 @click.confirmation_option(prompt='Are you sure?')
 @click.argument('name')
 @click.pass_obj
 @handle_api_error
-def attach_control(controller, name):
+def detach_control(controller, name):
     """ Detach an existing control from your account """
     controller.detach_control(name=name)
 
 
 @iam.command('purge')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
```

### Comparing `prelude-cli-0.9.95/prelude_cli/views/interactive.py` & `prelude-cli-0.9.96/prelude_cli/views/interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -905,13 +905,16 @@
             print(Padding('Goodbye. May Verified Security Tests be with you.', 1))
             break
         except PermissionError as pe:
             yes = Confirm.ask(str(pe))
             if not yes:
                 break
 
-            wizard.iam.new_account(handle=os.getlogin())
+            email = Prompt.ask('Enter your email handle')
+            wizard.iam.new_account(handle=email)
             keychain = PurePath(Path.home(), '.prelude', 'keychain.ini')
             print(f'Account created! Credentials are stored in your keychain: {keychain}')
+            print('Check your email to verify your account, then restart the wizard to continue.')
+            break
         except Exception as ex:
             wizard.console.print(str(ex), style='red')
             break
```

### Comparing `prelude-cli-0.9.95/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-0.9.96/prelude_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 0.9.95
+Version: 0.9.96
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-0.9.95/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-0.9.96/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.95/setup.cfg` & `prelude-cli-0.9.96/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 0.9.95
+version = 0.9.96
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 0.9.95
+	prelude-sdk == 0.9.96
 	click
 	rich
 	simple-term-menu
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

