# Comparing `tmp/python-geofs-0.1.4rc2.tar.gz` & `tmp/python-geofs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-geofs-0.1.4rc2.tar", last modified: Mon Apr  3 17:32:23 2023, max compression
+gzip compressed data, was "python-geofs-0.1.5.tar", last modified: Fri Apr  7 17:59:50 2023, max compression
```

## Comparing `python-geofs-0.1.4rc2.tar` & `python-geofs-0.1.5.tar`

### file list

```diff
@@ -1,1887 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.167474 python-geofs-0.1.4rc2/
--rw-rw-rw-   0        0        0       84 2023-04-02 00:10:51.000000 python-geofs-0.1.4rc2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1045 2023-04-01 14:20:41.000000 python-geofs-0.1.4rc2/LICENSE.txt
--rw-rw-rw-   0        0        0       66 2023-04-03 17:31:36.000000 python-geofs-0.1.4rc2/MANIFEST.in
--rw-rw-rw-   0        0        0      308 2023-04-03 17:32:23.166478 python-geofs-0.1.4rc2/PKG-INFO
--rw-rw-rw-   0        0        0     2166 2023-04-02 00:07:29.000000 python-geofs-0.1.4rc2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.810475 python-geofs-0.1.4rc2/geofs/
--rw-rw-rw-   0        0        0       95 2023-04-03 17:21:28.000000 python-geofs-0.1.4rc2/geofs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.131479 python-geofs-0.1.4rc2/geofs/data/
--rw-rw-rw-   0        0        0     7411 2023-04-03 16:34:02.000000 python-geofs-0.1.4rc2/geofs/data/aircraftcodes.json
--rw-rw-rw-   0        0        0     3176 2023-04-03 17:21:36.000000 python-geofs-0.1.4rc2/geofs/mapAPI.py
--rw-rw-rw-   0        0        0     5371 2023-04-03 17:21:47.000000 python-geofs-0.1.4rc2/geofs/multiplayerAPI.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.788478 python-geofs-0.1.4rc2/geofs-env/
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.572490 python-geofs-0.1.4rc2/geofs-env/Lib/
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.813476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.818483 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/Pygments-2.14.0.dist-info/
--rw-rw-rw-   0        0        0       53 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/Pygments-2.14.0.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/Pygments-2.14.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.822483 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/_distutils_hack/
--rw-rw-rw-   0        0        0     6128 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/_distutils_hack/__init__.py
--rw-rw-rw-   0        0        0       44 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/_distutils_hack/override.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.844476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/
--rw-rw-rw-   0        0        0     3649 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.854476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.877475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/
--rw-rw-rw-   0        0        0     1143 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/__init__.py
--rw-rw-rw-   0        0        0    16728 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/_ihatexml.py
--rw-rw-rw-   0        0        0    32300 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/_inputstream.py
--rw-rw-rw-   0        0        0    77028 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.887474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/_trie/
--rw-rw-rw-   0        0        0      109 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
--rw-rw-rw-   0        0        0     1013 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/_trie/_base.py
--rw-rw-rw-   0        0        0     1763 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/_trie/py.py
--rw-rw-rw-   0        0        0     4919 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/_utils.py
--rw-rw-rw-   0        0        0    83464 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.915475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/filters/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/filters/__init__.py
--rw-rw-rw-   0        0        0      919 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-rw-rw-   0        0        0      286 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/filters/base.py
--rw-rw-rw-   0        0        0     2945 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
--rw-rw-rw-   0        0        0     3631 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/filters/lint.py
--rw-rw-rw-   0        0        0    10588 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
--rw-rw-rw-   0        0        0    26885 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
--rw-rw-rw-   0        0        0     1214 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
--rw-rw-rw-   0        0        0   117174 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/html5parser.py
--rw-rw-rw-   0        0        0    15747 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/serializer.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.925475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/
--rw-rw-rw-   0        0        0      650 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
--rw-rw-rw-   0        0        0     1715 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
--rw-rw-rw-   0        0        0     1776 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.941475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/
--rw-rw-rw-   0        0        0     3592 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
--rw-rw-rw-   0        0        0    14553 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
--rw-rw-rw-   0        0        0     8925 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
--rw-rw-rw-   0        0        0    12824 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
--rw-rw-rw-   0        0        0    14754 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.957488 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/
--rw-rw-rw-   0        0        0     5719 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
--rw-rw-rw-   0        0        0     7476 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
--rw-rw-rw-   0        0        0     1413 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
--rw-rw-rw-   0        0        0     4539 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
--rw-rw-rw-   0        0        0     6345 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-rw-rw-   0        0        0     2309 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.879476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/
--rw-rw-rw-   0        0        0        9 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
--rw-rw-rw-   0        0        0    39023 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/parse.py
--rw-rw-rw-   0        0        0      184 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/_vendor/vendor.txt
--rw-rw-rw-   0        0        0      752 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/callbacks.py
--rw-rw-rw-   0        0        0     2526 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/css_sanitizer.py
--rw-rw-rw-   0        0        0    22779 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/html5lib_shim.py
--rw-rw-rw-   0        0        0    22350 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/linkifier.py
--rw-rw-rw-   0        0        0       50 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/parse_shim.py
--rw-rw-rw-   0        0        0    21934 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach/sanitizer.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.847476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach-6.0.0.dist-info/
--rw-rw-rw-   0        0        0        7 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/bleach-6.0.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.968477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/certifi/
--rw-rw-rw-   0        0        0       94 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/certifi/__init__.py
--rw-rw-rw-   0        0        0      243 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/certifi/__main__.py
--rw-rw-rw-   0        0        0     4219 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/certifi/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.971479 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/certifi-2022.12.7.dist-info/
--rw-rw-rw-   0        0        0        8 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/certifi-2022.12.7.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.998478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/
--rw-rw-rw-   0        0        0     1594 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/__init__.py
--rw-rw-rw-   0        0        0    19178 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/api.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.007475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/assets/
--rw-rw-rw-   0        0        0    21509 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/assets/__init__.py
--rw-rw-rw-   0        0        0    12944 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/cd.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.012475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/cli/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/cli/__init__.py
--rw-rw-rw-   0        0        0    10040 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/cli/normalizer.py
--rw-rw-rw-   0        0        0    19596 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/constant.py
--rw-rw-rw-   0        0        0     2125 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/legacy.py
--rw-rw-rw-   0        0        0    18829 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/md.py
--rw-rw-rw-   0        0        0    11829 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/models.py
--rw-rw-rw-   0        0        0    11958 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/utils.py
--rw-rw-rw-   0        0        0       85 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.004475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer-3.1.0.dist-info/
--rw-rw-rw-   0        0        0       76 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer-3.1.0.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/charset_normalizer-3.1.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.037475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/
--rw-rw-rw-   0        0        0    10039 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/__init__.py
--rw-rw-rw-   0        0        0     3588 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/__main__.py
--rw-rw-rw-   0        0        0    30945 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/core.py
--rw-rw-rw-   0        0        0     3961 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/examples.py
--rw-rw-rw-   0        0        0    39697 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/frontend.py
--rw-rw-rw-   0        0        0    21271 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/io.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.120478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/
--rw-rw-rw-   0        0        0     2921 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/__init__.py
--rw-rw-rw-   0        0        0     1831 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/af.py
--rw-rw-rw-   0        0        0     1943 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/ar.py
--rw-rw-rw-   0        0        0     1912 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/ca.py
--rw-rw-rw-   0        0        0     1900 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/cs.py
--rw-rw-rw-   0        0        0     1856 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/da.py
--rw-rw-rw-   0        0        0     1728 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/de.py
--rw-rw-rw-   0        0        0     1854 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/en.py
--rw-rw-rw-   0        0        0     1931 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/eo.py
--rw-rw-rw-   0        0        0     1906 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/es.py
--rw-rw-rw-   0        0        0     1958 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/fa.py
--rw-rw-rw-   0        0        0     1964 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/fi.py
--rw-rw-rw-   0        0        0     1831 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/fr.py
--rw-rw-rw-   0        0        0     1990 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/gl.py
--rw-rw-rw-   0        0        0     2692 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/he.py
--rw-rw-rw-   0        0        0     1814 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/it.py
--rw-rw-rw-   0        0        0     1890 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/ja.py
--rw-rw-rw-   0        0        0     1832 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/ko.py
--rw-rw-rw-   0        0        0     1919 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/lt.py
--rw-rw-rw-   0        0        0     1851 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/lv.py
--rw-rw-rw-   0        0        0     1871 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/nl.py
--rw-rw-rw-   0        0        0     1866 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/pl.py
--rw-rw-rw-   0        0        0     1929 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/pt_br.py
--rw-rw-rw-   0        0        0     2070 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/ru.py
--rw-rw-rw-   0        0        0     1832 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/sk.py
--rw-rw-rw-   0        0        0     1863 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/sv.py
--rw-rw-rw-   0        0        0     1974 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/zh_cn.py
--rw-rw-rw-   0        0        0     2742 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/languages/zh_tw.py
--rw-rw-rw-   0        0        0    80986 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/nodes.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.131476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/
--rw-rw-rw-   0        0        0     3724 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/__init__.py
--rw-rw-rw-   0        0        0     1765 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/commonmark_wrapper.py
--rw-rw-rw-   0        0        0      445 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/null.py
--rw-rw-rw-   0        0        0     5100 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/recommonmark_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.143475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/
--rw-rw-rw-   0        0        0    15985 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.167476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/
--rw-rw-rw-   0        0        0    14653 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/__init__.py
--rw-rw-rw-   0        0        0     2405 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/admonitions.py
--rw-rw-rw-   0        0        0     9883 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/body.py
--rw-rw-rw-   0        0        0      695 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/html.py
--rw-rw-rw-   0        0        0     6799 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/images.py
--rw-rw-rw-   0        0        0    26770 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/misc.py
--rw-rw-rw-   0        0        0     4247 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/parts.py
--rw-rw-rw-   0        0        0      831 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/references.py
--rw-rw-rw-   0        0        0    22227 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/directives/tables.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.261475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/
--rw-rw-rw-   0        0        0      670 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/README.txt
--rw-rw-rw-   0        0        0    10925 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isoamsa.txt
--rw-rw-rw-   0        0        0     7242 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isoamsb.txt
--rw-rw-rw-   0        0        0     1723 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isoamsc.txt
--rw-rw-rw-   0        0        0     6721 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isoamsn.txt
--rw-rw-rw-   0        0        0     3825 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isoamso.txt
--rw-rw-rw-   0        0        0    11763 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isoamsr.txt
--rw-rw-rw-   0        0        0     3101 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isobox.txt
--rw-rw-rw-   0        0        0     4241 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isocyr1.txt
--rw-rw-rw-   0        0        0     1882 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isocyr2.txt
--rw-rw-rw-   0        0        0      869 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isodia.txt
--rw-rw-rw-   0        0        0     3010 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isogrk1.txt
--rw-rw-rw-   0        0        0     1705 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isogrk2.txt
--rw-rw-rw-   0        0        0     2880 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isogrk3.txt
--rw-rw-rw-   0        0        0     3035 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
--rw-rw-rw-   0        0        0      372 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isogrk4.txt
--rw-rw-rw-   0        0        0     4397 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isolat1.txt
--rw-rw-rw-   0        0        0     8466 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isolat2.txt
--rw-rw-rw-   0        0        0     3334 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
--rw-rw-rw-   0        0        0      519 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isomfrk.txt
--rw-rw-rw-   0        0        0     1931 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
--rw-rw-rw-   0        0        0      639 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isomopf.txt
--rw-rw-rw-   0        0        0     3231 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
--rw-rw-rw-   0        0        0      776 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isomscr.txt
--rw-rw-rw-   0        0        0     4066 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isonum.txt
--rw-rw-rw-   0        0        0     4613 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isopub.txt
--rw-rw-rw-   0        0        0     9726 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/isotech.txt
--rw-rw-rw-   0        0        0    45428 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/mmlalias.txt
--rw-rw-rw-   0        0        0     9010 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
--rw-rw-rw-   0        0        0     6800 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/mmlextra.txt
--rw-rw-rw-   0        0        0     1036 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/s5defs.txt
--rw-rw-rw-   0        0        0     6112 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
--rw-rw-rw-   0        0        0     1945 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
--rw-rw-rw-   0        0        0     7028 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.333476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/
--rw-rw-rw-   0        0        0     1222 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/__init__.py
--rw-rw-rw-   0        0        0     3688 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/af.py
--rw-rw-rw-   0        0        0     3051 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/ar.py
--rw-rw-rw-   0        0        0     4406 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/ca.py
--rw-rw-rw-   0        0        0     4808 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/cs.py
--rw-rw-rw-   0        0        0     3680 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/da.py
--rw-rw-rw-   0        0        0     3443 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/de.py
--rw-rw-rw-   0        0        0     3336 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/en.py
--rw-rw-rw-   0        0        0     3825 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/eo.py
--rw-rw-rw-   0        0        0     4119 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/es.py
--rw-rw-rw-   0        0        0     3171 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/fa.py
--rw-rw-rw-   0        0        0     3526 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/fi.py
--rw-rw-rw-   0        0        0     3656 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/fr.py
--rw-rw-rw-   0        0        0     3632 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/gl.py
--rw-rw-rw-   0        0        0     3641 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/he.py
--rw-rw-rw-   0        0        0     3283 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/it.py
--rw-rw-rw-   0        0        0     3776 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/ja.py
--rw-rw-rw-   0        0        0     3377 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/ko.py
--rw-rw-rw-   0        0        0     3519 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/lt.py
--rw-rw-rw-   0        0        0     3376 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/lv.py
--rw-rw-rw-   0        0        0     3722 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/nl.py
--rw-rw-rw-   0        0        0     3357 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/pl.py
--rw-rw-rw-   0        0        0     3960 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/pt_br.py
--rw-rw-rw-   0        0        0     3398 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/ru.py
--rw-rw-rw-   0        0        0     3947 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/sk.py
--rw-rw-rw-   0        0        0     3261 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/sv.py
--rw-rw-rw-   0        0        0     3925 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/zh_cn.py
--rw-rw-rw-   0        0        0     5160 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/languages/zh_tw.py
--rw-rw-rw-   0        0        0    16119 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/roles.py
--rw-rw-rw-   0        0        0   132550 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/states.py
--rw-rw-rw-   0        0        0    20912 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/parsers/rst/tableparser.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.342474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/readers/
--rw-rw-rw-   0        0        0     3538 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/readers/__init__.py
--rw-rw-rw-   0        0        0     1607 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/readers/doctree.py
--rw-rw-rw-   0        0        0     1537 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/readers/pep.py
--rw-rw-rw-   0        0        0     2335 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/readers/standalone.py
--rw-rw-rw-   0        0        0    56956 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/statemachine.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.368476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/
--rw-rw-rw-   0        0        0     6532 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/__init__.py
--rw-rw-rw-   0        0        0     2151 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/components.py
--rw-rw-rw-   0        0        0    20276 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/frontmatter.py
--rw-rw-rw-   0        0        0     4873 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/misc.py
--rw-rw-rw-   0        0        0     6912 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/parts.py
--rw-rw-rw-   0        0        0    11111 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/peps.py
--rw-rw-rw-   0        0        0    36544 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/references.py
--rw-rw-rw-   0        0        0    12446 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/universal.py
--rw-rw-rw-   0        0        0     3057 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/transforms/writer_aux.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.387477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/
--rw-rw-rw-   0        0        0    28742 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/__init__.py
--rw-rw-rw-   0        0        0     4943 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/code_analyzer.py
--rw-rw-rw-   0        0        0     8105 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/error_reporting.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.403475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/math/
--rw-rw-rw-   0        0        0     1825 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/math/__init__.py
--rw-rw-rw-   0        0        0    51043 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/math/latex2mathml.py
--rw-rw-rw-   0        0        0    98692 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/math/math2html.py
--rw-rw-rw-   0        0        0     5631 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/math/tex2mathml_extern.py
--rw-rw-rw-   0        0        0    36734 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/math/tex2unichar.py
--rw-rw-rw-   0        0        0    18393 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/math/unichar2tex.py
--rw-rw-rw-   0        0        0     6418 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/punctuation_chars.py
--rw-rw-rw-   0        0        0     2695 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/roman.py
--rw-rw-rw-   0        0        0    38945 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/smartquotes.py
--rw-rw-rw-   0        0        0     6299 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/utils/urischemes.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.418476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/
--rw-rw-rw-   0        0        0     4815 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/__init__.py
--rw-rw-rw-   0        0        0    70253 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/_html_base.py
--rw-rw-rw-   0        0        0     6835 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/docutils_xml.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.424479 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/html4css1/
--rw-rw-rw-   0        0        0    37638 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/html4css1/__init__.py
--rw-rw-rw-   0        0        0      114 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/html4css1/template.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.429476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/html5_polyglot/
--rw-rw-rw-   0        0        0    18212 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/html5_polyglot/__init__.py
--rw-rw-rw-   0        0        0      114 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/html5_polyglot/template.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.431475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/latex2e/
--rw-rw-rw-   0        0        0   136872 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/latex2e/__init__.py
--rw-rw-rw-   0        0        0    36527 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/manpage.py
--rw-rw-rw-   0        0        0      450 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/null.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.436475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/odf_odt/
--rw-rw-rw-   0        0        0   132399 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/odf_odt/__init__.py
--rw-rw-rw-   0        0        0     4681 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.442477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/pep_html/
--rw-rw-rw-   0        0        0     3505 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/pep_html/__init__.py
--rw-rw-rw-   0        0        0     1002 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/pep_html/template.txt
--rw-rw-rw-   0        0        0     1032 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/pseudoxml.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.444475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/s5_html/
--rw-rw-rw-   0        0        0    14627 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/s5_html/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.446475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/s5_html/themes/
--rw-rw-rw-   0        0        0      278 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/s5_html/themes/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.448477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/xetex/
--rw-rw-rw-   0        0        0     5842 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils/writers/xetex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.046476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils-0.19.dist-info/
--rw-rw-rw-   0        0        0     6218 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils-0.19.dist-info/COPYING.txt
--rw-rw-rw-   0        0        0       53 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils-0.19.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/docutils-0.19.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.472478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/idna/
--rw-rw-rw-   0        0        0      849 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/idna/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/idna/codec.py
--rw-rw-rw-   0        0        0      321 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/idna/compat.py
--rw-rw-rw-   0        0        0    12950 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/idna/core.py
--rw-rw-rw-   0        0        0    44375 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/idna/idnadata.py
--rw-rw-rw-   0        0        0     1881 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/idna/package_data.py
--rw-rw-rw-   0        0        0   206539 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.496475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/
--rw-rw-rw-   0        0        0    26518 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/__init__.py
--rw-rw-rw-   0        0        0     2454 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/_adapters.py
--rw-rw-rw-   0        0        0      743 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/_collections.py
--rw-rw-rw-   0        0        0     1857 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/_compat.py
--rw-rw-rw-   0        0        0     2895 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/_functools.py
--rw-rw-rw-   0        0        0     2068 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/_itertools.py
--rw-rw-rw-   0        0        0     1368 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/_meta.py
--rw-rw-rw-   0        0        0     1098 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/_py39compat.py
--rw-rw-rw-   0        0        0     2166 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata/_text.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.498480 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata-6.1.0.dist-info/
--rw-rw-rw-   0        0        0       19 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/importlib_metadata-6.1.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:18.618488 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/jaraco/
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.510489 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/jaraco/classes/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/jaraco/classes/__init__.py
--rw-rw-rw-   0        0        0     1464 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/jaraco/classes/ancestry.py
--rw-rw-rw-   0        0        0     1853 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/jaraco/classes/meta.py
--rw-rw-rw-   0        0        0     3996 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/jaraco/classes/properties.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.500475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/jaraco.classes-3.2.3.dist-info/
--rw-rw-rw-   0        0        0        7 2023-04-01 14:18:00.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/jaraco.classes-3.2.3.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.542476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/
--rw-rw-rw-   0        0        0      271 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/__init__.py
--rw-rw-rw-   0        0        0       71 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/__main__.py
--rw-rw-rw-   0        0        0      185 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/_compat.py
--rw-rw-rw-   0        0        0     3886 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/_properties_compat.py
--rw-rw-rw-   0        0        0     7587 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backend.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.569476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/
--rw-rw-rw-   0        0        0      222 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/OS_X.py
--rw-rw-rw-   0        0        0     4685 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/SecretService.py
--rw-rw-rw-   0        0        0     5807 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/Windows.py
--rw-rw-rw-   0        0        0        0 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/__init__.py
--rw-rw-rw-   0        0        0     2167 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/chainer.py
--rw-rw-rw-   0        0        0      836 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/fail.py
--rw-rw-rw-   0        0        0     5821 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/kwallet.py
--rw-rw-rw-   0        0        0     5973 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/libsecret.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.574476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/macOS/
--rw-rw-rw-   0        0        0     2363 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/macOS/__init__.py
--rw-rw-rw-   0        0        0     4341 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/macOS/api.py
--rw-rw-rw-   0        0        0      360 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/backends/null.py
--rw-rw-rw-   0        0        0     4000 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/cli.py
--rw-rw-rw-   0        0        0     1324 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/completion.py
--rw-rw-rw-   0        0        0     5215 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/core.py
--rw-rw-rw-   0        0        0     1593 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/credentials.py
--rw-rw-rw-   0        0        0      752 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/devpi_client.py
--rw-rw-rw-   0        0        0     1430 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/errors.py
--rw-rw-rw-   0        0        0     1231 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/http.py
--rw-rw-rw-   0        0        0      175 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/py312compat.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.580475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/testing/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/testing/__init__.py
--rw-rw-rw-   0        0        0     6598 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/testing/backend.py
--rw-rw-rw-   0        0        0     1918 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/testing/util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.589475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/util/
--rw-rw-rw-   0        0        0      868 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/util/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/util/platform_.py
--rw-rw-rw-   0        0        0      318 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring/util/properties.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.546475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring-23.13.1.dist-info/
--rw-rw-rw-   0        0        0      334 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring-23.13.1.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/keyring-23.13.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.618489 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/
--rw-rw-rw-   0        0        0      113 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/__init__.py
--rw-rw-rw-   0        0        0      248 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/_compat.py
--rw-rw-rw-   0        0        0     2317 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/_punycode.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.622489 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/cli/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/cli/__init__.py
--rw-rw-rw-   0        0        0     2901 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/cli/parse.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.638477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/common/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/common/__init__.py
--rw-rw-rw-   0        0        0      156 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/common/entities.py
--rw-rw-rw-   0        0        0      932 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/common/html_blocks.py
--rw-rw-rw-   0        0        0      929 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/common/html_re.py
--rw-rw-rw-   0        0        0     2631 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/common/normalize_url.py
--rw-rw-rw-   0        0        0    10894 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.648477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/helpers/
--rw-rw-rw-   0        0        0      253 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/helpers/__init__.py
--rw-rw-rw-   0        0        0     1953 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/helpers/parse_link_destination.py
--rw-rw-rw-   0        0        0     1070 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/helpers/parse_link_label.py
--rw-rw-rw-   0        0        0     1410 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/helpers/parse_link_title.py
--rw-rw-rw-   0        0        0    12228 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/main.py
--rw-rw-rw-   0        0        0     3662 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/parser_block.py
--rw-rw-rw-   0        0        0      835 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/parser_core.py
--rw-rw-rw-   0        0        0     4130 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/parser_inline.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.658474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/presets/
--rw-rw-rw-   0        0        0      898 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/presets/__init__.py
--rw-rw-rw-   0        0        0     2809 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/presets/commonmark.py
--rw-rw-rw-   0        0        0     1765 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/presets/default.py
--rw-rw-rw-   0        0        0     2006 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/presets/zero.py
--rw-rw-rw-   0        0        0    10041 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/renderer.py
--rw-rw-rw-   0        0        0     8376 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/ruler.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.691491 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/
--rw-rw-rw-   0        0        0      553 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/__init__.py
--rw-rw-rw-   0        0        0     9057 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/blockquote.py
--rw-rw-rw-   0        0        0      886 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/code.py
--rw-rw-rw-   0        0        0     2704 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/fence.py
--rw-rw-rw-   0        0        0     1879 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/heading.py
--rw-rw-rw-   0        0        0     1309 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/hr.py
--rw-rw-rw-   0        0        0     2808 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/html_block.py
--rw-rw-rw-   0        0        0     2798 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/lheading.py
--rw-rw-rw-   0        0        0     9944 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/list.py
--rw-rw-rw-   0        0        0     1851 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/paragraph.py
--rw-rw-rw-   0        0        0     6323 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/reference.py
--rw-rw-rw-   0        0        0     7226 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/state_block.py
--rw-rw-rw-   0        0        0     7226 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_block/table.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.712477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_core/
--rw-rw-rw-   0        0        0      344 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_core/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_core/block.py
--rw-rw-rw-   0        0        0      325 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_core/inline.py
--rw-rw-rw-   0        0        0     4833 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_core/linkify.py
--rw-rw-rw-   0        0        0      402 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_core/normalize.py
--rw-rw-rw-   0        0        0     3560 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_core/replacements.py
--rw-rw-rw-   0        0        0     7251 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_core/smartquotes.py
--rw-rw-rw-   0        0        0      584 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_core/state_core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.751474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/
--rw-rw-rw-   0        0        0      649 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/autolink.py
--rw-rw-rw-   0        0        0     2112 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/backticks.py
--rw-rw-rw-   0        0        0     4062 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/balance_pairs.py
--rw-rw-rw-   0        0        0     2948 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/emphasis.py
--rw-rw-rw-   0        0        0     1653 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/entity.py
--rw-rw-rw-   0        0        0     1116 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/escape.py
--rw-rw-rw-   0        0        0     1019 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/html_inline.py
--rw-rw-rw-   0        0        0     4260 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/image.py
--rw-rw-rw-   0        0        0     4362 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/link.py
--rw-rw-rw-   0        0        0     1176 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/newline.py
--rw-rw-rw-   0        0        0     5388 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/state_inline.py
--rw-rw-rw-   0        0        0     3390 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/strikethrough.py
--rw-rw-rw-   0        0        0     1427 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/text.py
--rw-rw-rw-   0        0        0     1491 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/rules_inline/text_collapse.py
--rw-rw-rw-   0        0        0     6374 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/token.py
--rw-rw-rw-   0        0        0    11052 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/tree.py
--rw-rw-rw-   0        0        0     3262 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.753475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it_py-2.2.0.dist-info/
--rw-rw-rw-   0        0        0       58 2023-04-01 14:17:59.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/markdown_it_py-2.2.0.dist-info/entry_points.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.768486 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/mdurl/
--rw-rw-rw-   0        0        0      547 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/mdurl/__init__.py
--rw-rw-rw-   0        0        0     3004 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/mdurl/_decode.py
--rw-rw-rw-   0        0        0     2602 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/mdurl/_encode.py
--rw-rw-rw-   0        0        0      626 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/mdurl/_format.py
--rw-rw-rw-   0        0        0    11374 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/mdurl/_parse.py
--rw-rw-rw-   0        0        0      284 2023-04-01 14:17:55.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/mdurl/_url.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.777475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/more_itertools/
--rw-rw-rw-   0        0        0      148 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   134968 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/more_itertools/more.py
--rw-rw-rw-   0        0        0    25416 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/more_itertools/recipes.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.785475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/
--rw-rw-rw-   0        0        0      357 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/__main__.py
--rw-rw-rw-   0        0        0     1444 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/__pip-runner__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.815489 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/
--rw-rw-rw-   0        0        0      573 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/__init__.py
--rw-rw-rw-   0        0        0    10243 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/build_env.py
--rw-rw-rw-   0        0        0    10734 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.846474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/
--rw-rw-rw-   0        0        0      132 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-rw-   0        0        0     7842 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-rw-rw-   0        0        0    29497 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-rw-   0        0        0      774 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-rw-rw-   0        0        0     2472 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/main.py
--rw-rw-rw-   0        0        0     4338 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-rw-   0        0        0    10817 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/parser.py
--rw-rw-rw-   0        0        0     1968 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-rw-   0        0        0    18172 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-rw-rw-   0        0        0     5118 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-rw-rw-   0        0        0      116 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.889478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/
--rw-rw-rw-   0        0        0     3882 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-rw-rw-   0        0        0     7582 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/cache.py
--rw-rw-rw-   0        0        0     1685 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/check.py
--rw-rw-rw-   0        0        0     4129 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/completion.py
--rw-rw-rw-   0        0        0     9815 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-rw-rw-   0        0        0     6591 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/debug.py
--rw-rw-rw-   0        0        0     5289 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/download.py
--rw-rw-rw-   0        0        0     2951 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-rw-rw-   0        0        0     1703 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/hash.py
--rw-rw-rw-   0        0        0     1132 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/help.py
--rw-rw-rw-   0        0        0     4793 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/index.py
--rw-rw-rw-   0        0        0     3188 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-rw-rw-   0        0        0    32389 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/install.py
--rw-rw-rw-   0        0        0    12343 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/list.py
--rw-rw-rw-   0        0        0     5697 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/search.py
--rw-rw-rw-   0        0        0     6419 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/show.py
--rw-rw-rw-   0        0        0     3886 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-rw-   0        0        0     7396 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-rw-rw-   0        0        0    13529 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/configuration.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.901474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/distributions/
--rw-rw-rw-   0        0        0      858 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/distributions/base.py
--rw-rw-rw-   0        0        0      729 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-rw-rw-   0        0        0     6494 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-rw-   0        0        0     1164 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-rw-   0        0        0    24244 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.912480 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/index/
--rw-rw-rw-   0        0        0       30 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/index/__init__.py
--rw-rw-rw-   0        0        0    16504 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/index/collector.py
--rw-rw-rw-   0        0        0    37873 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-rw-rw-   0        0        0     6557 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/index/sources.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.921475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/locations/
--rw-rw-rw-   0        0        0    15365 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-rw-rw-   0        0        0     6100 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-rw-   0        0        0     7680 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-rw-   0        0        0     2556 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/locations/base.py
--rw-rw-rw-   0        0        0      340 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/main.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.932476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/
--rw-rw-rw-   0        0        0     4280 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-rw-rw-   0        0        0    25277 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/base.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.943476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/importlib/
--rw-rw-rw-   0        0        0      107 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-rw-   0        0        0     8181 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-rw-   0        0        0     7457 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-rw-   0        0        0     9773 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.974479 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/
--rw-rw-rw-   0        0        0       63 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/__init__.py
--rw-rw-rw-   0        0        0      990 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/candidate.py
--rw-rw-rw-   0        0        0     6626 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-rw-rw-   0        0        0     2520 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/format_control.py
--rw-rw-rw-   0        0        0     1030 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/index.py
--rw-rw-rw-   0        0        0     2617 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-rw-rw-   0        0        0    18602 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/link.py
--rw-rw-rw-   0        0        0      738 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/scheme.py
--rw-rw-rw-   0        0        0     4644 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-rw-rw-   0        0        0     1907 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-rw-   0        0        0     3858 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/target_python.py
--rw-rw-rw-   0        0        0     3600 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/models/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.996475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/network/
--rw-rw-rw-   0        0        0       50 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/network/__init__.py
--rw-rw-rw-   0        0        0    16507 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/network/auth.py
--rw-rw-rw-   0        0        0     2145 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/network/cache.py
--rw-rw-rw-   0        0        0     6096 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/network/download.py
--rw-rw-rw-   0        0        0     7638 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-rw-   0        0        0    18443 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/network/session.py
--rw-rw-rw-   0        0        0     4073 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/network/utils.py
--rw-rw-rw-   0        0        0     1791 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.006478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.026476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/build/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-rw-   0        0        0     1422 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-rw-   0        0        0     1474 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-rw-   0        0        0     2198 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-rw-   0        0        0     1075 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-rw-   0        0        0     1417 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-rw-   0        0        0     3064 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-rw-   0        0        0     5122 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/check.py
--rw-rw-rw-   0        0        0     9784 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/freeze.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.036476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/install/
--rw-rw-rw-   0        0        0       51 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-rw-   0        0        0     1354 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-rw-   0        0        0     4105 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/install/legacy.py
--rw-rw-rw-   0        0        0    27407 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-rw-   0        0        0    25091 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-rw-rw-   0        0        0     6987 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/pyproject.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.052477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/req/
--rw-rw-rw-   0        0        0     2807 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/req/__init__.py
--rw-rw-rw-   0        0        0    16611 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/req/constructors.py
--rw-rw-rw-   0        0        0    17646 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/req/req_file.py
--rw-rw-rw-   0        0        0    35763 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/req/req_install.py
--rw-rw-rw-   0        0        0     2858 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/req/req_set.py
--rw-rw-rw-   0        0        0    24045 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.056475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-rw-   0        0        0      583 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/base.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.060474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/legacy/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-rw-   0        0        0    24129 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.082476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-rw-   0        0        0     5220 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-rw-   0        0        0    18963 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-rw-   0        0        0    27878 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-rw-   0        0        0     5705 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-rw-   0        0        0     9914 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-rw-   0        0        0     2526 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-rw-   0        0        0     5455 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-rw-   0        0        0    11533 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-rw-   0        0        0     8167 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.152474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-rw-rw-   0        0        0     1015 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/_log.py
--rw-rw-rw-   0        0        0     1665 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-rw-   0        0        0     1884 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/compat.py
--rw-rw-rw-   0        0        0     5377 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-rw-   0        0        0      242 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-rw-rw-   0        0        0     5764 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-rw-   0        0        0     3206 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-rw-   0        0        0     1115 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/distutils_args.py
--rw-rw-rw-   0        0        0     2118 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-rw-   0        0        0     1169 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-rw-rw-   0        0        0     3064 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-rw-   0        0        0     5122 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-rw-   0        0        0      716 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-rw-   0        0        0     3110 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-rw-rw-   0        0        0     4831 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-rw-rw-   0        0        0      795 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-rw-   0        0        0    11632 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/logging.py
--rw-rw-rw-   0        0        0    22253 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/misc.py
--rw-rw-rw-   0        0        0     1193 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/models.py
--rw-rw-rw-   0        0        0     2108 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-rw-rw-   0        0        0     5662 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-rw-   0        0        0     9200 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-rw-   0        0        0     7702 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-rw-   0        0        0     8821 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-rw-   0        0        0     1759 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/urls.py
--rw-rw-rw-   0        0        0     3456 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-rw-   0        0        0     4549 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/utils/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.167477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/vcs/
--rw-rw-rw-   0        0        0      596 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-rw-   0        0        0     3519 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-rw-   0        0        0    18116 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/vcs/git.py
--rw-rw-rw-   0        0        0     5238 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-rw-   0        0        0    11729 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-rw-   0        0        0    22811 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-rw-   0        0        0    13079 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_internal/wheel_builder.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.178478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/
--rw-rw-rw-   0        0        0     4966 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.205475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/
--rw-rw-rw-   0        0        0      465 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-rw-   0        0        0     1379 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-rw-   0        0        0     5033 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-rw-   0        0        0     1535 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.213477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-rw-   0        0        0      242 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-rw-   0        0        0     5271 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-rw-   0        0        0     1033 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-rw-   0        0        0      778 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-rw-   0        0        0    16416 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-rw-   0        0        0     3946 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-rw-   0        0        0     4154 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-rw-   0        0        0     7105 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-rw-   0        0        0      774 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.220478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/certifi/
--rw-rw-rw-   0        0        0       94 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-rw-   0        0        0      255 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-rw-   0        0        0     4279 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/certifi/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.338478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/
--rw-rw-rw-   0        0        0     4797 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-rw-   0        0        0    31274 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-rw-   0        0        0     1763 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-rw-   0        0        0    10032 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-rw-   0        0        0     3915 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-rw-   0        0        0     5420 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.341488 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/cli/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-rw-   0        0        0     3242 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-rw-   0        0        0     3732 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-rw-   0        0        0      542 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-rw-rw-   0        0        0     1860 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-rw-   0        0        0     1683 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-rw-   0        0        0     4006 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-rw-   0        0        0    12176 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-rw-   0        0        0     3934 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-rw-   0        0        0    13566 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-rw-   0        0        0     1753 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-rw-   0        0        0    36913 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-rw-   0        0        0     1753 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-rw-   0        0        0    20735 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-rw-   0        0        0     1759 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-rw-   0        0        0    14537 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-rw-   0        0        0    25796 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-rw-   0        0        0    42498 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-rw-   0        0        0     1752 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-rw-   0        0        0    27055 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-rw-   0        0        0   104562 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-rw-   0        0        0    98484 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-rw-   0        0        0    98196 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-rw-   0        0        0   101363 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-rw-   0        0        0   128035 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-rw-   0        0        0   102774 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-rw-   0        0        0    95372 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-rw-   0        0        0     5380 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-rw-   0        0        0     6077 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-rw-rw-   0        0        0     3715 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-rw-   0        0        0     2131 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-rw-   0        0        0    30391 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.346476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-rw-   0        0        0    13560 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-rw-   0        0        0      402 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-rw-rw-   0        0        0     6400 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-rw-   0        0        0     4137 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-rw-   0        0        0     4007 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-rw-   0        0        0    14848 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-rw-   0        0        0     8505 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-rw-   0        0        0     2812 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-rw-   0        0        0      244 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/chardet/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.364478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/
--rw-rw-rw-   0        0        0      266 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-rw-   0        0        0    11128 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     3325 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/initialise.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.384477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/tests/
--rw-rw-rw-   0        0        0       75 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-rw-rw-   0        0        0     2839 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-rw-rw-   0        0        0    10678 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-rw-rw-   0        0        0     6741 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-rw-rw-   0        0        0     1866 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-rw-rw-   0        0        0     1079 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-rw-rw-   0        0        0     3709 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-rw-rw-   0        0        0     6181 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-rw-   0        0        0     7134 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.418474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/
--rw-rw-rw-   0        0        0      581 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-rw-   0        0        0    41259 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-rw-   0        0        0    51697 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-rw-rw-   0        0        0    20834 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-rw-rw-   0        0        0    51991 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-rw-   0        0        0    14811 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-rw-   0        0        0     5058 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-rw-   0        0        0    39801 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-rw-   0        0        0    10820 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-rw-   0        0        0    18102 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-rw-   0        0        0    66262 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-rw-rw-   0        0        0    23513 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/version.py
--rw-rw-rw-   0        0        0    43898 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.427479 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distro/
--rw-rw-rw-   0        0        0      981 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-rw-   0        0        0       64 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-rw-   0        0        0    49330 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/distro/distro.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.446488 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/idna/
--rw-rw-rw-   0        0        0      849 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-rw-rw-   0        0        0      321 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-rw-rw-   0        0        0    12950 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/idna/core.py
--rw-rw-rw-   0        0        0    44375 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-rw-   0        0        0     1881 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-rw-   0        0        0   206539 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.456489 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/msgpack/
--rw-rw-rw-   0        0        0     1132 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-rw-   0        0        0     6080 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-rw-   0        0        0    34557 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.483474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8487 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4676 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.490487 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pkg_resources/
--rw-rw-rw-   0        0        0   108287 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      562 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.509476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/platformdirs/
--rw-rw-rw-   0        0        0    12936 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-rw-   0        0        0     1176 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-rw-   0        0        0     4068 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-rw-   0        0        0     4910 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-rw-   0        0        0     2655 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-rw-   0        0        0     6911 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-rw-   0        0        0      160 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-rw-   0        0        0     6596 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.551476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/
--rw-rw-rw-   0        0        0     2999 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-rw-   0        0        0      353 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-rw-   0        0        0    23685 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-rw-   0        0        0     1697 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-rw-rw-   0        0        0     1938 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.553475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/filters/
--rw-rw-rw-   0        0        0    40386 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.587476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-rw-   0        0        0     4810 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-rw-   0        0        0     4104 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-rw-   0        0        0     3314 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-rw-   0        0        0     5086 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-rw-   0        0        0    35441 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-rw-   0        0        0    21938 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-rw-   0        0        0     5871 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-rw-   0        0        0    19351 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-rw-   0        0        0     5073 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-rw-   0        0        0     2212 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-rw-   0        0        0     5014 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-rw-   0        0        0     7335 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-rw-   0        0        0     4674 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-rw-   0        0        0    11753 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-rw-   0        0        0    32005 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.595476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-rw-   0        0        0    11174 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-rw-   0        0        0    70232 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-rw-   0        0        0    53376 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-rw-   0        0        0      986 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-rw-   0        0        0     2591 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-rw-   0        0        0     3072 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-rw-   0        0        0     3092 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-rw-   0        0        0     4630 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-rw-   0        0        0     6257 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/style.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.597475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/styles/
--rw-rw-rw-   0        0        0     3419 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-rw-   0        0        0     6184 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-rw-rw-   0        0        0    63187 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-rw-   0        0        0     9110 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pygments/util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.622475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9171 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213344 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.624475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23685 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.632475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyproject_hooks/
--rw-rw-rw-   0        0        0      491 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-rw-rw-   0        0        0      138 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-rw-rw-   0        0        0    11920 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.637476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-rw-rw-   0        0        0      546 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-rw-rw-   0        0        0    10927 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.682476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/
--rw-rw-rw-   0        0        0     5178 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-rw-   0        0        0      435 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-rw-   0        0        0     1397 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    21443 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-rw-   0        0        0     6377 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/api.py
--rw-rw-rw-   0        0        0    10187 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-rw-rw-   0        0        0      575 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-rw-rw-   0        0        0     1286 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-rw-rw-   0        0        0    18560 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-rw-   0        0        0     3823 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-rw-   0        0        0     3879 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/help.py
--rw-rw-rw-   0        0        0      733 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-rw-   0        0        0    35288 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/models.py
--rw-rw-rw-   0        0        0      695 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-rw-rw-   0        0        0    30180 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-rw-rw-   0        0        0    33240 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/requests/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.695478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/resolvelib/
--rw-rw-rw-   0        0        0      537 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.699475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-rw-   0        0        0      156 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-rw-   0        0        0     5872 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-rw-   0        0        0     1583 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-rw-   0        0        0    17592 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-rw-   0        0        0     4794 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.890484 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/
--rw-rw-rw-   0        0        0     6090 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-rw-   0        0        0     8478 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-rw-   0        0        0    10096 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-rw-   0        0        0   140235 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-rw-   0        0        0     1064 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-rw-   0        0        0     2114 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-rw-   0        0        0      265 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-rw-   0        0        0     9695 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-rw-   0        0        0     3225 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-rw-   0        0        0     1236 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-rw-   0        0        0     1643 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-rw-rw-   0        0        0     7063 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-rw-   0        0        0      423 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-rw-   0        0        0     5472 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-rw-   0        0        0    19919 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-rw-   0        0        0      351 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-rw-   0        0        0      417 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-rw-   0        0        0    22820 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-rw-   0        0        0     1926 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-rw-   0        0        0     2783 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-rw-   0        0        0     1840 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-rw-   0        0        0      890 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-rw-rw-   0        0        0    10368 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/align.py
--rw-rw-rw-   0        0        0     6819 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-rw-   0        0        0     3264 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-rw-rw-   0        0        0     9842 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/box.py
--rw-rw-rw-   0        0        0     4503 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-rw-rw-   0        0        0    18015 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/color.py
--rw-rw-rw-   0        0        0     1054 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-rw-   0        0        0     7131 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-rw-rw-   0        0        0    97992 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/console.py
--rw-rw-rw-   0        0        0     1288 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-rw-   0        0        0     5497 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-rw-rw-   0        0        0     6630 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/control.py
--rw-rw-rw-   0        0        0     7954 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-rw-   0        0        0      972 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-rw-   0        0        0     2501 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-rw-   0        0        0      642 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-rw-rw-   0        0        0     1616 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-rw-   0        0        0     2508 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-rw-   0        0        0     9585 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-rw-   0        0        0     5053 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/json.py
--rw-rw-rw-   0        0        0     3252 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-rw-   0        0        0    14007 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-rw-rw-   0        0        0    14172 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/live.py
--rw-rw-rw-   0        0        0     3667 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-rw-   0        0        0    11903 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-rw-rw-   0        0        0     8198 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-rw-rw-   0        0        0     5305 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-rw-rw-   0        0        0     4970 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-rw-rw-   0        0        0      828 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-rw-rw-   0        0        0     3396 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-rw-rw-   0        0        0    10574 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-rw-rw-   0        0        0    37414 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-rw-   0        0        0    59836 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-rw-rw-   0        0        0     8165 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-rw-   0        0        0    11303 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-rw-   0        0        0     1391 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-rw-   0        0        0      166 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/region.py
--rw-rw-rw-   0        0        0     4436 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-rw-rw-   0        0        0     4773 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-rw-rw-   0        0        0     2843 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-rw-rw-   0        0        0     1591 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-rw-rw-   0        0        0    24224 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-rw-rw-   0        0        0     4374 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-rw-   0        0        0     4425 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/status.py
--rw-rw-rw-   0        0        0    26332 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/style.py
--rw-rw-rw-   0        0        0     1258 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-rw-rw-   0        0        0    34995 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-rw-   0        0        0    39684 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/table.py
--rw-rw-rw-   0        0        0     3370 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-rw-   0        0        0    45686 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/text.py
--rw-rw-rw-   0        0        0     3627 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-rw-rw-   0        0        0      102 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-rw-rw-   0        0        0    26070 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-rw-   0        0        0     9169 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-rw-rw-   0        0        0    34549 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/six.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.920477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/
--rw-rw-rw-   0        0        0    18364 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-rw-   0        0        0     1944 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-rw-   0        0        0     1496 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-rw-   0        0        0     1376 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-rw-   0        0        0     1908 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-rw-   0        0        0     1383 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-rw-   0        0        0     7550 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-rw-   0        0        0     2790 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-rw-   0        0        0     2145 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-rw-   0        0        0     8011 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.929475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    80114 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.959476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/
--rw-rw-rw-   0        0        0     3333 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-rw-   0        0        0    10811 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-rw-   0        0        0       64 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-rw-   0        0        0    20070 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-rw-   0        0        0    39095 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.977474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-rw-   0        0        0      957 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.986476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    17632 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    13922 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    11036 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-rw-   0        0        0     4528 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-rw-   0        0        0    17081 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34448 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7097 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     8217 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-rw-   0        0        0     8579 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-rw-   0        0        0     2440 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.990477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:20.994474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-rw-   0        0        0    34665 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-rw-   0        0        0    19786 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0     5985 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-rw-   0        0        0    30641 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.027477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/
--rw-rw-rw-   0        0        0     1155 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1605 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0      498 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-rw-   0        0        0     3997 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3510 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-rw-   0        0        0    22003 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    17177 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     5758 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-rw-   0        0        0     6895 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10003 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    14298 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-rw-   0        0        0     5403 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-rw-   0        0        0      476 2023-04-01 14:12:36.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/vendor.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.039475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/webencodings/
--rw-rw-rw-   0        0        0    10579 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-rw-   0        0        0     8979 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-rw-   0        0        0     1305 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-rw-   0        0        0     6563 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-rw-   0        0        0     4307 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:19.793475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip-23.0.1.dist-info/
--rw-rw-rw-   0        0        0     1093 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip-23.0.1.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0      124 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip-23.0.1.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-04-01 14:12:37.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pip-23.0.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.041478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/
--rw-rw-rw-   0        0        0   108568 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.049475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-rw-rw-   0        0        0    24701 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/appdirs.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.070475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.078476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13515 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.080476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15526 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.087475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       83 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   132569 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    18410 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.114474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8496 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4706 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.143475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6429 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213278 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.145477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23003 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9030 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39007 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25353 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13388 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10381 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-rw-rw-   0        0        0     8425 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/_vendor/zipp.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.147475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/extern/
--rw-rw-rw-   0        0        0     2426 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkg_resources/extern/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.173477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/
--rw-rw-rw-   0        0        0      266 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/bdist.py
--rw-rw-rw-   0        0        0     7415 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/commandline.py
--rw-rw-rw-   0        0        0     1577 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/develop.py
--rw-rw-rw-   0        0        0     4627 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/distribution.py
--rw-rw-rw-   0        0        0      518 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/index.py
--rw-rw-rw-   0        0        0     2492 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/installed.py
--rw-rw-rw-   0        0        0     2347 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/sdist.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.206476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/
--rw-rw-rw-   0        0        0     1342 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/__init__.py
--rw-rw-rw-   0        0        0     2279 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/test_bdist.py
--rw-rw-rw-   0        0        0    11722 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/test_commandline.py
--rw-rw-rw-   0        0        0      831 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/test_develop.py
--rw-rw-rw-   0        0        0    19377 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/test_distribution.py
--rw-rw-rw-   0        0        0     2636 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/test_index.py
--rw-rw-rw-   0        0        0     5460 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/test_installed.py
--rw-rw-rw-   0        0        0     5481 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/test_sdist.py
--rw-rw-rw-   0        0        0     6835 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/test_utils.py
--rw-rw-rw-   0        0        0     4443 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/tests/test_wheel.py
--rw-rw-rw-   0        0        0     1786 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/utils.py
--rw-rw-rw-   0        0        0     1586 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.180474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo-1.9.6.dist-info/
--rw-rw-rw-   0        0        0     1084 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0       54 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo-1.9.6.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-04-01 14:17:54.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pkginfo-1.9.6.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.247476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/
--rw-rw-rw-   0        0        0     2975 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/__init__.py
--rw-rw-rw-   0        0        0      348 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/__main__.py
--rw-rw-rw-   0        0        0    23530 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/cmdline.py
--rw-rw-rw-   0        0        0     1697 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/console.py
--rw-rw-rw-   0        0        0     1938 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.249475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/filters/
--rw-rw-rw-   0        0        0    40338 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/filters/__init__.py
--rw-rw-rw-   0        0        0     2893 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.285475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/
--rw-rw-rw-   0        0        0     4764 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/__init__.py
--rw-rw-rw-   0        0        0     4104 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/_mapping.py
--rw-rw-rw-   0        0        0     3290 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/bbcode.py
--rw-rw-rw-   0        0        0     5062 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/groff.py
--rw-rw-rw-   0        0        0    35565 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/html.py
--rw-rw-rw-   0        0        0    21914 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/img.py
--rw-rw-rw-   0        0        0     4945 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/irc.py
--rw-rw-rw-   0        0        0    19303 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/latex.py
--rw-rw-rw-   0        0        0     5025 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/other.py
--rw-rw-rw-   0        0        0     2200 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/pangomarkup.py
--rw-rw-rw-   0        0        0     4990 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/rtf.py
--rw-rw-rw-   0        0        0     7299 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/svg.py
--rw-rw-rw-   0        0        0     4626 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/terminal.py
--rw-rw-rw-   0        0        0    11717 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/formatters/terminal256.py
--rw-rw-rw-   0        0        0    31987 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexer.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.874476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/
--rw-rw-rw-   0        0        0    11116 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/__init__.py
--rw-rw-rw-   0        0        0     1543 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_ada_builtins.py
--rw-rw-rw-   0        0        0    27287 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_asy_builtins.py
--rw-rw-rw-   0        0        0    13994 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_cl_builtins.py
--rw-rw-rw-   0        0        0   105182 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_cocoa_builtins.py
--rw-rw-rw-   0        0        0    18414 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_csound_builtins.py
--rw-rw-rw-   0        0        0    12446 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_css_builtins.py
--rw-rw-rw-   0        0        0    11883 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_julia_builtins.py
--rw-rw-rw-   0        0        0   134510 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_lasso_builtins.py
--rw-rw-rw-   0        0        0   106781 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_lilypond_builtins.py
--rw-rw-rw-   0        0        0     8080 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_lua_builtins.py
--rw-rw-rw-   0        0        0    64980 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_mapping.py
--rw-rw-rw-   0        0        0    24713 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_mql_builtins.py
--rw-rw-rw-   0        0        0    25806 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_mysql_builtins.py
--rw-rw-rw-   0        0        0    49398 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_openedge_builtins.py
--rw-rw-rw-   0        0        0   107876 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_php_builtins.py
--rw-rw-rw-   0        0        0    12316 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_postgres_builtins.py
--rw-rw-rw-   0        0        0    12595 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_qlik_builtins.py
--rw-rw-rw-   0        0        0    32564 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_scheme_builtins.py
--rw-rw-rw-   0        0        0    52377 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_scilab_builtins.py
--rw-rw-rw-   0        0        0    26745 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_sourcemod_builtins.py
--rw-rw-rw-   0        0        0    13445 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_stan_builtins.py
--rw-rw-rw-   0        0        0    27227 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_stata_builtins.py
--rw-rw-rw-   0        0        0    15460 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_tsql_builtins.py
--rw-rw-rw-   0        0        0     1658 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_usd_builtins.py
--rw-rw-rw-   0        0        0     4225 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_vbscript_builtins.py
--rw-rw-rw-   0        0        0    57066 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/_vim_builtins.py
--rw-rw-rw-   0        0        0    11676 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/actionscript.py
--rw-rw-rw-   0        0        0     5320 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ada.py
--rw-rw-rw-   0        0        0      876 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/agile.py
--rw-rw-rw-   0        0        0     9873 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/algebra.py
--rw-rw-rw-   0        0        0     2606 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ambient.py
--rw-rw-rw-   0        0        0     1603 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/amdgpu.py
--rw-rw-rw-   0        0        0     4177 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ampl.py
--rw-rw-rw-   0        0        0    26654 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/apdlexer.py
--rw-rw-rw-   0        0        0     3405 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/apl.py
--rw-rw-rw-   0        0        0    11469 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/archetype.py
--rw-rw-rw-   0        0        0     3565 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/arrow.py
--rw-rw-rw-   0        0        0    11417 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/arturo.py
--rw-rw-rw-   0        0        0     1621 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/asc.py
--rw-rw-rw-   0        0        0    41243 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/asm.py
--rw-rw-rw-   0        0        0    19815 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/automation.py
--rw-rw-rw-   0        0        0     3021 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/bare.py
--rw-rw-rw-   0        0        0    27923 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/basic.py
--rw-rw-rw-   0        0        0     1652 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/bdd.py
--rw-rw-rw-   0        0        0     3211 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/berry.py
--rw-rw-rw-   0        0        0     4723 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/bibtex.py
--rw-rw-rw-   0        0        0     3915 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/boa.py
--rw-rw-rw-   0        0        0    28112 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/business.py
--rw-rw-rw-   0        0        0    17791 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/c_cpp.py
--rw-rw-rw-   0        0        0    29206 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/c_like.py
--rw-rw-rw-   0        0        0     2175 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/capnproto.py
--rw-rw-rw-   0        0        0     5182 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/cddl.py
--rw-rw-rw-   0        0        0     5014 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/chapel.py
--rw-rw-rw-   0        0        0     6395 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/clean.py
--rw-rw-rw-   0        0        0     3156 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/comal.py
--rw-rw-rw-   0        0        0     1407 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/compiled.py
--rw-rw-rw-   0        0        0    41825 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/configs.py
--rw-rw-rw-   0        0        0     4148 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/console.py
--rw-rw-rw-   0        0        0     1390 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/cplint.py
--rw-rw-rw-   0        0        0    15756 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/crystal.py
--rw-rw-rw-   0        0        0    16994 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/csound.py
--rw-rw-rw-   0        0        0    25314 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/css.py
--rw-rw-rw-   0        0        0     9875 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/d.py
--rw-rw-rw-   0        0        0     4607 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/dalvik.py
--rw-rw-rw-   0        0        0    26940 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/data.py
--rw-rw-rw-   0        0        0     4020 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/devicetree.py
--rw-rw-rw-   0        0        0     5164 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/diff.py
--rw-rw-rw-   0        0        0    29696 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/dotnet.py
--rw-rw-rw-   0        0        0    36774 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/dsls.py
--rw-rw-rw-   0        0        0    10380 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/dylan.py
--rw-rw-rw-   0        0        0     6372 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ecl.py
--rw-rw-rw-   0        0        0     2690 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/eiffel.py
--rw-rw-rw-   0        0        0     3152 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/elm.py
--rw-rw-rw-   0        0        0     6370 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/elpi.py
--rw-rw-rw-   0        0        0     4742 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/email.py
--rw-rw-rw-   0        0        0    19170 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/erlang.py
--rw-rw-rw-   0        0        0    10396 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/esoteric.py
--rw-rw-rw-   0        0        0     3273 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ezhil.py
--rw-rw-rw-   0        0        0    19531 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/factor.py
--rw-rw-rw-   0        0        0    10197 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/fantom.py
--rw-rw-rw-   0        0        0     9646 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/felix.py
--rw-rw-rw-   0        0        0     1621 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/fift.py
--rw-rw-rw-   0        0        0     2668 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/floscript.py
--rw-rw-rw-   0        0        0     7194 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/forth.py
--rw-rw-rw-   0        0        0    10336 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/fortran.py
--rw-rw-rw-   0        0        0    26212 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/foxpro.py
--rw-rw-rw-   0        0        0    26914 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/freefem.py
--rw-rw-rw-   0        0        0     3622 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/func.py
--rw-rw-rw-   0        0        0      674 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/functional.py
--rw-rw-rw-   0        0        0     3732 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/futhark.py
--rw-rw-rw-   0        0        0      826 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/gcodelexer.py
--rw-rw-rw-   0        0        0     7543 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/gdscript.py
--rw-rw-rw-   0        0        0     3761 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/go.py
--rw-rw-rw-   0        0        0     7980 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/grammar_notation.py
--rw-rw-rw-   0        0        0     3861 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/graph.py
--rw-rw-rw-   0        0        0    38931 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/graphics.py
--rw-rw-rw-   0        0        0     1935 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/graphviz.py
--rw-rw-rw-   0        0        0     3991 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/gsql.py
--rw-rw-rw-   0        0        0    32898 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/haskell.py
--rw-rw-rw-   0        0        0    30976 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/haxe.py
--rw-rw-rw-   0        0        0    22520 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/hdl.py
--rw-rw-rw-   0        0        0     3603 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/hexdump.py
--rw-rw-rw-   0        0        0    19879 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/html.py
--rw-rw-rw-   0        0        0    15450 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/idl.py
--rw-rw-rw-   0        0        0    30631 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/igor.py
--rw-rw-rw-   0        0        0     3136 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/inferno.py
--rw-rw-rw-   0        0        0    13178 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/installers.py
--rw-rw-rw-   0        0        0    57119 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/int_fiction.py
--rw-rw-rw-   0        0        0     1906 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/iolang.py
--rw-rw-rw-   0        0        0     4854 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/j.py
--rw-rw-rw-   0        0        0    62859 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/javascript.py
--rw-rw-rw-   0        0        0     2059 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/jmespath.py
--rw-rw-rw-   0        0        0     3701 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/jslt.py
--rw-rw-rw-   0        0        0     5635 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/jsonnet.py
--rw-rw-rw-   0        0        0    11646 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/julia.py
--rw-rw-rw-   0        0        0    72929 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/jvm.py
--rw-rw-rw-   0        0        0    11406 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/kuin.py
--rw-rw-rw-   0        0        0     9753 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/lilypond.py
--rw-rw-rw-   0        0        0   144039 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/lisp.py
--rw-rw-rw-   0        0        0    31914 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/macaulay2.py
--rw-rw-rw-   0        0        0     7550 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/make.py
--rw-rw-rw-   0        0        0    26797 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/markup.py
--rw-rw-rw-   0        0        0      676 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/math.py
--rw-rw-rw-   0        0        0   132852 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/matlab.py
--rw-rw-rw-   0        0        0     2716 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/maxima.py
--rw-rw-rw-   0        0        0     4337 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/meson.py
--rw-rw-rw-   0        0        0     7538 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/mime.py
--rw-rw-rw-   0        0        0    13846 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/minecraft.py
--rw-rw-rw-   0        0        0     4604 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/mips.py
--rw-rw-rw-   0        0        0    35324 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ml.py
--rw-rw-rw-   0        0        0    13524 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/modeling.py
--rw-rw-rw-   0        0        0    53073 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/modula2.py
--rw-rw-rw-   0        0        0     6290 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/monte.py
--rw-rw-rw-   0        0        0     9187 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/mosel.py
--rw-rw-rw-   0        0        0    63962 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ncl.py
--rw-rw-rw-   0        0        0     6416 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/nimrod.py
--rw-rw-rw-   0        0        0     2726 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/nit.py
--rw-rw-rw-   0        0        0     4015 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/nix.py
--rw-rw-rw-   0        0        0     4169 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/oberon.py
--rw-rw-rw-   0        0        0    22961 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/objective.py
--rw-rw-rw-   0        0        0     2982 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ooc.py
--rw-rw-rw-   0        0        0     1744 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/other.py
--rw-rw-rw-   0        0        0     2720 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/parasail.py
--rw-rw-rw-   0        0        0    25904 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/parsers.py
--rw-rw-rw-   0        0        0    30880 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/pascal.py
--rw-rw-rw-   0        0        0     8146 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/pawn.py
--rw-rw-rw-   0        0        0    39170 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/perl.py
--rw-rw-rw-   0        0        0    23252 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/phix.py
--rw-rw-rw-   0        0        0    12505 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/php.py
--rw-rw-rw-   0        0        0     1975 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/pointless.py
--rw-rw-rw-   0        0        0     3244 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/pony.py
--rw-rw-rw-   0        0        0    12677 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/praat.py
--rw-rw-rw-   0        0        0     1156 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/procfile.py
--rw-rw-rw-   0        0        0    12351 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/prolog.py
--rw-rw-rw-   0        0        0     4715 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/promql.py
--rw-rw-rw-   0        0        0    53524 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/python.py
--rw-rw-rw-   0        0        0     6932 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/q.py
--rw-rw-rw-   0        0        0     3665 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/qlik.py
--rw-rw-rw-   0        0        0     6072 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/qvt.py
--rw-rw-rw-   0        0        0     6185 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/r.py
--rw-rw-rw-   0        0        0    15790 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/rdf.py
--rw-rw-rw-   0        0        0    18600 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/rebol.py
--rw-rw-rw-   0        0        0     2902 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/resource.py
--rw-rw-rw-   0        0        0     5056 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ride.py
--rw-rw-rw-   0        0        0     1128 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/rita.py
--rw-rw-rw-   0        0        0     1973 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/rnc.py
--rw-rw-rw-   0        0        0     1962 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/roboconf.py
--rw-rw-rw-   0        0        0    18449 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/robotframework.py
--rw-rw-rw-   0        0        0    22775 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ruby.py
--rw-rw-rw-   0        0        0     8216 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/rust.py
--rw-rw-rw-   0        0        0     9400 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/sas.py
--rw-rw-rw-   0        0        0     4645 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/savi.py
--rw-rw-rw-   0        0        0     2239 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/scdoc.py
--rw-rw-rw-   0        0        0    70014 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/scripting.py
--rw-rw-rw-   0        0        0     1986 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/sgf.py
--rw-rw-rw-   0        0        0    36344 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/shell.py
--rw-rw-rw-   0        0        0     2441 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/sieve.py
--rw-rw-rw-   0        0        0     8482 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/slash.py
--rw-rw-rw-   0        0        0     7206 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/smalltalk.py
--rw-rw-rw-   0        0        0     2660 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/smithy.py
--rw-rw-rw-   0        0        0     2773 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/smv.py
--rw-rw-rw-   0        0        0     2732 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/snobol.py
--rw-rw-rw-   0        0        0     3127 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/solidity.py
--rw-rw-rw-   0        0        0     3330 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/sophia.py
--rw-rw-rw-   0        0        0     3414 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/special.py
--rw-rw-rw-   0        0        0     2694 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/spice.py
--rw-rw-rw-   0        0        0    34151 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/sql.py
--rw-rw-rw-   0        0        0     1693 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/srcinfo.py
--rw-rw-rw-   0        0        0     6416 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/stata.py
--rw-rw-rw-   0        0        0     3698 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/supercollider.py
--rw-rw-rw-   0        0        0     2639 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/tal.py
--rw-rw-rw-   0        0        0     5513 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/tcl.py
--rw-rw-rw-   0        0        0     3523 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/teal.py
--rw-rw-rw-   0        0        0    72695 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/templates.py
--rw-rw-rw-   0        0        0     9719 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/teraterm.py
--rw-rw-rw-   0        0        0    10767 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/testing.py
--rw-rw-rw-   0        0        0     1029 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/text.py
--rw-rw-rw-   0        0        0     7609 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/textedit.py
--rw-rw-rw-   0        0        0    15192 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/textfmts.py
--rw-rw-rw-   0        0        0    20157 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/theorem.py
--rw-rw-rw-   0        0        0     4228 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/thingsdb.py
--rw-rw-rw-   0        0        0     1377 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/tlb.py
--rw-rw-rw-   0        0        0    10457 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/tnt.py
--rw-rw-rw-   0        0        0     1474 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/trafficscript.py
--rw-rw-rw-   0        0        0     8207 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/typoscript.py
--rw-rw-rw-   0        0        0     8956 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/ul4.py
--rw-rw-rw-   0        0        0    18512 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/unicon.py
--rw-rw-rw-   0        0        0     6037 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/urbi.py
--rw-rw-rw-   0        0        0     3513 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/usd.py
--rw-rw-rw-   0        0        0     7273 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/varnish.py
--rw-rw-rw-   0        0        0     3885 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/verification.py
--rw-rw-rw-   0        0        0      894 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/web.py
--rw-rw-rw-   0        0        0     5699 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/webassembly.py
--rw-rw-rw-   0        0        0    10517 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/webidl.py
--rw-rw-rw-   0        0        0    40549 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/webmisc.py
--rw-rw-rw-   0        0        0     4018 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/whiley.py
--rw-rw-rw-   0        0        0     4021 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/wowtoc.py
--rw-rw-rw-   0        0        0     3239 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/wren.py
--rw-rw-rw-   0        0        0     1920 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/x10.py
--rw-rw-rw-   0        0        0      902 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/xorg.py
--rw-rw-rw-   0        0        0     4500 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/yang.py
--rw-rw-rw-   0        0        0     3953 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/lexers/zig.py
--rw-rw-rw-   0        0        0      986 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/modeline.py
--rw-rw-rw-   0        0        0     2579 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/plugin.py
--rw-rw-rw-   0        0        0     3072 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/regexopt.py
--rw-rw-rw-   0        0        0     3092 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/scanner.py
--rw-rw-rw-   0        0        0     6816 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/sphinxext.py
--rw-rw-rw-   0        0        0     6245 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/style.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.988474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/
--rw-rw-rw-   0        0        0     3395 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/__init__.py
--rw-rw-rw-   0        0        0      705 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/abap.py
--rw-rw-rw-   0        0        0     2216 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/algol.py
--rw-rw-rw-   0        0        0     2231 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/algol_nu.py
--rw-rw-rw-   0        0        0     4443 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/arduino.py
--rw-rw-rw-   0        0        0     2096 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/autumn.py
--rw-rw-rw-   0        0        0     1514 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/borland.py
--rw-rw-rw-   0        0        0     1308 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/bw.py
--rw-rw-rw-   0        0        0     2730 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/colorful.py
--rw-rw-rw-   0        0        0     2488 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/default.py
--rw-rw-rw-   0        0        0     3314 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/dracula.py
--rw-rw-rw-   0        0        0     2439 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/emacs.py
--rw-rw-rw-   0        0        0     2502 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/friendly.py
--rw-rw-rw-   0        0        0     2707 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/friendly_grayscale.py
--rw-rw-rw-   0        0        0     1274 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/fruity.py
--rw-rw-rw-   0        0        0     3481 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/gh_dark.py
--rw-rw-rw-   0        0        0     3230 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/gruvbox.py
--rw-rw-rw-   0        0        0      692 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/igor.py
--rw-rw-rw-   0        0        0     2302 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/inkpot.py
--rw-rw-rw-   0        0        0     2016 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/lilypond.py
--rw-rw-rw-   0        0        0     3117 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/lovelace.py
--rw-rw-rw-   0        0        0     2350 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/manni.py
--rw-rw-rw-   0        0        0     4083 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/material.py
--rw-rw-rw-   0        0        0     5063 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/monokai.py
--rw-rw-rw-   0        0        0     2703 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/murphy.py
--rw-rw-rw-   0        0        0     1948 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/native.py
--rw-rw-rw-   0        0        0     5244 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/nord.py
--rw-rw-rw-   0        0        0     1664 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/onedark.py
--rw-rw-rw-   0        0        0     5526 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/paraiso_dark.py
--rw-rw-rw-   0        0        0     5530 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/paraiso_light.py
--rw-rw-rw-   0        0        0     2425 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/pastie.py
--rw-rw-rw-   0        0        0     2128 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/perldoc.py
--rw-rw-rw-   0        0        0     2432 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/rainbow_dash.py
--rw-rw-rw-   0        0        0      874 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/rrt.py
--rw-rw-rw-   0        0        0     1393 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/sas.py
--rw-rw-rw-   0        0        0     4078 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/solarized.py
--rw-rw-rw-   0        0        0      770 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/staroffice.py
--rw-rw-rw-   0        0        0     1198 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/stata_dark.py
--rw-rw-rw-   0        0        0     1227 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/stata_light.py
--rw-rw-rw-   0        0        0     7039 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/tango.py
--rw-rw-rw-   0        0        0     1885 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/trac.py
--rw-rw-rw-   0        0        0     1922 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/vim.py
--rw-rw-rw-   0        0        0     1026 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/vs.py
--rw-rw-rw-   0        0        0     1453 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/xcode.py
--rw-rw-rw-   0        0        0     2148 2023-04-01 14:17:49.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/styles/zenburn.py
--rw-rw-rw-   0        0        0     6184 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/token.py
--rw-rw-rw-   0        0        0    63187 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/unistring.py
--rw-rw-rw-   0        0        0     9110 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pygments/util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:21.993476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/
--rw-rw-rw-   0        0        0     1644 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0       12 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/pywin32_ctypes-0.2.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.009476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer/
--rw-rw-rw-   0        0        0     1119 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer/__about__.py
--rw-rw-rw-   0        0        0      573 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer/__init__.py
--rw-rw-rw-   0        0        0      625 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer/__main__.py
--rw-rw-rw-   0        0        0     4290 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer/clean.py
--rw-rw-rw-   0        0        0     3595 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer/markdown.py
--rw-rw-rw-   0        0        0     4460 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer/rst.py
--rw-rw-rw-   0        0        0      823 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer/txt.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.012476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer-37.3.dist-info/
--rw-rw-rw-   0        0        0       16 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/readme_renderer-37.3.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.056476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/
--rw-rw-rw-   0        0        0     4972 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/__init__.py
--rw-rw-rw-   0        0        0      435 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/__version__.py
--rw-rw-rw-   0        0        0     1397 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    21287 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/adapters.py
--rw-rw-rw-   0        0        0     6377 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/api.py
--rw-rw-rw-   0        0        0    10187 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/auth.py
--rw-rw-rw-   0        0        0      429 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/certs.py
--rw-rw-rw-   0        0        0     1451 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/compat.py
--rw-rw-rw-   0        0        0    18560 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/cookies.py
--rw-rw-rw-   0        0        0     3811 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/exceptions.py
--rw-rw-rw-   0        0        0     3875 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/help.py
--rw-rw-rw-   0        0        0      733 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/hooks.py
--rw-rw-rw-   0        0        0    35223 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/models.py
--rw-rw-rw-   0        0        0      957 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/packages.py
--rw-rw-rw-   0        0        0    30180 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/structures.py
--rw-rw-rw-   0        0        0    33228 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.058476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests-2.28.2.dist-info/
--rw-rw-rw-   0        0        0        9 2023-04-01 14:17:58.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests-2.28.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.070476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/
--rw-rw-rw-   0        0        0     1189 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/__init__.py
--rw-rw-rw-   0        0        0     9512 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/_compat.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.093476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/adapters/
--rw-rw-rw-   0        0        0      370 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/adapters/__init__.py
--rw-rw-rw-   0        0        0     7539 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/adapters/appengine.py
--rw-rw-rw-   0        0        0     1404 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/adapters/fingerprint.py
--rw-rw-rw-   0        0        0     1396 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/adapters/host_header_ssl.py
--rw-rw-rw-   0        0        0     4789 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/adapters/socket_options.py
--rw-rw-rw-   0        0        0     2608 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/adapters/source.py
--rw-rw-rw-   0        0        0     2399 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/adapters/ssl.py
--rw-rw-rw-   0        0        0     7854 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/adapters/x509.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.105478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/auth/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/auth/__init__.py
--rw-rw-rw-   0        0        0      910 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
--rw-rw-rw-   0        0        0     4944 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/auth/guess.py
--rw-rw-rw-   0        0        0     4407 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/auth/handler.py
--rw-rw-rw-   0        0        0     3706 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/auth/http_proxy_digest.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.109476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/cookies/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/cookies/__init__.py
--rw-rw-rw-   0        0        0      213 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/cookies/forgetful.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.115475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/downloadutils/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/downloadutils/__init__.py
--rw-rw-rw-   0        0        0     6024 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/downloadutils/stream.py
--rw-rw-rw-   0        0        0     4365 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/downloadutils/tee.py
--rw-rw-rw-   0        0        0     1135 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.123477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/multipart/
--rw-rw-rw-   0        0        0      854 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/multipart/__init__.py
--rw-rw-rw-   0        0        0     4861 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/multipart/decoder.py
--rw-rw-rw-   0        0        0    20769 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/multipart/encoder.py
--rw-rw-rw-   0        0        0     3102 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/sessions.py
--rw-rw-rw-   0        0        0     4044 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/streaming_iterator.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.130483 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/threaded/
--rw-rw-rw-   0        0        0     3213 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/threaded/__init__.py
--rw-rw-rw-   0        0        0     6628 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/threaded/pool.py
--rw-rw-rw-   0        0        0     1465 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/threaded/thread.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.144476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/utils/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/utils/__init__.py
--rw-rw-rw-   0        0        0     2558 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/utils/deprecated.py
--rw-rw-rw-   0        0        0     6522 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/utils/dump.py
--rw-rw-rw-   0        0        0     3233 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/utils/formdata.py
--rw-rw-rw-   0        0        0     4524 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt/utils/user_agent.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.073477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/
--rw-rw-rw-   0        0        0       18 2023-04-01 14:18:02.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/requests_toolbelt-0.10.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.177476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/
--rw-rw-rw-   0        0        0     1565 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/__init__.py
--rw-rw-rw-   0        0        0    13297 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/_mixin.py
--rw-rw-rw-   0        0        0     9048 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/abnf_regexp.py
--rw-rw-rw-   0        0        0     3862 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/api.py
--rw-rw-rw-   0        0        0    12709 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/builder.py
--rw-rw-rw-   0        0        0     1620 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/compat.py
--rw-rw-rw-   0        0        0     3614 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/exceptions.py
--rw-rw-rw-   0        0        0     5477 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/iri.py
--rw-rw-rw-   0        0        0     4114 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/misc.py
--rw-rw-rw-   0        0        0     5261 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/normalizers.py
--rw-rw-rw-   0        0        0    14599 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/parseresult.py
--rw-rw-rw-   0        0        0     5183 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/uri.py
--rw-rw-rw-   0        0        0    13676 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.180476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986-2.0.0.dist-info/
--rw-rw-rw-   0        0        0        8 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.377475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/
--rw-rw-rw-   0        0        0     6066 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/__init__.py
--rw-rw-rw-   0        0        0     8334 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/__main__.py
--rw-rw-rw-   0        0        0    10096 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_cell_widths.py
--rw-rw-rw-   0        0        0   140235 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_emoji_codes.py
--rw-rw-rw-   0        0        0     1064 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_emoji_replace.py
--rw-rw-rw-   0        0        0     2100 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_export_format.py
--rw-rw-rw-   0        0        0      241 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_extension.py
--rw-rw-rw-   0        0        0      799 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_fileno.py
--rw-rw-rw-   0        0        0     9695 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_inspect.py
--rw-rw-rw-   0        0        0     3213 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_log_render.py
--rw-rw-rw-   0        0        0     1236 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_loop.py
--rw-rw-rw-   0        0        0     1387 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_null_file.py
--rw-rw-rw-   0        0        0     7063 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_palettes.py
--rw-rw-rw-   0        0        0      423 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_pick.py
--rw-rw-rw-   0        0        0     5460 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_ratio.py
--rw-rw-rw-   0        0        0    19919 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_spinners.py
--rw-rw-rw-   0        0        0      351 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_stack.py
--rw-rw-rw-   0        0        0      417 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_timer.py
--rw-rw-rw-   0        0        0    22784 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_win32_console.py
--rw-rw-rw-   0        0        0     1902 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_windows.py
--rw-rw-rw-   0        0        0     2759 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_windows_renderer.py
--rw-rw-rw-   0        0        0     1840 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/_wrap.py
--rw-rw-rw-   0        0        0      878 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/abc.py
--rw-rw-rw-   0        0        0    10320 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/align.py
--rw-rw-rw-   0        0        0     6906 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/ansi.py
--rw-rw-rw-   0        0        0     3264 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/bar.py
--rw-rw-rw-   0        0        0     9794 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/box.py
--rw-rw-rw-   0        0        0     4509 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/cells.py
--rw-rw-rw-   0        0        0    18224 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/color.py
--rw-rw-rw-   0        0        0     1054 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/color_triplet.py
--rw-rw-rw-   0        0        0     7131 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/columns.py
--rw-rw-rw-   0        0        0    99123 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/console.py
--rw-rw-rw-   0        0        0     1288 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/constrain.py
--rw-rw-rw-   0        0        0     5497 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/containers.py
--rw-rw-rw-   0        0        0     6606 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/control.py
--rw-rw-rw-   0        0        0     8046 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/default_styles.py
--rw-rw-rw-   0        0        0      924 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/diagnose.py
--rw-rw-rw-   0        0        0     2465 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/emoji.py
--rw-rw-rw-   0        0        0      642 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/errors.py
--rw-rw-rw-   0        0        0     1683 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/file_proxy.py
--rw-rw-rw-   0        0        0     2508 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/filesize.py
--rw-rw-rw-   0        0        0     9584 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/highlighter.py
--rw-rw-rw-   0        0        0     5020 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/json.py
--rw-rw-rw-   0        0        0     3228 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/jupyter.py
--rw-rw-rw-   0        0        0    13947 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/layout.py
--rw-rw-rw-   0        0        0    14273 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/live.py
--rw-rw-rw-   0        0        0     3655 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/live_render.py
--rw-rw-rw-   0        0        0    11891 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/logging.py
--rw-rw-rw-   0        0        0    22368 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/markdown.py
--rw-rw-rw-   0        0        0     8174 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/markup.py
--rw-rw-rw-   0        0        0     5305 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/measure.py
--rw-rw-rw-   0        0        0     4958 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/padding.py
--rw-rw-rw-   0        0        0      828 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/pager.py
--rw-rw-rw-   0        0        0     3288 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/palette.py
--rw-rw-rw-   0        0        0    10574 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/panel.py
--rw-rw-rw-   0        0        0    35816 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/pretty.py
--rw-rw-rw-   0        0        0    59694 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/progress.py
--rw-rw-rw-   0        0        0     8165 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/progress_bar.py
--rw-rw-rw-   0        0        0    11291 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/prompt.py
--rw-rw-rw-   0        0        0     1367 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/protocol.py
--rw-rw-rw-   0        0        0      166 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/region.py
--rw-rw-rw-   0        0        0     4419 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/repr.py
--rw-rw-rw-   0        0        0     4590 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/rule.py
--rw-rw-rw-   0        0        0     2831 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/scope.py
--rw-rw-rw-   0        0        0     1579 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/screen.py
--rw-rw-rw-   0        0        0    24211 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/segment.py
--rw-rw-rw-   0        0        0     4339 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/spinner.py
--rw-rw-rw-   0        0        0     4425 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/status.py
--rw-rw-rw-   0        0        0    27073 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/style.py
--rw-rw-rw-   0        0        0     1234 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/styled.py
--rw-rw-rw-   0        0        0    35045 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/syntax.py
--rw-rw-rw-   0        0        0    39648 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/table.py
--rw-rw-rw-   0        0        0     3370 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/terminal_theme.py
--rw-rw-rw-   0        0        0    45513 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/text.py
--rw-rw-rw-   0        0        0     3777 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/theme.py
--rw-rw-rw-   0        0        0      102 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/themes.py
--rw-rw-rw-   0        0        0    29532 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/traceback.py
--rw-rw-rw-   0        0        0     9109 2023-04-01 14:18:01.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/rich/tree.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.450476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/
--rw-rw-rw-   0        0        0     5528 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/__init__.py
--rw-rw-rw-   0        0        0      218 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_deprecation_warning.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.540476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/
--rw-rw-rw-   0        0        0      537 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/_collections.py
--rw-rw-rw-   0        0        0      411 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/_functools.py
--rw-rw-rw-   0        0        0      239 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-rw-rw-   0        0        0    20662 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-rw-   0        0        0     8601 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-rw-   0        0        0    14515 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-rw-   0        0        0    47023 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-rw-   0        0        0    17943 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.606476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/
--rw-rw-rw-   0        0        0      626 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-rw-   0        0        0     1614 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-rw-rw-   0        0        0     5253 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-rw-   0        0        0     4654 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-rw-   0        0        0    39304 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py
--rw-rw-rw-   0        0        0    21882 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-rw-   0        0        0    15683 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rw-rw-rw-   0        0        0     5593 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-rw-rw-   0        0        0     7710 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-rw-   0        0        0    31359 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-rw-   0        0        0    16552 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-rw-   0        0        0     5610 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-rw-   0        0        0     4889 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-rw-rw-   0        0        0     2603 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-rw-   0        0        0    13131 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-rw-rw-   0        0        0    30191 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-rw-rw-   0        0        0     2779 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-rw-   0        0        0     2771 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-rw-   0        0        0     1189 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-rw-   0        0        0     8434 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-rw-   0        0        0     1936 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-rw-   0        0        0      672 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-rw-   0        0        0    11764 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-rw-rw-   0        0        0    19237 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-rw-   0        0        0     7451 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-rw-   0        0        0     4906 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/config.py
--rw-rw-rw-   0        0        0     9251 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/core.py
--rw-rw-rw-   0        0        0    15157 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-rw-   0        0        0      139 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/debug.py
--rw-rw-rw-   0        0        0     3425 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-rw-   0        0        0     8023 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-rw-   0        0        0    50131 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/dist.py
--rw-rw-rw-   0        0        0     3589 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/errors.py
--rw-rw-rw-   0        0        0    10248 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/extension.py
--rw-rw-rw-   0        0        0    17781 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-rw-   0        0        0     8092 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-rw-rw-   0        0        0    13683 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-rw-rw-   0        0        0     1972 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/log.py
--rw-rw-rw-   0        0        0    29873 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-rw-   0        0        0    23279 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-rw-   0        0        0      213 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-rw-   0        0        0      639 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/py39compat.py
--rw-rw-rw-   0        0        0     3469 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-rw-rw-   0        0        0    18577 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-rw-   0        0        0    12094 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-rw-rw-   0        0        0    15588 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-rw-   0        0        0    18208 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/util.py
--rw-rw-rw-   0        0        0    12934 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/version.py
--rw-rw-rw-   0        0        0     5248 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-rw-   0        0        0     1972 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_entry_points.py
--rw-rw-rw-   0        0        0     2392 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_imp.py
--rw-rw-rw-   0        0        0     1311 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_importlib.py
--rw-rw-rw-   0        0        0      675 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_itertools.py
--rw-rw-rw-   0        0        0      176 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_path.py
--rw-rw-rw-   0        0        0      501 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_reqs.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.616490 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.637476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_metadata/
--rw-rw-rw-   0        0        0    30130 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-rw-rw-   0        0        0     1862 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-rw-rw-   0        0        0      743 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-rw-rw-   0        0        0     1828 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-rw-rw-   0        0        0     2895 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-rw-rw-   0        0        0     2068 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-rw-rw-   0        0        0     1154 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-rw-rw-   0        0        0     2166 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.660479 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.669474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13512 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.671476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15517 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.679476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       82 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   117959 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    16256 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-rw-   0        0        0    15130 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.708476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8493 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4700 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.734474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6429 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213278 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.736474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23003 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9030 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39007 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25353 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13388 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10381 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.748479 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    87149 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-rw-rw-   0        0        0     8425 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/_vendor/zipp.py
--rw-rw-rw-   0        0        0     7346 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/archive_util.py
--rw-rw-rw-   0        0        0    10875 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/build_meta.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.814476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/
--rw-rw-rw-   0        0        0      217 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/__init__.py
--rw-rw-rw-   0        0        0     2381 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/alias.py
--rw-rw-rw-   0        0        0    16623 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-rw-rw-   0        0        0     1182 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-rw-   0        0        0      835 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/build.py
--rw-rw-rw-   0        0        0     4415 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/build_clib.py
--rw-rw-rw-   0        0        0    13212 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/build_ext.py
--rw-rw-rw-   0        0        0    10935 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/build_py.py
--rw-rw-rw-   0        0        0     7012 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/develop.py
--rw-rw-rw-   0        0        0     2106 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/dist_info.py
--rw-rw-rw-   0        0        0    85662 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/easy_install.py
--rw-rw-rw-   0        0        0    26216 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/egg_info.py
--rw-rw-rw-   0        0        0     5163 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/install.py
--rw-rw-rw-   0        0        0     2226 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-rw-rw-   0        0        0     3875 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/install_lib.py
--rw-rw-rw-   0        0        0     2612 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/install_scripts.py
--rw-rw-rw-   0        0        0     4946 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/py36compat.py
--rw-rw-rw-   0        0        0      468 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/register.py
--rw-rw-rw-   0        0        0     2128 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/rotate.py
--rw-rw-rw-   0        0        0      658 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/saveopts.py
--rw-rw-rw-   0        0        0     6422 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/sdist.py
--rw-rw-rw-   0        0        0     5086 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/setopt.py
--rw-rw-rw-   0        0        0     8133 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/test.py
--rw-rw-rw-   0        0        0      462 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/upload.py
--rw-rw-rw-   0        0        0     7492 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/command/upload_docs.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.829476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/
--rw-rw-rw-   0        0        0     1121 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/__init__.py
--rw-rw-rw-   0        0        0    13398 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.845479 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/_validate_pyproject/
--rw-rw-rw-   0        0        0     1038 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-rw-rw-   0        0        0    11266 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-rw-rw-   0        0        0     1181 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-rw-rw-   0        0        0     1612 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-rw-rw-   0        0        0   269900 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-rw-rw-   0        0        0     8647 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-rw-rw-   0        0        0    16779 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/expand.py
--rw-rw-rw-   0        0        0    18950 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-rw-rw-   0        0        0    23009 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/config/setupcfg.py
--rw-rw-rw-   0        0        0      949 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/dep_util.py
--rw-rw-rw-   0        0        0     5499 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/depends.py
--rw-rw-rw-   0        0        0    20785 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/discovery.py
--rw-rw-rw-   0        0        0    45578 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/dist.py
--rw-rw-rw-   0        0        0     2464 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/errors.py
--rw-rw-rw-   0        0        0     5270 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/extension.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.847476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/extern/
--rw-rw-rw-   0        0        0     2512 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/extern/__init__.py
--rw-rw-rw-   0        0        0     4873 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/glob.py
--rw-rw-rw-   0        0        0     3824 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/installer.py
--rw-rw-rw-   0        0        0      812 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/launch.py
--rw-rw-rw-   0        0        0     1149 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/logging.py
--rw-rw-rw-   0        0        0     5217 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/monkey.py
--rw-rw-rw-   0        0        0    50561 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/msvc.py
--rw-rw-rw-   0        0        0     3093 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/namespaces.py
--rw-rw-rw-   0        0        0    40020 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/package_index.py
--rw-rw-rw-   0        0        0      245 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/py34compat.py
--rw-rw-rw-   0        0        0    14348 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/sandbox.py
--rw-rw-rw-   0        0        0      941 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/unicode_utils.py
--rw-rw-rw-   0        0        0      144 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/version.py
--rw-rw-rw-   0        0        0     8303 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/wheel.py
--rw-rw-rw-   0        0        0      718 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools/windows_support.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.455475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools-63.2.0.dist-info/
--rw-rw-rw-   0        0        0     2674 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools-63.2.0.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-04-01 14:06:53.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/setuptools-63.2.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.849477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/six-1.16.0.dist-info/
--rw-rw-rw-   0        0        0        4 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/six-1.16.0.dist-info/top_level.txt
--rw-rw-rw-   0        0        0    34549 2023-04-01 14:17:48.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/six.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.878476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/
--rw-rw-rw-   0        0        0     1343 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/__init__.py
--rw-rw-rw-   0        0        0     1475 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/__main__.py
--rw-rw-rw-   0        0        0     3129 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/auth.py
--rw-rw-rw-   0        0        0     3738 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.892478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/commands/
--rw-rw-rw-   0        0        0     1802 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/commands/__init__.py
--rw-rw-rw-   0        0        0     5727 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/commands/check.py
--rw-rw-rw-   0        0        0     2904 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/commands/register.py
--rw-rw-rw-   0        0        0     7469 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/commands/upload.py
--rw-rw-rw-   0        0        0     3814 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/exceptions.py
--rw-rw-rw-   0        0        0    11024 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/package.py
--rw-rw-rw-   0        0        0     8713 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/repository.py
--rw-rw-rw-   0        0        0    12269 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/settings.py
--rw-rw-rw-   0        0        0    10867 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/utils.py
--rw-rw-rw-   0        0        0     3049 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/wheel.py
--rw-rw-rw-   0        0        0     1795 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine/wininst.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.883474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine-4.0.2.dist-info/
--rw-rw-rw-   0        0        0      185 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine-4.0.2.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-01 14:18:03.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/twine-4.0.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.919475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/
--rw-rw-rw-   0        0        0     3333 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/__init__.py
--rw-rw-rw-   0        0        0    10811 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/_collections.py
--rw-rw-rw-   0        0        0       64 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/_version.py
--rw-rw-rw-   0        0        0    20300 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/connection.py
--rw-rw-rw-   0        0        0    39128 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.941476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/__init__.py
--rw-rw-rw-   0        0        0      957 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/_appengine_environ.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.948475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    17632 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    13922 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    11012 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/appengine.py
--rw-rw-rw-   0        0        0     4528 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/ntlmpool.py
--rw-rw-rw-   0        0        0    17055 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34416 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7097 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     8217 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/exceptions.py
--rw-rw-rw-   0        0        0     8579 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/fields.py
--rw-rw-rw-   0        0        0     2440 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/filepost.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.952474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/packages/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.957477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/packages/backports/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/packages/backports/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/packages/backports/makefile.py
--rw-rw-rw-   0        0        0    34665 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/packages/six.py
--rw-rw-rw-   0        0        0    19786 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0     5985 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/request.py
--rw-rw-rw-   0        0        0    30761 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.990478 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/
--rw-rw-rw-   0        0        0     1155 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1605 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0      498 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/queue.py
--rw-rw-rw-   0        0        0     4225 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3510 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/response.py
--rw-rw-rw-   0        0        0    22003 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    17165 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     5758 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/ssl_match_hostname.py
--rw-rw-rw-   0        0        0     6895 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10168 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    14279 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/url.py
--rw-rw-rw-   0        0        0     5403 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3/util/wait.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:22.925480 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3-1.26.15.dist-info/
--rw-rw-rw-   0        0        0     1115 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3-1.26.15.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0        8 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/urllib3-1.26.15.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.005476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/webencodings/
--rw-rw-rw-   0        0        0    10579 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/webencodings/__init__.py
--rw-rw-rw-   0        0        0     8979 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/webencodings/labels.py
--rw-rw-rw-   0        0        0     1305 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/webencodings/mklabels.py
--rw-rw-rw-   0        0        0     6563 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/webencodings/tests.py
--rw-rw-rw-   0        0        0     4307 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/webencodings/x_user_defined.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.007475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/webencodings-0.5.1.dist-info/
--rw-rw-rw-   0        0        0       13 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/webencodings-0.5.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.020475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/
--rw-rw-rw-   0        0        0      214 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.027476 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/
--rw-rw-rw-   0        0        0     1864 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/__init__.py
--rw-rw-rw-   0        0        0      199 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/_winerrors.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.048474 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/__init__.py
--rw-rw-rw-   0        0        0     4964 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/_authentication.py
--rw-rw-rw-   0        0        0      554 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/_common.py
--rw-rw-rw-   0        0        0      866 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/_dll.py
--rw-rw-rw-   0        0        0      355 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/_nl_support.py
--rw-rw-rw-   0        0        0     4584 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/_resource.py
--rw-rw-rw-   0        0        0      882 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/_system_information.py
--rw-rw-rw-   0        0        0      374 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/_time.py
--rw-rw-rw-   0        0        0     2723 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/cffi/_util.py
--rw-rw-rw-   0        0        0      560 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/compat.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.072475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/
--rw-rw-rw-   0        0        0        0 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/__init__.py
--rw-rw-rw-   0        0        0     3627 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/_authentication.py
--rw-rw-rw-   0        0        0     1502 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/_common.py
--rw-rw-rw-   0        0        0      594 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/_dll.py
--rw-rw-rw-   0        0        0      357 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/_nl_support.py
--rw-rw-rw-   0        0        0     4252 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/_resource.py
--rw-rw-rw-   0        0        0      983 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/_system_information.py
--rw-rw-rw-   0        0        0      384 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/_time.py
--rw-rw-rw-   0        0        0     2049 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/core/ctypes/_util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.081475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/pywin32/
--rw-rw-rw-   0        0        0      396 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/pywin32/__init__.py
--rw-rw-rw-   0        0        0      954 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/pywin32/pywintypes.py
--rw-rw-rw-   0        0        0     7768 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/pywin32/win32api.py
--rw-rw-rw-   0        0        0     2850 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/pywin32/win32cred.py
--rw-rw-rw-   0        0        0      342 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/pywintypes.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.091475 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/tests/
--rw-rw-rw-   0        0        0      612 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/tests/__init__.py
--rw-rw-rw-   0        0        0     2545 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/tests/compat.py
--rw-rw-rw-   0        0        0    11110 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/tests/test_win32api.py
--rw-rw-rw-   0        0        0     5710 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/tests/test_win32cred.py
--rw-rw-rw-   0        0        0       21 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/version.py
--rw-rw-rw-   0        0        0      338 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/win32api.py
--rw-rw-rw-   0        0        0      340 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/win32ctypes/win32cred.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.096486 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/zipp/
--rw-rw-rw-   0        0        0    10676 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/zipp/__init__.py
--rw-rw-rw-   0        0        0      309 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/zipp/py310compat.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.099477 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/zipp-3.15.0.dist-info/
--rw-rw-rw-   0        0        0        5 2023-04-01 14:17:47.000000 python-geofs-0.1.4rc2/geofs-env/Lib/site-packages/zipp-3.15.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.127475 python-geofs-0.1.4rc2/geofs-env/Scripts/
--rw-rw-rw-   0        0        0      646 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2html.py
--rw-rw-rw-   0        0        0      768 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2html4.py
--rw-rw-rw-   0        0        0     1113 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2html5.py
--rw-rw-rw-   0        0        0      845 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2latex.py
--rw-rw-rw-   0        0        0      668 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2man.py
--rw-rw-rw-   0        0        0      834 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2odt.py
--rw-rw-rw-   0        0        0     1772 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2odt_prepstyles.py
--rw-rw-rw-   0        0        0      653 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2pseudoxml.py
--rw-rw-rw-   0        0        0      689 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2s5.py
--rw-rw-rw-   0        0        0      925 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2xetex.py
--rw-rw-rw-   0        0        0      654 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rst2xml.py
--rw-rw-rw-   0        0        0      722 2023-04-01 14:17:56.000000 python-geofs-0.1.4rc2/geofs-env/Scripts/rstpep2html.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:32:23.163475 python-geofs-0.1.4rc2/python_geofs.egg-info/
--rw-rw-rw-   0        0        0      308 2023-04-03 17:32:17.000000 python-geofs-0.1.4rc2/python_geofs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    99548 2023-04-03 17:32:18.000000 python-geofs-0.1.4rc2/python_geofs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 17:32:17.000000 python-geofs-0.1.4rc2/python_geofs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-03 17:32:17.000000 python-geofs-0.1.4rc2/python_geofs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 17:32:23.167474 python-geofs-0.1.4rc2/setup.cfg
--rw-rw-rw-   0        0        0      664 2023-04-03 17:32:11.000000 python-geofs-0.1.4rc2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 17:59:50.793202 python-geofs-0.1.5/
+-rw-rw-rw-   0        0        0       84 2023-04-02 00:10:51.000000 python-geofs-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1045 2023-04-01 14:20:41.000000 python-geofs-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       57 2023-04-03 18:39:42.000000 python-geofs-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      305 2023-04-07 17:59:50.792192 python-geofs-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2166 2023-04-02 00:07:29.000000 python-geofs-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-07 17:59:50.794184 python-geofs-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-04-07 17:59:19.000000 python-geofs-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 17:59:50.688912 python-geofs-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-07 17:59:50.751899 python-geofs-0.1.5/src/geofs/
+-rw-rw-rw-   0        0        0       95 2023-04-03 17:21:28.000000 python-geofs-0.1.5/src/geofs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 17:59:50.760152 python-geofs-0.1.5/src/geofs/data/
+-rw-rw-rw-   0        0        0     7413 2023-04-03 17:35:49.000000 python-geofs-0.1.5/src/geofs/data/aircraftcodes.json
+-rw-rw-rw-   0        0        0     3197 2023-04-06 12:49:18.000000 python-geofs-0.1.5/src/geofs/mapAPI.py
+-rw-rw-rw-   0        0        0     4995 2023-04-06 15:37:23.000000 python-geofs-0.1.5/src/geofs/multiplayerAPI.py
+drwxrwxrwx   0        0        0        0 2023-04-07 17:59:50.789183 python-geofs-0.1.5/src/python_geofs.egg-info/
+-rw-rw-rw-   0        0        0      305 2023-04-07 17:59:50.000000 python-geofs-0.1.5/src/python_geofs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-04-07 17:59:50.000000 python-geofs-0.1.5/src/python_geofs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 17:59:50.000000 python-geofs-0.1.5/src/python_geofs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-07 17:59:50.000000 python-geofs-0.1.5/src/python_geofs.egg-info/top_level.txt
```

### Comparing `python-geofs-0.1.4rc2/LICENSE.txt` & `python-geofs-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-geofs-0.1.4rc2/README.md` & `python-geofs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `python-geofs-0.1.4rc2/geofs/data/aircraftcodes.json` & `python-geofs-0.1.5/src/geofs/data/aircraftcodes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982394366197183%*

 * *Differences: {"'2852'": "{'name': 'Rozi�re Balloon'}"}*

```diff
@@ -242,15 +242,15 @@
     "2843": {
         "name": "A220-300 (Air Tanzania)"
     },
     "2844": {
         "name": "Falcon 9"
     },
     "2852": {
-        "name": "Rozire Balloon"
+        "name": "Rozi\ufffdre Balloon"
     },
     "2856": {
         "name": "Airbus A400M Atlas"
     },
     "2857": {
         "name": "F-22 Raptor"
     },
```

### Comparing `python-geofs-0.1.4rc2/geofs/mapAPI.py` & `python-geofs-0.1.5/src/geofs/mapAPI.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,62 +13,70 @@
     def __init__ (self,userobj):
         #add grounded
         self.airspeed = userobj['st']['as']
         self.userInfo = {'id':userobj['acid'],'callsign':userobj['cs']}
         self.coordinates = (userobj['co'][0],userobj['co'][1])
         self.altitude = round(userobj['co'][2]*3.28084,2) # meters to feet
         self.verticalSpeed = round(userobj['co'][3]*3.28084,2) # meters to feet
-        aircraftcodesPath = pkg_resources.resource_filename(__name__, "data/aircraftcodes.json")
         try:
-            self.aircraft = {'type':json.loads(open(aircraftcodesPath).read())[str(userobj['ac'])],'id':userobj['ac']}
+            with pkg_resources.resource_stream("geofs", "data/aircraftcodes.json") as reader:
+                aircrafCodes = json.load(reader)
+            self.aircraft = {
+                'type':aircrafCodes[str(userobj['ac'])],
+                'id':userobj['ac']
+            }
         except KeyError:
-            print("hello")
-            self.aircraft = {'type':"Unknown",'id':userobj['ac']}
+            self.aircraft = {
+                'type':"Unknown",
+                'id':userobj['ac']
+            }
 ## MAIN CLASS ##
 class MapAPI:
     def __init__(self):
         self._responseList = []
         self._utilizeResponseList = True
+        self.error = False
     def getUsers(self,foos):
-        while True:
-            try:
-                response = requests.post(
-                    "https://mps.geo-fs.com/map",
-                    json = {
-                        "id":"",
-                        "gid": None
-                    }
-                )
-                response_body = json.loads(response.text)
-                userList = []
-                if foos == False:
-                    for user in response_body['users']:
-                        if user['cs'] == "Foo" or user['cs'] == '':
-                            pass
-                        else:
-                            userList.append(Player(user))
-                elif foos == True:
-                    for user in response_body['users']:
-                        if user['cs'] != "Foo":
-                            pass
-                        else:
-                            userList.append(Player(user))
-                elif foos == None:
-                    userList.append(Player(user))
+        self.error = False
+        try:
+            response = requests.post(
+                "https://mps.geo-fs.com/map",
+                json = {
+                    "id":"",
+                    "gid": None
+                }
+            )
+            response_body = json.loads(response.text)
+            userList = []
+            if foos == False:
+                for user in response_body['users']:
+                    if user['cs'] == "Foo" or user['cs'] == '':
+                        pass
+                    else:
+                        userList.append(Player(user))
+            elif foos == True:
+                for user in response_body['users']:
+                    if user['cs'] != "Foo":
+                        pass
+                    else:
+                        userList.append(Player(user))
+            elif foos == None:
+                userList.append(Player(user))
             
             
-                else:
-                    raise AttributeError('"Foos" attribute must be boolean or NoneType.')
-                if self._utilizeResponseList == True:
-                    self._responseList.append(userList)
-                return userList
-            except Exception as e:
-                print("Unable to connect to GeoFS. Check your connection and restart the application.")
-                print(f"Error Code 1: {e}")
-                time.sleep(5)
+            else:
+                raise AttributeError('"Foos" attribute must be boolean or NoneType.')
+            if self._utilizeResponseList == True:
+                self._responseList.append(userList)
+            return userList
+        except Exception as e:
+            self.error = True
+            print("Unable to connect to GeoFS. Check your connection and restart the application.")
+            print(f"Error Code 1: {e}")
+            return None
 
     def returnResponseList(self,reset:bool):
         if reset == True:
             before = self._responseList
             self._responseList = []
             return before
         return self._responseList
```

### Comparing `python-geofs-0.1.4rc2/geofs/multiplayerAPI.py` & `python-geofs-0.1.5/src/geofs/multiplayerAPI.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,122 +4,124 @@
 
 class multiplayerAPI:
     def __init__(self, sessionID, accountID):
         self.sessionID = sessionID
         self.accountID = accountID
         self.myID = None
         self.lastMsgID = 0
+        self.error = False
     
     def handshake(self): # initializes connection and gains mandatory variables from server.
         # initializes server connection and gets details from server.
-        while True:
-            body = {
+        self.error = False
+        body = {
+            "origin": "https://www.geo-fs.com",
+            "acid": self.accountID,
+            "sid": self.sessionID,
+            "id": "",
+            "ac": "1",
+            "co": [42.36021568682466,-70.98767598755524,4.589746820023676,-103.04273973572526,-15.919583740307557,-0.376840533503692],
+            "ve": [2.7011560632672626e-10,7.436167948071671e-11,0.000004503549489433212,0,0,0],
+            "st": {"gr":True,"as":0},
+            "ti": 1678751444055,
+            "m": "", 
+            "ci": 0
+        }
+        try:
+            response = requests.post(
+                "https://mps.geo-fs.com/update",
+                json = body,
+                cookies = {"PHPSESSID": self.sessionID}
+            )
+            print("Successfully connect to server.")
+            response_body = json.loads(response.text)
+            self.myID = response_body["myId"]
+
+
+            body2 = {
                 "origin": "https://www.geo-fs.com",
                 "acid": self.accountID,
                 "sid": self.sessionID,
-                "id": "",
+                "id": self.myID,
                 "ac": "1",
                 "co": [42.36021568682466,-70.98767598755524,4.589746820023676,-103.04273973572526,-15.919583740307557,-0.376840533503692],
                 "ve": [2.7011560632672626e-10,7.436167948071671e-11,0.000004503549489433212,0,0,0],
                 "st": {"gr":True,"as":0},
                 "ti": 1678751444055,
                 "m": "", 
-                "ci": 0
+                "ci": self.lastMsgID
             }
-            try:
-                response = requests.post(
-                    "https://mps.geo-fs.com/update",
-                    json = body,
-                    cookies = {"PHPSESSID": self.sessionID}
-                )
-                print("Successfully connect to server.")
-                response_body = json.loads(response.text)
-                self.myID = response_body["myId"]
-
-
-                body2 = {
-                    "origin": "https://www.geo-fs.com",
-                    "acid": self.accountID,
-                    "sid": self.sessionID,
-                    "id": self.myID,
-                    "ac": "1",
-                    "co": [42.36021568682466,-70.98767598755524,4.589746820023676,-103.04273973572526,-15.919583740307557,-0.376840533503692],
-                    "ve": [2.7011560632672626e-10,7.436167948071671e-11,0.000004503549489433212,0,0,0],
-                    "st": {"gr":True,"as":0},
-                    "ti": 1678751444055,
-                    "m": "", 
-                    "ci": self.lastMsgID
-                }
-                response = requests.post(
-                    "https://mps.geo-fs.com/update",
-                    json = body2,
-                    cookies = {"PHPSESSID": self.sessionID}
-                )
-                response_body = json.loads(response.text)
-                self.myID = response_body["myId"]
-                self.lastMsgID = response_body["lastMsgId"]
-                break
-            except Exception as e:
-                print("Unable to connect to GeoFS. Check your connection and restart the application.")
-                print(f"Error Code 4: {e}")
-                time.sleep(5)
+            response = requests.post(
+                "https://mps.geo-fs.com/update",
+                json = body2,
+                cookies = {"PHPSESSID": self.sessionID}
+            )
+            response_body = json.loads(response.text)
+            self.myID = response_body["myId"]
+            self.lastMsgID = response_body["lastMsgId"]
+            return
+        except Exception as e:
+            self.error = True
+            print("Unable to connect to GeoFS. Check your connection and restart the application.")
+            print(f"Error Code 4: {e}")
+            return
 
     def sendMsg(self, msg):
-        while True:
-            body = {
-                "origin": "https://www.geo-fs.com",
-                "acid": self.accountID,
-                "sid": self.sessionID,
-                "id": self.myID,
-                "ac": "1",
-                "co": [42.36021568682466,-70.98767598755524,4.589746820023676,-103.04273973572526,-15.919583740307557,-0.376840533503692],
-                "ve": [2.7011560632672626e-10,7.436167948071671e-11,0.000004503549489433212,0,0,0],
-                "st": {"gr":True,"as":0},
-                "ti": None,
-                "m": msg,
-                "ci": 0
-            }
-            try:
-                response = requests.post(
-                    "https://mps.geo-fs.com/update",
-                    json = body,
-                    cookies = {"PHPSESSID": self.sessionID}
-                )
-                response_body = json.loads(response.text)
-                self.myID = response_body["myId"]
-                break
-            except Exception as e:
-                print("Unable to connect to GeoFS. Check your connection and restart the application.")
-                print(f"Error Code 3: {e}")
-                time.sleep(5)
+        self.error = False
+        body = {
+            "origin": "https://www.geo-fs.com",
+            "acid": self.accountID,
+            "sid": self.sessionID,
+            "id": self.myID,
+            "ac": "1",
+            "co": [42.36021568682466,-70.98767598755524,4.589746820023676,-103.04273973572526,-15.919583740307557,-0.376840533503692],
+            "ve": [2.7011560632672626e-10,7.436167948071671e-11,0.000004503549489433212,0,0,0],
+            "st": {"gr":True,"as":0},
+            "ti": None,
+            "m": msg,
+            "ci": 0
+        }
+        try:
+            response = requests.post(
+                "https://mps.geo-fs.com/update",
+                json = body,
+                cookies = {"PHPSESSID": self.sessionID}
+            )
+            response_body = json.loads(response.text)
+            self.myID = response_body["myId"]
+            return
+        except Exception as e:
+            self.error = True
+            print("Unable to connect to GeoFS. Check your connection and restart the application.")
+            print(f"Error Code 3: {e}")
 
     def getMessages(self):
-        while True:
-            print(self.accountID, self.sessionID, self.myID, self.lastMsgID)
-            body = {
-                "origin": "https://www.geo-fs.com",
-                "acid": self.accountID,
-                "sid": self.sessionID,
-                "id": self.myID,
-                "ac": "1",
-                "co": [42.36021568682466,-70.98767598755524,4.589746820023676,-103.04273973572526,-15.919583740307557,-0.376840533503692],
-                "ve": [2.7011560632672626e-10,7.436167948071671e-11,0.000004503549489433212,0,0,0],
-                "st": {"gr":True,"as":0},
-                "ti": None,
-                "m": "",
-                "ci": self.lastMsgID
-            }
-            try:
-                response = requests.post(
-                    "https://mps.geo-fs.com/update",
-                    json = body,
-                    cookies = {"PHPSESSID": self.sessionID}
-                )
-                response_body = json.loads(response.text)
-                self.myID = response_body["myId"]
-                self.lastMsgID = response_body["lastMsgId"]
-
-                return response_body["chatMessages"]
-            except Exception as e:
-                print("Unable to connect to GeoFS. Check your connection and restart the application.")
-                print(f"Error Code 2: {e}")
-                time.sleep(5)
+        self.error = False
+        body = {
+            "origin": "https://www.geo-fs.com",
+            "acid": self.accountID,
+            "sid": self.sessionID,
+            "id": self.myID,
+            "ac": "1",
+            "co": [42.36021568682466,-70.98767598755524,4.589746820023676,-103.04273973572526,-15.919583740307557,-0.376840533503692],
+            "ve": [2.7011560632672626e-10,7.436167948071671e-11,0.000004503549489433212,0,0,0],
+            "st": {"gr":True,"as":0},
+            "ti": None,
+            "m": "",
+            "ci": self.lastMsgID
+        }
+        try:
+            response = requests.post(
+                "https://mps.geo-fs.com/update",
+                json = body,
+                cookies = {"PHPSESSID": self.sessionID}
+            )
+            response_body = json.loads(response.text)
+            self.myID = response_body["myId"]
+            self.lastMsgID = response_body["lastMsgId"]
+
+            return response_body["chatMessages"]
+        except Exception as e:
+            self.error = True
+            print("Unable to connect to GeoFS. Check your connection and restart the application.")
+            print(f"Error Code 2: {e}")
+            return None
```

