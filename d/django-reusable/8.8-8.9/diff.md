# Comparing `tmp/django-reusable-8.8.tar.gz` & `tmp/django-reusable-8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-reusable-8.8.tar", last modified: Tue Feb 28 06:06:56 2023, max compression
+gzip compressed data, was "dist/django-reusable-8.9.tar", last modified: Fri Apr  7 20:44:25 2023, max compression
```

## Comparing `django-reusable-8.8.tar` & `django-reusable-8.9.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/
--rw-r--r--   0 narangwa   (501) staff       (20)       90 2022-04-27 23:42:19.000000 django-reusable-8.8/AUTHORS
--rw-r--r--   0 narangwa   (501) staff       (20)     2952 2022-04-27 23:43:03.000000 django-reusable-8.8/COPYING
--rw-r--r--   0 narangwa   (501) staff       (20)      121 2022-06-29 20:32:10.000000 django-reusable-8.8/MANIFEST.in
--rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-02-28 06:06:56.000000 django-reusable-8.8/PKG-INFO
--rw-r--r--   0 narangwa   (501) staff       (20)      399 2022-05-12 17:29:25.000000 django-reusable-8.8/README.md
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/
--rw-r--r--   0 narangwa   (501) staff       (20)      397 2022-09-19 22:17:44.000000 django-reusable-8.8/django_reusable/__init__.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/admin/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:06:59.000000 django-reusable-8.8/django_reusable/admin/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1830 2022-09-19 20:52:10.000000 django-reusable-8.8/django_reusable/admin/actions.py
--rw-r--r--   0 narangwa   (501) staff       (20)      613 2022-09-19 20:52:10.000000 django-reusable-8.8/django_reusable/admin/filters.py
--rw-r--r--   0 narangwa   (501) staff       (20)    13625 2022-12-06 19:00:19.000000 django-reusable-8.8/django_reusable/admin/mixins.py
--rw-r--r--   0 narangwa   (501) staff       (20)     5061 2022-09-19 20:52:10.000000 django-reusable-8.8/django_reusable/admin/suit_multi_admin.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-19 22:30:31.000000 django-reusable-8.8/django_reusable/admin/theme.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1820 2022-12-06 18:45:43.000000 django-reusable-8.8/django_reusable/admin/urls.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1136 2022-09-19 20:52:12.000000 django-reusable-8.8/django_reusable/admin/utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)      120 2022-12-21 20:19:38.000000 django-reusable-8.8/django_reusable/constants.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/db/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:18:47.000000 django-reusable-8.8/django_reusable/db/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      125 2023-02-09 20:02:21.000000 django-reusable-8.8/django_reusable/db/query.py
--rw-r--r--   0 narangwa   (501) staff       (20)      827 2022-09-19 20:52:10.000000 django-reusable-8.8/django_reusable/db/queryset.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/django_tables2/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-04-29 02:26:18.000000 django-reusable-8.8/django_reusable/django_tables2/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     4605 2022-09-19 20:52:11.000000 django-reusable-8.8/django_reusable/django_tables2/columns.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2713 2022-09-08 17:23:58.000000 django-reusable-8.8/django_reusable/django_tables2/table_mixins.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/error_tracker/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:09:01.000000 django-reusable-8.8/django_reusable/error_tracker/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)    12001 2022-09-08 21:34:35.000000 django-reusable-8.8/django_reusable/error_tracker/error_tracker.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2085 2022-09-19 20:52:11.000000 django-reusable-8.8/django_reusable/error_tracker/views.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/forms/
--rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:25:55.000000 django-reusable-8.8/django_reusable/forms/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      313 2022-09-19 20:52:11.000000 django-reusable-8.8/django_reusable/forms/fields.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1489 2022-09-19 20:52:11.000000 django-reusable-8.8/django_reusable/forms/forms.py
--rw-r--r--   0 narangwa   (501) staff       (20)      802 2022-09-19 20:52:10.000000 django-reusable-8.8/django_reusable/forms/validators.py
--rw-r--r--   0 narangwa   (501) staff       (20)     3609 2023-02-28 06:04:37.000000 django-reusable-8.8/django_reusable/forms/widgets.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/logging/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:20:29.000000 django-reusable-8.8/django_reusable/logging/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      977 2022-12-17 02:19:01.000000 django-reusable-8.8/django_reusable/logging/loggers.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/middleware/
--rw-r--r--   0 narangwa   (501) staff       (20)       26 2022-09-08 21:25:38.000000 django-reusable-8.8/django_reusable/middleware/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     3383 2022-12-21 20:26:26.000000 django-reusable-8.8/django_reusable/middleware/middleware.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/migrations/
--rw-r--r--   0 narangwa   (501) staff       (20)      973 2022-06-29 20:33:31.000000 django-reusable-8.8/django_reusable/migrations/0001_initial.py
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-06-29 17:35:27.000000 django-reusable-8.8/django_reusable/migrations/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     7348 2023-01-08 22:06:09.000000 django-reusable-8.8/django_reusable/models.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/static/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/static/django_reusable/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/static/django_reusable/css/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/static/django_reusable/css/admin/
--rw-r--r--   0 narangwa   (501) staff       (20)     1960 2022-09-19 20:52:10.000000 django-reusable-8.8/django_reusable/static/django_reusable/css/admin/overrides.css
--rw-r--r--   0 narangwa   (501) staff       (20)     1133 2022-09-19 22:23:56.000000 django-reusable-8.8/django_reusable/static/django_reusable/css/admin/theme.css
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/static/django_reusable/js/
--rw-r--r--   0 narangwa   (501) staff       (20)     4589 2022-05-03 18:09:49.000000 django-reusable-8.8/django_reusable/static/django_reusable/js/dynamic-formsets.js
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templates/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templates/admin/
--rw-r--r--   0 narangwa   (501) staff       (20)      942 2022-09-19 21:46:11.000000 django-reusable-8.8/django_reusable/templates/admin/base.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templates/django_reusable/
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templates/django_reusable/crud/
--rw-r--r--   0 narangwa   (501) staff       (20)     2338 2022-05-17 23:13:44.000000 django-reusable-8.8/django_reusable/templates/django_reusable/crud/add_wizard.pug
--rw-r--r--   0 narangwa   (501) staff       (20)     1561 2022-06-20 18:41:42.000000 django-reusable-8.8/django_reusable/templates/django_reusable/crud/create_or_update.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      702 2022-04-17 01:16:14.000000 django-reusable-8.8/django_reusable/templates/django_reusable/crud/delete.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      487 2022-09-19 21:02:31.000000 django-reusable-8.8/django_reusable/templates/django_reusable/crud/index.pug
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templates/django_reusable/dynamic-formset/
--rw-r--r--   0 narangwa   (501) staff       (20)     1153 2022-05-17 23:09:53.000000 django-reusable-8.8/django_reusable/templates/django_reusable/dynamic-formset/formset.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      312 2020-04-03 06:54:46.000000 django-reusable-8.8/django_reusable/templates/django_reusable/dynamic-formset/stacked-row.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      505 2020-04-03 06:54:46.000000 django-reusable-8.8/django_reusable/templates/django_reusable/dynamic-formset/tabular-row.pug
--rw-r--r--   0 narangwa   (501) staff       (20)      311 2022-05-17 23:09:58.000000 django-reusable-8.8/django_reusable/templates/django_reusable/dynamic-formset/tabular-table.pug
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templates/django_reusable/error_tracker/
--rwxr-xr-x   0 narangwa   (501) staff       (20)     3962 2022-11-27 21:01:44.000000 django-reusable-8.8/django_reusable/templates/django_reusable/error_tracker/detail.html
--rwxr-xr-x   0 narangwa   (501) staff       (20)     2663 2022-11-27 21:00:29.000000 django-reusable-8.8/django_reusable/templates/django_reusable/error_tracker/list.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templates/django_reusable/filters/
--rw-r--r--   0 narangwa   (501) staff       (20)      129 2022-07-05 21:52:13.000000 django-reusable-8.8/django_reusable/templates/django_reusable/filters/input-filter.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templates/django_reusable/forms/
--rw-r--r--   0 narangwa   (501) staff       (20)      715 2019-10-14 17:10:39.000000 django-reusable-8.8/django_reusable/templates/django_reusable/forms/table_form.html
--rw-r--r--   0 narangwa   (501) staff       (20)      727 2020-04-03 06:54:46.000000 django-reusable-8.8/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html
--rw-r--r--   0 narangwa   (501) staff       (20)      345 2019-10-14 17:10:39.000000 django-reusable-8.8/django_reusable/templates/django_reusable/forms/tabular_inline_header.html
--rw-r--r--   0 narangwa   (501) staff       (20)      593 2020-04-03 06:54:46.000000 django-reusable-8.8/django_reusable/templates/django_reusable/forms/tabular_inline_row.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templates/django_reusable/tables/
--rw-r--r--   0 narangwa   (501) staff       (20)      867 2022-09-07 19:14:43.000000 django-reusable-8.8/django_reusable/templates/django_reusable/tables/enhanced-table.html
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/templatetags/
--rw-r--r--   0 narangwa   (501) staff       (20)        0 2019-10-23 04:20:41.000000 django-reusable-8.8/django_reusable/templatetags/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2539 2022-09-19 22:13:59.000000 django-reusable-8.8/django_reusable/templatetags/template_helpers.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/urls/
--rw-r--r--   0 narangwa   (501) staff       (20)       20 2022-09-08 21:25:04.000000 django-reusable-8.8/django_reusable/urls/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)      804 2022-12-21 20:19:38.000000 django-reusable-8.8/django_reusable/urls/urls.py
--rw-r--r--   0 narangwa   (501) staff       (20)      727 2022-12-22 00:17:21.000000 django-reusable-8.8/django_reusable/urls/utils.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/utils/
--rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:28:04.000000 django-reusable-8.8/django_reusable/utils/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)     4454 2023-02-20 01:44:34.000000 django-reusable-8.8/django_reusable/utils/date_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)     2472 2023-02-12 20:30:56.000000 django-reusable-8.8/django_reusable/utils/decorators.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1531 2023-02-01 18:37:30.000000 django-reusable-8.8/django_reusable/utils/export_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-08 20:57:31.000000 django-reusable-8.8/django_reusable/utils/file_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)     3609 2022-09-19 20:52:11.000000 django-reusable-8.8/django_reusable/utils/user_utils.py
--rw-r--r--   0 narangwa   (501) staff       (20)    16117 2023-02-28 06:04:05.000000 django-reusable-8.8/django_reusable/utils/utils.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable/views/
--rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-12-21 20:16:59.000000 django-reusable-8.8/django_reusable/views/__init__.py
--rw-r--r--   0 narangwa   (501) staff       (20)    12338 2022-11-01 19:32:29.000000 django-reusable-8.8/django_reusable/views/mixins.py
--rw-r--r--   0 narangwa   (501) staff       (20)      718 2022-12-21 20:38:18.000000 django-reusable-8.8/django_reusable/views/views.py
-drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable.egg-info/
--rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-02-28 06:06:55.000000 django-reusable-8.8/django_reusable.egg-info/PKG-INFO
--rw-r--r--   0 narangwa   (501) staff       (20)     3197 2023-02-28 06:06:56.000000 django-reusable-8.8/django_reusable.egg-info/SOURCES.txt
--rw-r--r--   0 narangwa   (501) staff       (20)        1 2023-02-28 06:06:55.000000 django-reusable-8.8/django_reusable.egg-info/dependency_links.txt
--rw-r--r--   0 narangwa   (501) staff       (20)       62 2023-02-28 06:06:55.000000 django-reusable-8.8/django_reusable.egg-info/requires.txt
--rw-r--r--   0 narangwa   (501) staff       (20)       16 2023-02-28 06:06:55.000000 django-reusable-8.8/django_reusable.egg-info/top_level.txt
--rwxr-xr-x   0 narangwa   (501) staff       (20)      539 2022-06-29 20:32:34.000000 django-reusable-8.8/manage.py
--rw-r--r--   0 narangwa   (501) staff       (20)       38 2023-02-28 06:06:56.000000 django-reusable-8.8/setup.cfg
--rw-r--r--   0 narangwa   (501) staff       (20)     1483 2022-09-19 20:52:10.000000 django-reusable-8.8/setup.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/
+-rw-r--r--   0 narangwa   (501) staff       (20)       90 2022-04-27 23:42:19.000000 django-reusable-8.9/AUTHORS
+-rw-r--r--   0 narangwa   (501) staff       (20)     2952 2022-04-27 23:43:03.000000 django-reusable-8.9/COPYING
+-rw-r--r--   0 narangwa   (501) staff       (20)      121 2022-06-29 20:32:10.000000 django-reusable-8.9/MANIFEST.in
+-rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-07 20:44:25.000000 django-reusable-8.9/PKG-INFO
+-rw-r--r--   0 narangwa   (501) staff       (20)      399 2022-05-12 17:29:25.000000 django-reusable-8.9/README.md
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/
+-rw-r--r--   0 narangwa   (501) staff       (20)      397 2022-09-19 22:17:44.000000 django-reusable-8.9/django_reusable/__init__.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/admin/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:06:59.000000 django-reusable-8.9/django_reusable/admin/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1830 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/admin/actions.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      613 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/admin/filters.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    16952 2023-04-07 20:40:01.000000 django-reusable-8.9/django_reusable/admin/mixins.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     5061 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/admin/suit_multi_admin.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-19 22:30:31.000000 django-reusable-8.9/django_reusable/admin/theme.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1820 2022-12-06 18:45:43.000000 django-reusable-8.9/django_reusable/admin/urls.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1136 2022-09-19 20:52:12.000000 django-reusable-8.9/django_reusable/admin/utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      120 2022-12-21 20:19:38.000000 django-reusable-8.9/django_reusable/constants.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/db/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:18:47.000000 django-reusable-8.9/django_reusable/db/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      125 2023-02-09 20:02:21.000000 django-reusable-8.9/django_reusable/db/query.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      827 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/db/queryset.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/django_tables2/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-04-29 02:26:18.000000 django-reusable-8.9/django_reusable/django_tables2/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     4605 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/django_tables2/columns.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2713 2022-09-08 17:23:58.000000 django-reusable-8.9/django_reusable/django_tables2/table_mixins.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/error_tracker/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:09:01.000000 django-reusable-8.9/django_reusable/error_tracker/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    12001 2022-09-08 21:34:35.000000 django-reusable-8.9/django_reusable/error_tracker/error_tracker.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2085 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/error_tracker/views.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/forms/
+-rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:25:55.000000 django-reusable-8.9/django_reusable/forms/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      313 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/forms/fields.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1489 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/forms/forms.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      802 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/forms/validators.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     3609 2023-02-28 06:04:37.000000 django-reusable-8.9/django_reusable/forms/widgets.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/logging/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-09-08 21:20:29.000000 django-reusable-8.9/django_reusable/logging/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      977 2022-12-17 02:19:01.000000 django-reusable-8.9/django_reusable/logging/loggers.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/middleware/
+-rw-r--r--   0 narangwa   (501) staff       (20)       26 2022-09-08 21:25:38.000000 django-reusable-8.9/django_reusable/middleware/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     3383 2022-12-21 20:26:26.000000 django-reusable-8.9/django_reusable/middleware/middleware.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/migrations/
+-rw-r--r--   0 narangwa   (501) staff       (20)      973 2022-06-29 20:33:31.000000 django-reusable-8.9/django_reusable/migrations/0001_initial.py
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2022-06-29 17:35:27.000000 django-reusable-8.9/django_reusable/migrations/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     7348 2023-01-08 22:06:09.000000 django-reusable-8.9/django_reusable/models.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/django_reusable/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/django_reusable/css/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/django_reusable/css/admin/
+-rw-r--r--   0 narangwa   (501) staff       (20)     1960 2022-09-19 20:52:10.000000 django-reusable-8.9/django_reusable/static/django_reusable/css/admin/overrides.css
+-rw-r--r--   0 narangwa   (501) staff       (20)     1133 2022-09-19 22:23:56.000000 django-reusable-8.9/django_reusable/static/django_reusable/css/admin/theme.css
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/static/django_reusable/js/
+-rw-r--r--   0 narangwa   (501) staff       (20)     4589 2022-05-03 18:09:49.000000 django-reusable-8.9/django_reusable/static/django_reusable/js/dynamic-formsets.js
+-rw-r--r--   0 narangwa   (501) staff       (20)     1542 2023-04-07 18:14:43.000000 django-reusable-8.9/django_reusable/static/django_reusable/js/enhanced-admin-mixin.js
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/admin/
+-rw-r--r--   0 narangwa   (501) staff       (20)      942 2022-09-19 21:46:11.000000 django-reusable-8.9/django_reusable/templates/admin/base.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/
+-rw-r--r--   0 narangwa   (501) staff       (20)     2338 2022-05-17 23:13:44.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/add_wizard.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)     1561 2022-06-20 18:41:42.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/create_or_update.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      702 2022-04-17 01:16:14.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/delete.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      487 2022-09-19 21:02:31.000000 django-reusable-8.9/django_reusable/templates/django_reusable/crud/index.pug
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/
+-rw-r--r--   0 narangwa   (501) staff       (20)     1153 2022-05-17 23:09:53.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/formset.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      312 2020-04-03 06:54:46.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/stacked-row.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      505 2020-04-03 06:54:46.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/tabular-row.pug
+-rw-r--r--   0 narangwa   (501) staff       (20)      311 2022-05-17 23:09:58.000000 django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/tabular-table.pug
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/
+-rwxr-xr-x   0 narangwa   (501) staff       (20)     3962 2022-11-27 21:01:44.000000 django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/detail.html
+-rwxr-xr-x   0 narangwa   (501) staff       (20)     2663 2022-11-27 21:00:29.000000 django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/list.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/filters/
+-rw-r--r--   0 narangwa   (501) staff       (20)      129 2022-07-05 21:52:13.000000 django-reusable-8.9/django_reusable/templates/django_reusable/filters/input-filter.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/
+-rw-r--r--   0 narangwa   (501) staff       (20)      715 2019-10-14 17:10:39.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/table_form.html
+-rw-r--r--   0 narangwa   (501) staff       (20)      727 2020-04-03 06:54:46.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html
+-rw-r--r--   0 narangwa   (501) staff       (20)      345 2019-10-14 17:10:39.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_header.html
+-rw-r--r--   0 narangwa   (501) staff       (20)      593 2020-04-03 06:54:46.000000 django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_row.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templates/django_reusable/tables/
+-rw-r--r--   0 narangwa   (501) staff       (20)      867 2022-09-07 19:14:43.000000 django-reusable-8.9/django_reusable/templates/django_reusable/tables/enhanced-table.html
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/templatetags/
+-rw-r--r--   0 narangwa   (501) staff       (20)        0 2019-10-23 04:20:41.000000 django-reusable-8.9/django_reusable/templatetags/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2539 2022-09-19 22:13:59.000000 django-reusable-8.9/django_reusable/templatetags/template_helpers.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/urls/
+-rw-r--r--   0 narangwa   (501) staff       (20)       20 2022-09-08 21:25:04.000000 django-reusable-8.9/django_reusable/urls/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      804 2022-12-21 20:19:38.000000 django-reusable-8.9/django_reusable/urls/urls.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      727 2022-12-22 00:17:21.000000 django-reusable-8.9/django_reusable/urls/utils.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/utils/
+-rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-09-08 21:28:04.000000 django-reusable-8.9/django_reusable/utils/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     4454 2023-02-20 01:44:34.000000 django-reusable-8.9/django_reusable/utils/date_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     2472 2023-02-12 20:30:56.000000 django-reusable-8.9/django_reusable/utils/decorators.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1531 2023-02-01 18:37:30.000000 django-reusable-8.9/django_reusable/utils/export_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     1898 2022-09-08 20:57:31.000000 django-reusable-8.9/django_reusable/utils/file_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)     3609 2022-09-19 20:52:11.000000 django-reusable-8.9/django_reusable/utils/user_utils.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    16117 2023-02-28 06:04:05.000000 django-reusable-8.9/django_reusable/utils/utils.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable/views/
+-rw-r--r--   0 narangwa   (501) staff       (20)       21 2022-12-21 20:16:59.000000 django-reusable-8.9/django_reusable/views/__init__.py
+-rw-r--r--   0 narangwa   (501) staff       (20)    12338 2022-11-01 19:32:29.000000 django-reusable-8.9/django_reusable/views/mixins.py
+-rw-r--r--   0 narangwa   (501) staff       (20)      718 2022-12-21 20:38:18.000000 django-reusable-8.9/django_reusable/views/views.py
+drwxr-xr-x   0 narangwa   (501) staff       (20)        0 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable.egg-info/
+-rw-r--r--   0 narangwa   (501) staff       (20)     1091 2023-04-07 20:44:24.000000 django-reusable-8.9/django_reusable.egg-info/PKG-INFO
+-rw-r--r--   0 narangwa   (501) staff       (20)     3263 2023-04-07 20:44:25.000000 django-reusable-8.9/django_reusable.egg-info/SOURCES.txt
+-rw-r--r--   0 narangwa   (501) staff       (20)        1 2023-04-07 20:44:24.000000 django-reusable-8.9/django_reusable.egg-info/dependency_links.txt
+-rw-r--r--   0 narangwa   (501) staff       (20)       62 2023-04-07 20:44:24.000000 django-reusable-8.9/django_reusable.egg-info/requires.txt
+-rw-r--r--   0 narangwa   (501) staff       (20)       16 2023-04-07 20:44:24.000000 django-reusable-8.9/django_reusable.egg-info/top_level.txt
+-rwxr-xr-x   0 narangwa   (501) staff       (20)      539 2022-06-29 20:32:34.000000 django-reusable-8.9/manage.py
+-rw-r--r--   0 narangwa   (501) staff       (20)       38 2023-04-07 20:44:25.000000 django-reusable-8.9/setup.cfg
+-rw-r--r--   0 narangwa   (501) staff       (20)     1483 2022-09-19 20:52:10.000000 django-reusable-8.9/setup.py
```

### Comparing `django-reusable-8.8/COPYING` & `django-reusable-8.9/COPYING`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/PKG-INFO` & `django-reusable-8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reusable
-Version: 8.8
+Version: 8.9
 Summary: Agnostic and easy to use reusable library for django
 Home-page: https://github.com/navedr/django-reusable
 Author: Naved Rangwala
 Author-email: naved@ecarone.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-reusable-8.8/django_reusable/admin/actions.py` & `django-reusable-8.9/django_reusable/admin/actions.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/admin/filters.py` & `django-reusable-8.9/django_reusable/admin/filters.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/admin/mixins.py` & `django-reusable-8.9/django_reusable/admin/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from copy import deepcopy
 
 from django.contrib import admin, messages
 from django.contrib.admin.options import BaseModelAdmin, InlineModelAdmin
 from django.core.exceptions import PermissionDenied
-from django.http import HttpResponseRedirect
+from django.http import HttpResponseRedirect, JsonResponse
 from django.shortcuts import redirect
 from django.urls import reverse, path
 from django.utils.safestring import mark_safe
 
 from django_reusable.admin.urls import ModelURLs
 from django_reusable.admin.utils import remove_from_fieldsets
 from django_reusable.admin.filters import SearchInFilter
+from django_reusable.constants import URLNames
 from django_reusable.forms.forms import EnhancedBaseInlineFormSet
-from django_reusable.utils import ifilter
+from django_reusable.utils import ifilter, CustomEncoder
 
 
 class EnhancedAdminInlineMixin(InlineModelAdmin):
     select2_inlines_fields = []
     default_field_queryset = dict()
     limit_field_queryset_model_fields = dict()
     limit_saved_queryset_value_fields = []
@@ -78,44 +79,132 @@
             btn_text = config.get('btn_text', 'Button')
             btn_class = config.get('btn_class', 'btn btn-warning')
 
             @mark_safe
             def func(instance):
                 if not instance.id:
                     return ''
-                url = reverse('django_reusable:ajax_callback_handler',
+                url = reverse(f'django_reusable:{URLNames.AJAX_CALLBACK_HANDLER}',
                               args=(instance.pk, self.get_callback_key(name)))
                 return (f'<button class="{btn_class} ajax-action-btn" data-url="{url}">{btn_text}</button>' +
                         config.get('additional_html', ''))
 
             func.short_description = config.get('short_desc', btn_text)
             func.__name__ = name
             setattr(self, func.__name__, func)
 
             self.register_callback(name, config['callback'])
 
 
-class EnhancedAdminMixin(admin.ModelAdmin, EnhancedBaseAdminMixin):
-    default_filters = []
-    search_in_choices = []
+class ExtraChangelistLinksMixin:
     """
         List of tuples:
-        ('field_name', lambda instance: instance.field.name, optional short_desc)
+        (url, dict(link_text, link_class, new_tab, user_passes_test))
     """
-    custom_fields = []
+    extra_changelist_links = []
+
+    def _get_applicable_extra_changelist_links(self, request):
+        def _add_default_values(config):
+            config['link_class'] = config.get('link_class', 'btn-link')
+            config['link_text'] = config.get('link_text', 'Link')
+            config['new_tab'] = config.get('new_tab', False)
+            return config
+
+        return [(url, _add_default_values(config)) for (url, config) in self.get_extra_changelist_links(request)
+                if config.get('user_passes_test', lambda u: True)(request.user)]
+
+    def _add_extra_changelist_links(self, request, extra_context):
+        extra_context.update(
+            extra_links=[
+                (url,
+                 config['link_class'],
+                 config['link_text'],
+                 config['new_tab'])
+                for (url, config) in self._get_applicable_extra_changelist_links(request)
+            ]
+        )
+
+    def get_extra_changelist_links(self, request):
+        return self.extra_changelist_links
+
+    def _changelist_mixin_js_data(self, request):
+        return dict(
+            extra_links=[dict(url=url, config=config) for (url, config) in
+                         self._get_applicable_extra_changelist_links(request)]
+        )
+
+
+class ExtraChangeFormButtonsMixin:
     """
         List of tuples:
-        ('name', dict(btn_text, btn_class, stay_on_page, callback))
+        ('name', dict(btn_text, btn_class, stay_on_page, callback, user_passes_test, pk_passes_test))
     """
     extra_change_form_buttons = []
+
+    def _get_applicable_extra_change_form_buttons(self, request, pk):
+        def _add_default_values(config):
+            config['btn_class'] = config.get('btn_class', 'btn-primary')
+            config['btn_text'] = config.get('btn_text', 'Button')
+            return config
+
+        return [
+            (name, _add_default_values(config)) for (name, config) in self.extra_change_form_buttons
+            if (config.get('user_passes_test', lambda u: True)(request.user) and
+                config.get('pk_passes_test', lambda _pk: True)(pk))
+        ]
+
+    def _add_extra_change_form_buttons(self, request, pk, extra_context):
+        extra_context.update(
+            extra_submit_buttons=[
+                (f'__{name}', config['btn_class'], config['btn_text'])
+                for (name, config) in self._get_applicable_extra_change_form_buttons(request, pk)
+            ]
+        )
+
+    def _handle_extra_change_form_buttons(self, request, object_id):
+        for (name, config) in self.extra_change_form_buttons:
+            if f'__{name}' not in request.POST:
+                continue
+            callback = config.get('callback')
+            if callback:
+                r = callback(self, request, object_id)
+                if r:
+                    messages.info(request, r)
+            if config.get('stay_on_page', False):
+                return HttpResponseRedirect(
+                    ModelURLs(self.model, self.admin_site.name, object_id).get_obj_change_url()
+                )
+            break
+        return None
+
+    def _change_form_mixin_js_data(self, request, object_id=None):
+        return dict(
+            object_id=object_id,
+            extra_submit_buttons=[
+                dict(name=name, config=config)
+                for (name, config) in self._get_applicable_extra_change_form_buttons(request, object_id)
+            ]
+        )
+
+
+class EnhancedAdminMixin(admin.ModelAdmin,
+                         EnhancedBaseAdminMixin,
+                         ExtraChangelistLinksMixin,
+                         ExtraChangeFormButtonsMixin):
+    """
+    Auto update template with all the extras and
+    """
+    auto_update_template = True
+    default_filters = []
+    search_in_choices = []
     """
         List of tuples:
-        (url, dict(link_text, link_class, new_tab, user_passes_test, pk_passes_test))
+        ('field_name', lambda instance: instance.field.name, optional short_desc)
     """
-    extra_changelist_links = []
+    custom_fields = []
     """
         List of tuples:
         ('name', dict(btn_text, btn_class, callback, short_desc, custom_redirect))
         Note: callback is called with args (instance)
     """
     action_links = []
 
@@ -176,56 +265,19 @@
 
     def get_changelist_extra_context(self, request):
         return {}
 
     def custom_changelist_actions(self, request):
         pass
 
-    def _add_extra_change_form_buttons(self, request, pk, extra_context):
-        extra_context.update(
-            extra_submit_buttons=[
-                (f'__{name}', config.get('btn_class', 'btn-primary'), config.get('btn_text', 'Button'))
-                for (name, config) in self.extra_change_form_buttons
-                if (config.get('user_passes_test', lambda u: True)(request.user) and
-                    config.get('pk_passes_test', lambda _pk: True)(pk))
-            ]
-        )
-
-    def _handle_extra_change_form_buttons(self, request, object_id):
-        for (name, config) in self.extra_change_form_buttons:
-            if f'__{name}' not in request.POST:
-                continue
-            callback = config.get('callback')
-            if callback:
-                r = callback(self, request, object_id)
-                if r:
-                    messages.info(request, r)
-            if config.get('stay_on_page', False):
-                return HttpResponseRedirect(
-                    ModelURLs(self.model, self.admin_site.name, object_id).get_obj_change_url()
-                )
-            break
-        return None
-
-    def _add_extra_changelist_links(self, request, extra_context):
-        extra_context.update(
-            extra_links=[
-                (url,
-                 config.get('link_class', 'btn-link'),
-                 config.get('link_text', 'Link'),
-                 config.get('new_tab', False))
-                for (url, config) in self.get_extra_changelist_links(request)
-                if config.get('user_passes_test', lambda u: True)(request.user)
-            ]
-        )
-
     def changelist_view(self, request, extra_context=None):
         extra_context = extra_context or {}
         self.custom_changelist_actions(request)
-        self._add_extra_changelist_links(request, extra_context)
+        if not self.auto_update_template:
+            self._add_extra_changelist_links(request, extra_context)
         if self.default_filters:
             try:
                 test = request.META['HTTP_REFERER'].split(request.META['PATH_INFO'])
                 if test and test[-1] and not test[-1].startswith('?'):
                     url = reverse('admin:%s_%s_changelist' % (self.opts.app_label, self.opts.model_name))
                     filters = []
                     for f in self.default_filters:
@@ -237,18 +289,19 @@
             except:
                 pass
         extra_context.update(self.get_changelist_extra_context(request) or {})
         return super(EnhancedAdminMixin, self).changelist_view(request, extra_context)
 
     def change_view(self, request, object_id, form_url='', extra_context=None):
         extra_context = extra_context or {}
-        extra_context.update(
-            hide_save_buttons=self.hide_save_buttons(request, object_id)
-        )
-        self._add_extra_change_form_buttons(request, object_id, extra_context)
+        if not self.auto_update_template:
+            self._add_extra_change_form_buttons(request, object_id, extra_context)
+            extra_context.update(
+                hide_save_buttons=self.hide_save_buttons(request, object_id)
+            )
         if request.method == 'POST' and extra_context['hide_save_buttons']:
             raise PermissionDenied()
         response = super().change_view(request, object_id, form_url, extra_context)
         if request.method == 'POST':
             return self._handle_extra_change_form_buttons(request, object_id) or response
         return response
 
@@ -264,17 +317,14 @@
                 inline_instances.remove(inline)
 
     def get_readonly_fields(self, request, obj=None):
         return (list(super().get_readonly_fields(request, obj)) +
                 [x[0] for x in self.custom_fields] +
                 [x[0] for x in self.action_links])
 
-    def get_extra_changelist_links(self, request):
-        return self.extra_changelist_links
-
     def get_fieldset_section_exclusions(self, request, obj):
         return []
 
     def get_fieldset_field_exclusions(self, request, obj):
         return []
 
     def get_fieldsets(self, request, obj=None):
@@ -286,17 +336,48 @@
         fieldsets = deepcopy(original_fieldsets)
         if section_exclusions:
             fieldsets = [(title, attributes) for title, attributes in fieldsets if title not in section_exclusions]
         if field_exclusions:
             remove_from_fieldsets(fieldsets, field_exclusions)
         return fieldsets
 
+    def _get_common_mixin_js_data(self):
+        return dict(
+            app=self.model._meta.app_label,
+            model=self.model._meta.model_name,
+            enabled=self.auto_update_template
+        )
+
+    def _changelist_mixin_js_data(self, request):
+        return JsonResponse(dict(
+            **self._get_common_mixin_js_data(),
+            **super()._changelist_mixin_js_data(request)
+        ), encoder=CustomEncoder)
+
+    def _change_form_mixin_js_data(self, request, object_id=None):
+        return JsonResponse(dict(
+            **self._get_common_mixin_js_data(),
+            hide_save_buttons=self.hide_save_buttons(request, object_id),
+            **super()._change_form_mixin_js_data(request, object_id)
+        ), encoder=CustomEncoder)
+
     def get_urls(self):
         urls = super().get_urls()
-        my_urls = []
+        info = self.model._meta.app_label, self.model._meta.model_name
+        my_urls = [
+            path('<path:object_id>/change/dr-admin-mixin-js-data/',
+                 self._change_form_mixin_js_data,
+                 name='%s_%s-dr-admin-mixin-js-data_change' % info),
+            path('add/dr-admin-mixin-js-data/',
+                 self._change_form_mixin_js_data,
+                 name='%s_%s-dr-admin-mixin-js-data_add' % info),
+            path('dr-admin-mixin-js-data/',
+                 self._changelist_mixin_js_data,
+                 name='%s_%s_dr-admin-mixin-js-data-changelist' % info),
+        ]
 
         def get_action_link_view(_view_name, _attrs):
             def action_link_view(request, pk):
                 obj = self.model.objects.get(id=pk)
                 response = _attrs['callback'](obj)
                 if _attrs.get('custom_redirect'):
                     return response
@@ -311,14 +392,17 @@
             view_name = f'{self.model._meta.app_label}_{self.model._meta.model_name}_action_view_{name}'
 
             my_urls.append(path(f'<path:pk>/action-link/{name}/',
                                 self.admin_site.admin_view(get_action_link_view(view_name, attrs)),
                                 name=view_name))
         return my_urls + urls
 
+    class Media:
+        js = ['django_reusable/js/enhanced-admin-mixin.js']
+
 
 class ReadonlyAdmin(admin.ModelAdmin):
 
     def has_delete_permission(self, request, obj=None):
         return False
 
     def has_add_permission(self, request):
```

### Comparing `django-reusable-8.8/django_reusable/admin/suit_multi_admin.py` & `django-reusable-8.9/django_reusable/admin/suit_multi_admin.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/admin/theme.py` & `django-reusable-8.9/django_reusable/admin/theme.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/admin/urls.py` & `django-reusable-8.9/django_reusable/admin/urls.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/admin/utils.py` & `django-reusable-8.9/django_reusable/admin/utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/db/queryset.py` & `django-reusable-8.9/django_reusable/db/queryset.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/django_tables2/columns.py` & `django-reusable-8.9/django_reusable/django_tables2/columns.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/django_tables2/table_mixins.py` & `django-reusable-8.9/django_reusable/django_tables2/table_mixins.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/error_tracker/error_tracker.py` & `django-reusable-8.9/django_reusable/error_tracker/error_tracker.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/error_tracker/views.py` & `django-reusable-8.9/django_reusable/error_tracker/views.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/forms/forms.py` & `django-reusable-8.9/django_reusable/forms/forms.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/forms/validators.py` & `django-reusable-8.9/django_reusable/forms/validators.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/forms/widgets.py` & `django-reusable-8.9/django_reusable/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/logging/loggers.py` & `django-reusable-8.9/django_reusable/logging/loggers.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/middleware/middleware.py` & `django-reusable-8.9/django_reusable/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/migrations/0001_initial.py` & `django-reusable-8.9/django_reusable/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/models.py` & `django-reusable-8.9/django_reusable/models.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/static/django_reusable/css/admin/overrides.css` & `django-reusable-8.9/django_reusable/static/django_reusable/css/admin/overrides.css`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/static/django_reusable/css/admin/theme.css` & `django-reusable-8.9/django_reusable/static/django_reusable/css/admin/theme.css`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/static/django_reusable/js/dynamic-formsets.js` & `django-reusable-8.9/django_reusable/static/django_reusable/js/dynamic-formsets.js`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/admin/base.html` & `django-reusable-8.9/django_reusable/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/crud/add_wizard.pug` & `django-reusable-8.9/django_reusable/templates/django_reusable/crud/add_wizard.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/crud/create_or_update.pug` & `django-reusable-8.9/django_reusable/templates/django_reusable/crud/create_or_update.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/crud/delete.pug` & `django-reusable-8.9/django_reusable/templates/django_reusable/crud/delete.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/dynamic-formset/formset.pug` & `django-reusable-8.9/django_reusable/templates/django_reusable/dynamic-formset/formset.pug`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/error_tracker/detail.html` & `django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/detail.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/error_tracker/list.html` & `django-reusable-8.9/django_reusable/templates/django_reusable/error_tracker/list.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/forms/table_form.html` & `django-reusable-8.9/django_reusable/templates/django_reusable/forms/table_form.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html` & `django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_formset.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/forms/tabular_inline_row.html` & `django-reusable-8.9/django_reusable/templates/django_reusable/forms/tabular_inline_row.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templates/django_reusable/tables/enhanced-table.html` & `django-reusable-8.9/django_reusable/templates/django_reusable/tables/enhanced-table.html`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/templatetags/template_helpers.py` & `django-reusable-8.9/django_reusable/templatetags/template_helpers.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/urls/urls.py` & `django-reusable-8.9/django_reusable/urls/urls.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/urls/utils.py` & `django-reusable-8.9/django_reusable/urls/utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/utils/date_utils.py` & `django-reusable-8.9/django_reusable/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/utils/decorators.py` & `django-reusable-8.9/django_reusable/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/utils/export_utils.py` & `django-reusable-8.9/django_reusable/utils/export_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/utils/file_utils.py` & `django-reusable-8.9/django_reusable/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/utils/user_utils.py` & `django-reusable-8.9/django_reusable/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/utils/utils.py` & `django-reusable-8.9/django_reusable/utils/utils.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/views/mixins.py` & `django-reusable-8.9/django_reusable/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable/views/views.py` & `django-reusable-8.9/django_reusable/views/views.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/django_reusable.egg-info/PKG-INFO` & `django-reusable-8.9/django_reusable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reusable
-Version: 8.8
+Version: 8.9
 Summary: Agnostic and easy to use reusable library for django
 Home-page: https://github.com/navedr/django-reusable
 Author: Naved Rangwala
 Author-email: naved@ecarone.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-reusable-8.8/django_reusable.egg-info/SOURCES.txt` & `django-reusable-8.9/django_reusable.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 django_reusable/middleware/__init__.py
 django_reusable/middleware/middleware.py
 django_reusable/migrations/0001_initial.py
 django_reusable/migrations/__init__.py
 django_reusable/static/django_reusable/css/admin/overrides.css
 django_reusable/static/django_reusable/css/admin/theme.css
 django_reusable/static/django_reusable/js/dynamic-formsets.js
+django_reusable/static/django_reusable/js/enhanced-admin-mixin.js
 django_reusable/templates/admin/base.html
 django_reusable/templates/django_reusable/crud/add_wizard.pug
 django_reusable/templates/django_reusable/crud/create_or_update.pug
 django_reusable/templates/django_reusable/crud/delete.pug
 django_reusable/templates/django_reusable/crud/index.pug
 django_reusable/templates/django_reusable/dynamic-formset/formset.pug
 django_reusable/templates/django_reusable/dynamic-formset/stacked-row.pug
```

### Comparing `django-reusable-8.8/manage.py` & `django-reusable-8.9/manage.py`

 * *Files identical despite different names*

### Comparing `django-reusable-8.8/setup.py` & `django-reusable-8.9/setup.py`

 * *Files identical despite different names*

