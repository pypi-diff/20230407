# Comparing `tmp/django-aux-0.0.8.tar.gz` & `tmp/django-aux-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-aux-0.0.8.tar", last modified: Wed Jul  6 13:08:02 2022, max compression
+gzip compressed data, was "django-aux-0.0.9.tar", last modified: Wed Jul  6 13:38:58 2022, max compression
```

## Comparing `django-aux-0.0.8.tar` & `django-aux-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-07-06 13:08:02.864881 django-aux-0.0.8/
--rw-rw-rw-   0        0        0     1090 2022-07-05 14:54:23.000000 django-aux-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      143 2022-07-05 21:15:46.000000 django-aux-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2022-07-06 13:08:02.865880 django-aux-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      112 2022-07-05 14:54:23.000000 django-aux-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-07-06 13:08:02.827884 django-aux-0.0.8/django_aux/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django-aux-0.0.8/django_aux/__init__.py
--rw-rw-rw-   0        0        0       66 2022-07-04 12:21:58.000000 django-aux-0.0.8/django_aux/admin.py
--rw-rw-rw-   0        0        0      157 2022-07-04 12:21:58.000000 django-aux-0.0.8/django_aux/apps.py
--rw-rw-rw-   0        0        0     7360 2022-07-06 12:31:42.000000 django-aux-0.0.8/django_aux/columns.py
--rw-rw-rw-   0        0        0      389 2022-07-06 13:07:44.000000 django-aux-0.0.8/django_aux/decorators.py
--rw-rw-rw-   0        0        0     4365 2022-07-06 12:30:45.000000 django-aux-0.0.8/django_aux/filters.py
-drwxrwxrwx   0        0        0        0 2022-07-06 13:08:02.853878 django-aux-0.0.8/django_aux/migrations/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django-aux-0.0.8/django_aux/migrations/__init__.py
--rw-rw-rw-   0        0        0     2341 2022-07-06 12:27:03.000000 django-aux-0.0.8/django_aux/models.py
-drwxrwxrwx   0        0        0        0 2022-07-06 13:08:02.855882 django-aux-0.0.8/django_aux/static/
--rw-rw-rw-   0        0        0     2647 2022-07-04 12:21:58.000000 django-aux-0.0.8/django_aux/static/main.css
-drwxrwxrwx   0        0        0        0 2022-07-06 13:08:02.797878 django-aux-0.0.8/django_aux/templates/
-drwxrwxrwx   0        0        0        0 2022-07-06 13:08:02.860879 django-aux-0.0.8/django_aux/templates/django_aux/
--rw-rw-rw-   0        0        0     7346 2022-07-05 21:35:24.000000 django-aux-0.0.8/django_aux/templates/django_aux/base.html
--rw-rw-rw-   0        0        0     2082 2022-07-05 22:03:29.000000 django-aux-0.0.8/django_aux/templates/django_aux/standard.html
-drwxrwxrwx   0        0        0        0 2022-07-06 13:08:02.863879 django-aux-0.0.8/django_aux/templatetags/
--rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django-aux-0.0.8/django_aux/templatetags/__init__.py
--rw-rw-rw-   0        0        0      645 2022-07-04 12:21:58.000000 django-aux-0.0.8/django_aux/templatetags/aux_tags.py
--rw-rw-rw-   0        0        0       63 2022-07-04 12:21:58.000000 django-aux-0.0.8/django_aux/tests.py
--rw-rw-rw-   0        0        0       56 2022-07-05 21:41:23.000000 django-aux-0.0.8/django_aux/urls.py
--rw-rw-rw-   0        0        0    12848 2022-07-06 12:30:20.000000 django-aux-0.0.8/django_aux/views.py
-drwxrwxrwx   0        0        0        0 2022-07-06 13:08:02.851876 django-aux-0.0.8/django_aux.egg-info/
--rw-rw-rw-   0        0        0     1101 2022-07-06 13:08:02.000000 django-aux-0.0.8/django_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      664 2022-07-06 13:08:02.000000 django-aux-0.0.8/django_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-06 13:08:02.000000 django-aux-0.0.8/django_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2022-07-06 13:08:02.000000 django-aux-0.0.8/django_aux.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-07-06 13:08:02.000000 django-aux-0.0.8/django_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2022-07-05 14:54:23.000000 django-aux-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1157 2022-07-06 13:08:02.868877 django-aux-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-07-05 14:54:23.000000 django-aux-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.748368 django-aux-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2022-07-05 14:54:23.000000 django-aux-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      143 2022-07-05 21:15:46.000000 django-aux-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2022-07-06 13:38:58.748368 django-aux-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2022-07-05 14:54:23.000000 django-aux-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.723368 django-aux-0.0.9/django_aux/
+-rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/__init__.py
+-rw-rw-rw-   0        0        0       66 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/admin.py
+-rw-rw-rw-   0        0        0      157 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/apps.py
+-rw-rw-rw-   0        0        0     7360 2022-07-06 12:31:42.000000 django-aux-0.0.9/django_aux/columns.py
+-rw-rw-rw-   0        0        0      389 2022-07-06 13:07:44.000000 django-aux-0.0.9/django_aux/decorators.py
+-rw-rw-rw-   0        0        0     4365 2022-07-06 12:30:45.000000 django-aux-0.0.9/django_aux/filters.py
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.742367 django-aux-0.0.9/django_aux/migrations/
+-rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2371 2022-07-06 13:33:21.000000 django-aux-0.0.9/django_aux/models.py
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.743368 django-aux-0.0.9/django_aux/static/
+-rw-rw-rw-   0        0        0     2647 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/static/main.css
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.706367 django-aux-0.0.9/django_aux/templates/
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.745367 django-aux-0.0.9/django_aux/templates/django_aux/
+-rw-rw-rw-   0        0        0     7346 2022-07-05 21:35:24.000000 django-aux-0.0.9/django_aux/templates/django_aux/base.html
+-rw-rw-rw-   0        0        0     2082 2022-07-05 22:03:29.000000 django-aux-0.0.9/django_aux/templates/django_aux/standard.html
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.747367 django-aux-0.0.9/django_aux/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      645 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/templatetags/aux_tags.py
+-rw-rw-rw-   0        0        0       63 2022-07-04 12:21:58.000000 django-aux-0.0.9/django_aux/tests.py
+-rw-rw-rw-   0        0        0       56 2022-07-05 21:41:23.000000 django-aux-0.0.9/django_aux/urls.py
+-rw-rw-rw-   0        0        0    13049 2022-07-06 13:38:15.000000 django-aux-0.0.9/django_aux/views.py
+drwxrwxrwx   0        0        0        0 2022-07-06 13:38:58.741367 django-aux-0.0.9/django_aux.egg-info/
+-rw-rw-rw-   0        0        0     1101 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      664 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-07-06 13:38:58.000000 django-aux-0.0.9/django_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2022-07-05 14:54:23.000000 django-aux-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1196 2022-07-06 13:38:58.749368 django-aux-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-07-05 14:54:23.000000 django-aux-0.0.9/setup.py
```

### Comparing `django-aux-0.0.8/LICENSE` & `django-aux-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-aux-0.0.8/PKG-INFO` & `django-aux-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-aux
-Version: 0.0.8
+Version: 0.0.9
 Summary: Useful Mixins for Django Projects
 Home-page: https://github.com/JordanHyatt
 Author: Jordan Hyatt
 Author-email: jordan.hyatt@auxiliasystems.com
 License: MIT  # Example license
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-aux-0.0.8/django_aux/columns.py` & `django-aux-0.0.9/django_aux/columns.py`

 * *Files identical despite different names*

### Comparing `django-aux-0.0.8/django_aux/filters.py` & `django-aux-0.0.9/django_aux/filters.py`

 * *Files identical despite different names*

### Comparing `django-aux-0.0.8/django_aux/models.py` & `django-aux-0.0.9/django_aux/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db import models
 from django.core.exceptions import ValidationError
-
+from django.db.models import Q
 
 class CheckOverlapMixin:
     ''' 
         This mixin adds cleaning functionality to a model that will not allow a range overlap defined by two attributes.
         default behavior is to include the boundaries, but can be overwritten
     '''
     start_attr = '' # Name of the attr that starts the range (must be overwritten)
```

### Comparing `django-aux-0.0.8/django_aux/static/main.css` & `django-aux-0.0.9/django_aux/static/main.css`

 * *Files identical despite different names*

### Comparing `django-aux-0.0.8/django_aux/templates/django_aux/base.html` & `django-aux-0.0.9/django_aux/templates/django_aux/base.html`

 * *Files identical despite different names*

### Comparing `django-aux-0.0.8/django_aux/templates/django_aux/standard.html` & `django-aux-0.0.9/django_aux/templates/django_aux/standard.html`

 * *Files identical despite different names*

### Comparing `django-aux-0.0.8/django_aux/templatetags/aux_tags.py` & `django-aux-0.0.9/django_aux/templatetags/aux_tags.py`

 * *Files identical despite different names*

### Comparing `django-aux-0.0.8/django_aux/views.py` & `django-aux-0.0.9/django_aux/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from django.shortcuts import render
 from django_tables2 import SingleTableMixin
 from django.shortcuts import redirect
 from django.http import HttpResponseRedirect
-from pandas import isna
-
+from pandas import isna, DataFrame as DF, to_datetime
+import inspect
+from django.contrib import messages
+from django.db.models import F
+from django_pandas.io import read_frame
+import plotly.express as px
+from plotly import offline
 
 class SaveFilterMixin(SingleTableMixin):
     """ This Mixin Can be used with a FilterView SingleTable in order to save
     the users filter selections after navegating away from the lookup page"""
 
     def get(self, request, *args, **kwargs):
         view_name = self.__class__
@@ -215,15 +220,15 @@
 
         if color and color not in keep_vals:
             keep_vals.append(color)
         df = read_frame(qs.values(*keep_vals))
         if df.empty:
             self.plot_df = df
             return
-        df.dtg_ = pd.to_datetime(df.dtg_)
+        df.dtg_ = to_datetime(df.dtg_)
 
         period_dict = {
             'day': {'pcode': 'd', 'date_format': "%Y-%m-%d"},
             'week': {'pcode': 'W', 'date_format': "%Y-W%U"},
             'month': {'pcode': 'M', 'date_format': "%Y-%m"},
             'quarter': {'pcode': 'Q', 'date_format': "%Y-Q%q"},
             'year': {'pcode': 'Y', 'date_format': "%Y"},
@@ -288,15 +293,15 @@
             fig.update_xaxes(
                 tickvals=tvals,
                 tickformat=date_format,
             )
         fig.update_layout(
             xaxis_title=x_verbose, yaxis_title=y_verbose
         )
-        return plotly.offline.plot(fig, auto_open=False, output_type="div")
+        return offline.plot(fig, auto_open=False, output_type="div")
 
     def get_filterset_kwargs(self, filterset_class):
         kwargs = super().get_filterset_kwargs(filterset_class)
         choices = dict(
             X_CHOICES=[('year', 'Year'), ('quarter', 'Quarter'),
                        ('month', 'Month'), ('week', 'Week'), ('day', 'Day'), ],
             Y_CHOICES=[],
```

### Comparing `django-aux-0.0.8/django_aux.egg-info/PKG-INFO` & `django-aux-0.0.9/django_aux.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-aux
-Version: 0.0.8
+Version: 0.0.9
 Summary: Useful Mixins for Django Projects
 Home-page: https://github.com/JordanHyatt
 Author: Jordan Hyatt
 Author-email: jordan.hyatt@auxiliasystems.com
 License: MIT  # Example license
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-aux-0.0.8/django_aux.egg-info/SOURCES.txt` & `django-aux-0.0.9/django_aux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-aux-0.0.8/setup.cfg` & `django-aux-0.0.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6175 780d 0a76   = django-aux..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e38 0d0a  ersion = 0.0.8..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e39 0d0a  ersion = 0.0.9..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 5573  description = Us
 00000040: 6566 756c 204d 6978 696e 7320 666f 7220  eful Mixins for 
 00000050: 446a 616e 676f 2050 726f 6a65 6374 730d  Django Projects.
 00000060: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000070: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
 00000080: 2e6d 640d 0a75 726c 203d 2068 7474 7073  .md..url = https
 00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a6f  ://github.com/Jo
@@ -63,11 +63,13 @@
 000003e0: 300d 0a09 6e75 6d70 7920 3e3d 2031 2e32  0...numpy >= 1.2
 000003f0: 300d 0a09 646a 616e 676f 2d62 6f6f 7473  0...django-boots
 00000400: 7472 6170 2d64 6174 6570 6963 6b65 722d  trap-datepicker-
 00000410: 706c 7573 203e 3d20 332e 300d 0a09 646a  plus >= 3.0...dj
 00000420: 616e 676f 2d63 7269 7370 792d 666f 726d  ango-crispy-form
 00000430: 7320 3e3d 2031 2e31 342e 300d 0a09 646a  s >= 1.14.0...dj
 00000440: 616e 676f 2d62 6f6f 7473 7472 6170 3420  ango-bootstrap4 
-00000450: 3e3d 2032 312e 300d 0a0d 0a5b 6567 675f  >= 21.0....[egg_
-00000460: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000470: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000480: 300d 0a0d 0a                             0....
+00000450: 3e3d 2032 312e 300d 0a09 646a 616e 676f  >= 21.0...django
+00000460: 2d70 616e 6461 7320 3e3d 2030 2e36 0d0a  -pandas >= 0.6..
+00000470: 0970 6c6f 746c 7920 3e3d 2035 2e30 0d0a  .plotly >= 5.0..
+00000480: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000490: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000004a0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

