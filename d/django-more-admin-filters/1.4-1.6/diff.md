# Comparing `tmp/django-more-admin-filters-1.4.tar.gz` & `tmp/django-more-admin-filters-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-more-admin-filters-1.4.tar", last modified: Sun Feb 12 21:12:27 2023, max compression
+gzip compressed data, was "django-more-admin-filters-1.6.tar", last modified: Fri Apr  7 20:38:06 2023, max compression
```

## Comparing `django-more-admin-filters-1.4.tar` & `django-more-admin-filters-1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2020-09-04 13:10:12.000000 django-more-admin-filters-1.4/LICENSE
--rw-r--r--   0 thomas    (1000) thomas    (1000)       84 2020-09-05 09:10:25.000000 django-more-admin-filters-1.4/MANIFEST.in
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5033 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3066 2023-02-12 20:54:52.000000 django-more-admin-filters-1.4/README.rst
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/django_more_admin_filters.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5033 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/django_more_admin_filters.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)      596 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/django_more_admin_filters.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/django_more_admin_filters.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       17 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/django_more_admin_filters.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       19 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/django_more_admin_filters.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2020-09-05 09:15:06.000000 django-more-admin-filters-1.4/django_more_admin_filters.egg-info/zip-safe
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/more_admin_filters/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      284 2023-02-12 20:36:36.000000 django-more-admin-filters-1.4/more_admin_filters/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      661 2023-02-12 20:55:37.000000 django-more-admin-filters-1.4/more_admin_filters/__version__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      116 2021-07-16 10:17:35.000000 django-more-admin-filters-1.4/more_admin_filters/apps.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14116 2023-02-12 20:36:36.000000 django-more-admin-filters-1.4/more_admin_filters/filters.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/more_admin_filters/templates/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/more_admin_filters/templates/more_admin_filters/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      962 2020-09-05 11:29:15.000000 django-more-admin-filters-1.4/more_admin_filters/templates/more_admin_filters/dropdownfilter.html
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1909 2020-09-05 11:29:18.000000 django-more-admin-filters-1.4/more_admin_filters/templates/more_admin_filters/multiselectdropdownfilter.html
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-02-12 21:12:27.000000 django-more-admin-filters-1.4/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2164 2023-02-12 20:40:42.000000 django-more-admin-filters-1.4/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2020-09-04 13:10:12.000000 django-more-admin-filters-1.6/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       84 2020-09-05 09:10:25.000000 django-more-admin-filters-1.6/MANIFEST.in
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4473 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3127 2023-04-07 13:11:30.000000 django-more-admin-filters-1.6/README.rst
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.612347 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4473 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      596 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       17 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       19 2023-04-07 20:38:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2020-09-05 09:15:06.000000 django-more-admin-filters-1.6/django_more_admin_filters.egg-info/zip-safe
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/more_admin_filters/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      284 2023-02-12 20:36:36.000000 django-more-admin-filters-1.6/more_admin_filters/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      661 2023-04-07 20:37:08.000000 django-more-admin-filters-1.6/more_admin_filters/__version__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      116 2021-07-16 10:17:35.000000 django-more-admin-filters-1.6/more_admin_filters/apps.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14116 2023-02-12 20:36:36.000000 django-more-admin-filters-1.6/more_admin_filters/filters.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.612347 django-more-admin-filters-1.6/more_admin_filters/templates/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      962 2020-09-05 11:29:15.000000 django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/dropdownfilter.html
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1909 2020-09-05 11:29:18.000000 django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/multiselectdropdownfilter.html
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-04-07 20:38:06.616347 django-more-admin-filters-1.6/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2252 2023-04-07 13:55:38.000000 django-more-admin-filters-1.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-more-admin-filters-1.4/LICENSE` & `django-more-admin-filters-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-more-admin-filters-1.4/PKG-INFO` & `django-more-admin-filters-1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,120 +1,123 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-more-admin-filters
-Version: 1.4
+Version: 1.6
 Summary: Additional filters for django-admin.
 Home-page: https://github.com/thomst/django-more-admin-filters
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
-Description: ====================================
-        Welcome to django-more-admin-filters
-        ====================================
-        
-        .. image:: https://github.com/thomst/django-more-admin-filters/actions/workflows/ci.yml/badge.svg
-            :target: https://github.com/thomst/django-more-admin-filters/actions/workflows/ci.yml
-            :alt: Run tests for django-more-admin-filters
-        
-        .. image:: https://coveralls.io/repos/github/thomst/django-more-admin-filters/badge.svg?branch=master
-            :target: https://coveralls.io/github/thomst/django-more-admin-filters?branch=master
-            :alt: coveralls badge
-        
-        .. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-           :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-           :alt: python: 3.6, 3.7, 3.8, 3.9
-        
-        .. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0-orange
-           :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0-orange
-           :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0
-        
-        
-        Description
-        ===========
-        Django-more-admin-filters is a collection of django admin filters with a focus
-        on filters using dropdown widgets, multiple choice filters and filters working
-        with annotated attributes.
-        
-        
-        Installation
-        ============
-        Install from pypi.org::
-        
-            pip install django-more-admin-filters
-        
-        Add more_admin_filters to your installed apps::
-        
-            INSTALLED_APPS = [
-                'more_admin_filters',
-                ...
-            ]
-        
-        Use the filter classes with your ModelAdmin::
-        
-            from more_admin_filters import MultiSelectDropdownFilter
-        
-            class MyModelAdmin(admin.ModelAdmin):
-                ...
-                list_filter = [
-                    ('myfield', MultiSelectDropdownFilter),
-                    ...
-                ]
-        
-        Since the ModelAdmin routine to initialize the list filters doesn't work with
-        annotated attributes the usage for an annotation filter is a little bit special.
-        The filter class needs to be equipped with the attribute's name::
-        
-            MyModelAdmin(admin.ModelAdmin):
-            list_filter = [
-                BooleanAnnotationFilter.init('my_annotated_attribute'),
-                ...
-            ]
-        
-        
-        Filter classes
-        ==============
-        
-        * **DropdownFilter**
-            Dropdown filter for all kind of fields.
-        * **ChoicesDropdownFilter**
-            Dropdown filter for fields using choices.
-        * **RelatedDropdownFilter**
-            Dropdown filter for relation fields.
-        * **RelatedOnlyDropdownFilter**
-            Dropdown filter for relation fields using limit_choices_to.
-        * **MultiSelectFilter**
-            Multi select filter for all kind of fields.
-        * **MultiSelectRelatedFilter**
-            Multi select filter for relation fields.
-        * **MultiSelectRelatedOnlyFilter**
-            Multi select filter for related fields with choices limited to the objects
-            involved in that relation
-        * **MultiSelectDropdownFilter**
-            Multi select dropdown filter for all kind of fields.
-        * **MultiSelectRelatedDropdownFilter**
-            Multi select dropdown filter for relation fields.
-        * **BooleanAnnotationFilter**
-            Filter for annotated boolean-attributes.
-        
-        
-        .. note:: More kind of annotation filters will be added in future versions.
-        
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+License-File: LICENSE
+
+====================================
+Welcome to django-more-admin-filters
+====================================
+
+.. image:: https://github.com/thomst/django-more-admin-filters/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thomst/django-more-admin-filters/actions/workflows/ci.yml
+    :alt: Run tests for django-more-admin-filters
+
+.. image:: https://coveralls.io/repos/github/thomst/django-more-admin-filters/badge.svg?branch=master
+    :target: https://coveralls.io/github/thomst/django-more-admin-filters?branch=master
+    :alt: coveralls badge
+
+.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10
+
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
+
+
+Description
+===========
+Django-more-admin-filters is a collection of django admin filters with a focus
+on filters using dropdown widgets, multiple choice filters and filters working
+with annotated attributes.
+
+
+Installation
+============
+Install from pypi.org::
+
+    pip install django-more-admin-filters
+
+Add more_admin_filters to your installed apps::
+
+    INSTALLED_APPS = [
+        'more_admin_filters',
+        ...
+    ]
+
+Use the filter classes with your ModelAdmin::
+
+    from more_admin_filters import MultiSelectDropdownFilter
+
+    class MyModelAdmin(admin.ModelAdmin):
+        ...
+        list_filter = [
+            ('myfield', MultiSelectDropdownFilter),
+            ...
+        ]
+
+Since the ModelAdmin routine to initialize the list filters doesn't work with
+annotated attributes the usage for an annotation filter is a little bit special.
+The filter class needs to be equipped with the attribute's name::
+
+    MyModelAdmin(admin.ModelAdmin):
+    list_filter = [
+        BooleanAnnotationFilter.init('my_annotated_attribute'),
+        ...
+    ]
+
+
+Filter classes
+==============
+
+* **DropdownFilter**
+    Dropdown filter for all kind of fields.
+* **ChoicesDropdownFilter**
+    Dropdown filter for fields using choices.
+* **RelatedDropdownFilter**
+    Dropdown filter for relation fields.
+* **RelatedOnlyDropdownFilter**
+    Dropdown filter for relation fields using limit_choices_to.
+* **MultiSelectFilter**
+    Multi select filter for all kind of fields.
+* **MultiSelectRelatedFilter**
+    Multi select filter for relation fields.
+* **MultiSelectRelatedOnlyFilter**
+    Multi select filter for related fields with choices limited to the objects
+    involved in that relation
+* **MultiSelectDropdownFilter**
+    Multi select dropdown filter for all kind of fields.
+* **MultiSelectRelatedDropdownFilter**
+    Multi select dropdown filter for relation fields.
+* **BooleanAnnotationFilter**
+    Filter for annotated boolean-attributes.
+
+
+.. note:: More kind of annotation filters will be added in future versions.
```

### Comparing `django-more-admin-filters-1.4/README.rst` & `django-more-admin-filters-1.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     :target: https://github.com/thomst/django-more-admin-filters/actions/workflows/ci.yml
     :alt: Run tests for django-more-admin-filters
 
 .. image:: https://coveralls.io/repos/github/thomst/django-more-admin-filters/badge.svg?branch=master
     :target: https://coveralls.io/github/thomst/django-more-admin-filters?branch=master
     :alt: coveralls badge
 
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-   :alt: python: 3.6, 3.7, 3.8, 3.9
+.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10
 
-.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0-orange
-   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0-orange
-   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
 
 
 Description
 ===========
 Django-more-admin-filters is a collection of django admin filters with a focus
 on filters using dropdown widgets, multiple choice filters and filters working
 with annotated attributes.
```

### Comparing `django-more-admin-filters-1.4/django_more_admin_filters.egg-info/PKG-INFO` & `django-more-admin-filters-1.6/django_more_admin_filters.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,120 +1,123 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-more-admin-filters
-Version: 1.4
+Version: 1.6
 Summary: Additional filters for django-admin.
 Home-page: https://github.com/thomst/django-more-admin-filters
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
-Description: ====================================
-        Welcome to django-more-admin-filters
-        ====================================
-        
-        .. image:: https://github.com/thomst/django-more-admin-filters/actions/workflows/ci.yml/badge.svg
-            :target: https://github.com/thomst/django-more-admin-filters/actions/workflows/ci.yml
-            :alt: Run tests for django-more-admin-filters
-        
-        .. image:: https://coveralls.io/repos/github/thomst/django-more-admin-filters/badge.svg?branch=master
-            :target: https://coveralls.io/github/thomst/django-more-admin-filters?branch=master
-            :alt: coveralls badge
-        
-        .. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-           :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue
-           :alt: python: 3.6, 3.7, 3.8, 3.9
-        
-        .. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0-orange
-           :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0-orange
-           :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0
-        
-        
-        Description
-        ===========
-        Django-more-admin-filters is a collection of django admin filters with a focus
-        on filters using dropdown widgets, multiple choice filters and filters working
-        with annotated attributes.
-        
-        
-        Installation
-        ============
-        Install from pypi.org::
-        
-            pip install django-more-admin-filters
-        
-        Add more_admin_filters to your installed apps::
-        
-            INSTALLED_APPS = [
-                'more_admin_filters',
-                ...
-            ]
-        
-        Use the filter classes with your ModelAdmin::
-        
-            from more_admin_filters import MultiSelectDropdownFilter
-        
-            class MyModelAdmin(admin.ModelAdmin):
-                ...
-                list_filter = [
-                    ('myfield', MultiSelectDropdownFilter),
-                    ...
-                ]
-        
-        Since the ModelAdmin routine to initialize the list filters doesn't work with
-        annotated attributes the usage for an annotation filter is a little bit special.
-        The filter class needs to be equipped with the attribute's name::
-        
-            MyModelAdmin(admin.ModelAdmin):
-            list_filter = [
-                BooleanAnnotationFilter.init('my_annotated_attribute'),
-                ...
-            ]
-        
-        
-        Filter classes
-        ==============
-        
-        * **DropdownFilter**
-            Dropdown filter for all kind of fields.
-        * **ChoicesDropdownFilter**
-            Dropdown filter for fields using choices.
-        * **RelatedDropdownFilter**
-            Dropdown filter for relation fields.
-        * **RelatedOnlyDropdownFilter**
-            Dropdown filter for relation fields using limit_choices_to.
-        * **MultiSelectFilter**
-            Multi select filter for all kind of fields.
-        * **MultiSelectRelatedFilter**
-            Multi select filter for relation fields.
-        * **MultiSelectRelatedOnlyFilter**
-            Multi select filter for related fields with choices limited to the objects
-            involved in that relation
-        * **MultiSelectDropdownFilter**
-            Multi select dropdown filter for all kind of fields.
-        * **MultiSelectRelatedDropdownFilter**
-            Multi select dropdown filter for relation fields.
-        * **BooleanAnnotationFilter**
-            Filter for annotated boolean-attributes.
-        
-        
-        .. note:: More kind of annotation filters will be added in future versions.
-        
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+License-File: LICENSE
+
+====================================
+Welcome to django-more-admin-filters
+====================================
+
+.. image:: https://github.com/thomst/django-more-admin-filters/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thomst/django-more-admin-filters/actions/workflows/ci.yml
+    :alt: Run tests for django-more-admin-filters
+
+.. image:: https://coveralls.io/repos/github/thomst/django-more-admin-filters/badge.svg?branch=master
+    :target: https://coveralls.io/github/thomst/django-more-admin-filters?branch=master
+    :alt: coveralls badge
+
+.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :target: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue
+   :alt: python: 3.6, 3.7, 3.8, 3.9, 3.10
+
+.. image:: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :target: https://img.shields.io/badge/django-2.2%20%7C%203.0%20%7C%203.1%20%7C%203.2%20%7C%204.0%20%7C%204.1-orange
+   :alt: django: 2.2, 3.0, 3.1, 3.2, 4.0, 4.1
+
+
+Description
+===========
+Django-more-admin-filters is a collection of django admin filters with a focus
+on filters using dropdown widgets, multiple choice filters and filters working
+with annotated attributes.
+
+
+Installation
+============
+Install from pypi.org::
+
+    pip install django-more-admin-filters
+
+Add more_admin_filters to your installed apps::
+
+    INSTALLED_APPS = [
+        'more_admin_filters',
+        ...
+    ]
+
+Use the filter classes with your ModelAdmin::
+
+    from more_admin_filters import MultiSelectDropdownFilter
+
+    class MyModelAdmin(admin.ModelAdmin):
+        ...
+        list_filter = [
+            ('myfield', MultiSelectDropdownFilter),
+            ...
+        ]
+
+Since the ModelAdmin routine to initialize the list filters doesn't work with
+annotated attributes the usage for an annotation filter is a little bit special.
+The filter class needs to be equipped with the attribute's name::
+
+    MyModelAdmin(admin.ModelAdmin):
+    list_filter = [
+        BooleanAnnotationFilter.init('my_annotated_attribute'),
+        ...
+    ]
+
+
+Filter classes
+==============
+
+* **DropdownFilter**
+    Dropdown filter for all kind of fields.
+* **ChoicesDropdownFilter**
+    Dropdown filter for fields using choices.
+* **RelatedDropdownFilter**
+    Dropdown filter for relation fields.
+* **RelatedOnlyDropdownFilter**
+    Dropdown filter for relation fields using limit_choices_to.
+* **MultiSelectFilter**
+    Multi select filter for all kind of fields.
+* **MultiSelectRelatedFilter**
+    Multi select filter for relation fields.
+* **MultiSelectRelatedOnlyFilter**
+    Multi select filter for related fields with choices limited to the objects
+    involved in that relation
+* **MultiSelectDropdownFilter**
+    Multi select dropdown filter for all kind of fields.
+* **MultiSelectRelatedDropdownFilter**
+    Multi select dropdown filter for relation fields.
+* **BooleanAnnotationFilter**
+    Filter for annotated boolean-attributes.
+
+
+.. note:: More kind of annotation filters will be added in future versions.
```

### Comparing `django-more-admin-filters-1.4/django_more_admin_filters.egg-info/SOURCES.txt` & `django-more-admin-filters-1.6/django_more_admin_filters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-more-admin-filters-1.4/more_admin_filters/__version__.py` & `django-more-admin-filters-1.6/more_admin_filters/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 internal code changes that do not affect the API. Development versions are
 incomplete states of a release .
 
 Version 0.x should be considered a development version with an unstable API,
 and backwards compatibility is not guaranteed for minor versions.
 """
 
-__version__ = "1.4"
+__version__ = "1.6"
```

### Comparing `django-more-admin-filters-1.4/more_admin_filters/filters.py` & `django-more-admin-filters-1.6/more_admin_filters/filters.py`

 * *Files identical despite different names*

### Comparing `django-more-admin-filters-1.4/more_admin_filters/templates/more_admin_filters/dropdownfilter.html` & `django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/dropdownfilter.html`

 * *Files identical despite different names*

### Comparing `django-more-admin-filters-1.4/more_admin_filters/templates/more_admin_filters/multiselectdropdownfilter.html` & `django-more-admin-filters-1.6/more_admin_filters/templates/more_admin_filters/multiselectdropdownfilter.html`

 * *Files identical despite different names*

### Comparing `django-more-admin-filters-1.4/setup.py` & `django-more-admin-filters-1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,33 +38,35 @@
     author_email="thomas.leichtfuss@posteo.de",
     url="https://github.com/thomst/django-more-admin-filters",
     license="BSD License",
     platforms=["OS Independent"],
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
     install_requires=[
-        "Django>=2.2,<4.1",
+        "Django>=2.2,<4.2",
     ],
     classifiers=[
         dev_status,
         "Framework :: Django",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
     ],
     zip_safe=True,
 )
```

