# Comparing `tmp/django-autocomplete-light-3.9.5rc4.tar.gz` & `tmp/django-autocomplete-light-3.9.5rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-autocomplete-light-3.9.5rc4.tar", last modified: Fri Apr  7 16:57:48 2023, max compression
+gzip compressed data, was "django-autocomplete-light-3.9.5rc5.tar", last modified: Fri Apr  7 16:59:20 2023, max compression
```

## Comparing `django-autocomplete-light-3.9.5rc4.tar` & `django-autocomplete-light-3.9.5rc5.tar`

### file list

```diff
@@ -1,739 +1,739 @@
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.218032 django-autocomplete-light-3.9.5rc4/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1625 2020-07-14 22:32:02.000000 django-autocomplete-light-3.9.5rc4/AUTHORS
--rw-r--r--   0 jpic      (1000) jpic      (1000)    46684 2023-04-07 16:57:47.000000 django-autocomplete-light-3.9.5rc4/CHANGELOG
--rw-r--r--   0 jpic      (1000) jpic      (1000)    46684 2023-04-07 16:57:47.000000 django-autocomplete-light-3.9.5rc4/CHANGES.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1076 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/LICENSE
--rw-r--r--   0 jpic      (1000) jpic      (1000)      302 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/MANIFEST.in
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3209 2023-04-07 16:57:48.218032 django-autocomplete-light-3.9.5rc4/PKG-INFO
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2221 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/README
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2221 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/README.rst
--rw-r--r--   0 jpic      (1000) jpic      (1000)       38 2023-04-07 16:57:48.218032 django-autocomplete-light-3.9.5rc4/setup.cfg
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1685 2023-04-07 16:57:18.000000 django-autocomplete-light-3.9.5rc4/setup.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.171366 django-autocomplete-light-3.9.5rc4/src/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       37 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/__init__.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.171366 django-autocomplete-light-3.9.5rc4/src/dal/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      112 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2751 2021-05-03 22:49:43.000000 django-autocomplete-light-3.9.5rc4/src/dal/autocomplete.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6762 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal/forms.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4633 2020-07-14 22:32:02.000000 django-autocomplete-light-3.9.5rc4/src/dal/forward.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal/static/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.171366 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    18327 2022-11-22 18:42:05.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/autocomplete_light.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5423 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/autocomplete_light.min.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.174699 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      950 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/af.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      989 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ar.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      805 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/az.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1052 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/bg.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1359 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/bn.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1019 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/bs.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      968 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ca.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1364 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/cs.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      912 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/da.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      949 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/de.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1093 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/dsb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1266 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/el.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1005 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/en.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      943 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/eo.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      990 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/es.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      882 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/et.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      948 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/eu.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1107 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/fa.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      887 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/fi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1053 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/fr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      998 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/gl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1056 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/he.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1246 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      936 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1094 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hsb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1003 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hu.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1112 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hy.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      852 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/id.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      890 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/is.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/it.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      946 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ja.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1279 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ka.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1172 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/km.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      939 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ko.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      998 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/lt.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      959 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/lv.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1122 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/mk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      895 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ms.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      862 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/nb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1438 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ne.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      985 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/nl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1450 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/pa.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1022 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/pl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1127 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ps.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      963 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/pt-BR.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      946 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/pt.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1021 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ro.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1233 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ru.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1382 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1009 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      987 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sq.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1168 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sr-Cyrl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1034 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      870 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sv.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1433 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/te.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1158 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/th.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/tk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      859 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/tr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1240 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/uk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      880 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/vi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/zh-CN.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      794 2023-04-07 16:57:17.000000 django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/zh-TW.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal/test/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       36 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal/test/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3375 2020-02-04 10:01:44.000000 django-autocomplete-light-3.9.5rc4/src/dal/test/case.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)    13964 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal/test/stories.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1926 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal/test/utils.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7695 2022-11-22 19:18:36.000000 django-autocomplete-light-3.9.5rc4/src/dal/views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6595 2023-04-07 12:28:05.000000 django-autocomplete-light-3.9.5rc4/src/dal/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_contenttypes/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       53 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_contenttypes/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1962 2020-02-04 10:01:44.000000 django-autocomplete-light-3.9.5rc4/src/dal_contenttypes/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_genericm2m/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       42 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_genericm2m/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      708 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_genericm2m/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_genericm2m_queryset_sequence/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       65 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_genericm2m_queryset_sequence/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      424 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_genericm2m_queryset_sequence/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_gm2m/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       35 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_gm2m/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      534 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_gm2m/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_gm2m_queryset_sequence/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       70 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_gm2m_queryset_sequence/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      377 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_gm2m_queryset_sequence/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       37 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/__init__.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     8440 2021-05-03 22:49:43.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/css/autocomplete.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/css/vendor/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/css/vendor/select2/
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)    17636 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/css/vendor/select2/select2.css
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)    15196 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/css/vendor/select2/select2.min.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1124 2021-05-03 22:49:43.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/autocomplete.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.178032 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      887 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ar.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      701 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/az.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      906 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/bg.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      876 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ca.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1236 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/cs.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      818 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/da.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      775 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/de.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1132 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/el.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      827 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/en.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      871 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/es.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      775 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/et.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      844 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/eu.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1004 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fa.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      703 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fi.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      902 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fr.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      800 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/gl.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      951 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/he.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1125 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hi.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      839 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hr.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      727 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hu.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      752 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/id.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      773 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/is.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      876 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/it.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      848 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ja.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1065 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/km.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      854 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ko.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      913 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lt.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      872 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lv.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      979 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/mk.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      791 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ms.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      785 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nb.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      896 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nl.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      925 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pl.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      853 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt-BR.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      859 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      909 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ro.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1127 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ru.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1184 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sk.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1067 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      938 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      786 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sv.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      951 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/th.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      720 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/tr.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1117 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/uk.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      801 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/vi.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      769 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-CN.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      708 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-TW.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)   161832 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)    75005 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.min.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       40 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6355 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/tests/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1545 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/tests/test_views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2298 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1703 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_select2/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      149 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      274 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/apps.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1795 2022-11-22 19:23:02.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/bg/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/bg/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      508 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      671 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/cs/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/cs/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      528 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      691 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/de/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/de/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      501 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      664 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/es/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/es/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fi/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fi/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      488 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      684 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.164699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fr/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/it/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.181366 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/it/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      498 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      661 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ja/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ja/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/nl/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/nl/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      500 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      663 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pl/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pl/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      557 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      723 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pt-br/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pt-br/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      503 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pt-br/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      670 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pt-br/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ru/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ru/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      644 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      813 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/tr/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/tr/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      492 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      741 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/uk/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/uk/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      582 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      748 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/zh-cn/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/zh-cn/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      458 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      617 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.po
--rw-r--r--   0 jpic      (1000) jpic      (1000)       46 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/models.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/autocomplete_light/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2765 2022-11-22 18:42:05.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/autocomplete_light/select2.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4937 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/autocomplete_light/select2.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2014 2023-04-07 16:57:18.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/autocomplete_light/select2.min.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6128 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/Gruntfile.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      384 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/bower.json
--rw-r--r--   0 jpic      (1000) jpic      (1000)      463 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/component.json
--rw-r--r--   0 jpic      (1000) jpic      (1000)      462 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/composer.json
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    18931 2023-04-07 16:57:16.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/css/select2.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)    16264 2023-04-07 16:57:16.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/css/select2.min.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.184699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.188032 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      866 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/af.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      905 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ar.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      721 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/az.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      968 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/bg.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1291 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/bn.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      965 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/bs.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      900 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ca.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1292 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/cs.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      828 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/da.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      866 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/de.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1017 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/dsb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1182 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/el.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      844 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/en.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      922 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/es.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      801 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/et.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      868 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/eu.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1023 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/fa.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      803 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/fi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      924 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/fr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      924 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/gl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      984 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/he.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1175 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      852 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1018 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hsb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      831 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hu.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1028 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hy.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      768 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/id.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      807 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/is.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      897 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/it.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      862 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ja.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1195 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ka.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1088 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/km.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ko.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      944 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/lt.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      900 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/lv.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1038 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/mk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      811 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ms.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      778 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/nb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1357 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ne.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      904 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/nl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      947 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/pl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1049 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ps.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      876 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/pt-BR.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      878 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/pt.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      938 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ro.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1171 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ru.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1306 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      925 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      903 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sq.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1109 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sr-Cyrl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      980 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      786 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sv.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1074 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/th.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      771 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/tk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      775 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/tr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1156 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/uk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      796 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/vi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      768 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/zh-CN.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      707 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/zh-TW.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)   173566 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/select2.full.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)    79212 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/select2.full.min.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)   153589 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/select2.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)    70891 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/select2.min.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.188032 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/assets/
--rw-r--r--   0 jpic      (1000) jpic      (1000)   134486 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/assets/rtfm-screenshot.png
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.191366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.194699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2212 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ak.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2623 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/al.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    10871 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ar.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5448 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/az.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7159 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ca.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2593 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/co.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     9209 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ct.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7903 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/de.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     9018 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/fl.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4765 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ga.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3170 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/hi.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7102 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ia.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7319 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/id.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    10352 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/il.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6988 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/in.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7758 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ks.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    10162 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ky.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    11486 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/la.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3985 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ma.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4103 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/md.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6238 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/me.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    10471 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mi.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7938 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mn.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7495 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mo.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6088 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ms.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7344 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mt.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3995 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nc.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    11795 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nd.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    13899 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ne.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    12792 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nh.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7098 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nj.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1523 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nm.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4268 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nv.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     9732 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ny.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7666 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/oh.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7290 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ok.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     9530 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/or.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    11193 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/pa.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6927 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ri.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4485 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/sc.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    10252 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/sd.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4005 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/tn.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1324 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/tx.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    10674 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ut.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    10138 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/va.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6397 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/vt.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    45254 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wa.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     8539 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wi.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)    45254 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wv.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4343 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wy.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2501 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/logo.png
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/anchors/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.194699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/anchors/js/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5272 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/anchors/js/anchor.min.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.194699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/assets/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    61887 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/assets/readme_1.png
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.194699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      295 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/css/breadcrumbs.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/error/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.194699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/error/assets/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    41685 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/error/assets/readme_1.png
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.194699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/assets/
--rw-r--r--   0 jpic      (1000) jpic      (1000)   167622 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/assets/readme_1.png
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.198032 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1276 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/agate.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      774 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/androidstudio.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1054 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/arduino-light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      852 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/arta.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      591 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/ascetic.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1926 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-cave.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1927 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-cave.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1668 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-dune.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1669 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-dune.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1956 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-estuary.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1957 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-estuary.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1688 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-forest.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1689 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-forest.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1678 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-heath.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1679 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-heath.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1708 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-lakeside.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1709 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-lakeside.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1956 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-plateau.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1957 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-plateau.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1956 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-savanna.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1957 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-savanna.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1698 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-seaside.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1699 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-seaside.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1738 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-sulphurpool.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1739 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-sulphurpool.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      842 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/brown-paper.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      842 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/codepen-embed.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      884 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/color-brewer.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      794 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      890 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/darkula.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      952 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/default.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1141 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/docco.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      849 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/far.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1086 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/foundation.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      919 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/github-gist.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1148 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/github.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1053 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/googlecode.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1966 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/grayscale.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1059 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/hopscotch.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1342 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/hybrid.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1173 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/idea.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      871 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/ir-black.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1067 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/kimbie.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1068 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/kimbie.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      839 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/learn.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      891 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/magula.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      749 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/mono-blue.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1026 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/monokai-sublime.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      938 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/monokai.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1079 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/obsidian.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1014 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso-dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1015 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso-light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1558 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso.dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1559 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso.light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1124 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/pojoaque.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1211 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/railscasts.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      983 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/rainbow.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      999 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/school-book.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1145 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/solarized-dark.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1145 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/solarized-light.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1183 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/sunburst.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1152 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-blue.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1082 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-bright.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1086 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-eighties.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1149 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      978 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      837 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/vs.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1071 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/xcode.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      947 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/zenburn.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.198032 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    44929 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/highlight.pack.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      794 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/highlightjs-line-numbers.min.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.198032 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/assets/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    72908 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/assets/readme_1.png
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.198032 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1155 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/problems.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)    21132 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/template.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.198032 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/html/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1164 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/html/problems.html
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/
--rw-r--r--   0 jpic      (1000) jpic      (1000)   113109 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/readme_1.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/search.svg
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      514 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/css/simplesearch.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/js/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1089 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/js/simplesearch.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1448 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/featherlight.min.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)    31000 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/font-awesome.min.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      117 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/nucleus-ie10.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      575 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/nucleus-ie9.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/pure-0.5.0/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3857 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/pure-0.5.0/grids-min.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    11928 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/nucleus.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)    23480 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/theme.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/
--rw-r--r--   0 jpic      (1000) jpic      (1000)   165742 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.eot
--rw-r--r--   0 jpic      (1000) jpic      (1000)   444379 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.svg
--rw-r--r--   0 jpic      (1000) jpic      (1000)   165548 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 jpic      (1000) jpic      (1000)    98024 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.woff
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      519 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/clippy.svg
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1177 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/favicon.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1215 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/logo.png
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     8855 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/clipboard.min.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7257 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/featherlight.min.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4133 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/html5shiv-printshiv.min.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)    12188 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/jquery.scrollbar.min.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)    11180 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/learn.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     9093 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/modernizr.custom.71422.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.201366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    15257 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/css/s2-docs.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)      916 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/css/theme.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.204699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      916 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-36x36.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1109 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-48x48.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1533 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-72x72.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1894 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-57x57.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1952 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-60x60.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1626 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-72x72.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1586 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-precomposed.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1626 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)      655 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon-16x16.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1155 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon-32x32.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1155 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)      439 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/manifest.json
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1394 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-150x150.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1281 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-310x150.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1546 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-70x70.png
--rw-r--r--   0 jpic      (1000) jpic      (1000)      771 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/safari-pinned-tab.svg
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.204699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/js/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      299 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/js/data-fill-from.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1525 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/package.json
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.168033 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.204699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      149 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/banner.end.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      259 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/banner.start.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      111 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/jquery.mousewheel.shim.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1497 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/jquery.select2.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      357 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/jquery.shim.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.204699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.204699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1455 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/containerCss.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1423 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/dropdownCss.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1121 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/initSelection.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3036 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/inputData.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      955 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/matcher.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      665 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/query.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      971 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/utils.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)    16923 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/core.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.204699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2890 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/ajax.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2094 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/array.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1005 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/base.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      720 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/maximumInputLength.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1360 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/maximumSelectionLength.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      682 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/minimumInputLength.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6038 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/select.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2504 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/tags.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2788 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/tokenizer.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)    12139 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/defaults.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)    16225 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/diacritics.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.208032 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6919 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/attachBody.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      476 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/attachContainer.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      789 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/closeOnSelect.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      976 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/hidePlaceholder.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2273 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/infiniteScroll.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      880 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/minimumResultsForSearch.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3032 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/search.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1214 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/selectOnClose.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      669 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/stopPropagation.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      903 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.211366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1107 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/af.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      988 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ar.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      786 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/az.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1264 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bg.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1611 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bn.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1381 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bs.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1262 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ca.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1743 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/cs.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/da.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1029 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/de.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1544 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/dsb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1519 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/el.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1085 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/en.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1298 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/es.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1150 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/et.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1228 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/eu.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1248 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fa.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      887 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1073 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1134 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/gl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1389 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/he.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1390 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1105 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1545 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hsb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      917 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hu.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1219 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hy.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/id.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1034 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/is.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1211 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/it.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1033 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ja.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1378 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ka.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1260 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/km.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1028 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ko.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1462 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/lt.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1262 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/lv.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1305 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/mk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      892 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ms.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      874 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/nb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1698 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ne.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1165 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/nl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1371 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1338 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ps.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1162 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pt-BR.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1103 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pt.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1201 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ro.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1623 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ru.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1939 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1347 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1156 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sq.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1528 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sr-Cyrl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1396 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      980 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sv.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1245 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/th.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      976 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/tk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      952 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/tr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1475 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/uk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      971 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/vi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      957 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/zh-CN.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      875 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/zh-TW.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      315 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/keys.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4158 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/options.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)    13413 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/results.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.211366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2774 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/allowClear.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4898 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/base.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      652 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/clickMask.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1139 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/eventRelay.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2804 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/multiple.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1290 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/placeholder.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6656 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/search.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2698 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/single.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      710 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/stopPropagation.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      717 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/translation.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     8645 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/utils.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      459 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/wrapper.end.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1250 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/wrapper.start.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.211366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.211366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/a11y/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4642 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/a11y/selection-tests.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.211366 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7952 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/array-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      667 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/base-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3328 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/inputData-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2732 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/maximumInputLength-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3278 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/maximumSelectionLength-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2642 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/minimumInputLength-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)    12543 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/select-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6068 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/tags-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5131 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/tokenizer-tests.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.214699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2982 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/dropdownCss-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2197 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/dropdownParent-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5866 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/positioning-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4899 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/search-a11y-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3155 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/selectOnClose-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      931 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/stopPropagation-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1050 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/helpers.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.214699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6326 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration/dom-changes.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2229 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration/jquery-calls.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2695 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration/select2-methods.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      818 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration-jq1.html
--rw-r--r--   0 jpic      (1000) jpic      (1000)      818 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration-jq2.html
--rw-r--r--   0 jpic      (1000) jpic      (1000)      818 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration-jq3.html
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.214699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1200 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/ajax-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1061 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/data-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5226 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/deprecated-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6156 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/translation-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2208 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/width-tests.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.214699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/results/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      649 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/results/a11y-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5483 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/results/focusing-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2801 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/results/infiniteScroll-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3188 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/results/option-tests.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.214699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     8538 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/allowClear-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3045 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/containerCss-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      908 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/focusing-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5585 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/multiple-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5030 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/openOnKeyDown-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1794 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/placeholder-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6325 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/search-a11y-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1624 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/search-placeholder-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7716 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/search-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4867 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/single-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/stopPropagation-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4765 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/unit-jq1.html
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4765 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/unit-jq2.html
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4765 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/unit-jq3.html
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.214699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/utils/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      927 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/utils/data-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4114 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/utils/decorator-tests.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      954 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/utils/escapeMarkup-tests.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.214699 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/
--rw-r--r--   0 jpic      (1000) jpic      (1000)   252879 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/jquery-1.7.2.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)   257551 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/jquery-2.2.4.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)   280364 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/jquery-3.4.1.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5399 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/qunit-1.23.1.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)   115069 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/qunit-1.23.1.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1071 2020-07-14 22:32:02.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/test.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)    10574 2022-11-22 19:20:07.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6206 2020-10-12 12:17:35.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.218032 django-autocomplete-light-3.9.5rc4/src/dal_select2_queryset_sequence/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      580 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2_queryset_sequence/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2704 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2_queryset_sequence/fields.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3501 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2_queryset_sequence/views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      975 2020-07-14 22:32:02.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2_queryset_sequence/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.218032 django-autocomplete-light-3.9.5rc4/src/dal_select2_tagging/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       50 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2_tagging/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      895 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2_tagging/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.218032 django-autocomplete-light-3.9.5rc4/src/dal_select2_taggit/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       42 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2_taggit/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1834 2020-02-04 10:01:44.000000 django-autocomplete-light-3.9.5rc4/src/dal_select2_taggit/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:57:48.218032 django-autocomplete-light-3.9.5rc4/src/django_autocomplete_light.egg-info/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3209 2023-04-07 16:57:47.000000 django-autocomplete-light-3.9.5rc4/src/django_autocomplete_light.egg-info/PKG-INFO
--rw-r--r--   0 jpic      (1000) jpic      (1000)    38476 2023-04-07 16:57:48.000000 django-autocomplete-light-3.9.5rc4/src/django_autocomplete_light.egg-info/SOURCES.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2023-04-07 16:57:47.000000 django-autocomplete-light-3.9.5rc4/src/django_autocomplete_light.egg-info/dependency_links.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2019-07-20 16:56:42.000000 django-autocomplete-light-3.9.5rc4/src/django_autocomplete_light.egg-info/not-zip-safe
--rw-r--r--   0 jpic      (1000) jpic      (1000)      134 2023-04-07 16:57:47.000000 django-autocomplete-light-3.9.5rc4/src/django_autocomplete_light.egg-info/requires.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)      226 2023-04-07 16:57:47.000000 django-autocomplete-light-3.9.5rc4/src/django_autocomplete_light.egg-info/top_level.txt
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.518032 django-autocomplete-light-3.9.5rc5/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1625 2020-07-14 22:32:02.000000 django-autocomplete-light-3.9.5rc5/AUTHORS
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    46685 2023-04-07 16:59:19.000000 django-autocomplete-light-3.9.5rc5/CHANGELOG
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    46685 2023-04-07 16:59:19.000000 django-autocomplete-light-3.9.5rc5/CHANGES.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1076 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/LICENSE
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      302 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/MANIFEST.in
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3209 2023-04-07 16:59:20.514699 django-autocomplete-light-3.9.5rc5/PKG-INFO
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2221 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/README
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2221 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/README.rst
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       38 2023-04-07 16:59:20.518032 django-autocomplete-light-3.9.5rc5/setup.cfg
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1685 2023-04-07 16:59:19.000000 django-autocomplete-light-3.9.5rc5/setup.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.468032 django-autocomplete-light-3.9.5rc5/src/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       37 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/__init__.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.468032 django-autocomplete-light-3.9.5rc5/src/dal/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      112 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2751 2021-05-03 22:49:43.000000 django-autocomplete-light-3.9.5rc5/src/dal/autocomplete.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6762 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal/forms.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4633 2020-07-14 22:32:02.000000 django-autocomplete-light-3.9.5rc5/src/dal/forward.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.461365 django-autocomplete-light-3.9.5rc5/src/dal/static/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.468032 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    18327 2022-11-22 18:42:05.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/autocomplete_light.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5423 2023-04-07 16:59:18.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/autocomplete_light.min.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      950 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/af.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      989 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ar.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      805 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/az.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1052 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/bg.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1359 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/bn.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1019 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/bs.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      968 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ca.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1364 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/cs.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      912 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/da.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      949 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/de.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1093 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/dsb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1266 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/el.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1005 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/en.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      943 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/eo.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      990 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/es.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      882 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/et.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      948 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/eu.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1107 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/fa.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      887 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/fi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1053 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/fr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      998 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/gl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1056 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/he.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1246 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      936 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1094 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hsb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1003 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hu.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1112 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hy.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      852 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/id.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      890 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/is.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/it.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      946 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ja.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1279 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ka.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1172 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/km.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      939 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ko.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      998 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/lt.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      959 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/lv.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1122 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/mk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      895 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ms.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      862 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/nb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1438 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ne.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      985 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/nl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1450 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/pa.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1022 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/pl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1127 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ps.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      963 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/pt-BR.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      946 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/pt.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1021 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ro.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1233 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ru.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1382 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1009 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      987 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sq.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1168 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sr-Cyrl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1034 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      870 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sv.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1433 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/te.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1158 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/th.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/tk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      859 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/tr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1240 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/uk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      880 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/vi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/zh-CN.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      794 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/zh-TW.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal/test/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       36 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal/test/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3375 2020-02-04 10:01:44.000000 django-autocomplete-light-3.9.5rc5/src/dal/test/case.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    13964 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal/test/stories.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1926 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal/test/utils.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7695 2022-11-22 19:18:36.000000 django-autocomplete-light-3.9.5rc5/src/dal/views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6595 2023-04-07 12:28:05.000000 django-autocomplete-light-3.9.5rc5/src/dal/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_contenttypes/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       53 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_contenttypes/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1962 2020-02-04 10:01:44.000000 django-autocomplete-light-3.9.5rc5/src/dal_contenttypes/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_genericm2m/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       42 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_genericm2m/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      708 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_genericm2m/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_genericm2m_queryset_sequence/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       65 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_genericm2m_queryset_sequence/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      424 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_genericm2m_queryset_sequence/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_gm2m/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       35 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_gm2m/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      534 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_gm2m/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_gm2m_queryset_sequence/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       70 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_gm2m_queryset_sequence/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      377 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_gm2m_queryset_sequence/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       37 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/__init__.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.461365 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.461365 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     8440 2021-05-03 22:49:43.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/css/autocomplete.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.461365 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/css/vendor/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/css/vendor/select2/
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)    17636 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/css/vendor/select2/select2.css
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)    15196 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/css/vendor/select2/select2.min.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1124 2021-05-03 22:49:43.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/autocomplete.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.474699 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.478032 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      887 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ar.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      701 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/az.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      906 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/bg.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      876 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ca.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1236 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/cs.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      818 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/da.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      775 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/de.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1132 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/el.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      827 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/en.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      871 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/es.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      775 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/et.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      844 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/eu.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1004 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fa.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      703 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fi.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      902 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fr.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      800 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/gl.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      951 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/he.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1125 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hi.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      839 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hr.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      727 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hu.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      752 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/id.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      773 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/is.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      876 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/it.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      848 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ja.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1065 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/km.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      854 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ko.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      913 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lt.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      872 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lv.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      979 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/mk.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      791 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ms.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      785 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nb.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      896 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nl.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      925 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pl.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      853 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt-BR.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      859 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      909 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ro.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1127 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ru.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1184 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sk.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1067 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      938 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      786 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sv.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      951 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/th.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      720 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/tr.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1117 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/uk.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      801 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/vi.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      769 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-CN.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      708 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-TW.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)   161832 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)    75005 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.min.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.478032 django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       40 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6355 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.478032 django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/tests/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1545 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/tests/test_views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2298 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1703 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.478032 django-autocomplete-light-3.9.5rc5/src/dal_select2/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      149 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      274 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/apps.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1795 2022-11-22 19:23:02.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/bg/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.478032 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      508 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      671 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/cs/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      528 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      691 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/de/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      501 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      664 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/es/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fi/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      488 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      684 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fr/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/it/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/it/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      498 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      661 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ja/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/nl/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      500 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      663 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pl/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      557 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      723 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pt-br/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pt-br/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      503 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pt-br/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      670 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pt-br/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ru/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      644 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      813 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/tr/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      492 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      741 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/uk/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      582 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      748 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/zh-cn/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/zh-cn/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      458 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      617 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.po
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       46 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/models.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/autocomplete_light/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2765 2022-11-22 18:42:05.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/autocomplete_light/select2.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4937 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/autocomplete_light/select2.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2014 2023-04-07 16:59:18.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/autocomplete_light/select2.min.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6128 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/Gruntfile.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      384 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/bower.json
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      463 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/component.json
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      462 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/composer.json
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    18931 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/css/select2.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    16264 2023-04-07 16:59:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/css/select2.min.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.481365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.488032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      866 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/af.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      905 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ar.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      721 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/az.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      968 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/bg.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1291 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/bn.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      965 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/bs.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      900 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ca.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1292 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/cs.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      828 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/da.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      866 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/de.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1017 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/dsb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1182 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/el.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      844 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/en.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      922 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/es.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      801 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/et.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      868 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/eu.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1023 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/fa.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      803 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/fi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      924 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/fr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      924 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/gl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      984 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/he.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1175 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      852 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1018 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hsb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      831 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hu.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1028 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hy.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      768 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/id.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      807 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/is.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      897 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/it.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      862 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ja.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1195 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ka.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1088 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/km.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ko.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      944 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/lt.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      900 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/lv.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1038 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/mk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      811 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ms.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      778 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/nb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1357 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ne.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      904 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/nl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      947 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/pl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1049 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ps.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      876 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/pt-BR.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      878 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/pt.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      938 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ro.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1171 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ru.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1306 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      925 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      903 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sq.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1109 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sr-Cyrl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      980 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      786 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sv.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1074 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/th.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      771 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/tk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      775 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/tr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1156 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/uk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      796 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/vi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      768 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/zh-CN.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      707 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/zh-TW.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   173566 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/select2.full.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    79212 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/select2.full.min.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   153589 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/select2.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    70891 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/select2.min.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.488032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/assets/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   134486 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/assets/rtfm-screenshot.png
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.488032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.491365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2212 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ak.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2623 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/al.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    10871 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ar.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5448 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/az.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7159 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ca.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2593 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/co.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     9209 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ct.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7903 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/de.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     9018 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/fl.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4765 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ga.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3170 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/hi.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7102 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ia.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7319 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/id.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    10352 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/il.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6988 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/in.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7758 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ks.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    10162 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ky.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    11486 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/la.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3985 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ma.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4103 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/md.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6238 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/me.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    10471 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mi.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7938 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mn.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7495 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mo.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6088 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ms.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7344 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mt.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3995 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nc.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    11795 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nd.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    13899 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ne.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    12792 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nh.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7098 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nj.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1523 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nm.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4268 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nv.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     9732 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ny.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7666 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/oh.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7290 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ok.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     9530 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/or.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    11193 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/pa.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6927 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ri.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4485 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/sc.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    10252 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/sd.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4005 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/tn.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1324 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/tx.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    10674 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ut.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    10138 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/va.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6397 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/vt.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    45254 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wa.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     8539 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wi.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    45254 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wv.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4343 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wy.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2501 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/logo.png
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/anchors/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.491365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/anchors/js/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5272 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/anchors/js/anchor.min.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.491365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/assets/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    61887 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/assets/readme_1.png
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.491365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      295 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/css/breadcrumbs.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/error/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.491365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/error/assets/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    41685 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/error/assets/readme_1.png
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.491365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/assets/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   167622 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/assets/readme_1.png
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1276 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/agate.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      774 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/androidstudio.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1054 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/arduino-light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      852 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/arta.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      591 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/ascetic.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1926 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-cave.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1927 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-cave.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1668 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-dune.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1669 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-dune.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1956 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-estuary.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1957 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-estuary.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1688 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-forest.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1689 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-forest.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1678 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-heath.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1679 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-heath.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1708 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-lakeside.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1709 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-lakeside.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1956 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-plateau.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1957 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-plateau.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1956 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-savanna.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1957 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-savanna.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1698 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-seaside.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1699 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-seaside.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1738 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-sulphurpool.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1739 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-sulphurpool.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      842 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/brown-paper.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      842 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/codepen-embed.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      884 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/color-brewer.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      794 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      890 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/darkula.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      952 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/default.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1141 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/docco.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      849 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/far.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1086 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/foundation.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      919 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/github-gist.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1148 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/github.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1053 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/googlecode.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1966 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/grayscale.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1059 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/hopscotch.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1342 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/hybrid.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1173 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/idea.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      871 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/ir-black.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1067 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/kimbie.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1068 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/kimbie.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      839 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/learn.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      891 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/magula.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      749 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/mono-blue.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1026 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/monokai-sublime.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      938 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/monokai.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1079 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/obsidian.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1014 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso-dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1015 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso-light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1558 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso.dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1559 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso.light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1124 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/pojoaque.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1211 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/railscasts.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      983 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/rainbow.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      999 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/school-book.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1145 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/solarized-dark.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1145 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/solarized-light.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1183 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/sunburst.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1152 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-blue.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1082 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-bright.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1086 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-eighties.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1149 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      978 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      837 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/vs.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1071 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/xcode.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      947 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/zenburn.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    44929 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/highlight.pack.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      794 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/highlightjs-line-numbers.min.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/assets/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    72908 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/assets/readme_1.png
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1155 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/problems.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    21132 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/template.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/html/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1164 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/html/problems.html
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.464699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   113109 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/readme_1.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/search.svg
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      514 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/css/simplesearch.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/js/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1089 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/js/simplesearch.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.468032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.468032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1448 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/featherlight.min.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    31000 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/font-awesome.min.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      117 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/nucleus-ie10.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      575 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/nucleus-ie9.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/pure-0.5.0/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3857 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/pure-0.5.0/grids-min.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    11928 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/nucleus.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    23480 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/theme.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.498032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   165742 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   444379 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   165548 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    98024 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.woff
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.501365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      519 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/clippy.svg
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1177 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/favicon.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1215 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/logo.png
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.501365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     8855 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/clipboard.min.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7257 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/featherlight.min.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4133 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    12188 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/jquery.scrollbar.min.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    11180 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/learn.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     9093 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/modernizr.custom.71422.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.468032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.501365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    15257 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/css/s2-docs.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      916 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/css/theme.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.501365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      916 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-36x36.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1109 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-48x48.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1533 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-72x72.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1894 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-57x57.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1952 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-60x60.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1626 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-72x72.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1586 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-precomposed.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1626 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      655 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon-16x16.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1155 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon-32x32.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1155 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      439 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/manifest.json
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1394 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-150x150.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1281 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-310x150.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1546 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-70x70.png
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      771 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/safari-pinned-tab.svg
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.501365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/js/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      299 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/js/data-fill-from.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1525 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/package.json
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.468032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.501365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      149 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/banner.end.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      259 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/banner.start.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      111 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/jquery.mousewheel.shim.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1497 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/jquery.select2.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      357 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/jquery.shim.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.504699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.504699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1455 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/containerCss.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1423 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/dropdownCss.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1121 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/initSelection.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3036 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/inputData.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      955 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/matcher.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      665 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/query.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      971 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/utils.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    16923 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/core.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.504699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2890 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/ajax.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2094 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/array.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1005 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/base.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      720 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/maximumInputLength.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1360 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/maximumSelectionLength.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      682 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/minimumInputLength.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6038 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/select.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2504 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/tags.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2788 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/tokenizer.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    12139 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/defaults.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    16225 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/diacritics.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.504699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6919 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/attachBody.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      476 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/attachContainer.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      789 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/closeOnSelect.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      976 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/hidePlaceholder.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2273 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/infiniteScroll.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      880 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/minimumResultsForSearch.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3032 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/search.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1214 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/selectOnClose.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      669 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/stopPropagation.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      903 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.508032 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1107 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/af.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      988 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ar.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      786 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/az.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1264 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bg.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1611 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bn.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1381 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bs.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1262 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ca.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1743 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/cs.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/da.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1029 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/de.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1544 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/dsb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1519 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/el.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1085 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/en.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1298 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/es.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1150 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/et.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1228 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/eu.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1248 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fa.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      887 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1073 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1134 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/gl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1389 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/he.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1390 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1105 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1545 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hsb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      917 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hu.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1219 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hy.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/id.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1034 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/is.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1211 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/it.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1033 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ja.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1378 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ka.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1260 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/km.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1028 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ko.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1462 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/lt.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1262 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/lv.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1305 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/mk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      892 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ms.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      874 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/nb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1698 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ne.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1165 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/nl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1371 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1338 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ps.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1162 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pt-BR.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1103 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pt.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1201 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ro.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1623 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ru.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1939 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1347 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1156 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sq.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1528 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sr-Cyrl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1396 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      980 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sv.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1245 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/th.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      976 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/tk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      952 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/tr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1475 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/uk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      971 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/vi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      957 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/zh-CN.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      875 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/zh-TW.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      315 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/keys.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4158 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/options.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    13413 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/results.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.511365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2774 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/allowClear.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4898 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/base.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      652 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/clickMask.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1139 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/eventRelay.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2804 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/multiple.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1290 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/placeholder.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6656 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/search.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2698 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/single.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      710 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/stopPropagation.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      717 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/translation.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     8645 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/utils.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      459 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/wrapper.end.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1250 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/wrapper.start.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.511365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.511365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/a11y/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4642 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/a11y/selection-tests.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.511365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7952 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/array-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      667 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/base-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3328 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/inputData-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2732 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/maximumInputLength-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3278 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/maximumSelectionLength-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2642 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/minimumInputLength-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    12543 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/select-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6068 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/tags-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5131 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/tokenizer-tests.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.511365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2982 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/dropdownCss-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2197 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/dropdownParent-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5866 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/positioning-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4899 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/search-a11y-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3155 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/selectOnClose-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      931 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/stopPropagation-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1050 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/helpers.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.511365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6326 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration/dom-changes.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2229 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration/jquery-calls.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2695 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration/select2-methods.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      818 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration-jq1.html
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      818 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration-jq2.html
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      818 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration-jq3.html
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.511365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1200 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/ajax-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1061 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/data-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5226 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/deprecated-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6156 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/translation-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2208 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/width-tests.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.511365 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/results/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      649 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/results/a11y-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5483 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/results/focusing-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2801 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/results/infiniteScroll-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3188 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/results/option-tests.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.514699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     8538 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/allowClear-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3045 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/containerCss-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      908 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/focusing-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5585 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/multiple-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5030 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/openOnKeyDown-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1794 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/placeholder-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6325 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/search-a11y-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1624 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/search-placeholder-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7716 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/search-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4867 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/single-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/stopPropagation-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4765 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/unit-jq1.html
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4765 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/unit-jq2.html
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4765 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/unit-jq3.html
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.514699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/utils/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      927 2021-03-15 02:05:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/utils/data-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4114 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/utils/decorator-tests.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      954 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/utils/escapeMarkup-tests.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.514699 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   252879 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/jquery-1.7.2.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   257551 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/jquery-2.2.4.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   280364 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/jquery-3.4.1.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5399 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/qunit-1.23.1.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)   115069 2019-07-20 16:55:17.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/qunit-1.23.1.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1071 2020-07-14 22:32:02.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/test.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    10574 2022-11-22 19:20:07.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6206 2020-10-12 12:17:35.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.514699 django-autocomplete-light-3.9.5rc5/src/dal_select2_queryset_sequence/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      580 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2_queryset_sequence/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2704 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2_queryset_sequence/fields.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3501 2022-11-22 18:30:38.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2_queryset_sequence/views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      975 2020-07-14 22:32:02.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2_queryset_sequence/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.514699 django-autocomplete-light-3.9.5rc5/src/dal_select2_tagging/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       50 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2_tagging/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      895 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2_tagging/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.514699 django-autocomplete-light-3.9.5rc5/src/dal_select2_taggit/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       42 2019-07-20 16:54:41.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2_taggit/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1834 2020-02-04 10:01:44.000000 django-autocomplete-light-3.9.5rc5/src/dal_select2_taggit/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-04-07 16:59:20.514699 django-autocomplete-light-3.9.5rc5/src/django_autocomplete_light.egg-info/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3209 2023-04-07 16:59:20.000000 django-autocomplete-light-3.9.5rc5/src/django_autocomplete_light.egg-info/PKG-INFO
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    38476 2023-04-07 16:59:20.000000 django-autocomplete-light-3.9.5rc5/src/django_autocomplete_light.egg-info/SOURCES.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2023-04-07 16:59:20.000000 django-autocomplete-light-3.9.5rc5/src/django_autocomplete_light.egg-info/dependency_links.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2019-07-20 16:56:42.000000 django-autocomplete-light-3.9.5rc5/src/django_autocomplete_light.egg-info/not-zip-safe
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      134 2023-04-07 16:59:20.000000 django-autocomplete-light-3.9.5rc5/src/django_autocomplete_light.egg-info/requires.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      226 2023-04-07 16:59:20.000000 django-autocomplete-light-3.9.5rc5/src/django_autocomplete_light.egg-info/top_level.txt
```

### Comparing `django-autocomplete-light-3.9.5rc4/AUTHORS` & `django-autocomplete-light-3.9.5rc5/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/CHANGELOG` & `django-autocomplete-light-3.9.5rc5/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 3.9.5-rc4
 
 
 3.9.5-rc3,
 
     2023-4-7 Release 3.9.5-rc3
     0cd3b7b Support releases without rebuild by jpic
```

### Comparing `django-autocomplete-light-3.9.5rc4/CHANGES.txt` & `django-autocomplete-light-3.9.5rc5/CHANGES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 3.9.5-rc4
 
 
 3.9.5-rc3,
 
     2023-4-7 Release 3.9.5-rc3
     0cd3b7b Support releases without rebuild by jpic
```

### Comparing `django-autocomplete-light-3.9.5rc4/LICENSE` & `django-autocomplete-light-3.9.5rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/PKG-INFO` & `django-autocomplete-light-3.9.5rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-autocomplete-light
-Version: 3.9.5rc4
+Version: 3.9.5rc5
 Summary: Fresh autocompletes for Django
 Home-page: http://django-autocomplete-light.rtfd.org
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/yourlabs/django-autocomplete-light
 Keywords: django autocomplete
```

### Comparing `django-autocomplete-light-3.9.5rc4/README` & `django-autocomplete-light-3.9.5rc5/README`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/README.rst` & `django-autocomplete-light-3.9.5rc5/README.rst`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/setup.py` & `django-autocomplete-light-3.9.5rc5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='django-autocomplete-light',
-    version='3.9.5-rc4',
+    version='3.9.5-rc5',
     description='Fresh autocompletes for Django',
     author='James Pic',
     author_email='jamespic@gmail.com',
     url='http://django-autocomplete-light.rtfd.org',
     project_urls={
         'Source': 'https://github.com/yourlabs/django-autocomplete-light',
     },
```

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/autocomplete.py` & `django-autocomplete-light-3.9.5rc5/src/dal/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/forms.py` & `django-autocomplete-light-3.9.5rc5/src/dal/forms.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/forward.py` & `django-autocomplete-light-3.9.5rc5/src/dal/forward.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/autocomplete_light.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/autocomplete_light.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/autocomplete_light.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/autocomplete_light.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/af.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/af.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ar.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/az.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/az.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/bg.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/bn.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/bs.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ca.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/cs.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/da.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/da.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/de.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/dsb.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/el.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/el.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/en.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/eo.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/eo.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/es.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/et.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/et.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/eu.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/fa.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/fi.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/fr.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/gl.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/he.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/he.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hi.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hr.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hsb.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hu.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/hy.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/id.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/id.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/is.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/is.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/it.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ja.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ka.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/km.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/km.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ko.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/lt.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/lv.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/mk.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ms.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/nb.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ne.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/nl.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/pa.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/pa.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/pl.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ps.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/pt-BR.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/pt.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ro.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/ru.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sk.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sl.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sq.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sr-Cyrl.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sr.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/sv.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/te.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/te.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/th.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/th.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/tk.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/tr.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/uk.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/vi.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/zh-CN.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/static/autocomplete_light/i18n/zh-TW.js` & `django-autocomplete-light-3.9.5rc5/src/dal/static/autocomplete_light/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/test/case.py` & `django-autocomplete-light-3.9.5rc5/src/dal/test/case.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/test/stories.py` & `django-autocomplete-light-3.9.5rc5/src/dal/test/stories.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/test/utils.py` & `django-autocomplete-light-3.9.5rc5/src/dal/test/utils.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/views.py` & `django-autocomplete-light-3.9.5rc5/src/dal/views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal/widgets.py` & `django-autocomplete-light-3.9.5rc5/src/dal/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_contenttypes/fields.py` & `django-autocomplete-light-3.9.5rc5/src/dal_contenttypes/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_genericm2m/fields.py` & `django-autocomplete-light-3.9.5rc5/src/dal_genericm2m/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_gm2m/fields.py` & `django-autocomplete-light-3.9.5rc5/src/dal_gm2m/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/css/autocomplete.css` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/css/vendor/select2/select2.css` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/css/vendor/select2/select2.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/css/vendor/select2/select2.min.css` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/css/vendor/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/autocomplete.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ar.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/az.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/bg.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ca.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/cs.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/da.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/de.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/el.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/el.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/en.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/es.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/et.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/eu.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fa.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fi.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/gl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/he.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hi.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hu.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/id.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/is.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/it.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ja.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/km.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/km.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ko.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lt.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lv.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/mk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ms.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nb.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt-BR.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ro.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ru.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr-Cyrl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sv.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/th.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/tr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/uk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/vi.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-CN.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-TW.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/fields.py` & `django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/tests/test_views.py` & `django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/views.py` & `django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_queryset_sequence/widgets.py` & `django-autocomplete-light-3.9.5rc5/src/dal_queryset_sequence/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/fields.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/bg/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/cs/LC_MESSAGES/django.mo` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/cs/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/de/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/es/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fi/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/fr/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/it/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ja/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/nl/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pl/LC_MESSAGES/django.mo` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pl/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/pt-br/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/pt-br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ru/LC_MESSAGES/django.mo` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/ru/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/tr/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/uk/LC_MESSAGES/django.mo` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/uk/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/autocomplete_light/select2.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/autocomplete_light/select2.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/autocomplete_light/select2.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/autocomplete_light/select2.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/autocomplete_light/select2.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/autocomplete_light/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/Gruntfile.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/Gruntfile.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/css/select2.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/css/select2.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/css/select2.min.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/af.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/af.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ar.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/az.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/az.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/bg.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/bn.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/bs.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ca.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/cs.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/da.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/da.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/de.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/dsb.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/el.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/el.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/en.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/es.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/et.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/et.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/eu.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/fa.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/fi.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/fr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/gl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/he.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/he.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hi.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hsb.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hu.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/hy.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/id.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/id.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/is.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/is.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/it.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ja.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ka.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/km.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/km.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ko.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/lt.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/lv.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/mk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ms.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/nb.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ne.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/nl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/pl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ps.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/pt-BR.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/pt.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ro.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/ru.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sq.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sr-Cyrl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/sv.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/th.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/th.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/tk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/tr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/uk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/vi.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/zh-CN.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/i18n/zh-TW.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/select2.full.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/select2.full.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/select2.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/select2.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/dist/js/select2.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/dist/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/assets/rtfm-screenshot.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/assets/rtfm-screenshot.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ak.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ak.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/al.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/al.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ar.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ar.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/az.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/az.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ca.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ca.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/co.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/co.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ct.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ct.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/de.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/de.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/fl.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/fl.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ga.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ga.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/hi.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/hi.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ia.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ia.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/id.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/id.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/il.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/il.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/in.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/in.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ks.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ks.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ky.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ky.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/la.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/la.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ma.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ma.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/md.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/md.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/me.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/me.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mi.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mi.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mn.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mn.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mo.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mo.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ms.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ms.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mt.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/mt.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nc.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nc.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nd.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nd.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ne.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ne.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nh.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nh.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nj.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nj.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nm.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nm.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nv.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/nv.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ny.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ny.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/oh.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/oh.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ok.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ok.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/or.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/or.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/pa.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/pa.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ri.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ri.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/sc.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/sc.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/sd.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/sd.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/tn.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/tn.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/tx.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/tx.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ut.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/ut.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/va.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/va.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/vt.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/vt.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wa.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wa.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wi.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wi.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wv.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wv.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wy.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/flags/wy.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/pages/images/logo.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/pages/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/anchors/js/anchor.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/anchors/js/anchor.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/assets/readme_1.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/breadcrumbs/assets/readme_1.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/error/assets/readme_1.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/error/assets/readme_1.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/assets/readme_1.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/assets/readme_1.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/agate.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/agate.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/androidstudio.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/androidstudio.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/arduino-light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/arduino-light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/arta.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/arta.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/ascetic.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/ascetic.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-cave.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-cave.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-cave.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-cave.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-dune.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-dune.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-dune.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-dune.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-estuary.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-estuary.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-estuary.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-estuary.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-forest.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-forest.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-forest.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-forest.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-heath.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-heath.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-heath.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-heath.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-lakeside.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-lakeside.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-lakeside.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-lakeside.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-plateau.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-plateau.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-plateau.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-plateau.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-savanna.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-savanna.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-savanna.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-savanna.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-seaside.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-seaside.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-seaside.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-seaside.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-sulphurpool.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-sulphurpool.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-sulphurpool.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/atelier-sulphurpool.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/brown-paper.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/brown-paper.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/codepen-embed.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/codepen-embed.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/color-brewer.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/color-brewer.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/darkula.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/darkula.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/default.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/default.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/docco.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/docco.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/far.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/far.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/foundation.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/foundation.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/github-gist.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/github-gist.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/github.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/github.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/googlecode.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/googlecode.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/grayscale.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/grayscale.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/hopscotch.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/hopscotch.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/hybrid.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/hybrid.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/idea.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/idea.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/ir-black.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/ir-black.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/kimbie.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/kimbie.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/kimbie.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/kimbie.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/learn.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/learn.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/magula.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/magula.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/mono-blue.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/mono-blue.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/monokai-sublime.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/monokai-sublime.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/monokai.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/monokai.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/obsidian.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/obsidian.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso-dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso-dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso-light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso-light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso.dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso.dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso.light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/paraiso.light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/pojoaque.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/pojoaque.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/railscasts.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/railscasts.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/rainbow.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/rainbow.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/school-book.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/school-book.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/solarized-dark.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/solarized-light.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/solarized-light.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/sunburst.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/sunburst.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-blue.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-blue.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-bright.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-bright.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-eighties.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night-eighties.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow-night.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/tomorrow.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/vs.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/vs.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/xcode.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/xcode.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/zenburn.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/css/zenburn.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/highlight.pack.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/highlightjs-line-numbers.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/highlight/js/highlightjs-line-numbers.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/assets/readme_1.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/assets/readme_1.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/problems.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/problems.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/template.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/css/template.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/problems/html/problems.html` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/problems/html/problems.html`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/readme_1.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/readme_1.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/search.svg` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/assets/search.svg`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/css/simplesearch.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/css/simplesearch.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/js/simplesearch.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/plugins/simplesearch/js/simplesearch.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/featherlight.min.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/featherlight.min.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/font-awesome.min.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/nucleus-ie9.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/nucleus-ie9.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/pure-0.5.0/grids-min.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css/pure-0.5.0/grids-min.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/nucleus.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/nucleus.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/theme.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/css-compiled/theme.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.eot` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.svg` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.ttf` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.woff` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/clippy.svg` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/clippy.svg`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/favicon.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/logo.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/clipboard.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/featherlight.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/featherlight.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/html5shiv-printshiv.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/jquery.scrollbar.min.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/jquery.scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/learn.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/learn.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/modernizr.custom.71422.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/learn2/js/modernizr.custom.71422.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/css/s2-docs.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/css/s2-docs.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/css/theme.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/css/theme.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-36x36.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-36x36.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-48x48.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-48x48.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-72x72.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/android-chrome-72x72.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-57x57.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-60x60.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-72x72.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-precomposed.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon-16x16.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon-32x32.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-150x150.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-310x150.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-70x70.png` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/docs/themes/site/images/safari-pinned-tab.svg` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/docs/themes/site/images/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/package.json` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/package.json`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/jquery.select2.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/jquery.select2.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/containerCss.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/containerCss.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/dropdownCss.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/dropdownCss.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/initSelection.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/initSelection.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/inputData.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/inputData.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/matcher.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/matcher.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/query.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/query.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/compat/utils.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/compat/utils.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/core.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/core.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/ajax.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/ajax.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/array.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/array.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/base.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/base.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/maximumInputLength.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/maximumInputLength.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/maximumSelectionLength.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/maximumSelectionLength.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/minimumInputLength.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/minimumInputLength.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/select.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/select.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/tags.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/tags.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/data/tokenizer.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/data/tokenizer.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/defaults.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/defaults.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/diacritics.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/diacritics.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/attachBody.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/attachBody.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/closeOnSelect.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/closeOnSelect.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/hidePlaceholder.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/hidePlaceholder.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/infiniteScroll.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/infiniteScroll.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/minimumResultsForSearch.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/minimumResultsForSearch.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/search.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/search.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/selectOnClose.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/selectOnClose.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/stopPropagation.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown/stopPropagation.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/dropdown.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/dropdown.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/af.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/af.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ar.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/az.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bg.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bn.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bs.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ca.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/cs.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/da.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/de.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/dsb.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/el.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/el.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/en.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/es.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/et.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/eu.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fa.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fi.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/gl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/he.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hi.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hsb.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hu.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hy.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/id.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/is.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/it.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ja.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ka.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/km.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/km.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ko.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/lt.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/lv.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/mk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ms.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/nb.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ne.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/nl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ps.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pt-BR.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pt.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ro.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ru.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sq.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sr-Cyrl.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sv.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/th.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/tk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/tr.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/uk.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/vi.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/zh-CN.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/i18n/zh-TW.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/options.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/options.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/results.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/results.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/allowClear.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/allowClear.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/base.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/base.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/clickMask.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/clickMask.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/eventRelay.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/eventRelay.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/multiple.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/multiple.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/placeholder.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/placeholder.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/search.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/search.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/single.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/single.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/selection/stopPropagation.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/selection/stopPropagation.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/translation.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/translation.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/select2/utils.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/select2/utils.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/src/js/wrapper.start.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/src/js/wrapper.start.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/a11y/selection-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/a11y/selection-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/array-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/array-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/base-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/base-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/inputData-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/inputData-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/maximumInputLength-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/maximumInputLength-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/maximumSelectionLength-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/maximumSelectionLength-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/minimumInputLength-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/minimumInputLength-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/select-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/select-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/tags-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/tags-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/data/tokenizer-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/data/tokenizer-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/dropdownCss-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/dropdownCss-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/dropdownParent-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/dropdownParent-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/positioning-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/positioning-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/search-a11y-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/search-a11y-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/selectOnClose-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/selectOnClose-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/dropdown/stopPropagation-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/dropdown/stopPropagation-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/helpers.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/helpers.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration/dom-changes.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration/dom-changes.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration/jquery-calls.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration/jquery-calls.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration/select2-methods.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration/select2-methods.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration-jq1.html` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration-jq1.html`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration-jq2.html` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration-jq2.html`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/integration-jq3.html` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/integration-jq3.html`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/ajax-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/ajax-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/data-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/data-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/deprecated-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/deprecated-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/translation-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/translation-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/options/width-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/options/width-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/results/a11y-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/results/a11y-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/results/focusing-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/results/focusing-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/results/infiniteScroll-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/results/infiniteScroll-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/results/option-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/results/option-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/allowClear-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/allowClear-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/containerCss-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/containerCss-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/focusing-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/focusing-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/multiple-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/multiple-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/openOnKeyDown-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/openOnKeyDown-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/placeholder-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/placeholder-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/search-a11y-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/search-a11y-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/search-placeholder-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/search-placeholder-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/search-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/search-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/single-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/single-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/selection/stopPropagation-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/selection/stopPropagation-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/unit-jq1.html` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/unit-jq1.html`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/unit-jq2.html` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/unit-jq2.html`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/unit-jq3.html` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/unit-jq3.html`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/utils/data-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/utils/data-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/utils/decorator-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/utils/decorator-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/utils/escapeMarkup-tests.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/utils/escapeMarkup-tests.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/jquery-1.7.2.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/jquery-1.7.2.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/jquery-2.2.4.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/jquery-2.2.4.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/jquery-3.4.1.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/qunit-1.23.1.css` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/qunit-1.23.1.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/static/vendor/select2/tests/vendor/qunit-1.23.1.js` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/static/vendor/select2/tests/vendor/qunit-1.23.1.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/test.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/test.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/views.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2/widgets.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2_queryset_sequence/__init__.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2_queryset_sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2_queryset_sequence/fields.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2_queryset_sequence/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2_queryset_sequence/views.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2_queryset_sequence/views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2_queryset_sequence/widgets.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2_queryset_sequence/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2_tagging/widgets.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2_tagging/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/dal_select2_taggit/widgets.py` & `django-autocomplete-light-3.9.5rc5/src/dal_select2_taggit/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.5rc4/src/django_autocomplete_light.egg-info/PKG-INFO` & `django-autocomplete-light-3.9.5rc5/src/django_autocomplete_light.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-autocomplete-light
-Version: 3.9.5rc4
+Version: 3.9.5rc5
 Summary: Fresh autocompletes for Django
 Home-page: http://django-autocomplete-light.rtfd.org
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/yourlabs/django-autocomplete-light
 Keywords: django autocomplete
```

### Comparing `django-autocomplete-light-3.9.5rc4/src/django_autocomplete_light.egg-info/SOURCES.txt` & `django-autocomplete-light-3.9.5rc5/src/django_autocomplete_light.egg-info/SOURCES.txt`

 * *Files identical despite different names*

