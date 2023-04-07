# Comparing `tmp/feedcrawler-18.0.0.tar.gz` & `tmp/feedcrawler-18.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedcrawler-18.0.0.tar", last modified: Fri Apr  7 10:15:49 2023, max compression
+gzip compressed data, was "feedcrawler-18.0.1.tar", last modified: Fri Apr  7 16:15:28 2023, max compression
```

## Comparing `feedcrawler-18.0.0.tar` & `feedcrawler-18.0.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.764019 feedcrawler-18.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-07 10:15:49.764019 feedcrawler-18.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7046 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.756019 feedcrawler-18.0.0/feedcrawler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.756019 feedcrawler-18.0.0/feedcrawler/external_sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.756019 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45464 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.756019 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.756019 feedcrawler-18.0.0/feedcrawler/external_sites/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/metadata/imdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.756019 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.760019 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_nx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.760019 feedcrawler-18.0.0/feedcrawler/external_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42356 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_tools/myjd_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_tools/ombi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_tools/overseerr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/external_tools/plex_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.760019 feedcrawler-18.0.0/feedcrawler/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/jobs/feed_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/jobs/package_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.760019 feedcrawler-18.0.0/feedcrawler/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.760019 feedcrawler-18.0.0/feedcrawler/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    44774 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/myjd_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/url_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.760019 feedcrawler-18.0.0/feedcrawler/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.756019 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.760019 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.764019 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
--rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
--rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
--rw-r--r--   0 runner    (1001) docker     (123)   144621 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
--rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
--rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-07 10:15:48.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    82664 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/feedcrawler/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:15:49.756019 feedcrawler-18.0.0/feedcrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 10:15:49.000000 feedcrawler-18.0.0/feedcrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 10:15:49.764019 feedcrawler-18.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-07 10:15:27.000000 feedcrawler-18.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.326677 feedcrawler-18.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-07 16:15:28.326677 feedcrawler-18.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.314676 feedcrawler-18.0.1/feedcrawler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.314676 feedcrawler-18.0.1/feedcrawler/external_sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.314676 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45464 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.318676 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.318676 feedcrawler-18.0.1/feedcrawler/external_sites/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/metadata/imdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.318676 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_nx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/external_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42359 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/myjd_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/ombi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/overseerr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/external_tools/plex_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/jobs/feed_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20896 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/jobs/package_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44933 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/myjd_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/url_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/providers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.310675 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.322676 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.326677 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
+-rw-r--r--   0 runner    (1001) docker     (123)   144621 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-07 16:15:27.000000 feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    82814 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/feedcrawler/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:15:28.314676 feedcrawler-18.0.1/feedcrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 16:15:28.000000 feedcrawler-18.0.1/feedcrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:15:28.326677 feedcrawler-18.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-07 16:14:59.000000 feedcrawler-18.0.1/setup.py
```

### Comparing `feedcrawler-18.0.0/LICENSE.md` & `feedcrawler-18.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/PKG-INFO` & `feedcrawler-18.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.0
+Version: 18.0.1
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -121,11 +121,11 @@
 und Passwort festlegen.
 
 Es empfiehlt sich, zusätzlich einen Reverse-Proxy mit HTTPs-Zertifikat,
 bspw. [kostenlos von letsencrypt](https://letsencrypt.org/), zu verwenden.
 
 ## Credits
 
-* [mmarquezs](https://github.com/mmarquezs/) (MyJDownloader-API für Python)
+* [mmarquezs](https://github.com/mmarquezs/) (My JDownloader-API für Python)
 * [JetBrains PyCharm](https://www.jetbrains.com/?from=FeedCrawler) (Open-Source-Lizenz für dieses Projekt)
```

### Comparing `feedcrawler-18.0.0/README.md` & `feedcrawler-18.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -106,9 +106,9 @@
 und Passwort festlegen.
 
 Es empfiehlt sich, zusätzlich einen Reverse-Proxy mit HTTPs-Zertifikat,
 bspw. [kostenlos von letsencrypt](https://letsencrypt.org/), zu verwenden.
 
 ## Credits
 
-* [mmarquezs](https://github.com/mmarquezs/) (MyJDownloader-API für Python)
+* [mmarquezs](https://github.com/mmarquezs/) (My JDownloader-API für Python)
 * [JetBrains PyCharm](https://www.jetbrains.com/?from=FeedCrawler) (Open-Source-Lizenz für dieses Projekt)
```

### Comparing `feedcrawler-18.0.0/feedcrawler/crawler.py` & `feedcrawler-18.0.1/feedcrawler/crawler.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from feedcrawler.jobs.package_watcher import watch_packages
 from feedcrawler.providers import gui
 from feedcrawler.providers import shared_state
 from feedcrawler.providers import version
 from feedcrawler.providers.common_functions import Unbuffered, check_ip, configpath
 from feedcrawler.providers.config import CrawlerConfig
 from feedcrawler.providers.myjd_connection import get_device, get_if_one_device, myjd_input
-from feedcrawler.providers.sqlite_database import FeedDb
+from feedcrawler.providers.sqlite_database import FeedDb, remove_redundant_db_tables
 from feedcrawler.web_interface.web_server import web_server
 
 version = "v." + version.get_version()
 
 
 def start_feedcrawler():
     parser = argparse.ArgumentParser()
@@ -41,20 +41,21 @@
     parser.add_argument("--remove_cloudflare_time", action='store_true',
                         help="Intern: Leere die Zeit des letzten Cloudflare-Umgehungs-Laufes vor dem ersten Suchlauf")
     parser.add_argument("--test_run", action='store_true', help="Intern: Führt einen Testlauf durch")
     parser.add_argument("--docker", action='store_true', help="Intern: Sperre Pfad und Port auf Docker-Standardwerte")
     arguments = parser.parse_args()
 
     if gui.enabled:
-        mem_size = 1024 * 1024  # 1 MB
-        shared_print_mem = multiprocessing.Array(ctypes.c_char, mem_size)
+        print_mem_size = 1024 * 1024  # 1 MB should handle very large print statements
+        shared_print_mem = multiprocessing.Array(ctypes.c_char, print_mem_size)
         window = gui.create_main_window()
         sys.stdout = gui.PrintToConsoleAndGui(window)
     else:
         shared_print_mem = False
+        window = False
         sys.stdout = Unbuffered(sys.stdout)
 
     print(u"┌──────────────────────────────────────────────┐")
     print(u"  FeedCrawler " + version + " von RiX")
     print(u"  https://github.com/rix1337/FeedCrawler")
     print(u"└──────────────────────────────────────────────┘")
 
@@ -99,141 +100,159 @@
         if gui.enabled:
             gui.no_hostnames_gui(shared_state.configfile)
         else:
             print(u'Keine Hostnamen in der FeedCrawler.ini gefunden! Beende FeedCrawler!')
             time.sleep(10)
         sys.exit(1)
 
-    FeedDb('cached_internals').delete("device")
-
-    if not arguments.test_run:
-        if not os.path.exists(shared_state.configfile):
-            if arguments.docker:
-                if arguments.jd_user and arguments.jd_pass:
+    device_mem_size = 8 * 1024  # 0.008 MB is eight times the size of pickled device objects
+    shared_device_mem = multiprocessing.Array(ctypes.c_char, device_mem_size)
+    shared_state.set_device_memory(shared_device_mem)
+
+    with multiprocessing.Manager() as manager:
+        shared_request_dict = manager.dict()
+
+        if not arguments.test_run:
+            if not os.path.exists(shared_state.configfile):
+                if arguments.docker:
+                    if arguments.jd_user and arguments.jd_pass:
+                        myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass, arguments.jd_device)
+                else:
                     myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass, arguments.jd_device)
             else:
-                myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass, arguments.jd_device)
-        else:
-            feedcrawler = CrawlerConfig('FeedCrawler')
-            user = feedcrawler.get('myjd_user')
-            password = feedcrawler.get('myjd_pass')
-            if user and password:
-                if not get_device():
-                    device_set = feedcrawler.get('myjd_device')
-                    if not device_set:
-                        one_device = get_if_one_device(user, password)
-                        if one_device:
-                            print(u'Gerätename "' + one_device + '" automatisch ermittelt.')
-                            feedcrawler.save('myjd_device', one_device)
-                            get_device()
-            else:
-                myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass,
-                           arguments.jd_device)
-
-    if not arguments.test_run:
-        if shared_state.device and shared_state.device.name:
-            success = True
-        else:
-            success = False
-            feedcrawler = CrawlerConfig('FeedCrawler')
-
-            device_name = feedcrawler.get('myjd_device')
-            if not device_name:
+                feedcrawler = CrawlerConfig('FeedCrawler')
                 user = feedcrawler.get('myjd_user')
                 password = feedcrawler.get('myjd_pass')
-                one_device = get_if_one_device(user, password)
-                if one_device:
-                    print(u'Gerätename "' + one_device + '" automatisch ermittelt.')
-                    feedcrawler.save('myjd_device', one_device)
-                    get_device()
-                    success = shared_state.device and shared_state.device.name
-            if not success:
-                i = 0
-                while i < 10:
-                    i += 1
-                    print(
-                        u'Verbindungsversuch %s mit My JDownloader gescheitert. Gerätename: "%s"' % (i, device_name))
-                    time.sleep(60)
-                    get_device()
-                    success = shared_state.device and shared_state.device.name
-                    if success:
-                        break
-        if success:
-            print(u'Erfolgreich mit My JDownloader verbunden. Gerätename: "' + shared_state.device.name + '"')
-        else:
-            print(u'My JDownloader Zugangsversuche nicht erfolgreich! Beende FeedCrawler!')
-            sys.exit(1)
-
-    feedcrawler = CrawlerConfig('FeedCrawler')
-    port = int(feedcrawler.get("port"))
-    docker = False
-    if arguments.docker:
-        port = int('9090')
-        docker = True
-    elif arguments.port:
-        port = int(arguments.port)
-
-    if feedcrawler.get("prefix"):
-        prefix = '/' + feedcrawler.get("prefix")
-    else:
-        prefix = ''
-    local_address = 'http://' + check_ip() + ':' + str(port) + prefix
-    if not arguments.docker:
-        print(u'Der Webserver ist erreichbar unter "' + local_address + u'"')
-
-    shared_state.set_connection_info(local_address, port, prefix, docker)
-
-    if arguments.keep_cdc:
-        print(u"CDC-Tabelle nicht geleert!")
-    else:
-        FeedDb('cdc').reset()
+                if user and password:
+                    if not get_device():
+                        device_set = feedcrawler.get('myjd_device')
+                        if not device_set:
+                            one_device = get_if_one_device(user, password)
+                            if one_device:
+                                print(u'Gerätename "' + one_device + '" automatisch ermittelt.')
+                                feedcrawler.save('myjd_device', one_device)
+                                get_device()
+                else:
+                    myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass,
+                               arguments.jd_device)
+
+        if not arguments.test_run:
+            if shared_state.device and shared_state.device.name:
+                success = True
+            else:
+                success = False
+                feedcrawler = CrawlerConfig('FeedCrawler')
 
-    global_variables = shared_state.get_globals()
+                device_name = feedcrawler.get('myjd_device')
+                if not device_name:
+                    user = feedcrawler.get('myjd_user')
+                    password = feedcrawler.get('myjd_pass')
+                    one_device = get_if_one_device(user, password)
+                    if one_device:
+                        print(u'Gerätename "' + one_device + '" automatisch ermittelt.')
+                        feedcrawler.save('myjd_device', one_device)
+                        get_device()
+                        success = shared_state.device and shared_state.device.name
+                if not success:
+                    i = 0
+                    while i < 10:
+                        i += 1
+                        print(
+                            u'Verbindungsversuch %s mit My JDownloader gescheitert. Gerätename: "%s"' % (
+                                i, device_name))
+                        time.sleep(60)
+                        get_device()
+                        success = shared_state.device and shared_state.device.name
+                        if success:
+                            break
+            if success:
+                print(u'Erfolgreich mit My JDownloader verbunden. Gerätename: "' + shared_state.device.name + '"')
+            else:
+                print(u'My JDownloader Zugangsversuche nicht erfolgreich! Beende FeedCrawler!')
+                sys.exit(1)
 
-    p = multiprocessing.Process(target=web_server, args=(shared_print_mem, global_variables,))
-    p.start()
+        feedcrawler = CrawlerConfig('FeedCrawler')
+        port = int(feedcrawler.get("port"))
+        docker = False
+        if arguments.docker:
+            port = int('9090')
+            docker = True
+        elif arguments.port:
+            port = int(arguments.port)
 
-    if arguments.delay:
-        delay = int(arguments.delay)
-        print(u"Verzögere den ersten Suchlauf um " + str(delay) + u" Sekunden")
-        time.sleep(delay)
+        if feedcrawler.get("prefix"):
+            prefix = '/' + feedcrawler.get("prefix")
+        else:
+            prefix = ''
+        local_address = 'http://' + check_ip() + ':' + str(port) + prefix
+        if not arguments.docker:
+            print(u'Der Webserver ist erreichbar unter "' + local_address + u'"')
 
-    if not arguments.test_run:
-        c = multiprocessing.Process(target=crawler,
-                                    args=(shared_print_mem, global_variables, arguments.remove_cloudflare_time, False,))
-        c.start()
+        shared_state.set_connection_info(local_address, port, prefix, docker)
 
-        w = multiprocessing.Process(target=watch_packages, args=(shared_print_mem, global_variables,))
-        w.start()
+        CrawlerConfig("FeedCrawler").remove_redundant_entries()
+        remove_redundant_db_tables(shared_state.dbfile)
 
-        if not arguments.docker and gui.enabled:  # replace true with check if we are a frozen windows exe
-            gui.main_gui(window, shared_print_mem)
+        if arguments.keep_cdc:
+            print(u"CDC-Tabelle nicht geleert!")
+        else:
+            FeedDb('cdc').reset()
 
-            sys.stdout = sys.__stdout__
-            p.terminate()
-            c.terminate()
-            w.terminate()
-            sys.exit(0)
+        global_variables = shared_state.get_globals()
 
-        else:  # regular console
-            def signal_handler(sig, frame):
-                p.terminate()
-                c.terminate()
-                w.terminate()
+        process_web_server = multiprocessing.Process(target=web_server,
+                                                     args=(shared_print_mem, global_variables, shared_request_dict,
+                                                           shared_device_mem,))
+        process_web_server.start()
+
+        if arguments.delay:
+            delay = int(arguments.delay)
+            print(u"Verzögere den ersten Suchlauf um " + str(delay) + u" Sekunden")
+            time.sleep(delay)
+
+        if not arguments.test_run:
+            process_crawler = multiprocessing.Process(target=crawler,
+                                                      args=(shared_print_mem, global_variables, shared_request_dict,
+                                                            shared_device_mem,
+                                                            arguments.remove_cloudflare_time, False,))
+            process_crawler.start()
+
+            process_watch_packages = multiprocessing.Process(target=watch_packages,
+                                                             args=(
+                                                                 shared_print_mem, global_variables,
+                                                                 shared_request_dict,
+                                                                 shared_device_mem,))
+            process_watch_packages.start()
+
+            if not arguments.docker and gui.enabled:
+                gui.main_gui(window, shared_print_mem)
+
+                sys.stdout = sys.__stdout__
+                process_web_server.terminate()
+                process_crawler.terminate()
+                process_watch_packages.terminate()
                 sys.exit(0)
 
-            signal.signal(signal.SIGINT, signal_handler)
-            print(u'Drücke [Strg] + [C] zum Beenden')
-            try:
-                while True:
-                    signal.pause()
-            except AttributeError:
-                while True:
-                    time.sleep(1)
-    else:
-        crawler(shared_print_mem, global_variables, arguments.remove_cloudflare_time, True)
-        p.terminate()
-        sys.exit(0)
+            else:  # regular console
+                def signal_handler(sig, frame):
+                    process_web_server.terminate()
+                    process_crawler.terminate()
+                    process_watch_packages.terminate()
+                    sys.exit(0)
+
+                signal.signal(signal.SIGINT, signal_handler)
+                print(u'Drücke [Strg] + [C] zum Beenden')
+                try:
+                    while True:
+                        signal.pause()
+                except AttributeError:
+                    while True:
+                        time.sleep(1)
+        else:
+            crawler(shared_print_mem, global_variables, shared_request_dict, shared_device_mem,
+                    arguments.remove_cloudflare_time, True)
+            process_web_server.terminate()
+            sys.exit(0)
 
 
 if __name__ == "__main__":
     start_feedcrawler()
```

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/content_all.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/content_shows.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/content_shows.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/shared.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_by.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_dw.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_ff.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_ff.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_fx.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_hw.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_nk.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_nx.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_all_ww.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_all_ww.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/metadata/imdb.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/metadata/imdb.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/web_search/content_all.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/web_search/content_shows.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/content_shows.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/web_search/shared.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_by.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_dw.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_fx.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_hw.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_nk.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_sites/web_search/sites/content_all_nx.py` & `feedcrawler-18.0.1/feedcrawler/external_sites/web_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_tools/myjd_api.py` & `feedcrawler-18.0.1/feedcrawler/external_tools/myjd_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- encoding: utf-8 -*-
 # FeedCrawler
 # Projekt von https://github.com/rix1337
-# Dieses Modul stellt die API von MyJDownloader in Form eines Python-Moduls zur Verfügung.
+# Dieses Modul stellt die API von My JDownloader in Form eines Python-Moduls zur Verfügung.
 #
 # Enthält Code von:
 # https://github.com/mmarquezs/My.Jdownloader-API-Python-Library/
 #
 # The MIT License (MIT)
 #
 # Copyright (c) 2015 Marc Marquez Santamaria
@@ -1144,15 +1144,15 @@
                                                   query[0] + "&".join(query[1:])))
                 ]
             query = query[0] + "&".join(query[1:])
             try:
                 encrypted_response = request(api + query, timeout=timeout, output_errors=output_errors)
             except URLError:
                 encrypted_response = request(api + query, timeout=timeout, output_errors=output_errors, verify=False)
-                print(u"Die sichere Verbindung zu MyJDownloader konnte nicht verifiziert werden.")
+                print(u"Die sichere Verbindung zu My JDownloader konnte nicht verifiziert werden.")
         else:
             params_request = []
             if params is not None:
                 for param in params:
                     if not isinstance(param, list):
                         params_request += [json.dumps(param)]
                     else:
@@ -1191,15 +1191,15 @@
                             "Content-Type": "application/aesjson-jd; charset=utf-8"
                         },
                         data=encrypted_data,
                         method="POST",
                         timeout=timeout,
                         output_errors=output_errors,
                         verify=False)
-                    print(u"Die sichere Verbindung zu MyJDownloader konnte nicht verifiziert werden.")
+                    print(u"Die sichere Verbindung zu My JDownloader konnte nicht verifiziert werden.")
                 except URLError:
                     return None
         if encrypted_response.status_code == 403:
             raise TokenExpiredException
         if encrypted_response.status_code == 503:
             raise RequestTimeoutException
         if encrypted_response.status_code != 200:
```

### Comparing `feedcrawler-18.0.0/feedcrawler/external_tools/ombi_api.py` & `feedcrawler-18.0.1/feedcrawler/external_tools/ombi_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_tools/overseerr_api.py` & `feedcrawler-18.0.1/feedcrawler/external_tools/overseerr_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/external_tools/plex_api.py` & `feedcrawler-18.0.1/feedcrawler/external_tools/plex_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/jobs/feed_search.py` & `feedcrawler-18.0.1/feedcrawler/jobs/feed_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,19 +79,23 @@
         SJ(filename='List_ContentAll_Seasons'),
         DJ(filename='List_CustomDJ_Documentaries'),
         DJ(filename='List_CustomDJ_Documentaries_Regex'),
         DD(filename='List_CustomDD_Feeds')
     ]
 
 
-def crawler(shared_print_mem, global_variables, remove_cloudflare_time, test_run):
+def crawler(shared_print_mem, global_variables, shared_request_dict, shared_device_mem, remove_cloudflare_time,
+            test_run):
     if gui.enabled and shared_print_mem:
         sys.stdout = gui.AppendToPrintQueue(shared_print_mem)
     else:
         sys.stdout = Unbuffered(sys.stdout)
+
+    shared_state.set_request_dict(shared_request_dict)
+    shared_state.set_device_memory(shared_device_mem)
     shared_state.set_globals(global_variables)
     logger = shared_state.logger
 
     request_management_first_run = True
     crawltimes = FeedDb("crawltimes")
     feedcrawler = CrawlerConfig('FeedCrawler')
 
@@ -100,16 +104,15 @@
         print(u"-----------Entferne Zeitpunkt des letzten Cloudflare-Umgehungs-Suchlaufes!-----------")
         FeedDb('crawltimes').delete("last_cloudflare_run")
 
     while True:
         try:
             if not shared_state.device or not is_device(shared_state.device):
                 get_device()
-            FeedDb('cached_requests').reset()
-            FeedDb('cached_requests').cleanup()
+            shared_state.request_dict.clear()
             start_time = time.time()
             check_url(start_time)
             crawltimes.update_store("active", "True")
             crawltimes.update_store("start_time", start_time * 1000)
             logger.debug("-----------Alle Suchläufe gestartet.-----------")
 
             # Connect to and run request management services
@@ -196,15 +199,15 @@
                 except Exception as e:
                     print(u"Fehler bei der Feed-Suche: " + str(e))
                 logger.debug("-----------Suchlauf (" + name + file + ") ausgeführt!-----------")
 
             # Finish feed search and log results
             if current_cloudflare_run:
                 crawltimes.update_store("last_cloudflare_run", current_cloudflare_run * 1000)
-            cached_requests = FeedDb('cached_requests').count()
+            cached_requests = len(shared_state.request_dict)
             request_cache_string = u"Der FeedCrawler-Cache hat " + str(cached_requests) + " HTTP-Requests gespart!"
             end_time = time.time()
             total_time = end_time - start_time
             interval = int(feedcrawler.get('interval')) * 60
             random_range = random.randrange(0, interval // 4)
             wait = interval + random_range
             next_start = end_time + wait
@@ -228,16 +231,15 @@
             logger.debug(time.strftime("%Y-%m-%d %H:%M:%S") + u" - " + request_cache_string)
             logger.debug("-----------Wartezeit bis zum nächsten Suchlauf: " + readable_time(wait) + '-----------')
             print(u"-----------Wartezeit bis zum nächsten Suchlauf: " + readable_time(wait) + '-----------')
             crawltimes.update_store("end_time", end_time * 1000)
             crawltimes.update_store("total_time", readable_time(total_time))
             crawltimes.update_store("next_start", next_start * 1000)
             crawltimes.update_store("active", "False")
-            FeedDb('cached_requests').reset()
-            FeedDb('cached_requests').cleanup()
+            shared_state.request_dict.clear()
 
             myjd_auto_update = feedcrawler.get("myjd_auto_update")
             if myjd_auto_update:
                 myjd_infos = get_info()
                 myjd_state = myjd_infos[1]
                 myjd_grabber_collecting = myjd_infos[2]
                 myjd_update_ready = myjd_infos[3]
```

### Comparing `feedcrawler-18.0.0/feedcrawler/jobs/package_watcher.py` & `feedcrawler-18.0.1/feedcrawler/jobs/package_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,22 @@
 from feedcrawler.providers.myjd_connection import rename_package_in_linkgrabber
 from feedcrawler.providers.myjd_connection import reset_in_downloads
 from feedcrawler.providers.myjd_connection import retry_decrypt
 from feedcrawler.providers.notifications import notify
 from feedcrawler.providers.sqlite_database import FeedDb
 
 
-def watch_packages(shared_print_mem, global_variables):
+def watch_packages(shared_print_mem, global_variables, shared_request_dict, shared_device_mem):
     if gui.enabled and shared_print_mem:
         sys.stdout = gui.AppendToPrintQueue(shared_print_mem)
     else:
         sys.stdout = Unbuffered(sys.stdout)
+
+    shared_state.set_request_dict(shared_request_dict)
+    shared_state.set_device_memory(shared_device_mem)
     shared_state.set_globals(global_variables)
 
     crawljobs = CrawlerConfig('Crawljobs')
     autostart = crawljobs.get("autostart")
     db = FeedDb('crawldog')
 
     grabber_was_collecting = False
```

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/common_functions.py` & `feedcrawler-18.0.1/feedcrawler/providers/common_functions.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/config.py` & `feedcrawler-18.0.1/feedcrawler/providers/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -176,7 +176,21 @@
         return
 
     def get(self, key):
         return self._get_from_config(self.__config__, key)
 
     def get_section(self):
         return self._config._sections[self._section]
+
+    def remove_redundant_entries(self):
+        for section in self._config.sections():
+            if section not in self._DEFAULT_CONFIG:
+                self._config.remove_section(section)
+                print(f"Entferne überflüssige Sektion '{section}' aus der Konfigurationsdatei.")
+            else:
+                for option in self._config.options(section):
+                    if option not in [param[0] for param in self._DEFAULT_CONFIG[section]]:
+                        self._config.remove_option(section, option)
+                        print(
+                            f"Entferne überflüssige Option '{option}' der Sektion '{section}' aus der Konfigurationsdatei.")
+        with open(self._configfile, 'w') as configfile:
+            self._config.write(configfile)
```

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/gui.py` & `feedcrawler-18.0.1/feedcrawler/providers/gui.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 # -*- coding: utf-8 -*-
 # FeedCrawler
 # Projekt von https://github.com/rix1337
 # Dieses Modul stellt eine GUI für den FeedCrawler bereit. Diese setzt die Dependencies PySimpleGUI und psgtray voraus.
 
 import base64
+import ctypes
 import os
 import platform
 import sys
 import webbrowser
 
 from feedcrawler.providers.version import get_version
 
 try:
     import PySimpleGUI as sg  # not in requirements.txt as we don't want to force users to install it
     from psgtray import SystemTray  # not in requirements.txt as we don't want to force users to install it
 
     enabled = True
 except ImportError:
-    print("GUI-Module sind nicht installiert.")
     enabled = False
 
 if platform.system() == 'Windows':
     font = ('Consolas', 12)
+    myappid = 'feedcrawler'  # arbitrary string
+    ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
 elif platform.system() == 'Linux':
     font = ('Monospace', 12)
 else:
     font = ('Monaco', 12)
 
 title = 'FeedCrawler v.' + get_version()
 
 
-def get_icon():
+def get_icon_path():
     base_dir = './feedcrawler'
     if getattr(sys, 'frozen', False):
         base_dir = os.path.join(sys._MEIPASS).replace("\\", "/")
 
     icon_path = base_dir + '/web_interface/vuejs_frontend/dist/favicon.ico'
+    return icon_path
+
+
+def get_icon():
+    icon_path = get_icon_path()
     with open(icon_path, 'rb') as f:
         icon_data = f.read()
     icon_base64 = base64.b64encode(icon_data)
     return icon_base64
 
 
 def create_main_window():
@@ -52,22 +59,26 @@
         [sg.Button('Web-Interface'), sg.Button('Beenden')],
     ]
 
     window = sg.Window(title,
                        layout,
                        finalize=True,
                        enable_close_attempted_event=True,
-                       element_justification='c')
+                       element_justification='c',
+                       icon=get_icon_path())
 
     window.hide()
 
     return window
 
 
 def main_gui(window, shared_mem):
+    if not window:
+        print("GUI-Fenster falsch initialisiert.")
+        window = create_main_window()
     try:
         menu = ['', [title,
                      '---',
                      'GUI',
                      'Web-Interface',
                      '---',
                      'Beenden']
@@ -111,48 +122,47 @@
     jd.set_app_key('FeedCrawler')
     try:
         jd.connect(myjd_user, myjd_pass)
         jd.update_devices()
         devices = jd.list_devices()
         return devices
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return []
 
 
 def no_hostnames_gui(configfile):
     # warn user if no hostnames are configured
     sg.theme('dark grey 9')
     layout = [
         [sg.Text('Keine Hostnamen in der FeedCrawler.ini gefunden! Beende FeedCrawler!')],
         [sg.Button('OK', bind_return_key=True)]
     ]
 
-    window = sg.Window('Warnung', layout, finalize=True, element_justification='c')
+    window = sg.Window('Warnung', layout, finalize=True, element_justification='c', icon=get_icon_path())
     webbrowser.open(configfile)
 
     while True:
         event, values = window.read()
         if event == sg.WIN_CLOSED:
             break
         window.close()
 
 
-
 def configpath_gui(current_path):
     configpath = ''
 
     sg.theme('dark grey 9')
     layout = [
         [sg.Button('"' + current_path + '" verwenden', bind_return_key=True)],
         [sg.Input(key='-FOLDER-', enable_events=True, visible=False),
          sg.FolderBrowse('Anderen Pfad wählen', target='-FOLDER-', initial_folder=current_path)]
     ]
 
-    window = sg.Window('Wo sollen Einstellungen und Logs abgelegt werden?', layout)
+    window = sg.Window('Wo sollen Einstellungen und Logs abgelegt werden?', layout, icon=get_icon_path())
 
     while True:
         event, values = window.read()
         if event == sg.WIN_CLOSED:
             break
         configpath = values['-FOLDER-']
         window.close()
@@ -171,15 +181,15 @@
     layout = [
         [sg.Text('Bitte die Zugangsdaten für My JDownloader angeben:')],
         [sg.Text('Benutzername', size=(15, 1)), sg.InputText(key='username')],
         [sg.Text('Passwort', size=(15, 1)), sg.InputText(key='password', password_char='*')],
         [sg.Button('OK', bind_return_key=True), sg.Button('Abbrechen')]
     ]
 
-    window = sg.Window('MyJDownloader Login', layout, finalize=True, element_justification='c')
+    window = sg.Window('My JDownloader Login', layout, finalize=True, element_justification='c', icon=get_icon_path())
 
     while True:
         event, values = window.read()
 
         if event in (sg.WIN_CLOSED, 'Abbrechen'):
             window.close()
             break
@@ -201,16 +211,17 @@
                         device_list.append(dv['name'])
 
                     layout = [
                         [sg.Text('Bitte den gewünschten JDownloader auswählen:')],
                         [sg.Listbox(values=device_list, size=(20, 5), key='device')],
                         [sg.Button('OK', bind_return_key=True), sg.Button('Abbrechen')]
                     ]
-                    device_selection = sg.Window('MyJDownloader Gerät', layout, finalize=True,
-                                                 element_justification='c')
+                    device_selection = sg.Window('My JDownloader Gerät', layout, finalize=True,
+                                                 element_justification='c',
+                                                 icon=get_icon_path())
                     while True:
                         event, values = device_selection.read()
 
                         if event in (sg.WIN_CLOSED, 'Abbrechen'):
                             device_selection.close()
                             break
                         elif event in 'OK':
@@ -250,14 +261,16 @@
 class PrintToConsoleAndGui(object):
     def __init__(self, window):
         class Unbuffered(object):
             def __init__(self, stream):
                 self.stream = stream
 
             def write(self, data):
+                if data != '\n' and data.endswith('\n'):
+                    data = data[:-1]
                 self.stream.write(data)
                 self.stream.flush()
 
             def writelines(self, datas):
                 self.stream.writelines(datas)
                 self.stream.flush()
```

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/http_requests/cache_handler.py` & `feedcrawler-18.0.1/feedcrawler/providers/http_requests/cache_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # FeedCrawler
 # Projekt von https://github.com/rix1337
 # Dieses Modul sorgt durch Caching dafür, dass derselbe Request nur einmal pro Suchlauf an den Server geht.
 
 import codecs
 import hashlib
 import pickle
+import sys
 from functools import wraps
 from urllib.error import URLError
 
 from feedcrawler.providers import shared_state
 from feedcrawler.providers.common_functions import check_is_site
 from feedcrawler.providers.common_functions import site_blocked, site_blocked_with_advanced_methods
 from feedcrawler.providers.http_requests.cloudflare_handlers import flaresolverr_task
@@ -32,23 +33,28 @@
             to_hash += codecs.encode(pickle.dumps(k), "base64").decode()
             to_hash += codecs.encode(pickle.dumps(kwargs[k]), "base64").decode()
             if k == "dont_cache" and k:
                 dont_cache = True
         # This hash is based on all arguments of the request
         hashed = hashlib.sha256(to_hash.encode('ascii', 'ignore')).hexdigest()
 
-        cached = FeedDb('cached_requests').retrieve(hashed)
+        try:
+            cached = shared_state.request_dict[hashed]
+        except KeyError:
+            cached = None
         if cached:
             # Unpack and return the cached result instead of processing the request
-            return pickle.loads(codecs.decode(cached.encode(), "base64"))
+            cached_response = pickle.loads(codecs.decode(cached.encode(), "base64"))
+            return cached_response
         else:
             #
             value = func(*args, **kwargs)
             if not dont_cache:
-                FeedDb('cached_requests').store(hashed, codecs.encode(pickle.dumps(value), "base64").decode())
+                cached_response = codecs.encode(pickle.dumps(value), "base64").decode()
+                shared_state.request_dict[hashed] = cached_response
             return value
 
     return cache_returned_values
 
 
 @cache
 def cached_request(url, method='get', params=None, headers=None, redirect_url=False, dont_cache=False):
```

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/http_requests/cloudflare_handlers.py` & `feedcrawler-18.0.1/feedcrawler/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/http_requests/request_handler.py` & `feedcrawler-18.0.1/feedcrawler/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/myjd_connection.py` & `feedcrawler-18.0.1/feedcrawler/providers/myjd_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 import re
 import time
 
 from bs4 import BeautifulSoup
 
 import feedcrawler.external_tools.myjd_api
 from feedcrawler.external_tools.myjd_api import TokenExpiredException, RequestTimeoutException, MYJDException
+from feedcrawler.providers import gui
 from feedcrawler.providers import shared_state
 from feedcrawler.providers.common_functions import check_hoster
 from feedcrawler.providers.common_functions import check_is_site
 from feedcrawler.providers.common_functions import is_device
 from feedcrawler.providers.common_functions import is_show
 from feedcrawler.providers.common_functions import longest_substr
 from feedcrawler.providers.common_functions import readable_size
 from feedcrawler.providers.common_functions import readable_time
 from feedcrawler.providers.common_functions import simplified_search_term_in_title
 from feedcrawler.providers.config import CrawlerConfig
 from feedcrawler.providers.sqlite_database import FeedDb
 from feedcrawler.providers.url_functions import get_redirected_url
-from feedcrawler.providers import gui
 from feedcrawler.providers.url_functions import get_url
 
 
 def split_urls(urls):
     if isinstance(urls, list):
         return urls
     elif '\\n' in urls:
@@ -58,57 +58,57 @@
 
     if myjd_user and myjd_pass and myjd_device:
         try:
             jd.connect(myjd_user, myjd_pass)
             jd.update_devices()
             device = jd.get_device(myjd_device)
         except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-            if not shared_state.synchronize_device():
-                print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e).replace("\n", " "))
+            if not shared_state.set_device_from_memory_to_state():
+                print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e).replace("\n", " "))
                 return False
             return True
         if not device or not is_device(device):
             return False
-        if not shared_state.synchronize_device():
-            shared_state.set_device(device)
+        if not shared_state.set_device_from_memory_to_state():
+            shared_state.set_device_to_memory_and_state(device)
         return True
     elif myjd_user and myjd_pass:
         myjd_device = get_if_one_device(myjd_user, myjd_pass)
         try:
             jd.connect(myjd_user, myjd_pass)
             jd.update_devices()
             device = jd.get_device(myjd_device)
         except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-            if not shared_state.synchronize_device():
-                print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e).replace("\n", " "))
+            if not shared_state.set_device_from_memory_to_state():
+                print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e).replace("\n", " "))
                 return False
             return True
         if not device or not is_device(device):
             return False
-        if not shared_state.synchronize_device():
-            shared_state.set_device(device)
+        if not shared_state.set_device_from_memory_to_state():
+            shared_state.set_device_to_memory_and_state(device)
         return True
     else:
         return False
 
 
 def check_device(myjd_user, myjd_pass, myjd_device):
     jd = feedcrawler.external_tools.myjd_api.Myjdapi()
     jd.set_app_key('FeedCrawler')
     try:
         jd.connect(myjd_user, myjd_pass)
         jd.update_devices()
         device = jd.get_device(myjd_device)
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        if not shared_state.synchronize_device():
-            print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        if not shared_state.set_device_from_memory_to_state():
+            print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
             return False
         return True
-    if not shared_state.synchronize_device():
-        shared_state.set_device(device)
+    if not shared_state.set_device_from_memory_to_state():
+        shared_state.set_device_to_memory_and_state(device)
     return True
 
 
 def get_if_one_device(myjd_user, myjd_pass):
     jd = feedcrawler.external_tools.myjd_api.Myjdapi()
     jd.set_app_key('FeedCrawler')
     try:
@@ -116,27 +116,28 @@
         jd.update_devices()
         devices = jd.list_devices()
         if len(devices) == 1:
             return devices[0].get('name')
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
+
 def get_devices(myjd_user, myjd_pass):
     jd = feedcrawler.external_tools.myjd_api.Myjdapi()
     jd.set_app_key('FeedCrawler')
     try:
         jd.connect(myjd_user, myjd_pass)
         jd.update_devices()
         devices = jd.list_devices()
         return devices
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return []
 
 
 def get_packages_in_downloader():
     links = shared_state.device.downloads.query_links()
 
     packages = shared_state.device.downloads.query_packages([{
@@ -348,15 +349,15 @@
                     return False
                 downloader_state = shared_state.device.downloadcontroller.get_current_state()
                 grabber_collecting = shared_state.device.linkgrabber.is_collecting()
             return [True, downloader_state, grabber_collecting]
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def cryptor_url_first(failed_package):
     resorted_failed_package = []
     for p in failed_package:
         pk = {
@@ -443,15 +444,15 @@
             return [True, downloader_state, grabber_collecting, update_ready,
                     [packages_in_downloader_decrypted, packages_in_linkgrabber_decrypted,
                      packages_offline,
                      packages_failed]]
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def set_enabled(enable, linkids, uuid):
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -470,15 +471,15 @@
                 if not shared_state.device or not is_device(shared_state.device):
                     return False
                 shared_state.device.linkgrabber.set_enabled(enable, linkids, uuid)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def move_to_downloads(linkids, uuid):
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -490,15 +491,15 @@
                 if not shared_state.device or not is_device(shared_state.device):
                     return False
                 shared_state.device.linkgrabber.move_to_downloadlist(linkids, uuid)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def reset_in_downloads(linkids, uuid):
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -510,15 +511,15 @@
                 if not shared_state.device or not is_device(shared_state.device):
                     return False
                 shared_state.device.downloads.reset_links(linkids, uuid)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def remove_from_linkgrabber(linkids, uuid):
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -532,15 +533,15 @@
                     return False
                 shared_state.device.linkgrabber.remove_links(linkids, uuid)
                 shared_state.device.downloads.remove_links(linkids, uuid)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def rename_package_in_linkgrabber(package_id, new_name):
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -552,15 +553,15 @@
                 if not shared_state.device or not is_device(shared_state.device):
                     return False
                 shared_state.device.linkgrabber.rename_package(package_id, new_name)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def move_to_new_package(linkids, package_id, new_title, new_path):
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -574,15 +575,15 @@
                     return False
                 shared_state.device.linkgrabber.move_to_new_package(linkids, package_id, new_title, new_path)
                 shared_state.device.downloads.move_to_new_package(linkids, package_id, new_title, new_path)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def download(title, subdir, old_links, password, full_path=None, autostart=False):
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -650,15 +651,15 @@
         if db.retrieve(title):
             db.delete(title)
             db.store(title, 'retried')
         else:
             db.store(title, 'added')
         return True
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def retry_decrypt(linkids, uuid, links):
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -755,15 +756,15 @@
                 download(title, None, links, None, full_path)
                 return True
             else:
                 return False
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def jdownloader_update():
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -775,15 +776,15 @@
                 if not shared_state.device or not is_device(shared_state.device):
                     return False
                 shared_state.device.update.restart_and_update()
             return True
         else:
             return False
     except feedcrawler.external_tools.myjd_api.MYJDException as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def jdownloader_start():
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -795,15 +796,15 @@
                 if not shared_state.device or not is_device(shared_state.device):
                     return False
                 shared_state.device.downloadcontroller.start_downloads()
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def jdownloader_pause(bl):
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -815,15 +816,15 @@
                 if not shared_state.device or not is_device(shared_state.device):
                     return False
                 shared_state.device.downloadcontroller.pause_downloads(bl)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def jdownloader_stop():
     try:
         if not shared_state.device or not is_device(shared_state.device):
             get_device()
@@ -835,15 +836,15 @@
                 if not shared_state.device or not is_device(shared_state.device):
                     return False
                 shared_state.device.downloadcontroller.stop_downloads()
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def check_failed_link_exists(links):
     failed = get_info()
     if failed[2]:
         time.sleep(5)
@@ -1036,15 +1037,15 @@
                 if not shared_state.device or not is_device(shared_state.device):
                     return False
                 move_to_new_package(linkids, uuids, title, "<jd:packagename>")
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
-        print(u"Fehler bei der Verbindung mit MyJDownloader: " + str(e))
+        print(u"Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def do_add_decrypted(title, password, cnl_packages):
     linkids = []
     uuids = []
     urls = ""
```

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/notifications.py` & `feedcrawler-18.0.1/feedcrawler/providers/notifications.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/shared_state.py` & `feedcrawler-18.0.1/feedcrawler/providers/shared_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import logging
 import os
 import pickle
 import sys
 from logging import handlers
 
 from feedcrawler.external_tools.myjd_api import TokenExpiredException, RequestTimeoutException, MYJDException
-from feedcrawler.providers.sqlite_database import FeedDb
 
+device_memory = False
+request_dict = False
 configpath = False
 log_level = False
 sites = False
 device = False
 configfile = False
 dbfile = False
 log_file = False
@@ -44,15 +45,15 @@
     }
 
 
 def set_globals(global_variables):
     set_files(global_variables["configpath"])
     set_sites()
     set_logger(global_variables["log_level"])
-    set_device(global_variables["device"])
+    set_device_to_memory_and_state(global_variables["device"])
     set_connection_info(global_variables["local_address"], global_variables["port"], global_variables["prefix"],
                         global_variables["docker"])
 
 
 def set_files(set_configpath):
     global configpath
     global configfile
@@ -67,33 +68,44 @@
 
 
 def set_sites():
     global sites
     sites = ["FX", "SF", "DW", "HW", "FF", "BY", "NK", "NX", "WW", "SJ", "DJ", "DD"]
 
 
-def synchronize_device():
+def set_request_dict(dict):
+    global request_dict
+    request_dict = dict
+
+
+def set_device_memory(memory):
+    global device_memory
+    device_memory = memory
+
+
+def set_device_from_memory_to_state():
     global device
-    cached = FeedDb('cached_internals').retrieve("device")
-    if cached:
-        untested_device = pickle.loads(codecs.decode(cached.encode(), "base64"))
+    cached_device = device_memory
+    if not device and cached_device and cached_device.value:
+        untested_device = pickle.loads(codecs.decode(device_memory.value, "base64"))
         try:
             test_device = untested_device.toolbar.get_status()
             if test_device:
-                set_device(untested_device)
+                device = untested_device
                 return True
         except (TokenExpiredException, RequestTimeoutException, MYJDException):
             pass
     return False
 
 
-def set_device(set_device):
+def set_device_to_memory_and_state(set_device):
     global device
-    device = set_device
-    FeedDb('cached_internals').store("device", codecs.encode(pickle.dumps(device), "base64").decode())
+    if not set_device_from_memory_to_state():
+        device = set_device
+        device_memory.value = codecs.encode(pickle.dumps(device), "base64")
 
 
 def set_logger(set_log_level):
     global log_level
     global logger
     log_level = set_log_level
```

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/sqlite_database.py` & `feedcrawler-18.0.1/feedcrawler/providers/sqlite_database.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,57 @@
 from feedcrawler.providers import shared_state
 
 
 def get_first(iterable):
     return iterable and list(iterable[:1]).pop() or None
 
 
+def remove_redundant_db_tables(file):
+    conn = sqlite3.connect(file)
+    cursor = conn.cursor()
+
+    keep_tables = [
+        'FeedCrawler',
+        'List_ContentAll_Movies',
+        'List_ContentAll_Movies_Regex',
+        'List_ContentAll_Seasons',
+        'List_ContentShows_Seasons_Regex',
+        'List_ContentShows_Shows',
+        'List_ContentShows_Shows_Regex',
+        'List_CustomDD_Feeds',
+        'List_CustomDJ_Documentaries',
+        'List_CustomDJ_Documentaries_Regex',
+        'Ombi',
+        'Overseerr',
+        'Plex',
+        'cdc',
+        'crawldog',
+        'crawltimes',
+        'episode_remover',
+        'site_status',
+        'flaresolverr',
+        'sponsors_helper',
+        'to_decrypt',
+    ]
+
+    cursor.execute("SELECT name FROM sqlite_master WHERE type='table'")
+    table_names = [row[0] for row in cursor.fetchall()]
+
+    tables_to_drop = set(table_names) - set(keep_tables)
+
+    for table in tables_to_drop:
+        cursor.execute(f"DROP TABLE IF EXISTS {table}")
+        print(f"Entferne überflüssige Tabelle '{table}' aus der Datenbank.")
+
+
+    conn.commit()
+    cursor.execute("VACUUM")
+    conn.close()
+
+
 class FeedDb(object):
     def __init__(self, table):
         try:
             self._conn = sqlite3.connect(shared_state.dbfile, check_same_thread=False, timeout=5)
             self._table = table
             if not self._conn.execute(
                     "SELECT sql FROM sqlite_master WHERE type = 'table' AND name = '%s';" % self._table).fetchall():
@@ -34,18 +77,14 @@
                         "SELECT sql FROM sqlite_master WHERE type = 'table' AND name = '%s';" % self._table).fetchall():
                     self._conn.execute("CREATE TABLE %s (key, value)" % self._table)
                     self._conn.commit()
                     shared_state.logger.debug("Zugriff auf FeedCrawler.db nach Wartezeit war erfolgreich.")
             except sqlite3.OperationalError as e:
                 print("Fehler bei Zugriff auf FeedCrawler.db: ", str(e))
 
-    def cleanup(self):
-        self._conn.execute("VACUUM")
-        return
-
     def count(self):
         res = self._conn.execute("SELECT Count() FROM %s" % self._table).fetchone()
         return res[0] if res else None
 
     def retrieve(self, key):
         res = self._conn.execute(
             "SELECT value FROM %s WHERE key='%s'" % (self._table, key)).fetchone()
```

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/url_functions.py` & `feedcrawler-18.0.1/feedcrawler/providers/url_functions.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/providers/version.py` & `feedcrawler-18.0.1/feedcrawler/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "18.0.0"
+    return "18.0.1"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/vuejs_frontend/dist/index.html` & `feedcrawler-18.0.1/feedcrawler/web_interface/vuejs_frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/feedcrawler/web_interface/web_server.py` & `feedcrawler-18.0.1/feedcrawler/web_interface/web_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -2016,15 +2016,18 @@
         updateversion = version.update_check()[1]
         print(u'Update steht bereit (' + updateversion +
               ')! Weitere Informationen unter https://github.com/rix1337/FeedCrawler/releases/latest')
 
     app_container()
 
 
-def web_server(shared_print_mem, global_variables):
+def web_server(shared_print_mem, global_variables, shared_request_dict, shared_device_mem):
     if gui.enabled and shared_print_mem:
         sys.stdout = gui.AppendToPrintQueue(shared_print_mem)
     else:
         sys.stdout = Unbuffered(sys.stdout)
+
+    shared_state.set_request_dict(shared_request_dict)
+    shared_state.set_device_memory(shared_device_mem)
     shared_state.set_globals(global_variables)
 
     start()
```

### Comparing `feedcrawler-18.0.0/feedcrawler.egg-info/PKG-INFO` & `feedcrawler-18.0.1/feedcrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.0
+Version: 18.0.1
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -121,11 +121,11 @@
 und Passwort festlegen.
 
 Es empfiehlt sich, zusätzlich einen Reverse-Proxy mit HTTPs-Zertifikat,
 bspw. [kostenlos von letsencrypt](https://letsencrypt.org/), zu verwenden.
 
 ## Credits
 
-* [mmarquezs](https://github.com/mmarquezs/) (MyJDownloader-API für Python)
+* [mmarquezs](https://github.com/mmarquezs/) (My JDownloader-API für Python)
 * [JetBrains PyCharm](https://www.jetbrains.com/?from=FeedCrawler) (Open-Source-Lizenz für dieses Projekt)
```

### Comparing `feedcrawler-18.0.0/feedcrawler.egg-info/SOURCES.txt` & `feedcrawler-18.0.1/feedcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.0/setup.py` & `feedcrawler-18.0.1/setup.py`

 * *Files identical despite different names*

