# Comparing `tmp/pywaclient-1.3.1.tar.gz` & `tmp/pywaclient-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywaclient-1.3.1.tar", last modified: Sun Apr  2 14:34:14 2023, max compression
+gzip compressed data, was "dist/pywaclient-1.3.2.tar", last modified: Fri Apr  7 16:18:52 2023, max compression
```

## Comparing `pywaclient-1.3.1.tar` & `pywaclient-1.3.2.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 14:34:14.000000 pywaclient-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-02 14:34:00.000000 pywaclient-1.3.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-04-02 14:34:00.000000 pywaclient-1.3.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-04-02 14:34:00.000000 pywaclient-1.3.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2208 2023-04-02 14:34:14.000000 pywaclient-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1759 2023-04-02 14:34:00.000000 pywaclient-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient/
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3560 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)     6851 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/articles.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/block_templates.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/canvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/categories.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/chronicles.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/histories.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/images.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/manuscripts.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/map_marker_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2374 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/maps.py
--rw-rw-rw-   0 root         (0) root         (0)     3076 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/notebooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/rpg_system.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/secrets.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/subscriber_groups.py
--rw-rw-rw-   0 root         (0) root         (0)      794 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/timelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/users.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/variables.py
--rw-rw-rw-   0 root         (0) root         (0)    14182 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/endpoints/worlds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)     2777 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/exceptions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6892 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/article.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/block.py
--rw-rw-rw-   0 root         (0) root         (0)     3532 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/category.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/entity.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     5558 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/manuscript.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/secret.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2023-04-02 14:34:00.000000 pywaclient-1.3.1/pywaclient/models/world.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2208 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2006 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-02 14:34:14.000000 pywaclient-1.3.1/pywaclient.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-02 14:34:00.000000 pywaclient-1.3.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-02 14:34:14.000000 pywaclient-1.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-04-02 14:34:00.000000 pywaclient-1.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 14:34:14.000000 pywaclient-1.3.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 14:34:14.000000 pywaclient-1.3.1/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)     1266 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/data/block.json
--rw-rw-rw-   0 root         (0) root         (0)     2469 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/data/form_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/init_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1534 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_article_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_block_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_block_template_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_block_template_part_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_canvas_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_category_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_chronicle_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1493 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_history_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_image_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_manuscript_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_map_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_notebook_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_rpg_system_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     4154 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_secret_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2556 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_subscriber_group_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_timeline_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_user_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_variable_collection_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_variable_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     4530 2023-04-02 14:34:00.000000 pywaclient-1.3.1/tests/test_world_endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:18:52.000000 pywaclient-1.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-07 16:18:38.000000 pywaclient-1.3.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-04-07 16:18:38.000000 pywaclient-1.3.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-04-07 16:18:38.000000 pywaclient-1.3.2/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-04-07 16:18:52.000000 pywaclient-1.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2023-04-07 16:18:38.000000 pywaclient-1.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)     7013 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/articles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/block_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/canvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/chronicles.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/histories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/images.py
+-rw-rw-rw-   0 root         (0) root         (0)     5984 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/manuscripts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/map_marker_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2427 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/notebooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/rpg_system.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/subscriber_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/timelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/variables.py
+-rw-rw-rw-   0 root         (0) root         (0)    14182 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/endpoints/worlds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/exceptions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6892 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/article.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/block.py
+-rw-rw-rw-   0 root         (0) root         (0)     3532 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/category.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     5558 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/manuscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-04-07 16:18:38.000000 pywaclient-1.3.2/pywaclient/models/world.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-07 16:18:52.000000 pywaclient-1.3.2/pywaclient.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-07 16:18:38.000000 pywaclient-1.3.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 16:18:52.000000 pywaclient-1.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-04-07 16:18:38.000000 pywaclient-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:18:52.000000 pywaclient-1.3.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:18:52.000000 pywaclient-1.3.2/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/data/block.json
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/data/form_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/init_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_article_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_block_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_block_template_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_block_template_part_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_canvas_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_category_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_chronicle_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_history_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_image_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_manuscript_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_map_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_notebook_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_parse_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_rpg_system_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_secret_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_subscriber_group_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_timeline_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_user_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_variable_collection_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_variable_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     4530 2023-04-07 16:18:38.000000 pywaclient-1.3.2/tests/test_world_endpoint.py
```

### Comparing `pywaclient-1.3.1/LICENCE` & `pywaclient-1.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/PKG-INFO` & `pywaclient-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.3.1
+Version: 1.3.2
 Summary: A small wrapper library around the World Anvil Aragorn API: https://www.worldanvil.com/api/aragorn/documentation.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.3.1/README.md` & `pywaclient-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/__init__.py` & `pywaclient-1.3.2/pywaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/api.py` & `pywaclient-1.3.2/pywaclient/api.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/__init__.py` & `pywaclient-1.3.2/pywaclient/endpoints/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
         r.raise_for_status()
         for chunk in r.iter_content(chunk_size=chunk_size):
             yield chunk
 
 def _parse_response(path: str, response: Response, params: Dict[str, Any], content: Dict[str, Any]) -> Dict[str, Any]:
     if response.ok:
         data = response.json()
+        if 'success' not in data:
+            raise UnexpectedStatusException(response.status_code, 'Response contained no success flag.', path, params, content)
         if data['success']:
             return data
         else:
             raise FailedRequest(response.status_code, path, data['error'], data, params, content)
     elif response.status_code == 401:
         raise AccessForbidden(path, params, content)
     elif response.status_code == 403:
```

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/articles.py` & `pywaclient-1.3.2/pywaclient/endpoints/articles.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/block_templates.py` & `pywaclient-1.3.2/pywaclient/endpoints/block_templates.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/blocks.py` & `pywaclient-1.3.2/pywaclient/endpoints/blocks.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/canvas.py` & `pywaclient-1.3.2/pywaclient/endpoints/canvas.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/categories.py` & `pywaclient-1.3.2/pywaclient/endpoints/categories.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/chronicles.py` & `pywaclient-1.3.2/pywaclient/endpoints/chronicles.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/histories.py` & `pywaclient-1.3.2/pywaclient/endpoints/histories.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/images.py` & `pywaclient-1.3.2/pywaclient/endpoints/images.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/manuscripts.py` & `pywaclient-1.3.2/pywaclient/endpoints/manuscripts.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/map_marker_types.py` & `pywaclient-1.3.2/pywaclient/endpoints/map_marker_types.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/maps.py` & `pywaclient-1.3.2/pywaclient/endpoints/maps.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,35 +12,37 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 from typing import Dict, Any, Iterable
 
 from pywaclient.endpoints import CrudEndpoint
 
 
-class MapLayerCrudEndpoint(CrudEndpoint):
+class MapMarkerCrudEndpoint(CrudEndpoint):
 
     def __init__(self, client: 'AragornApiClient'):
-        super().__init__(client, 'layer')
+        super().__init__(client, 'marker')
 
 
 class MapMarkerGroupCrudEndpoint(CrudEndpoint):
 
     def __init__(self, client: 'AragornApiClient'):
         super().__init__(client, 'markergroup')
+        self.marker = MapMarkerCrudEndpoint(client)
         self.path_markers = 'markergroup/markers'
 
     def markers(self, map_maker_group_id: str) -> Iterable[Dict[str, Any]]:
         """Iterate over all map markers in a map marker group.
         """
         return self._scroll_collection(self.path_markers, {'id': map_maker_group_id}, 'entities')
 
-class MapMarkerCrudEndpoint(CrudEndpoint):
+
+class MapLayerCrudEndpoint(CrudEndpoint):
 
     def __init__(self, client: 'AragornApiClient'):
-        super().__init__(client, 'marker')
+        super().__init__(client, 'layer')
 
 
 class MapCrudEndpoint(CrudEndpoint):
 
     def __init__(self, client: 'AragornApiClient'):
         super().__init__(client, 'map')
         self.path_layers = f'{self.path}/layers'
```

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/notebooks.py` & `pywaclient-1.3.2/pywaclient/endpoints/notebooks.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/rpg_system.py` & `pywaclient-1.3.2/pywaclient/endpoints/rpg_system.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/secrets.py` & `pywaclient-1.3.2/pywaclient/endpoints/secrets.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/subscriber_groups.py` & `pywaclient-1.3.2/pywaclient/endpoints/subscriber_groups.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/timelines.py` & `pywaclient-1.3.2/pywaclient/endpoints/timelines.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/users.py` & `pywaclient-1.3.2/pywaclient/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/variables.py` & `pywaclient-1.3.2/pywaclient/endpoints/variables.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/endpoints/worlds.py` & `pywaclient-1.3.2/pywaclient/endpoints/worlds.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/exceptions/__init__.py` & `pywaclient-1.3.2/pywaclient/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/models/article.py` & `pywaclient-1.3.2/pywaclient/models/article.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/models/block.py` & `pywaclient-1.3.2/pywaclient/models/block.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/models/category.py` & `pywaclient-1.3.2/pywaclient/models/category.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/models/entity.py` & `pywaclient-1.3.2/pywaclient/models/entity.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/models/genre.py` & `pywaclient-1.3.2/pywaclient/models/genre.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/models/manuscript.py` & `pywaclient-1.3.2/pywaclient/models/manuscript.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/models/secret.py` & `pywaclient-1.3.2/pywaclient/models/secret.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/models/user.py` & `pywaclient-1.3.2/pywaclient/models/user.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient/models/world.py` & `pywaclient-1.3.2/pywaclient/models/world.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/pywaclient.egg-info/PKG-INFO` & `pywaclient-1.3.2/pywaclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.3.1
+Version: 1.3.2
 Summary: A small wrapper library around the World Anvil Aragorn API: https://www.worldanvil.com/api/aragorn/documentation.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.3.1/pywaclient.egg-info/SOURCES.txt` & `pywaclient-1.3.2/pywaclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 tests/test_category_endpoint.py
 tests/test_chronicle_endpoint.py
 tests/test_history_endpoint.py
 tests/test_image_endpoint.py
 tests/test_manuscript_endpoint.py
 tests/test_map_endpoint.py
 tests/test_notebook_endpoint.py
+tests/test_parse_response.py
 tests/test_rpg_system_endpoint.py
 tests/test_secret_endpoint.py
 tests/test_subscriber_group_endpoint.py
 tests/test_timeline_endpoint.py
 tests/test_user_endpoint.py
 tests/test_variable_collection_endpoint.py
 tests/test_variable_endpoint.py
```

### Comparing `pywaclient-1.3.1/setup.py` & `pywaclient-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/data/block.json` & `pywaclient-1.3.2/tests/data/block.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/data/form_schema.json` & `pywaclient-1.3.2/tests/data/form_schema.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/init_client.py` & `pywaclient-1.3.2/tests/init_client.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_article_endpoint.py` & `pywaclient-1.3.2/tests/test_article_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from init_client import world_id, client
 
 if __name__ == '__main__':
+
     test_article_1 = client.article.put(
         {
             'title': 'Test Article Creation',
             'templateType': 'article',
             'world': {
-                'id': world_id}
+                'id': world_id
+            }
         }
     )
     test_article_2 = client.article.put(
         {
             'title': 'Test Article Creation 2',
             'templateType': 'article',
             'world': {
```

### Comparing `pywaclient-1.3.1/tests/test_block_endpoint.py` & `pywaclient-1.3.2/tests/test_block_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_block_template_endpoint.py` & `pywaclient-1.3.2/tests/test_block_template_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_block_template_part_endpoint.py` & `pywaclient-1.3.2/tests/test_block_template_part_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_canvas_endpoint.py` & `pywaclient-1.3.2/tests/test_canvas_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_category_endpoint.py` & `pywaclient-1.3.2/tests/test_category_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_chronicle_endpoint.py` & `pywaclient-1.3.2/tests/test_chronicle_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_history_endpoint.py` & `pywaclient-1.3.2/tests/test_history_endpoint.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,27 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from init_client import world_id, client
 
 if __name__ == '__main__':
+    for history in client.world.histories(world_id):
+        print(history['title'])
+        client.history.delete(history['id'])
+
+    test_timeline_1 = client.timeline.put(
+        {
+            'title': 'Test Timeline Creation',
+            'world': {
+                'id': world_id
+            }
+        }
+    )
+
     test_histories_1 = client.history.put(
         {
             'title': 'Test Histories Creation',
             "year":"5545",
             'world': {
                 'id': world_id
             }
@@ -26,15 +39,20 @@
     )
     test_histories_2 = client.history.put(
         {
             'title': 'Test Histories Creation 2',
             'year': '2992',
             'world': {
                 'id': world_id
-            }
+            },
+            # 'timelines': [
+            #     {
+            #         'id': test_timeline_1['id']
+            #     }
+            #]
         }
     )
     response_patch_histories_2 = client.history.patch(
         test_histories_2['id'],
         {
             'hour': '2001ad'
         }
@@ -45,7 +63,11 @@
         2
     )
 
     assert full_test_histories_2['hour'] == 2001
 
     client.history.delete(test_histories_1['id'])
     client.history.delete(test_histories_2['id'])
+    client.history.delete(test_timeline_1['id'])
+
+    for history in client.world.histories(world_id):
+        client.history.delete(history['id'])
```

### Comparing `pywaclient-1.3.1/tests/test_image_endpoint.py` & `pywaclient-1.3.2/tests/test_image_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_manuscript_endpoint.py` & `pywaclient-1.3.2/tests/test_manuscript_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_map_endpoint.py` & `pywaclient-1.3.2/tests/test_map_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_notebook_endpoint.py` & `pywaclient-1.3.2/tests/test_notebook_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_rpg_system_endpoint.py` & `pywaclient-1.3.2/tests/test_rpg_system_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_secret_endpoint.py` & `pywaclient-1.3.2/tests/test_secret_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_subscriber_group_endpoint.py` & `pywaclient-1.3.2/tests/test_subscriber_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_timeline_endpoint.py` & `pywaclient-1.3.2/tests/test_timeline_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_user_endpoint.py` & `pywaclient-1.3.2/tests/test_user_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_variable_collection_endpoint.py` & `pywaclient-1.3.2/tests/test_variable_collection_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_variable_endpoint.py` & `pywaclient-1.3.2/tests/test_variable_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.3.1/tests/test_world_endpoint.py` & `pywaclient-1.3.2/tests/test_world_endpoint.py`

 * *Files identical despite different names*

