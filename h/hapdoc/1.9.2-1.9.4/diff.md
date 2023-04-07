# Comparing `tmp/hapdoc-1.9.2.tar.gz` & `tmp/hapdoc-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hapdoc-1.9.2.tar", last modified: Wed Apr  5 14:13:26 2023, max compression
+gzip compressed data, was "hapdoc-1.9.4.tar", last modified: Fri Apr  7 16:11:40 2023, max compression
```

## Comparing `hapdoc-1.9.2.tar` & `hapdoc-1.9.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 14:13:26.890080 hapdoc-1.9.2/
--rw-rw-rw-   0        0        0     1085 2023-02-05 04:11:14.000000 hapdoc-1.9.2/LICENSE
--rw-rw-rw-   0        0        0       33 2023-03-26 12:25:42.000000 hapdoc-1.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3386 2023-04-05 14:13:26.889082 hapdoc-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     2546 2023-04-05 05:08:04.000000 hapdoc-1.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 14:13:26.862076 hapdoc-1.9.2/hapdoc/
--rw-rw-rw-   0        0        0     1527 2023-04-02 09:25:10.000000 hapdoc-1.9.2/hapdoc/__init__.py
--rw-rw-rw-   0        0        0      143 2023-03-24 08:02:32.000000 hapdoc-1.9.2/hapdoc/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:13:26.883080 hapdoc-1.9.2/hapdoc/autodocker/
--rw-rw-rw-   0        0        0     3445 2023-04-05 12:30:09.000000 hapdoc-1.9.2/hapdoc/autodocker/__init__.py
--rw-rw-rw-   0        0        0     1802 2023-04-04 15:32:08.000000 hapdoc-1.9.2/hapdoc/autodocker/abc.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:13:26.886076 hapdoc-1.9.2/hapdoc/autodocker/filetypes/
--rw-rw-rw-   0        0        0      141 2023-04-04 15:28:59.000000 hapdoc-1.9.2/hapdoc/autodocker/filetypes/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-04-04 15:28:21.000000 hapdoc-1.9.2/hapdoc/autodocker/filetypes/fastapi.py
--rw-rw-rw-   0        0        0     3499 2023-04-05 04:49:11.000000 hapdoc-1.9.2/hapdoc/autodocker/filetypes/js.py
--rw-rw-rw-   0        0        0     4955 2023-04-02 09:14:56.000000 hapdoc-1.9.2/hapdoc/autodocker/filetypes/py.py
--rw-rw-rw-   0        0        0    12369 2023-04-05 14:06:34.000000 hapdoc-1.9.2/hapdoc/hapdoc.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:13:26.887076 hapdoc-1.9.2/hapdoc/md/
--rw-rw-rw-   0        0        0     3936 2023-04-05 14:12:12.000000 hapdoc-1.9.2/hapdoc/md/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:13:26.855075 hapdoc-1.9.2/hapdoc/templates/
-drwxrwxrwx   0        0        0        0 2023-04-05 14:13:26.888078 hapdoc-1.9.2/hapdoc/templates/vitepress/
--rw-rw-rw-   0        0        0    18025 2023-04-05 14:10:00.000000 hapdoc-1.9.2/hapdoc/templates/vitepress/index.html
--rw-rw-rw-   0        0        0     4982 2023-04-05 12:43:48.000000 hapdoc-1.9.2/hapdoc/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:13:26.881075 hapdoc-1.9.2/hapdoc.egg-info/
--rw-rw-rw-   0        0        0     3386 2023-04-05 14:13:26.000000 hapdoc-1.9.2/hapdoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-04-05 14:13:26.000000 hapdoc-1.9.2/hapdoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 14:13:26.000000 hapdoc-1.9.2/hapdoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-05 14:13:26.000000 hapdoc-1.9.2/hapdoc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2023-04-05 14:13:26.000000 hapdoc-1.9.2/hapdoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-05 14:13:26.000000 hapdoc-1.9.2/hapdoc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 14:13:26.891083 hapdoc-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1890 2023-04-05 14:13:14.000000 hapdoc-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.467656 hapdoc-1.9.4/
+-rw-rw-rw-   0        0        0     1085 2023-02-05 04:11:14.000000 hapdoc-1.9.4/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-03-26 12:25:42.000000 hapdoc-1.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3386 2023-04-07 16:11:40.467656 hapdoc-1.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2546 2023-04-05 05:08:04.000000 hapdoc-1.9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.431823 hapdoc-1.9.4/hapdoc/
+-rw-rw-rw-   0        0        0     1552 2023-04-07 03:20:08.000000 hapdoc-1.9.4/hapdoc/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-03-24 08:02:32.000000 hapdoc-1.9.4/hapdoc/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.459632 hapdoc-1.9.4/hapdoc/autodocker/
+-rw-rw-rw-   0        0        0     3445 2023-04-05 12:30:09.000000 hapdoc-1.9.4/hapdoc/autodocker/__init__.py
+-rw-rw-rw-   0        0        0     1802 2023-04-04 15:32:08.000000 hapdoc-1.9.4/hapdoc/autodocker/abc.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.463656 hapdoc-1.9.4/hapdoc/autodocker/filetypes/
+-rw-rw-rw-   0        0        0      141 2023-04-04 15:28:59.000000 hapdoc-1.9.4/hapdoc/autodocker/filetypes/__init__.py
+-rw-rw-rw-   0        0        0     1588 2023-04-04 15:28:21.000000 hapdoc-1.9.4/hapdoc/autodocker/filetypes/fastapi.py
+-rw-rw-rw-   0        0        0     3499 2023-04-05 04:49:11.000000 hapdoc-1.9.4/hapdoc/autodocker/filetypes/js.py
+-rw-rw-rw-   0        0        0     4955 2023-04-02 09:14:56.000000 hapdoc-1.9.4/hapdoc/autodocker/filetypes/py.py
+-rw-rw-rw-   0        0        0    13119 2023-04-07 16:11:06.000000 hapdoc-1.9.4/hapdoc/hapdoc.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.465645 hapdoc-1.9.4/hapdoc/md/
+-rw-rw-rw-   0        0        0     3936 2023-04-05 14:12:12.000000 hapdoc-1.9.4/hapdoc/md/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.424741 hapdoc-1.9.4/hapdoc/templates/
+drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.466645 hapdoc-1.9.4/hapdoc/templates/vitepress/
+-rw-rw-rw-   0        0        0    18129 2023-04-07 03:35:17.000000 hapdoc-1.9.4/hapdoc/templates/vitepress/index.html
+-rw-rw-rw-   0        0        0     4982 2023-04-05 12:43:48.000000 hapdoc-1.9.4/hapdoc/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-07 16:11:40.457988 hapdoc-1.9.4/hapdoc.egg-info/
+-rw-rw-rw-   0        0        0     3386 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-07 16:11:40.000000 hapdoc-1.9.4/hapdoc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 16:11:40.467656 hapdoc-1.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1878 2023-04-07 16:11:13.000000 hapdoc-1.9.4/setup.py
```

### Comparing `hapdoc-1.9.2/LICENSE` & `hapdoc-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/PKG-INFO` & `hapdoc-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapdoc
-Version: 1.9.2
+Version: 1.9.4
 Summary: autodoc tool for everything
 Home-page: https://github.com/HapticX/hapdoc
 Author: Ethosa
 Author-email: social.ethosa@gmail.com
 Maintainer: HapticX
 Maintainer-email: hapticx.company@gmail.com
 License: MIT
```

### Comparing `hapdoc-1.9.2/README.md` & `hapdoc-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/hapdoc/__init__.py` & `hapdoc-1.9.4/hapdoc/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,7 +33,9 @@
 - `md2json`: Generates JSON file from directory of Markdown files.
 - `project-types`: Displays available project types.
 - `serve`: Starts server at host and port.
 - `tmpl-list`: List of saved templates.
 - `tmpl-new`: Create a new template.
 
 """
+
+__version__ = '1.9.3'
```

### Comparing `hapdoc-1.9.2/hapdoc/autodocker/__init__.py` & `hapdoc-1.9.4/hapdoc/autodocker/__init__.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/hapdoc/autodocker/abc.py` & `hapdoc-1.9.4/hapdoc/autodocker/abc.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/hapdoc/autodocker/filetypes/fastapi.py` & `hapdoc-1.9.4/hapdoc/autodocker/filetypes/fastapi.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/hapdoc/autodocker/filetypes/js.py` & `hapdoc-1.9.4/hapdoc/autodocker/filetypes/js.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/hapdoc/autodocker/filetypes/py.py` & `hapdoc-1.9.4/hapdoc/autodocker/filetypes/py.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/hapdoc/hapdoc.py` & `hapdoc-1.9.4/hapdoc/hapdoc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Autodoc CLI
 """
 from json import dumps
 from os import path, remove, makedirs, getcwd
-from pprint import pprint
 
 import click
 import uvicorn
 
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import HTMLResponse
@@ -17,34 +16,41 @@
 
 from .md import Md2Html
 from .utils import (
     show_all_projects, generate_md_files,
     cast_md_dir_to_json, load_user_templates,
     create_new_user_template, get_user_template_path
 )
+from . import __version__
 
 
 app = FastAPI(docs_url=None, redoc_url=None)
 app.add_middleware(
     CORSMiddleware,
     allow_origins=['*'],
     allow_methods=['*'],
     allow_headers=['*'],
     allow_credentials=True
 )
 
 
-@click.group()
-def hapdoc():
+@click.group(invoke_without_command=True)
+@click.option(
+    '-v/--version', 'show_version',
+    default=False, type=bool
+)
+def hapdoc(show_version: bool):
     """
     HapDoc is a powerful command-line interface tool that automates the process of
     generating documentation for various types of projects.
     With HapDoc, you can easily create high-quality documentation for
     Python, FastAPI, Vue, and many other types of projects.
     """
+    if show_version:
+        click.echo(click.style(f'HapDoc v{__version__}', fg='bright_blue'))
 
 
 @hapdoc.command()
 def project_types():
     """
     This command displays a list of all available project
     types that can be used in doc generating.
@@ -70,30 +76,30 @@
     """
     create_new_user_template()
 
 
 @hapdoc.command()
 @click.argument("directory", type=str)
 @click.option(
-    '--output', '-o', 'output_file',
+    '-o', '--output', 'output_file',
     help='Output file name',
     default='overview.json', type=str
 )
 @click.option(
-    '--outdir', '-O', 'output_directory',
+    '-O', '--outdir', 'output_directory',
     help='Output directory path',
     default=None, type=str
 )
 @click.option(
-    '--root', '-r', 'root',
+    '-r', '--root', 'root',
     help='Root path, by default uses working directory',
     default='', type=str
 )
 @click.option(
-    '--extension', '-e', 'ext',
+    '-e', '--extension', 'ext',
     help='File extensions in generated JSON',
     default=None, type=str
 )
 def md2json(directory: str, output_directory: str, output_file: str, root: str, ext: str):
     """
     The md2json command converts Markdown files (.md) in a directory to JSON format,
     which can be used for rendering the files using the jinja2 templating engine.
@@ -115,30 +121,30 @@
             file.write(dumps(data, indent=4))
         click.echo(click.style(f"Saved at {output_file}", fg="bright_green"))
 
 
 @hapdoc.command()
 @click.argument('project_path', type=str)
 @click.option(
-    '--doctype', '-d', 'document_type',
+    '-d', '--doctype', 'document_type',
     help='Select project type',
     default='py', type=str
 )
 @click.option(
-    '--ignore', '-i', 'ignore',
+    '-i', '--ignore', 'ignore',
     help='Ignore file extensions separated by comma',
     default='', type=str
 )
 @click.option(
-    '--extend', '-e', 'extend',
+    '-e', '--extend', 'extend',
     help='Extend doc by specified doctypes separated by comma',
     default='', type=str
 )
 @click.option(
-    '--out', '-o', 'output',
+    '-o', '--out', 'output',
     help='Output docs folder',
     default='docs', type=str
 )
 def gen(
         project_path: str,
         document_type: str,
         ignore: str,
@@ -193,26 +199,32 @@
     default='#cacaca', type=str
 )
 @click.option(
     '-ls', '--light-surface', 'light_surface_color',
     help='Light Surface color',
     default='#dedede', type=str
 )
+@click.option(
+    '-dv', '--doc-version', 'doc_version',
+    help='Generated documentation version',
+    default='1.0.0', type=str
+)
 def serve(
         host: str,
         port: str,
         docs: str,
         templates_folder: str,
         title: str,
         accent_color: str,
         background_color: str,
         surface_color: str,
         light_accent_color: str,
         light_background_color: str,
         light_surface_color: str,
+        doc_version: str,
 ):
     """
     The `serve` command starts a web server using FastAPI and uvicorn and
     provides access to Markdown files in a web browser.
     """
     user_template = get_user_template_path(templates_folder)
     env = Environment(
@@ -242,14 +254,15 @@
                         {
                             "title": "Github",
                             "icon": "fab fa-github",
                             "show_text": True,
                             "url": "https://github.com/hapticx/hapdoc"
                         },
                     ]},
+                    docVersion=doc_version,
                     accentColor=accent_color,
                     backgroundColor=background_color,
                     surfaceColor=surface_color,
                     lightAccentColor=light_accent_color,
                     lightBackgroundColor=light_background_color,
                     lightSurfaceColor=light_surface_color,
                     selected=f'/{doc}'
@@ -262,30 +275,30 @@
     click.echo(f'Your server runs at http://{host}:{port}')
     uvicorn.run(app, host=host, port=int(port))
 
 
 @hapdoc.command()
 @click.argument('docs', type=str)
 @click.option(
-    '--doctype', '-d', 'document_type',
+    '-d', '--doctype', 'document_type',
     help='Select project type',
     default='py', type=str
 )
 @click.option(
-    '--ignore', '-i', 'ignore',
+    '-i', '--ignore', 'ignore',
     help='Ignore file extensions separated by comma',
     default='', type=str
 )
 @click.option(
-    '--extend', '-e', 'extend',
+    '-e', '--extend', 'extend',
     help='Extend doc by specified docs types separated by comma',
     default='', type=str
 )
 @click.option(
-    '--out', '-o', 'output',
+    '-o', '--out', 'output',
     help='Output docs folder',
     default='buildocs', type=str
 )
 @click.option(
     '-t', '--template', 'templates_folder',
     default='hapdoc/templates/vitepress', type=str
 )
@@ -325,14 +338,19 @@
     default='#cacaca', type=str
 )
 @click.option(
     '-r', '--root', 'root',
     help='Root path, by default uses working directory',
     default=None, type=str
 )
+@click.option(
+    '-dv', '--doc-version', 'doc_version',
+    help='Generated documentation version',
+    default='1.0.0', type=str
+)
 def build(
         docs: str,
         templates_folder: str,
         title: str,
         accent_color: str,
         background_color: str,
         surface_color: str,
@@ -340,21 +358,23 @@
         light_background_color: str,
         light_surface_color: str,
         document_type: str,
         ignore: str,
         extend: str,
         output: str,
         root: str,
+        doc_version: str,
 ):
     """
     This command generates documentation for a project by first creating Markdown
     files and then converting them to HTML files.
     """
+    user_template = get_user_template_path(templates_folder)
     env = Environment(
-        loader=FileSystemLoader(templates_folder),
+        loader=FileSystemLoader(user_template if user_template else templates_folder),
         autoescape=select_autoescape()
     )
     template = env.get_template('index.html')
     generate_md_files(docs, document_type, ignore, extend, output)
     if root is None:
         root = path.join(getcwd(), output, docs)
 
@@ -383,14 +403,15 @@
                         {
                             "title": "Github",
                             "icon": "fab fa-github",
                             "show_text": True,
                             "url": "https://github.com/hapticx/hapdoc"
                         },
                     ]},
+                    docVersion=doc_version,
                     accentColor=accent_color,
                     backgroundColor=background_color,
                     surfaceColor=surface_color,
                     lightAccentColor=light_accent_color,
                     lightBackgroundColor=light_background_color,
                     lightSurfaceColor=light_surface_color,
                     selected=f'{root}{filename[:-len(extension)]}.html'.replace('\\', '/')
```

### Comparing `hapdoc-1.9.2/hapdoc/md/__init__.py` & `hapdoc-1.9.4/hapdoc/md/__init__.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/hapdoc/templates/vitepress/index.html` & `hapdoc-1.9.4/hapdoc/templates/vitepress/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,18 @@
 <body class="dark:bg-surface-color bg-light-surface-color dark:text-white text-black overflow-x-hidden">
   <div class="w-screen min-h-screen h-full flex">
     <div
       id="header"
       class="w-full h-14 xl:h-12 rounded-b-xl xl:rounded-none fixed left-0 z-50 top-0 px-5 xl:pl-44 xl:pr-80 flex justify-between items-center transition-all"
     >
       <i class="fas fa-bars text-xl block xl:hidden" id="sandwich"></i>
-      <div class="text-2xl">{{ title }}</div>
+      <div class="flex items-end gap-2 text-2xl">
+        <p>{{ title }}</p>
+        <p class="text-base">v{{ docVersion }}</p>
+      </div>
       <div class="flex gap-2">
         {% for link in nav.links %}
           <a href="{{ link.url }}" class="flex items-center gap-2 select-none dark:hover:text-accent-color hover:text-lightaccent-color transition-all duration-300" alt="{{ link.title }}"> 
             {% if link.title %}
               <p> {{ link.title }} </p>
             {% endif %}
             <i class="{{ link.icon }}"></i>
@@ -57,15 +60,15 @@
           </div>
           <p id="themeString" class="w-16">Dark</p>
         </div>
       </div>
     </div>
     <!-- SideBar (desktop) -->
     <div class="hidden xl:block xl:fixed left-0 top-12 flex flex-col w-3/12 z-40 dark:bg-surface-color bg-light-surface-color min-h-screen h-full">
-      <div class="ml-36 pt-2 mr-2 border-t-[1px] border-white border-opacity-10 border-t-[1px]" id="line"></div>
+      <div class="ml-36 pt-2 mr-2 border-t-[1px] dark:border-white/10 border-black/10 border-t-[1px]" id="line"></div>
       <div class="flex flex-col gap-2 pl-32 h-full">
         {% macro sidebar(key, item) %}
           <!-- SideBar item -->
           <div class="flex flex-col gap-2 border-white border-opacity-10 mt-2">
             <div class="flex pl-2 flex-col w-full font-bold">
               {% if item._items %}
                 <div class="flex w-full items-center gap-2 cursor-pointer" onclick="toggleList('{{ item._data.id }}')">
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 
 
 
 
 {{ title }}
+v{{ docVersion }}
 {% for link in nav.links %}
 {%_if_link.title_%}
 {{_link.title_}}
 {%_endif_%}
  {% endfor %}
 Dark
 {% macro sidebar(key, item) %}
```

### Comparing `hapdoc-1.9.2/hapdoc/utils.py` & `hapdoc-1.9.4/hapdoc/utils.py`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/hapdoc.egg-info/PKG-INFO` & `hapdoc-1.9.4/hapdoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapdoc
-Version: 1.9.2
+Version: 1.9.4
 Summary: autodoc tool for everything
 Home-page: https://github.com/HapticX/hapdoc
 Author: Ethosa
 Author-email: social.ethosa@gmail.com
 Maintainer: HapticX
 Maintainer-email: hapticx.company@gmail.com
 License: MIT
```

### Comparing `hapdoc-1.9.2/hapdoc.egg-info/SOURCES.txt` & `hapdoc-1.9.4/hapdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hapdoc-1.9.2/setup.py` & `hapdoc-1.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ethosa',
     author_email='social.ethosa@gmail.com',
     maintainer='HapticX',
     maintainer_email='hapticx.company@gmail.com',
     url='https://github.com/HapticX/hapdoc',
-    version='1.9.2',
+    version='1.9.4',
     packages=find_packages(),
     py_modules=['hapdoc'],
-    install_requires=['click', 'colorama', 'fastapi', 'uvicorn', 'jinja2'],
+    install_requires=['click', 'fastapi', 'uvicorn', 'jinja2'],
     package_data={
         'hapdoc': ['*.html']
     },
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'hapdoc = hapdoc.hapdoc:hapdoc'
```

