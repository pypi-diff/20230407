# Comparing `tmp/init_problem-0.3.8.tar.gz` & `tmp/init_problem-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "init_problem-0.3.8.tar", max compression
+gzip compressed data, was "init_problem-0.3.9.tar", max compression
```

## Comparing `init_problem-0.3.8.tar` & `init_problem-0.3.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-03-07 06:55:36.580031 init_problem-0.3.8/README.md
--rw-r--r--   0        0        0        0 2023-03-07 06:55:36.579965 init_problem-0.3.8/init_problem/__init__.py
--rw-r--r--   0        0        0       54 2023-03-07 07:04:56.685861 init_problem-0.3.8/init_problem/__main__.py
--rw-r--r--   0        0        0     1149 2023-03-09 06:00:45.501064 init_problem-0.3.8/init_problem/chapters.py
--rw-r--r--   0        0        0     1236 2023-03-07 07:03:44.750369 init_problem-0.3.8/init_problem/choice_option.py
--rw-r--r--   0        0        0     4266 2023-04-03 16:55:50.369882 init_problem-0.3.8/init_problem/main.py
--rw-r--r--   0        0        0     2912 2023-03-09 05:56:37.209420 init_problem-0.3.8/init_problem/problem.py
--rw-r--r--   0        0        0      412 2023-04-03 16:56:30.236425 init_problem-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 init_problem-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-07 06:55:36.580031 init_problem-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-07 06:55:36.579965 init_problem-0.3.9/init_problem/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-07 07:04:56.685861 init_problem-0.3.9/init_problem/__main__.py
+-rw-r--r--   0        0        0     1149 2023-03-09 06:00:45.501064 init_problem-0.3.9/init_problem/chapters.py
+-rw-r--r--   0        0        0     1236 2023-03-07 07:03:44.750369 init_problem-0.3.9/init_problem/choice_option.py
+-rw-r--r--   0        0        0     4327 2023-04-05 12:05:00.706646 init_problem-0.3.9/init_problem/main.py
+-rw-r--r--   0        0        0     2912 2023-03-09 05:56:37.209420 init_problem-0.3.9/init_problem/problem.py
+-rw-r--r--   0        0        0      405 2023-04-05 12:05:31.911646 init_problem-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      319 1970-01-01 00:00:00.000000 init_problem-0.3.9/PKG-INFO
```

### Comparing `init_problem-0.3.8/init_problem/chapters.py` & `init_problem-0.3.9/init_problem/chapters.py`

 * *Files identical despite different names*

### Comparing `init_problem-0.3.8/init_problem/choice_option.py` & `init_problem-0.3.9/init_problem/choice_option.py`

 * *Files identical despite different names*

### Comparing `init_problem-0.3.8/init_problem/main.py` & `init_problem-0.3.9/init_problem/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     path_problem= os.path.join(
             problem.path_problem_format(),
             f'problem-{problem_number:02}'
             )
 
 
     os.makedirs(path_problem, exist_ok=True)
+    os.makedirs(f'{path_problem}/downloads', exist_ok=True) 
     main_tex = os.path.join(path_problem, 'main.tex')
     with open(main_tex, 'w') as file:
         file.write(f'\\documentclass{{article}}\n')
         file.write(f'\\usepackage{{v-problem}}\n')
         if size == 'square':
             file.write(size_square)
         elif size == 'h-rectangle':
```

### Comparing `init_problem-0.3.8/init_problem/problem.py` & `init_problem-0.3.9/init_problem/problem.py`

 * *Files identical despite different names*

