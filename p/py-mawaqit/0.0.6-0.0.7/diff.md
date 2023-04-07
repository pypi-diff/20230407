# Comparing `tmp/py_mawaqit-0.0.6.tar.gz` & `tmp/py_mawaqit-0.0.7.tar.gz`

## Comparing `py_mawaqit-0.0.6.tar` & `py_mawaqit-0.0.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/.gitattributes
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/requirements.txt
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/setup.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/constants.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/google.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/helper.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/localMawaqit.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/mawaqit.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/mkdocs.yml
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/scraper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/test.py
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/docs/how-to-guides.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/docs/index.md
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/docs/reference.md
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/404.html
--rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/index.html
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/objects.inv
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/sitemap.xml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/sitemap.xml.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/_mkdocstrings.css
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/images/favicon.png
--rw-r--r--   0        0        0   113252 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/bundle.19047be9.min.js
--rw-r--r--   0        0        0   950772 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/bundle.19047be9.min.js.map
--rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677455 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    17074 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    38916 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0        0        0   209901 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/workers/search.208ed371.min.js.map
--rw-r--r--   0        0        0   113603 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/stylesheets/main.240905d7.min.css
--rw-r--r--   0        0        0    39058 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/stylesheets/main.240905d7.min.css.map
--rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/stylesheets/palette.a0c5b2b5.min.css
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
--rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/how-to-guides/index.html
--rw-r--r--   0        0        0   160900 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/MawaqitAPI/site/reference/index.html
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/example/example.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 py_mawaqit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/.gitattributes
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/setup.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/constants.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/google.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/helper.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/localMawaqit.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/mawaqit.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/mkdocs.yml
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/scraper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/test.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/docs/how-to-guides.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/docs/index.md
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/docs/reference.md
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/404.html
+-rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/index.html
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/objects.inv
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/sitemap.xml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/sitemap.xml.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/images/favicon.png
+-rw-r--r--   0        0        0   113252 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/bundle.19047be9.min.js
+-rw-r--r--   0        0        0   950772 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/bundle.19047be9.min.js.map
+-rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677455 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    17074 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    38916 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0   113603 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/stylesheets/main.240905d7.min.css
+-rw-r--r--   0        0        0    39058 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/stylesheets/main.240905d7.min.css.map
+-rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/stylesheets/palette.a0c5b2b5.min.css
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
+-rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/how-to-guides/index.html
+-rw-r--r--   0        0        0   160900 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/MawaqitAPI/site/reference/index.html
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/example/example.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 py_mawaqit-0.0.7/PKG-INFO
```

### Comparing `py_mawaqit-0.0.6/setup.py` & `py_mawaqit-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "py-mawaqit",
-    version = "0.0.6",
+    version = "0.0.7",
     author = "Riad Zaid",
     author_email = "riadzaid100@gmail..com",
     description = "An unofficial Mawaqit wrapper for python. It scrapes the mawaqit website to get the prayer times for a given mosque.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/RiadZX/py-mawaqit/",
     project_urls = {
```

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/google.py` & `py_mawaqit-0.0.7/MawaqitAPI/google.py`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/helper.py` & `py_mawaqit-0.0.7/MawaqitAPI/helper.py`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/localMawaqit.py` & `py_mawaqit-0.0.7/MawaqitAPI/localMawaqit.py`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/mawaqit.py` & `py_mawaqit-0.0.7/MawaqitAPI/mawaqit.py`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/scraper.py` & `py_mawaqit-0.0.7/MawaqitAPI/scraper.py`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/docs/how-to-guides.md` & `py_mawaqit-0.0.7/MawaqitAPI/docs/how-to-guides.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ```python
 from MawaqitAPI.mawaqit import Mawaqit
 from MawaqitAPI.google import ChromeCast
 from MawaqitAPI.constants import ADHAN_URL
 from dateutil import parser
 import time, threading
 
+
+
 def main(mosque_id, cast_name, fajr_vol, duhur_vol, asr_vol, maghrib_vol, isha_vol, adhan):
     #set the chromecast name
     cast = ChromeCast(cast_name)
 
     last_update = 0
     prayertimes = {}
     #initialize the mawaqit object
@@ -19,15 +21,15 @@
     mawaqitAPI = Mawaqit(mosque_id, new_data=True)
     next_prayer = ""
     data = mawaqitAPI.get_prayer_times()
 
     while True:
         
         #get new data at 03:00
-        if time.strftime("%H:%M") == "03:00" or time.strftime("%H:%M") == "03:01" or time.strftime("%H:%M") == "02:59" and time.time() - last_update > 60*60:
+        if (time.strftime("%H:%M") == "03:00" or time.strftime("%H:%M") == "03:01" or time.strftime("%H:%M") == "02:59") and time.time() - last_update > 60*60:
             data = mawaqitAPI.get_prayer_times()
             print(data)
             last_update = time.time()
 
 
         #convert prayer times to seconds
```

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/404.html` & `py_mawaqit-0.0.7/MawaqitAPI/site/404.html`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/index.html` & `py_mawaqit-0.0.7/MawaqitAPI/site/index.html`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/_mkdocstrings.css` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/_mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/images/favicon.png` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/bundle.19047be9.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/bundle.19047be9.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/bundle.19047be9.min.js.map` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/bundle.19047be9.min.js.map`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/tinyseg.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/wordcut.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.da.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.de.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.du.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.es.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.hi.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.it.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ko.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.no.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ta.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.th.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.zh.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/workers/search.208ed371.min.js` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/workers/search.208ed371.min.js`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/javascripts/workers/search.208ed371.min.js.map` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/javascripts/workers/search.208ed371.min.js.map`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/stylesheets/main.240905d7.min.css` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/stylesheets/main.240905d7.min.css`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/stylesheets/main.240905d7.min.css.map` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/stylesheets/main.240905d7.min.css.map`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/stylesheets/palette.a0c5b2b5.min.css` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/stylesheets/palette.a0c5b2b5.min.css`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/assets/stylesheets/palette.a0c5b2b5.min.css.map` & `py_mawaqit-0.0.7/MawaqitAPI/site/assets/stylesheets/palette.a0c5b2b5.min.css.map`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/how-to-guides/index.html` & `py_mawaqit-0.0.7/MawaqitAPI/site/how-to-guides/index.html`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/MawaqitAPI/site/reference/index.html` & `py_mawaqit-0.0.7/MawaqitAPI/site/reference/index.html`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/example/example.py` & `py_mawaqit-0.0.7/example/example.py`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/LICENSE.txt` & `py_mawaqit-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py_mawaqit-0.0.6/pyproject.toml` & `py_mawaqit-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py-mawaqit"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Riad Zaid", email="riadzaid100@gmail.com" },
 ]
 description = "An unofficial Mawaqit wrapper for python. It scrapes the mawaqit website to get the prayer times for a given mosque."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `py_mawaqit-0.0.6/PKG-INFO` & `py_mawaqit-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: py-mawaqit
-Version: 0.0.6
+Version: 0.0.7
 Summary: An unofficial Mawaqit wrapper for python. It scrapes the mawaqit website to get the prayer times for a given mosque.
 Project-URL: Homepage, https://github.com/RiadZX/py-mawaqit/
 Project-URL: Bug Tracker, https://github.com/RiadZX/py-mawaqit/issues
 Author-email: Riad Zaid <riadzaid100@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Unofficial Mawaqit Python wrapper
+An unofficial Mawaqit wrapper for python. It scrapes the mawaqit website to get the prayer times for a given mosque.
 ## Docs
 > https://riadzx.github.io/py-mawaqit/
```

