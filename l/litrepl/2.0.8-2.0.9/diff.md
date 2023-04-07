# Comparing `tmp/litrepl-2.0.8.tar.gz` & `tmp/litrepl-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litrepl-2.0.8.tar", last modified: Sat Mar 11 18:54:40 2023, max compression
+gzip compressed data, was "litrepl-2.0.9.tar", last modified: Fri Apr  7 19:59:29 2023, max compression
```

## Comparing `litrepl-2.0.8.tar` & `litrepl-2.0.9.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.027506 litrepl-2.0.8/
--rw-r--r--   0 grwlf     (1000) users      (100)      125 2022-12-28 09:58:29.000000 litrepl-2.0.8/.git_archival.txt
--rw-r--r--   0 grwlf     (1000) users      (100)       32 2022-12-28 09:58:47.000000 litrepl-2.0.8/.gitattributes
--rw-r--r--   0 grwlf     (1000) users      (100)      244 2023-03-11 13:22:10.000000 litrepl-2.0.8/.gitignore
--rw-r--r--   0 grwlf     (1000) users      (100)      106 2022-08-02 20:09:41.000000 litrepl-2.0.8/.gitmodules
--rw-r--r--   0 grwlf     (1000) users      (100)     1514 2022-08-28 13:12:33.000000 litrepl-2.0.8/LICENSE.txt
--rw-r--r--   0 grwlf     (1000) users      (100)      675 2023-03-11 13:26:24.000000 litrepl-2.0.8/Makefile
--rw-r--r--   0 grwlf     (1000) users      (100)      554 2023-03-11 18:54:40.027506 litrepl-2.0.8/PKG-INFO
--rw-r--r--   0 grwlf     (1000) users      (100)    14859 2023-02-20 20:00:48.000000 litrepl-2.0.8/README.md
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.025506 litrepl-2.0.8/data/
--rw-r--r--   0 grwlf     (1000) users      (100)      205 2022-08-15 20:25:40.000000 litrepl-2.0.8/data/test-1.md
--rw-r--r--   0 grwlf     (1000) users      (100)      148 2022-08-07 19:33:26.000000 litrepl-2.0.8/data/test-2.md
--rw-r--r--   0 grwlf     (1000) users      (100)      620 2022-08-19 20:07:39.000000 litrepl-2.0.8/data/test-3.tex
--rw-r--r--   0 grwlf     (1000) users      (100)    10830 2023-03-11 17:01:48.000000 litrepl-2.0.8/default.nix
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.026506 litrepl-2.0.8/doc/
--rw-r--r--   0 grwlf     (1000) users      (100)      729 2023-03-11 18:52:41.000000 litrepl-2.0.8/doc/example.md
--rw-r--r--   0 grwlf     (1000) users      (100)     1389 2022-08-22 18:37:32.000000 litrepl-2.0.8/doc/example.tex
--rw-r--r--   0 grwlf     (1000) users      (100)     3911 2022-08-22 21:31:59.000000 litrepl-2.0.8/doc/quickstart.tex
--rw-r--r--   0 grwlf     (1000) users      (100)      709 2022-08-21 15:54:58.000000 litrepl-2.0.8/env.sh
--rw-r--r--   0 grwlf     (1000) users      (100)      560 2023-03-11 10:23:50.000000 litrepl-2.0.8/flake.lock
--rw-r--r--   0 grwlf     (1000) users      (100)     1284 2023-03-11 12:33:28.000000 litrepl-2.0.8/flake.nix
--rw-r--r--   0 grwlf     (1000) users      (100)     1580 2022-08-20 07:35:40.000000 litrepl-2.0.8/ipython.sh
--rw-r--r--   0 grwlf     (1000) users      (100)     1740 2023-02-15 11:57:38.000000 litrepl-2.0.8/localrc.vim
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.026506 litrepl-2.0.8/nix/
--rw-r--r--   0 grwlf     (1000) users      (100)    21116 2023-01-14 19:29:12.000000 litrepl-2.0.8/nix/st-config.def.h
--rw-r--r--   0 grwlf     (1000) users      (100)      264 2022-08-07 19:31:18.000000 litrepl-2.0.8/pycodestyle.cfg
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.023506 litrepl-2.0.8/python/
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.025506 litrepl-2.0.8/python/bin/
--rwxr-xr-x   0 grwlf     (1000) users      (100)     4050 2023-03-11 18:42:35.000000 litrepl-2.0.8/python/bin/litrepl
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.026506 litrepl-2.0.8/python/litrepl/
--rw-r--r--   0 grwlf     (1000) users      (100)     1204 2023-03-11 13:23:32.000000 litrepl-2.0.8/python/litrepl/__init__.py
--rw-r--r--   0 grwlf     (1000) users      (100)    15652 2023-03-11 18:01:50.000000 litrepl-2.0.8/python/litrepl/base.py
--rw-r--r--   0 grwlf     (1000) users      (100)     7187 2023-03-11 16:26:18.000000 litrepl-2.0.8/python/litrepl/eval.py
--rw-r--r--   0 grwlf     (1000) users      (100)       88 2023-03-11 18:54:39.000000 litrepl-2.0.8/python/litrepl/revision.py
--rw-r--r--   0 grwlf     (1000) users      (100)       51 2023-03-11 18:54:39.000000 litrepl-2.0.8/python/litrepl/semver.py
--rw-r--r--   0 grwlf     (1000) users      (100)      950 2023-03-11 16:26:06.000000 litrepl-2.0.8/python/litrepl/types.py
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.027506 litrepl-2.0.8/python/litrepl.egg-info/
--rw-r--r--   0 grwlf     (1000) users      (100)      554 2023-03-11 18:54:39.000000 litrepl-2.0.8/python/litrepl.egg-info/PKG-INFO
--rw-r--r--   0 grwlf     (1000) users      (100)      796 2023-03-11 18:54:39.000000 litrepl-2.0.8/python/litrepl.egg-info/SOURCES.txt
--rw-r--r--   0 grwlf     (1000) users      (100)        1 2023-03-11 18:54:39.000000 litrepl-2.0.8/python/litrepl.egg-info/dependency_links.txt
--rw-r--r--   0 grwlf     (1000) users      (100)        1 2022-08-21 17:11:56.000000 litrepl-2.0.8/python/litrepl.egg-info/not-zip-safe
--rw-r--r--   0 grwlf     (1000) users      (100)        5 2023-03-11 18:54:39.000000 litrepl-2.0.8/python/litrepl.egg-info/requires.txt
--rw-r--r--   0 grwlf     (1000) users      (100)        8 2023-03-11 18:54:39.000000 litrepl-2.0.8/python/litrepl.egg-info/top_level.txt
--rw-r--r--   0 grwlf     (1000) users      (100)        6 2023-03-11 18:53:56.000000 litrepl-2.0.8/semver.txt
--rw-r--r--   0 grwlf     (1000) users      (100)       38 2023-03-11 18:54:40.027506 litrepl-2.0.8/setup.cfg
--rw-r--r--   0 grwlf     (1000) users      (100)     2099 2023-03-11 18:03:07.000000 litrepl-2.0.8/setup.py
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.027506 litrepl-2.0.8/sh/
--rwxr-xr-x   0 grwlf     (1000) users      (100)      531 2023-03-11 17:41:33.000000 litrepl-2.0.8/sh/mkpdflatex.sh
--rwxr-xr-x   0 grwlf     (1000) users      (100)     7088 2023-03-11 11:18:27.000000 litrepl-2.0.8/sh/test.sh
--rwxr-xr-x   0 grwlf     (1000) users      (100)      508 2022-09-10 21:39:56.000000 litrepl-2.0.8/sh/vim_litrepl_dev
--rw-r--r--   0 grwlf     (1000) users      (100)       32 2022-08-02 09:54:39.000000 litrepl-2.0.8/shell.nix
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.023506 litrepl-2.0.8/vim/
-drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-03-11 18:54:40.027506 litrepl-2.0.8/vim/plugin/
--rw-r--r--   0 grwlf     (1000) users      (100)     4036 2023-03-11 18:49:58.000000 litrepl-2.0.8/vim/plugin/litrepl.vim
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.861533 litrepl-2.0.9/
+-rw-r--r--   0 grwlf     (1000) users      (100)      125 2022-12-28 09:58:29.000000 litrepl-2.0.9/.git_archival.txt
+-rw-r--r--   0 grwlf     (1000) users      (100)       32 2022-12-28 09:58:47.000000 litrepl-2.0.9/.gitattributes
+-rw-r--r--   0 grwlf     (1000) users      (100)      244 2023-03-11 13:22:10.000000 litrepl-2.0.9/.gitignore
+-rw-r--r--   0 grwlf     (1000) users      (100)      106 2022-08-02 20:09:41.000000 litrepl-2.0.9/.gitmodules
+-rw-r--r--   0 grwlf     (1000) users      (100)     1514 2022-08-28 13:12:33.000000 litrepl-2.0.9/LICENSE.txt
+-rw-r--r--   0 grwlf     (1000) users      (100)      675 2023-03-11 13:26:24.000000 litrepl-2.0.9/Makefile
+-rw-r--r--   0 grwlf     (1000) users      (100)      554 2023-04-07 19:59:29.860533 litrepl-2.0.9/PKG-INFO
+-rw-r--r--   0 grwlf     (1000) users      (100)     9520 2023-04-07 19:45:13.000000 litrepl-2.0.9/README.md
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.858533 litrepl-2.0.9/data/
+-rw-r--r--   0 grwlf     (1000) users      (100)      205 2022-08-15 20:25:40.000000 litrepl-2.0.9/data/test-1.md
+-rw-r--r--   0 grwlf     (1000) users      (100)      148 2022-08-07 19:33:26.000000 litrepl-2.0.9/data/test-2.md
+-rw-r--r--   0 grwlf     (1000) users      (100)      620 2022-08-19 20:07:39.000000 litrepl-2.0.9/data/test-3.tex
+-rw-r--r--   0 grwlf     (1000) users      (100)    11061 2023-03-11 19:13:43.000000 litrepl-2.0.9/default.nix
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.859533 litrepl-2.0.9/doc/
+-rw-r--r--   0 grwlf     (1000) users      (100)     1897 2023-03-11 20:23:49.000000 litrepl-2.0.9/doc/develop.md
+-rw-r--r--   0 grwlf     (1000) users      (100)      729 2023-03-11 18:52:41.000000 litrepl-2.0.9/doc/example.md
+-rw-r--r--   0 grwlf     (1000) users      (100)     1588 2023-03-11 23:26:51.000000 litrepl-2.0.9/doc/example.tex
+-rw-r--r--   0 grwlf     (1000) users      (100)     4866 2023-03-12 08:12:32.000000 litrepl-2.0.9/doc/formatting.md
+-rw-r--r--   0 grwlf     (1000) users      (100)     3911 2022-08-22 21:31:59.000000 litrepl-2.0.9/doc/quickstart.tex
+-rw-r--r--   0 grwlf     (1000) users      (100)      709 2022-08-21 15:54:58.000000 litrepl-2.0.9/env.sh
+-rw-r--r--   0 grwlf     (1000) users      (100)      560 2023-03-11 10:23:50.000000 litrepl-2.0.9/flake.lock
+-rw-r--r--   0 grwlf     (1000) users      (100)     1284 2023-03-11 12:33:28.000000 litrepl-2.0.9/flake.nix
+-rw-r--r--   0 grwlf     (1000) users      (100)     1580 2022-08-20 07:35:40.000000 litrepl-2.0.9/ipython.sh
+-rw-r--r--   0 grwlf     (1000) users      (100)     2027 2023-03-13 10:59:13.000000 litrepl-2.0.9/localrc.vim
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.859533 litrepl-2.0.9/nix/
+-rw-r--r--   0 grwlf     (1000) users      (100)    21116 2023-01-14 19:29:12.000000 litrepl-2.0.9/nix/st-config.def.h
+-rw-r--r--   0 grwlf     (1000) users      (100)      264 2022-08-07 19:31:18.000000 litrepl-2.0.9/pycodestyle.cfg
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.856533 litrepl-2.0.9/python/
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.858533 litrepl-2.0.9/python/bin/
+-rwxr-xr-x   0 grwlf     (1000) users      (100)     4820 2023-04-07 19:57:32.000000 litrepl-2.0.9/python/bin/litrepl
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.859533 litrepl-2.0.9/python/litrepl/
+-rw-r--r--   0 grwlf     (1000) users      (100)     1204 2023-03-11 13:23:32.000000 litrepl-2.0.9/python/litrepl/__init__.py
+-rw-r--r--   0 grwlf     (1000) users      (100)    15784 2023-04-07 19:35:31.000000 litrepl-2.0.9/python/litrepl/base.py
+-rw-r--r--   0 grwlf     (1000) users      (100)     7254 2023-04-07 19:16:05.000000 litrepl-2.0.9/python/litrepl/eval.py
+-rw-r--r--   0 grwlf     (1000) users      (100)       88 2023-04-07 19:59:29.000000 litrepl-2.0.9/python/litrepl/revision.py
+-rw-r--r--   0 grwlf     (1000) users      (100)       51 2023-04-07 19:59:29.000000 litrepl-2.0.9/python/litrepl/semver.py
+-rw-r--r--   0 grwlf     (1000) users      (100)      950 2023-03-11 16:26:06.000000 litrepl-2.0.9/python/litrepl/types.py
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.860533 litrepl-2.0.9/python/litrepl.egg-info/
+-rw-r--r--   0 grwlf     (1000) users      (100)      554 2023-04-07 19:59:29.000000 litrepl-2.0.9/python/litrepl.egg-info/PKG-INFO
+-rw-r--r--   0 grwlf     (1000) users      (100)      829 2023-04-07 19:59:29.000000 litrepl-2.0.9/python/litrepl.egg-info/SOURCES.txt
+-rw-r--r--   0 grwlf     (1000) users      (100)        1 2023-04-07 19:59:29.000000 litrepl-2.0.9/python/litrepl.egg-info/dependency_links.txt
+-rw-r--r--   0 grwlf     (1000) users      (100)        1 2022-08-21 17:11:56.000000 litrepl-2.0.9/python/litrepl.egg-info/not-zip-safe
+-rw-r--r--   0 grwlf     (1000) users      (100)        5 2023-04-07 19:59:29.000000 litrepl-2.0.9/python/litrepl.egg-info/requires.txt
+-rw-r--r--   0 grwlf     (1000) users      (100)        8 2023-04-07 19:59:29.000000 litrepl-2.0.9/python/litrepl.egg-info/top_level.txt
+-rw-r--r--   0 grwlf     (1000) users      (100)        6 2023-04-07 19:58:04.000000 litrepl-2.0.9/semver.txt
+-rw-r--r--   0 grwlf     (1000) users      (100)       38 2023-04-07 19:59:29.861533 litrepl-2.0.9/setup.cfg
+-rw-r--r--   0 grwlf     (1000) users      (100)     2093 2023-03-11 20:18:17.000000 litrepl-2.0.9/setup.py
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.860533 litrepl-2.0.9/sh/
+-rwxr-xr-x   0 grwlf     (1000) users      (100)      531 2023-03-11 17:41:33.000000 litrepl-2.0.9/sh/mkpdflatex.sh
+-rwxr-xr-x   0 grwlf     (1000) users      (100)     7379 2023-04-07 19:42:43.000000 litrepl-2.0.9/sh/test.sh
+-rwxr-xr-x   0 grwlf     (1000) users      (100)      508 2022-09-10 21:39:56.000000 litrepl-2.0.9/sh/vim_litrepl_dev
+-rw-r--r--   0 grwlf     (1000) users      (100)       32 2022-08-02 09:54:39.000000 litrepl-2.0.9/shell.nix
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.856533 litrepl-2.0.9/vim/
+drwxr-xr-x   0 grwlf     (1000) users      (100)        0 2023-04-07 19:59:29.860533 litrepl-2.0.9/vim/plugin/
+-rw-r--r--   0 grwlf     (1000) users      (100)     4036 2023-04-04 09:34:56.000000 litrepl-2.0.9/vim/plugin/litrepl.vim
```

### Comparing `litrepl-2.0.8/LICENSE.txt` & `litrepl-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/Makefile` & `litrepl-2.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/PKG-INFO` & `litrepl-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litrepl
-Version: 2.0.8
+Version: 2.0.9
 Summary: LitREPL is a macroprocessing Python library for Litrate programming and code execution.
 Author: Sergei Mironov
 Author-email: grrwlf@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `litrepl-2.0.8/data/test-3.tex` & `litrepl-2.0.9/data/test-3.tex`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/default.nix` & `litrepl-2.0.9/default.nix`

 * *Files 5% similar despite different names*

```diff
@@ -81,21 +81,21 @@
         LITREPL_ROOT="`pwd`/python" \
         ${./sh/test.sh}
       '';
 
       doCheck = true;
     });
 
-    litrepl-pypy = (python: python.pkgs.buildPythonPackage rec {
+    litrepl-pypi = (python: python.pkgs.buildPythonPackage rec {
       pname = "litrepl";
       version = lib.fileContents "${litrepl_root}/semver.txt";
       propagatedBuildInputs = [(lark-parser112 python.pkgs) pkgs.socat];
       src = python.pkgs.fetchPypi {
         inherit pname version;
-        sha256 = "sha256-Av0lXAcn8PW5Tt/M8VFilYrhp0nJXYTly0dOzBTshlQ=";
+        sha256 = "sha256-Ex06917+Grhhv8hGEr59CUK0+5tsQ6+wNv+7to2WDrg=";
         # sha256 = "sha256-tiNqmVMM3JttYc8LNnmMdxw6cenogCAhFu9feVMsnq4=";
         # sha256 = "sha256:0vq2igzfi3din1fah18fzp7wdh089hf28s3lwm321k11jhycqgy9";
       };
     });
 
     mytexlive =
       (let
@@ -128,26 +128,29 @@
         if test -f ./env.sh ; then
           . ./env.sh
           export QT_QPA_PLATFORM_PLUGIN_PATH=`echo ${pkgs.qt5.qtbase.bin}/lib/qt-*/plugins/platforms/`
         fi
       '';
     };
 
-    vim-litrepl = (py : pkgs.vimUtils.buildVimPluginFrom2Nix {
+    vim-litrepl_ = (litrepl: py : pkgs.vimUtils.buildVimPluginFrom2Nix {
       pname = "vim-litrepl";
       version = "9999";
       src = builtins.filterSource (
         path: type: !( baseNameOf path == "bin" && type == "directory" )) ./vim;
       postInstall = ''
         mkdir -pv $target/bin
         ln -s ${pkgs.socat}/bin/socat $target/bin/socat
         ln -s ${litrepl py}/bin/litrepl $target/bin/litrepl
       '';
     });
 
+    vim-litrepl = py: vim-litrepl_ litrepl py;
+    vim-litrepl-pypi = py: vim-litrepl_ litrepl-pypi py;
+
     vim-terminal-images = pkgs.vimUtils.buildVimPluginFrom2Nix rec {
       name = "vim-terminal-images";
       # https://github.com/sergei-grechanik/vim-terminal-images/commits/master
       src = fetchFromGitHub {
         owner = "sergei-grechanik";
         repo = name;
         rev = "8e617d76bbd2555d466c36a783835e63001135e9";
@@ -349,15 +352,15 @@
     shell-demo = pkgs.mkShell {
       name = "shell-demo";
       buildInputs = [
         vim-demo
         latexrun
         mytexlive
         grechanik-st
-        (litrepl-release-pypy)
+        (litrepl-release-pypi)
       ] ++ (with pkgs ; [
         peek
         tmux
       ]);
       shellHook = with pkgs; ''
         export PS1="\n[DEMO] \[\033[1;32m\][nix-shell:\w]\$\[\033[0m\] "
         # exec ${grechanik-st}/bin/st
@@ -365,20 +368,22 @@
     };
 
     shell = shell-dev;
 
 
     litrepl-dev = litrepl python-dev;
     litrepl-release = litrepl python-release;
-    litrepl-release-pypy = litrepl-pypy python-release;
+    litrepl-release-pypi = litrepl-pypi python-release;
     vim-litrepl-release = vim-litrepl python-release;
+    vim-litrepl-release-pypi = vim-litrepl-pypi python-release;
 
     collection = rec {
       inherit pkgs shell shell-dev shell-demo vim-litrepl-release vim-test
-      vim-demo grechanik-st vimtex-local litrepl-release litrepl-dev;
+      vim-demo grechanik-st vimtex-local litrepl-release litrepl-dev
+      litrepl-release-pypi vim-litrepl-release-pypi;
     };
   };
 
 in
   local.collection
```

### Comparing `litrepl-2.0.8/doc/example.md` & `litrepl-2.0.9/doc/example.md`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/doc/quickstart.tex` & `litrepl-2.0.9/doc/quickstart.tex`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/env.sh` & `litrepl-2.0.9/env.sh`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/flake.lock` & `litrepl-2.0.9/flake.lock`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/flake.nix` & `litrepl-2.0.9/flake.nix`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/ipython.sh` & `litrepl-2.0.9/ipython.sh`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/nix/st-config.def.h` & `litrepl-2.0.9/nix/st-config.def.h`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/python/litrepl/__init__.py` & `litrepl-2.0.9/python/litrepl/__init__.py`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/python/litrepl/base.py` & `litrepl-2.0.9/python/litrepl/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,14 +270,26 @@
 def indent(col,lines:str)->str:
   return '\n'.join([' '*col+l for l in lines.split('\n')])
 
 def escape(text,pat):
   epat=''.join(['\\'+c for c in pat])
   return text.replace(pat,epat)
 
+def eval_code(a, code:str, runr:Optional[RunResult]=None) -> str:
+  fns=pipenames(a)
+  if runr is None:
+    code2,runr=rresultLoad(code)
+  else:
+    code2=code
+  if runr is None:
+    rr,runr=processAdapt(fns,code2,a.timeout_initial)
+  else:
+    rr=processCont(fns,runr,a.timeout_continue)
+  return rresultSave(rr.text,runr) if rr.timeout else rr.text
+
 def eval_section_(a, tree, secrec:SecRec)->None:
   """ Evaluate sections as specify by the `secrec` request.  """
   fns=pipenames(a)
   nsecs=secrec.nsecs
   if not running(a):
     start(a)
   ssrc:Dict[int,str]={} # Section sources
@@ -297,20 +309,15 @@
       bmarker=tree.children[0].children[0].value
       emarker=tree.children[2].children[0].value
       print(f"{bmarker}{t}{emarker}", end='')
       bm,em=tree.children[0].meta,tree.children[2].meta
       code=unindent(bm.column-1,t)
       ssrc[self.nsec]=code
       if self.nsec in nsecs:
-        runr:Optional[RunResult]=secrec.pending.get(self.nsec)
-        if runr is None:
-          rr,runr=processAdapt(fns,code,a.timeout_initial)
-        else:
-          rr=processCont(fns,runr,a.timeout_continue)
-        sres[self.nsec]=rresultSave(rr.text,runr) if rr.timeout else rr.text
+        sres[self.nsec]=eval_code(a,code,secrec.pending.get(self.nsec))
     def ocodesection(self,tree):
       bmarker=tree.children[0].children[0].value
       emarker=tree.children[2].children[0].value
       bm,em=tree.children[0].meta,tree.children[2].meta
       if self.nsec in nsecs:
         assert self.nsec in sres
         print(bmarker+"\n"+indent(bm.column-1,
```

### Comparing `litrepl-2.0.8/python/litrepl/eval.py` & `litrepl-2.0.9/python/litrepl/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,15 @@
       res=readout(fdr,prompt=mkre(r.pattern),merge=merge_rn2)
       return res
   finally:
     if fdr!=0:
       os.close(fdr)
 
 def processCont(fns:FileNames, r:RunResult, timeout:float=1.0)->ReadResult:
+  """ Continue reading from the already running readout process"""
   fdr=0
   rr:ReadResult
   try:
     with with_sigint(fns):
       fdr=os.open(r.fname,os.O_RDONLY|os.O_SYNC)
       assert fdr>0
       try:
```

### Comparing `litrepl-2.0.8/python/litrepl/types.py` & `litrepl-2.0.9/python/litrepl/types.py`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/python/litrepl.egg-info/PKG-INFO` & `litrepl-2.0.9/python/litrepl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litrepl
-Version: 2.0.8
+Version: 2.0.9
 Summary: LitREPL is a macroprocessing Python library for Litrate programming and code execution.
 Author: Sergei Mironov
 Author-email: grrwlf@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `litrepl-2.0.8/setup.py` & `litrepl-2.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   LITREPL_REVISION=environ["LITREPL_REVISION"]
 except Exception:
   warning("Couldn't read LITREPL_REVISION, trying `git rev-parse`")
   try:
     from subprocess import check_output
     import sys
     LITREPL_REVISION=check_output(['git', 'rev-parse', 'HEAD'],
-                                  cwd=environ['LITREPL_ROOT']).decode().strip()
+                                  cwd=dirname(__file__)).decode().strip()
   except Exception:
     warning("Couldn't use `git rev-parse`, no revision metadata will be set")
     LITREPL_REVISION=None
 
 
 LITREPL_SEMVER:Optional[str]
 try:
```

### Comparing `litrepl-2.0.8/sh/mkpdflatex.sh` & `litrepl-2.0.9/sh/mkpdflatex.sh`

 * *Files identical despite different names*

### Comparing `litrepl-2.0.8/sh/test.sh` & `litrepl-2.0.9/sh/test.sh`

 * *Files 4% similar despite different names*

```diff
@@ -366,26 +366,43 @@
 EOF
 cat source.md | runlitrepl --filetype=markdown --timeout-initial=1 eval-sections '0..$' >out1.md
 cat out1.md | runlitrepl --filetype=markdown --timeout-continue=1 eval-sections '0..$' >out2.md
 grep -q 'BG' out2.md
 runlitrepl stop
 )} #}}}
 
+test_eval_code() {( #{{{
+mktest "_test_eval_code"
+runlitrepl start
+cat >source.py <<"EOF"
+def hello(name):
+  print(f"Hello, {name}!")
+
+hello('World')
+EOF
+cat source.py | runlitrepl eval-code >out.txt
+diff -u out.txt - <<"EOF"
+Hello, World!
+
+EOF
+runlitrepl stop
+)} #}}}
 
 interpreters() {
   echo "$(which python)"
   echo "$(which ipython)"
 }
 
 tests() {
   echo test_parse_print
   echo test_eval_md
   echo test_tqdm
   echo test_eval_tex
   echo test_async
+  echo test_eval_code
 }
 
 runlitrepl() {
   test -n "$LITREPL_INTERPRETER"
   test -n "$LITREPL_BIN"
   $LITREPL_BIN --interpreter="$LITREPL_INTERPRETER" "$@"
 }
```

### Comparing `litrepl-2.0.8/vim/plugin/litrepl.vim` & `litrepl-2.0.9/vim/plugin/litrepl.vim`

 * *Files identical despite different names*

