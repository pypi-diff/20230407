# Comparing `tmp/fabric_fim-1.4.6.tar.gz` & `tmp/fabric_fim-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fim-1.4.6.tar", last modified: Fri Feb 24 21:47:17 2023, max compression
+gzip compressed data, was "fabric_fim-1.4.7.tar", last modified: Fri Apr  7 20:53:02 2023, max compression
```

## Comparing `fabric_fim-1.4.6.tar` & `fabric_fim-1.4.7.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.240759 fabric_fim-1.4.6/
--rw-r--r--   0 ibaldin    (502) staff       (20)       26 2020-07-24 21:42:44.000000 fabric_fim-1.4.6/AUTHORS
--rw-r--r--   0 ibaldin    (502) staff       (20)     1071 2020-07-14 22:09:49.000000 fabric_fim-1.4.6/LICENSE
--rw-r--r--   0 ibaldin    (502) staff       (20)      146 2022-04-27 22:22:19.000000 fabric_fim-1.4.6/MANIFEST.in
--rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-02-24 21:47:17.240486 fabric_fim-1.4.6/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)    10990 2023-02-24 21:11:28.000000 fabric_fim-1.4.6/README.md
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.199237 fabric_fim-1.4.6/fabric_fim.egg-info/
--rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-02-24 21:47:17.000000 fabric_fim-1.4.6/fabric_fim.egg-info/PKG-INFO
--rw-r--r--   0 ibaldin    (502) staff       (20)     2324 2023-02-24 21:47:17.000000 fabric_fim-1.4.6/fabric_fim.egg-info/SOURCES.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2023-02-24 21:47:17.000000 fabric_fim-1.4.6/fabric_fim.egg-info/dependency_links.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-02-24 21:47:17.000000 fabric_fim-1.4.6/fabric_fim.egg-info/requires.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)        4 2023-02-24 21:47:17.000000 fabric_fim-1.4.6/fabric_fim.egg-info/top_level.txt
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.200674 fabric_fim-1.4.6/fim/
--rw-r--r--   0 ibaldin    (502) staff       (20)       22 2023-02-24 21:46:26.000000 fabric_fim-1.4.6/fim/__init__.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.201742 fabric_fim-1.4.6/fim/authz/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2022-04-27 22:22:19.000000 fabric_fim-1.4.6/fim/authz/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    16139 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/authz/attribute_collector.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.207292 fabric_fim-1.4.6/fim/graph/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:31:38.000000 fabric_fim-1.4.6/fim/graph/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    69693 2023-02-24 21:11:28.000000 fabric_fim-1.4.6/fim/graph/abc_property_graph.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4093 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/graph/abc_property_graph_constants.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.211012 fabric_fim-1.4.6/fim/graph/data/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-08-18 21:34:07.000000 fabric_fim-1.4.6/fim/graph/data/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      283 2020-09-03 22:10:53.000000 fabric_fim-1.4.6/fim/graph/data/capacity_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)      100 2020-08-27 20:41:23.000000 fabric_fim-1.4.6/fim/graph/data/constraint_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)     3829 2023-02-24 21:11:28.000000 fabric_fim-1.4.6/fim/graph/data/graph_validation_rules.json
--rw-r--r--   0 ibaldin    (502) staff       (20)      547 2020-09-03 22:10:39.000000 fabric_fim-1.4.6/fim/graph/data/label_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)       91 2020-08-27 20:40:54.000000 fabric_fim-1.4.6/fim/graph/data/location_types.json
--rw-r--r--   0 ibaldin    (502) staff       (20)      367 2021-05-25 21:09:37.000000 fabric_fim-1.4.6/fim/graph/data/neo4j_indexes.json
--rw-r--r--   0 ibaldin    (502) staff       (20)    43467 2023-02-24 21:44:22.000000 fabric_fim-1.4.6/fim/graph/neo4j_property_graph.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     6160 2022-10-06 17:38:08.000000 fabric_fim-1.4.6/fim/graph/networkx_mixin.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    42040 2023-02-24 21:11:28.000000 fabric_fim-1.4.6/fim/graph/networkx_property_graph.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8354 2022-10-07 03:05:34.000000 fabric_fim-1.4.6/fim/graph/networkx_property_graph_disjoint.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.217319 fabric_fim-1.4.6/fim/graph/resources/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:04.000000 fabric_fim-1.4.6/fim/graph/resources/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4484 2021-05-25 21:09:37.000000 fabric_fim-1.4.6/fim/graph/resources/abc_adm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    13570 2023-02-24 21:11:28.000000 fabric_fim-1.4.6/fim/graph/resources/abc_arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2991 2022-02-18 19:27:15.000000 fabric_fim-1.4.6/fim/graph/resources/abc_bqm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4547 2021-03-31 01:14:29.000000 fabric_fim-1.4.6/fim/graph/resources/abc_cbm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2297 2021-03-07 22:42:30.000000 fabric_fim-1.4.6/fim/graph/resources/neo4j_adm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2106 2021-05-25 21:09:37.000000 fabric_fim-1.4.6/fim/graph/resources/neo4j_arm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    18425 2023-02-24 21:11:28.000000 fabric_fim-1.4.6/fim/graph/resources/neo4j_cbm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5017 2022-02-18 19:27:15.000000 fabric_fim-1.4.6/fim/graph/resources/networkx_abqm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2341 2021-03-07 22:42:30.000000 fabric_fim-1.4.6/fim/graph/resources/networkx_adm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2122 2021-05-25 21:09:37.000000 fabric_fim-1.4.6/fim/graph/resources/networkx_arm.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.219273 fabric_fim-1.4.6/fim/graph/slices/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:24.000000 fabric_fim-1.4.6/fim/graph/slices/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8223 2022-02-18 19:27:15.000000 fabric_fim-1.4.6/fim/graph/slices/abc_asm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3713 2021-06-04 19:43:14.000000 fabric_fim-1.4.6/fim/graph/slices/neo4j_asm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     4298 2021-06-04 19:43:14.000000 fabric_fim-1.4.6/fim/graph/slices/networkx_asm.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8615 2021-03-03 19:57:54.000000 fabric_fim-1.4.6/fim/graph/typed_tuples.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.219850 fabric_fim-1.4.6/fim/logging/
--rw-r--r--   0 ibaldin    (502) staff       (20)        0 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/logging/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9071 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/logging/log_collector.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9555 2021-03-24 00:18:51.000000 fabric_fim-1.4.6/fim/pluggable.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.231335 fabric_fim-1.4.6/fim/slivers/
--rw-r--r--   0 ibaldin    (502) staff       (20)      217 2021-06-14 18:36:21.000000 fabric_fim-1.4.6/fim/slivers/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3641 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/slivers/attached_components.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    13021 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/slivers/base_sliver.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    23768 2023-02-08 17:26:40.000000 fabric_fim-1.4.6/fim/slivers/capacities_labels.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    11247 2022-02-18 19:27:15.000000 fabric_fim-1.4.6/fim/slivers/component_catalog.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.232591 fabric_fim-1.4.6/fim/slivers/data/
--rw-r--r--   0 ibaldin    (502) staff       (20)        1 2021-03-03 19:57:54.000000 fabric_fim-1.4.6/fim/slivers/data/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1469 2023-02-08 17:26:40.000000 fabric_fim-1.4.6/fim/slivers/data/component_catalog.json
--rw-r--r--   0 ibaldin    (502) staff       (20)    76943 2022-09-10 21:18:41.000000 fabric_fim-1.4.6/fim/slivers/data/instance_sizes.json
--rw-r--r--   0 ibaldin    (502) staff       (20)    23524 2022-02-18 19:27:15.000000 fabric_fim-1.4.6/fim/slivers/delegations.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3593 2022-02-18 19:27:15.000000 fabric_fim-1.4.6/fim/slivers/gateway.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      919 2021-06-29 20:04:13.000000 fabric_fim-1.4.6/fim/slivers/identifiers.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3444 2022-02-18 19:27:15.000000 fabric_fim-1.4.6/fim/slivers/instance_catalog.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3225 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/slivers/interface_info.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2702 2021-09-22 14:46:40.000000 fabric_fim-1.4.6/fim/slivers/json.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3869 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/slivers/json_data.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5983 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/slivers/maintenance_mode.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1566 2021-03-03 19:57:54.000000 fabric_fim-1.4.6/fim/slivers/network_attached_storage.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3910 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/slivers/network_link.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    10209 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/slivers/network_node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    20924 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/slivers/network_service.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     6795 2021-06-04 19:43:14.000000 fabric_fim-1.4.6/fim/slivers/path_info.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     3024 2022-02-18 19:27:15.000000 fabric_fim-1.4.6/fim/slivers/tags.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     2622 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/slivers/topology_diff.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.237943 fabric_fim-1.4.6/fim/user/
--rw-r--r--   0 ibaldin    (502) staff       (20)     1914 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/user/__init__.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    11730 2022-09-10 21:18:41.000000 fabric_fim-1.4.6/fim/user/component.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     5668 2022-09-10 21:18:41.000000 fabric_fim-1.4.6/fim/user/composite_node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     7660 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/user/interface.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     8381 2022-09-10 21:18:41.000000 fabric_fim-1.4.6/fim/user/link.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     1219 2021-03-03 19:57:54.000000 fabric_fim-1.4.6/fim/user/measurement.py
--rw-r--r--   0 ibaldin    (502) staff       (20)     9668 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/fim/user/model_element.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    28500 2023-02-14 21:58:39.000000 fabric_fim-1.4.6/fim/user/network_service.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    22636 2023-02-14 21:58:39.000000 fabric_fim-1.4.6/fim/user/node.py
--rw-r--r--   0 ibaldin    (502) staff       (20)    58158 2023-02-14 21:58:39.000000 fabric_fim-1.4.6/fim/user/topology.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      595 2021-03-13 20:40:37.000000 fabric_fim-1.4.6/fim/view_only_dict.py
--rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/requirements.txt
--rw-r--r--   0 ibaldin    (502) staff       (20)       38 2023-02-24 21:47:17.240827 fabric_fim-1.4.6/setup.cfg
--rw-r--r--   0 ibaldin    (502) staff       (20)      874 2023-02-02 01:41:56.000000 fabric_fim-1.4.6/setup.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.238753 fabric_fim-1.4.6/test/
--rw-r--r--   0 ibaldin    (502) staff       (20)      654 2022-02-18 19:27:15.000000 fabric_fim-1.4.6/test/test_load.py
-drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-02-24 21:47:17.240032 fabric_fim-1.4.6/util/
--rw-r--r--   0 ibaldin    (502) staff       (20)    14115 2023-02-24 21:43:01.000000 fabric_fim-1.4.6/util/fim_util.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.673249 fabric_fim-1.4.7/
+-rw-r--r--   0 ibaldin    (502) staff       (20)       26 2020-07-24 21:42:44.000000 fabric_fim-1.4.7/AUTHORS
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1071 2020-07-14 22:09:49.000000 fabric_fim-1.4.7/LICENSE
+-rw-r--r--   0 ibaldin    (502) staff       (20)      146 2022-04-27 22:22:19.000000 fabric_fim-1.4.7/MANIFEST.in
+-rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-04-07 20:53:02.672887 fabric_fim-1.4.7/PKG-INFO
+-rw-r--r--   0 ibaldin    (502) staff       (20)    10990 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/README.md
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.533814 fabric_fim-1.4.7/fabric_fim.egg-info/
+-rw-r--r--   0 ibaldin    (502) staff       (20)    11437 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/PKG-INFO
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2324 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/SOURCES.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/dependency_links.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/requires.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)        4 2023-04-07 20:53:02.000000 fabric_fim-1.4.7/fabric_fim.egg-info/top_level.txt
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.535369 fabric_fim-1.4.7/fim/
+-rw-r--r--   0 ibaldin    (502) staff       (20)       22 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/__init__.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.537180 fabric_fim-1.4.7/fim/authz/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2022-04-27 22:22:19.000000 fabric_fim-1.4.7/fim/authz/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    16139 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/authz/attribute_collector.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.608058 fabric_fim-1.4.7/fim/graph/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:31:38.000000 fabric_fim-1.4.7/fim/graph/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    69693 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/abc_property_graph.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4093 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/graph/abc_property_graph_constants.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.621201 fabric_fim-1.4.7/fim/graph/data/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-08-18 21:34:07.000000 fabric_fim-1.4.7/fim/graph/data/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      283 2020-09-03 22:10:53.000000 fabric_fim-1.4.7/fim/graph/data/capacity_types.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)      100 2020-08-27 20:41:23.000000 fabric_fim-1.4.7/fim/graph/data/constraint_types.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3829 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/data/graph_validation_rules.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)      547 2020-09-03 22:10:39.000000 fabric_fim-1.4.7/fim/graph/data/label_types.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)       91 2020-08-27 20:40:54.000000 fabric_fim-1.4.7/fim/graph/data/location_types.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)      367 2021-05-25 21:09:37.000000 fabric_fim-1.4.7/fim/graph/data/neo4j_indexes.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)    43467 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/neo4j_property_graph.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     6160 2022-10-06 17:38:08.000000 fabric_fim-1.4.7/fim/graph/networkx_mixin.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    42040 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/networkx_property_graph.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     8354 2022-10-07 03:05:34.000000 fabric_fim-1.4.7/fim/graph/networkx_property_graph_disjoint.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.631858 fabric_fim-1.4.7/fim/graph/resources/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:04.000000 fabric_fim-1.4.7/fim/graph/resources/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4484 2021-05-25 21:09:37.000000 fabric_fim-1.4.7/fim/graph/resources/abc_adm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    13570 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/resources/abc_arm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2991 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/graph/resources/abc_bqm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4547 2021-03-31 01:14:29.000000 fabric_fim-1.4.7/fim/graph/resources/abc_cbm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2297 2021-03-07 22:42:30.000000 fabric_fim-1.4.7/fim/graph/resources/neo4j_adm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2106 2021-05-25 21:09:37.000000 fabric_fim-1.4.7/fim/graph/resources/neo4j_arm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    18425 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/graph/resources/neo4j_cbm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     5017 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/graph/resources/networkx_abqm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2341 2021-03-07 22:42:30.000000 fabric_fim-1.4.7/fim/graph/resources/networkx_adm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2122 2021-05-25 21:09:37.000000 fabric_fim-1.4.7/fim/graph/resources/networkx_arm.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.640574 fabric_fim-1.4.7/fim/graph/slices/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2020-09-02 18:32:24.000000 fabric_fim-1.4.7/fim/graph/slices/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     8223 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/graph/slices/abc_asm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3713 2021-06-04 19:43:14.000000 fabric_fim-1.4.7/fim/graph/slices/neo4j_asm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     4298 2021-06-04 19:43:14.000000 fabric_fim-1.4.7/fim/graph/slices/networkx_asm.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     8615 2021-03-03 19:57:54.000000 fabric_fim-1.4.7/fim/graph/typed_tuples.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.641525 fabric_fim-1.4.7/fim/logging/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        0 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/logging/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     9071 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/logging/log_collector.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     9555 2021-03-24 00:18:51.000000 fabric_fim-1.4.7/fim/pluggable.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.659857 fabric_fim-1.4.7/fim/slivers/
+-rw-r--r--   0 ibaldin    (502) staff       (20)      217 2021-06-14 18:36:21.000000 fabric_fim-1.4.7/fim/slivers/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3641 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/attached_components.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    13021 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/base_sliver.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    24088 2023-04-05 22:29:04.000000 fabric_fim-1.4.7/fim/slivers/capacities_labels.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    11269 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/slivers/component_catalog.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.661737 fabric_fim-1.4.7/fim/slivers/data/
+-rw-r--r--   0 ibaldin    (502) staff       (20)        1 2021-03-03 19:57:54.000000 fabric_fim-1.4.7/fim/slivers/data/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1657 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/fim/slivers/data/component_catalog.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)    76943 2022-09-10 21:18:41.000000 fabric_fim-1.4.7/fim/slivers/data/instance_sizes.json
+-rw-r--r--   0 ibaldin    (502) staff       (20)    23524 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/slivers/delegations.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3593 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/slivers/gateway.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      919 2021-06-29 20:04:13.000000 fabric_fim-1.4.7/fim/slivers/identifiers.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3444 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/slivers/instance_catalog.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3225 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/interface_info.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2702 2021-09-22 14:46:40.000000 fabric_fim-1.4.7/fim/slivers/json.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3869 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/json_data.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     5983 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/maintenance_mode.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1566 2021-03-03 19:57:54.000000 fabric_fim-1.4.7/fim/slivers/network_attached_storage.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3910 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/network_link.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    10209 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/network_node.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    22042 2023-04-05 22:02:35.000000 fabric_fim-1.4.7/fim/slivers/network_service.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     6795 2021-06-04 19:43:14.000000 fabric_fim-1.4.7/fim/slivers/path_info.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     3024 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/fim/slivers/tags.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     2622 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/slivers/topology_diff.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.670754 fabric_fim-1.4.7/fim/user/
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1914 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/user/__init__.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    11730 2022-09-10 21:18:41.000000 fabric_fim-1.4.7/fim/user/component.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     5668 2022-09-10 21:18:41.000000 fabric_fim-1.4.7/fim/user/composite_node.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     7660 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/fim/user/interface.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     8381 2022-09-10 21:18:41.000000 fabric_fim-1.4.7/fim/user/link.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     1219 2021-03-03 19:57:54.000000 fabric_fim-1.4.7/fim/user/measurement.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)     9668 2023-04-05 18:48:29.000000 fabric_fim-1.4.7/fim/user/model_element.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    29219 2023-04-05 22:02:45.000000 fabric_fim-1.4.7/fim/user/network_service.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    22636 2023-02-14 21:58:39.000000 fabric_fim-1.4.7/fim/user/node.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)    58158 2023-02-14 21:58:39.000000 fabric_fim-1.4.7/fim/user/topology.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      595 2021-03-13 20:40:37.000000 fabric_fim-1.4.7/fim/view_only_dict.py
+-rw-r--r--   0 ibaldin    (502) staff       (20)      118 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/requirements.txt
+-rw-r--r--   0 ibaldin    (502) staff       (20)       38 2023-04-07 20:53:02.673324 fabric_fim-1.4.7/setup.cfg
+-rw-r--r--   0 ibaldin    (502) staff       (20)      874 2023-02-02 01:41:56.000000 fabric_fim-1.4.7/setup.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.671686 fabric_fim-1.4.7/test/
+-rw-r--r--   0 ibaldin    (502) staff       (20)      654 2022-02-18 19:27:15.000000 fabric_fim-1.4.7/test/test_load.py
+drwxr-xr-x   0 ibaldin    (502) staff       (20)        0 2023-04-07 20:53:02.672244 fabric_fim-1.4.7/util/
+-rw-r--r--   0 ibaldin    (502) staff       (20)    14115 2023-04-05 20:55:22.000000 fabric_fim-1.4.7/util/fim_util.py
```

### Comparing `fabric_fim-1.4.6/LICENSE` & `fabric_fim-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/PKG-INFO` & `fabric_fim-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_fim
-Version: 1.4.6
+Version: 1.4.7
 Summary: FABRIC Information Model Library
 Home-page: https://github.com/fabric-testbed/InformationModel
 Author: Ilya Baldin, Komal Thareja
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `fabric_fim-1.4.6/README.md` & `fabric_fim-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fabric_fim.egg-info/PKG-INFO` & `fabric_fim-1.4.7/fabric_fim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-fim
-Version: 1.4.6
+Version: 1.4.7
 Summary: FABRIC Information Model Library
 Home-page: https://github.com/fabric-testbed/InformationModel
 Author: Ilya Baldin, Komal Thareja
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `fabric_fim-1.4.6/fabric_fim.egg-info/SOURCES.txt` & `fabric_fim-1.4.7/fabric_fim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/authz/attribute_collector.py` & `fabric_fim-1.4.7/fim/authz/attribute_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/abc_property_graph.py` & `fabric_fim-1.4.7/fim/graph/abc_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/abc_property_graph_constants.py` & `fabric_fim-1.4.7/fim/graph/abc_property_graph_constants.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/data/graph_validation_rules.json` & `fabric_fim-1.4.7/fim/graph/data/graph_validation_rules.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/data/label_types.json` & `fabric_fim-1.4.7/fim/graph/data/label_types.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/neo4j_property_graph.py` & `fabric_fim-1.4.7/fim/graph/neo4j_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/networkx_mixin.py` & `fabric_fim-1.4.7/fim/graph/networkx_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/networkx_property_graph.py` & `fabric_fim-1.4.7/fim/graph/networkx_property_graph.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/networkx_property_graph_disjoint.py` & `fabric_fim-1.4.7/fim/graph/networkx_property_graph_disjoint.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/abc_adm.py` & `fabric_fim-1.4.7/fim/graph/resources/abc_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/abc_arm.py` & `fabric_fim-1.4.7/fim/graph/resources/abc_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/abc_bqm.py` & `fabric_fim-1.4.7/fim/graph/resources/abc_bqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/abc_cbm.py` & `fabric_fim-1.4.7/fim/graph/resources/abc_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/neo4j_adm.py` & `fabric_fim-1.4.7/fim/graph/resources/neo4j_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/neo4j_arm.py` & `fabric_fim-1.4.7/fim/graph/resources/neo4j_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/neo4j_cbm.py` & `fabric_fim-1.4.7/fim/graph/resources/neo4j_cbm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/networkx_abqm.py` & `fabric_fim-1.4.7/fim/graph/resources/networkx_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/networkx_adm.py` & `fabric_fim-1.4.7/fim/graph/resources/networkx_adm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/resources/networkx_arm.py` & `fabric_fim-1.4.7/fim/graph/resources/networkx_arm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/slices/abc_asm.py` & `fabric_fim-1.4.7/fim/graph/slices/abc_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/slices/neo4j_asm.py` & `fabric_fim-1.4.7/fim/graph/slices/neo4j_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/slices/networkx_asm.py` & `fabric_fim-1.4.7/fim/graph/slices/networkx_asm.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/graph/typed_tuples.py` & `fabric_fim-1.4.7/fim/graph/typed_tuples.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/logging/log_collector.py` & `fabric_fim-1.4.7/fim/logging/log_collector.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/pluggable.py` & `fabric_fim-1.4.7/fim/pluggable.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/attached_components.py` & `fabric_fim-1.4.7/fim/slivers/attached_components.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/base_sliver.py` & `fabric_fim-1.4.7/fim/slivers/base_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/capacities_labels.py` & `fabric_fim-1.4.7/fim/slivers/capacities_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,14 +450,23 @@
         if len(d) == 0:
             return ''
         ret = "{ "
         for i, v in d.items():
             ret = ret + i + ": " + str(v) + ", "
         return ret[:-2] + "}"
 
+    def __eq__(self, other):
+        if not other:
+            return False
+        assert isinstance(other, Labels)
+        for f, v in self.__dict__.items():
+            if v != other.__dict__[f]:
+                return False
+        return True
+
 
 class ReservationInfo(JSONField):
     """
     Reservation info structure for ASM sliver objects
     """
 
     def __init__(self, **kwargs):
@@ -572,14 +581,15 @@
     """
     JSON-ified representation of various flags that can be attached to slivers
     """
     def __init__(self, **kwargs):
         self.auto_config = False # primarily for interfaces
         self.auto_mount = False # primarily for storage components
         self.ipv4_management = False # request ipv4 management IP
+        self.ptp_available = False # for advertisements of nodes/sites
         self._set_fields(**kwargs)
 
     def _set_fields(self, **kwargs):
         for k, v in kwargs.items():
             assert v is not None
             assert isinstance(v, bool)
             try:
```

### Comparing `fabric_fim-1.4.6/fim/slivers/component_catalog.py` & `fabric_fim-1.4.7/fim/slivers/component_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                                        f" component (need {len(interfaces_dict.keys())} instead of "
                                        f"{len(interface_labels)}")
             iinfo = InterfaceInfo()
             id_index = 0
             for interface_name in interfaces_dict.keys():
                 isliver = InterfaceSliver()
                 isliver.set_name(name + '-' + interface_name)
-                if cs.get_type() == ComponentType.SmartNIC:
+                if cs.get_type() in [ComponentType.SmartNIC, ComponentType.FPGA]:
                     isliver.set_type(InterfaceType.DedicatedPort)
                 elif cs.get_type() == ComponentType.SharedNIC:
                     isliver.set_type(InterfaceType.SharedPort)
                 if interface_node_ids is not None:
                     isliver.node_id = interface_node_ids[id_index]
                 else:
                     isliver.node_id = str(uuid.uuid4())
```

### Comparing `fabric_fim-1.4.6/fim/slivers/data/component_catalog.json` & `fabric_fim-1.4.7/fim/slivers/data/component_catalog.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {'insert': "[(10, OrderedDict([('Model', 'Xilinx-U280'), ('Type', 'FPGA'), ('Details', 'Xilinx "*

 * *           "U280 FPGA Dual 100G port accelerator card'), ('Interfaces', OrderedDict([('p1', "*

 * *           "'100'), ('p2', '100')]))]))]"}*

```diff
@@ -65,9 +65,18 @@
         "Model": "P4510",
         "Type": "NVME"
     },
     {
         "Details": "Site-local NAS share",
         "Model": "NAS",
         "Type": "Storage"
+    },
+    {
+        "Details": "Xilinx U280 FPGA Dual 100G port accelerator card",
+        "Interfaces": {
+            "p1": "100",
+            "p2": "100"
+        },
+        "Model": "Xilinx-U280",
+        "Type": "FPGA"
     }
 ]
```

### Comparing `fabric_fim-1.4.6/fim/slivers/data/instance_sizes.json` & `fabric_fim-1.4.7/fim/slivers/data/instance_sizes.json`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/delegations.py` & `fabric_fim-1.4.7/fim/slivers/delegations.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/gateway.py` & `fabric_fim-1.4.7/fim/slivers/gateway.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/identifiers.py` & `fabric_fim-1.4.7/fim/slivers/identifiers.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/instance_catalog.py` & `fabric_fim-1.4.7/fim/slivers/instance_catalog.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/interface_info.py` & `fabric_fim-1.4.7/fim/slivers/interface_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/json.py` & `fabric_fim-1.4.7/fim/slivers/json.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/json_data.py` & `fabric_fim-1.4.7/fim/slivers/json_data.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/maintenance_mode.py` & `fabric_fim-1.4.7/fim/slivers/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/network_attached_storage.py` & `fabric_fim-1.4.7/fim/slivers/network_attached_storage.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/network_link.py` & `fabric_fim-1.4.7/fim/slivers/network_link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/network_node.py` & `fabric_fim-1.4.7/fim/slivers/network_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/network_service.py` & `fabric_fim-1.4.7/fim/slivers/network_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 
     def __str__(self):
         return self.name
 
 
 ServiceConstraintRecord = recordclass('ServiceConstraintRecord',
                                       ['layer', 'desc',
+                                       'min_interfaces',
                                        'num_interfaces',
                                        'num_sites',
                                        'num_instances',
                                        'required_properties',
                                        'forbidden_properties',
                                        'required_interface_types'])
 
@@ -123,123 +124,138 @@
     # whenever there is no limit, num is set to 0
     NO_LIMIT = 0
     """
     Services can be limited by the number of interfaces/connection points they can connect
     The number of sites they may connect and the number of instances they may have in a slice.
     """
     ServiceConstraints = {
-        ServiceType.P4: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=NO_LIMIT, num_sites=1,
+        ServiceType.P4: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
+                                                num_interfaces=NO_LIMIT, num_sites=1,
                                                 num_instances=NO_LIMIT, required_properties=['controller_url'],
                                                 forbidden_properties=['mirror_port',
                                                                       'mirror_direction'],
                                                 required_interface_types=[],
                                                 desc='A P4 service.'),
-        ServiceType.OVS: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=NO_LIMIT, num_sites=1,
+        ServiceType.OVS: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
+                                                 num_interfaces=NO_LIMIT, num_sites=1,
                                                  num_instances=NO_LIMIT, required_properties=[],
                                                  forbidden_properties=['mirror_port',
                                                                        'mirror_direction'],
                                                  required_interface_types=[],
                                                  desc='An OVS generic service.'),
-        ServiceType.VLAN: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=NO_LIMIT, num_sites=1,
+        ServiceType.VLAN: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
+                                                  num_interfaces=NO_LIMIT, num_sites=1,
                                                   num_instances=NO_LIMIT, required_properties=[],
                                                   forbidden_properties=['mirror_port',
                                                                         'mirror_direction',
                                                                         'controller_url'],
                                                   required_interface_types=[],
                                                   desc='An local VLAN service in a site.'),
-        ServiceType.MPLS: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=NO_LIMIT, num_sites=1,
+        ServiceType.MPLS: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
+                                                  num_interfaces=NO_LIMIT, num_sites=1,
                                                   num_instances=NO_LIMIT, desc='An MPLS generic service',
                                                   required_properties=[],
                                                   forbidden_properties=['mirror_port',
                                                                         'mirror_direction',
                                                                         'controller_url'],
                                                   required_interface_types=[]),
-        ServiceType.L2Path: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=2, num_sites=2,
+        ServiceType.L2Path: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
+                                                    num_interfaces=2, num_sites=2,
                                                     num_instances=NO_LIMIT,
                                                     desc='A provider L2 Path e.g. from ESnet or Internet2.',
                                                     required_properties=[],
                                                     forbidden_properties=['mirror_port',
                                                                           'mirror_direction',
                                                                           'controller_url'],
                                                     required_interface_types=[]),
-        ServiceType.L2STS: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=NO_LIMIT, num_sites=2,
+        ServiceType.L2STS: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=2,
+                                                   num_interfaces=NO_LIMIT, num_sites=2,
                                                    num_instances=NO_LIMIT,
                                                    desc='A Site-to-Site service in FABRIC.',
                                                    required_properties=[],
                                                    forbidden_properties=['ero',
                                                                          'mirror_port',
                                                                          'mirror_direction',
                                                                          'controller_url'],
                                                    required_interface_types=[]),
-        ServiceType.L2PTP: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=2, num_sites=2,
+        ServiceType.L2PTP: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=2,
+                                                   num_interfaces=2, num_sites=2,
                                                    num_instances=NO_LIMIT,
                                                    desc='A Port-to-Port service in FABRIC.',
                                                    required_properties=[],
                                                    forbidden_properties=['mirror_port',
                                                                          'mirror_direction',
                                                                          'controller_url'],
                                                    required_interface_types=[InterfaceType.DedicatedPort,
                                                                              InterfaceType.FacilityPort]),
-        ServiceType.L2Multisite: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=NO_LIMIT, num_sites=NO_LIMIT,
+        ServiceType.L2Multisite: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
+                                                         num_interfaces=NO_LIMIT, num_sites=NO_LIMIT,
                                                          num_instances=NO_LIMIT,
                                                          desc='A Multi-Site L2 service in FABRIC.',
                                                          required_properties=[],
                                                          forbidden_properties=['mirror_port',
                                                                                'mirror_direction',
                                                                                'controller_url'],
                                                          required_interface_types=[]),
-        ServiceType.L2Bridge: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=NO_LIMIT, num_sites=1,
+        ServiceType.L2Bridge: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
+                                                      num_interfaces=NO_LIMIT, num_sites=1,
                                                       num_instances=NO_LIMIT,
                                                       desc='An L2 bridge service within a single FABRIC site.',
                                                       required_properties=[],
                                                       forbidden_properties=['mirror_port',
                                                                             'mirror_direction',
                                                                             'controller_url'],
                                                       required_interface_types=[]),
-        ServiceType.FABNetv4: ServiceConstraintRecord(layer=NSLayer.L3, num_interfaces=NO_LIMIT, num_sites=1,
+        ServiceType.FABNetv4: ServiceConstraintRecord(layer=NSLayer.L3, min_interfaces=1,
+                                                      num_interfaces=NO_LIMIT, num_sites=1,
                                                       num_instances=NO_LIMIT,
                                                       desc='A routed IPv4 (RFC1918 addressed) FABRIC network.',
                                                       required_properties=[],
                                                       forbidden_properties=['mirror_port',
                                                                             'mirror_direction',
                                                                             'controller_url'],
                                                       required_interface_types=[]),
-        ServiceType.FABNetv6: ServiceConstraintRecord(layer=NSLayer.L3, num_interfaces=NO_LIMIT, num_sites=1,
+        ServiceType.FABNetv6: ServiceConstraintRecord(layer=NSLayer.L3, min_interfaces=1,
+                                                      num_interfaces=NO_LIMIT, num_sites=1,
                                                       num_instances=NO_LIMIT,
                                                       desc='A routed IPv6 (publicly addressed) FABRIC network.',
                                                       required_properties=[],
                                                       forbidden_properties=['mirror_port',
                                                                             'mirror_direction',
                                                                             'controller_url'],
                                                       required_interface_types=[]),
-        ServiceType.PortMirror: ServiceConstraintRecord(layer=NSLayer.L2, num_interfaces=1, num_sites=1,
+        ServiceType.PortMirror: ServiceConstraintRecord(layer=NSLayer.L2, min_interfaces=1,
+                                                        num_interfaces=1, num_sites=1,
                                                         num_instances=NO_LIMIT,
                                                         desc='A port mirroring service in a FABRIC site.',
                                                         required_properties=['mirror_port',
                                                                              'mirror_direction', 'site'],
                                                         forbidden_properties=['controller_url'],
                                                         required_interface_types=[InterfaceType.DedicatedPort]),
-        ServiceType.L3VPN: ServiceConstraintRecord(layer=NSLayer.L3, num_interfaces=NO_LIMIT, num_sites=NO_LIMIT,
+        ServiceType.L3VPN: ServiceConstraintRecord(layer=NSLayer.L3, min_interfaces=1,
+                                                   num_interfaces=NO_LIMIT, num_sites=NO_LIMIT,
                                                    num_instances=NO_LIMIT,
                                                    desc='A L3 VPN service connecting to FABRIC.',
                                                    required_properties=[],
                                                    forbidden_properties=['mirror_port',
                                                                          'mirror_direction',
                                                                          'controller_url'],
                                                    required_interface_types=[]),
-        ServiceType.FABNetv4Ext: ServiceConstraintRecord(layer=NSLayer.L3, num_interfaces=NO_LIMIT, num_sites=1,
+        ServiceType.FABNetv4Ext: ServiceConstraintRecord(layer=NSLayer.L3, min_interfaces=1,
+                                                         num_interfaces=NO_LIMIT, num_sites=1,
                                                          num_instances=NO_LIMIT,
                                                          desc='A routed IPv4 publicly addressed FABRIC '
                                                               'network capable of external connectivity.',
                                                          required_properties=[],
                                                          forbidden_properties=['mirror_port',
                                                                                'mirror_direction',
                                                                                'controller_url'],
                                                          required_interface_types=[]),
-        ServiceType.FABNetv6Ext: ServiceConstraintRecord(layer=NSLayer.L3, num_interfaces=NO_LIMIT, num_sites=1,
+        ServiceType.FABNetv6Ext: ServiceConstraintRecord(layer=NSLayer.L3, min_interfaces=1,
+                                                         num_interfaces=NO_LIMIT, num_sites=1,
                                                          num_instances=NO_LIMIT,
                                                          desc='A routed IPv6 publicly addressed FABRIC network '
                                                               'capable of external connectivity.',
                                                          required_properties=[],
                                                          forbidden_properties=['mirror_port',
                                                                                'mirror_direction',
                                                                                'controller_url'],
```

### Comparing `fabric_fim-1.4.6/fim/slivers/path_info.py` & `fabric_fim-1.4.7/fim/slivers/path_info.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/tags.py` & `fabric_fim-1.4.7/fim/slivers/tags.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/slivers/topology_diff.py` & `fabric_fim-1.4.7/fim/slivers/topology_diff.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/user/__init__.py` & `fabric_fim-1.4.7/fim/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/user/component.py` & `fabric_fim-1.4.7/fim/user/component.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/user/composite_node.py` & `fabric_fim-1.4.7/fim/user/composite_node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/user/interface.py` & `fabric_fim-1.4.7/fim/user/interface.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/user/link.py` & `fabric_fim-1.4.7/fim/user/link.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/user/measurement.py` & `fabric_fim-1.4.7/fim/user/measurement.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/user/model_element.py` & `fabric_fim-1.4.7/fim/user/model_element.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/user/network_service.py` & `fabric_fim-1.4.7/fim/user/network_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #
 # Author: Ilya Baldin (ibaldin@renci.org)
 import logging
 from typing import Tuple, Any, List, Set
 
 import uuid
 
+import fim.user.topology
 from fim.view_only_dict import ViewOnlyDict
 
 from .model_element import ModelElement, ElementType, TopologyException
 
 from fim.graph.abc_property_graph import ABCPropertyGraph
 from fim.user.interface import Interface, InterfaceType
 from fim.user.link import Link, LinkType
@@ -224,19 +225,26 @@
         # check the number of instances of this service
         if NetworkServiceSliver.ServiceConstraints[nstype].num_instances != NetworkServiceSliver.NO_LIMIT:
             services = self.topo.graph_model.get_all_nodes_by_class_and_type(label=ABCPropertyGraph.CLASS_NetworkService,
                                                                              ntype=str(nstype))
             if len(services) + 1 > NetworkServiceSliver.ServiceConstraints[self.type].num_instances:
                 raise TopologyException(f"Service {self.name} type {nstype} cannot have {len(services) + 1} instances. "
                                         f"Limit: {NetworkServiceSliver.ServiceConstraints[nstype].num_instances}")
-        # check the number of interfaces
-        if NetworkServiceSliver.ServiceConstraints[nstype].num_interfaces != NetworkServiceSliver.NO_LIMIT:
-            if len(interfaces) > NetworkServiceSliver.ServiceConstraints[nstype].num_interfaces:
-                raise TopologyException(f"Service {self.name} of type {nstype} cannot have {len(interfaces)} interfaces. "
-                                        f"Limit: {NetworkServiceSliver.ServiceConstraints[nstype].num_interfaces}")
+
+        # check the number of interfaces only for experiment topologies
+        # in e.g. advertisements network services with no interfaces hang off dataplane switches
+        if isinstance(self.topo, fim.user.topology.ExperimentTopology):
+            if NetworkServiceSliver.ServiceConstraints[nstype].min_interfaces != NetworkServiceSliver.NO_LIMIT:
+                if len(interfaces) < NetworkServiceSliver.ServiceConstraints[nstype].min_interfaces:
+                    raise TopologyException(f"Service {self.name} of type {nstype} cannot have {len(interfaces)} interfaces. "
+                                            f"Limit at least: {NetworkServiceSliver.ServiceConstraints[nstype].min_interfaces}")
+            if NetworkServiceSliver.ServiceConstraints[nstype].num_interfaces != NetworkServiceSliver.NO_LIMIT:
+                if len(interfaces) > NetworkServiceSliver.ServiceConstraints[nstype].num_interfaces:
+                    raise TopologyException(f"Service {self.name} of type {nstype} cannot have {len(interfaces)} interfaces. "
+                                            f"Limit at most: {NetworkServiceSliver.ServiceConstraints[nstype].num_interfaces}")
         sites = set()
         # check the number of sites spanned by this service
         if NetworkServiceSliver.ServiceConstraints[nstype].num_sites != NetworkServiceSliver.NO_LIMIT:
             # trace ownership of each interface and count the sites involved
             for interface in interfaces:
                 owner = self.topo.get_owner_node(interface)
                 if owner is None:
```

### Comparing `fabric_fim-1.4.6/fim/user/node.py` & `fabric_fim-1.4.7/fim/user/node.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/user/topology.py` & `fabric_fim-1.4.7/fim/user/topology.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/fim/view_only_dict.py` & `fabric_fim-1.4.7/fim/view_only_dict.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/setup.py` & `fabric_fim-1.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/test/test_load.py` & `fabric_fim-1.4.7/test/test_load.py`

 * *Files identical despite different names*

### Comparing `fabric_fim-1.4.6/util/fim_util.py` & `fabric_fim-1.4.7/util/fim_util.py`

 * *Files identical despite different names*

