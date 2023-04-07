# Comparing `tmp/trame-vtk-2.4.2.tar.gz` & `tmp/trame-vtk-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-vtk-2.4.2.tar", last modified: Fri Mar 31 19:19:58 2023, max compression
+gzip compressed data, was "trame-vtk-2.4.3.tar", last modified: Fri Apr  7 19:04:12 2023, max compression
```

## Comparing `trame-vtk-2.4.2.tar` & `trame-vtk-2.4.3.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.865561 trame-vtk-2.4.2/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13038 2023-03-31 19:19:58.865561 trame-vtk-2.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12303 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/README.rst
--rw-r--r--   0 root         (0) root         (0)      878 2023-03-31 19:19:58.865561 trame-vtk-2.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.849561 trame-vtk-2.4.2/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.849561 trame-vtk-2.4.2/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame/modules/paraview.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame/modules/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.849561 trame-vtk-2.4.2/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame/widgets/paraview.py
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame/widgets/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.853561 trame-vtk-2.4.2/trame_vtk/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/LICENSE
--rw-r--r--   0 root         (0) root         (0)       91 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.853561 trame-vtk-2.4.2/trame_vtk/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.853561 trame-vtk-2.4.2/trame_vtk/modules/common/
--rw-r--r--   0 root         (0) root         (0)      354 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.853561 trame-vtk-2.4.2/trame_vtk/modules/common/serve/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/common/serve/.gitignore
--rw-r--r--   0 root         (0) root         (0)  1626752 2023-03-31 19:19:55.000000 trame-vtk-2.4.2/trame_vtk/modules/common/serve/trame-vtk.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.857560 trame-vtk-2.4.2/trame_vtk/modules/paraview/
--rw-r--r--   0 root         (0) root         (0)     7152 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/paraview/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/paraview/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.857560 trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/
--rw-r--r--   0 root         (0) root         (0)      363 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4655 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    23952 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.857560 trame-vtk-2.4.2/trame_vtk/modules/vtk/
--rw-r--r--   0 root         (0) root         (0)     7047 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2624 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.861561 trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/
--rw-r--r--   0 root         (0) root         (0)      322 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     3981 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    12797 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.865561 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/
--rw-r--r--   0 root         (0) root         (0)      661 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11702 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/actors.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/data.py
--rw-r--r--   0 root         (0) root         (0)     5785 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1354 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/lights.py
--rw-r--r--   0 root         (0) root         (0)     5724 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/lookup_tables.py
--rw-r--r--   0 root         (0) root         (0)     5093 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/mappers.py
--rw-r--r--   0 root         (0) root         (0)     6041 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/mesh.py
--rw-r--r--   0 root         (0) root         (0)     3272 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/properties.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/registry.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/render_windows.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/serialize.py
--rw-r--r--   0 root         (0) root         (0)     3541 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/synchronization_context.py
--rw-r--r--   0 root         (0) root         (0)     1337 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/textures.py
--rw-r--r--   0 root         (0) root         (0)     1946 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/utils.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/widgets.py
--rw-r--r--   0 root         (0) root         (0)     4551 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/modules/vtk/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.865561 trame-vtk-2.4.2/trame_vtk/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.865561 trame-vtk-2.4.2/trame_vtk/widgets/vtk/
--rw-r--r--   0 root         (0) root         (0)      645 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/widgets/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30817 2023-03-31 19:19:52.000000 trame-vtk-2.4.2/trame_vtk/widgets/vtk/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 19:19:58.853561 trame-vtk-2.4.2/trame_vtk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13038 2023-03-31 19:19:58.000000 trame-vtk-2.4.2/trame_vtk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2251 2023-03-31 19:19:58.000000 trame-vtk-2.4.2/trame_vtk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 19:19:58.000000 trame-vtk-2.4.2/trame_vtk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-31 19:19:58.000000 trame-vtk-2.4.2/trame_vtk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-31 19:19:58.000000 trame-vtk-2.4.2/trame_vtk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.016879 trame-vtk-2.4.3/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13038 2023-04-07 19:04:12.016879 trame-vtk-2.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)      878 2023-04-07 19:04:12.016879 trame-vtk-2.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/modules/paraview.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/modules/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/widgets/paraview.py
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame/widgets/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       91 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk/modules/common/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk/modules/common/serve/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/common/serve/.gitignore
+-rw-r--r--   0 root         (0) root         (0)  1626752 2023-04-07 19:04:08.000000 trame-vtk-2.4.3/trame_vtk/modules/common/serve/trame-vtk.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.008879 trame-vtk-2.4.3/trame_vtk/modules/paraview/
+-rw-r--r--   0 root         (0) root         (0)     7623 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.008879 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5356 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    23952 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.008879 trame-vtk-2.4.3/trame_vtk/modules/vtk/
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.012879 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.012879 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11702 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/actors.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/data.py
+-rw-r--r--   0 root         (0) root         (0)      796 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/export.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/lights.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/lookup_tables.py
+-rw-r--r--   0 root         (0) root         (0)     5093 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/mappers.py
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/properties.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/registry.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/render_windows.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     3541 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/synchronization_context.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/textures.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/widgets.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/modules/vtk/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.012879 trame-vtk-2.4.3/trame_vtk/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.012879 trame-vtk-2.4.3/trame_vtk/widgets/vtk/
+-rw-r--r--   0 root         (0) root         (0)      645 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/widgets/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32816 2023-04-07 19:04:07.000000 trame-vtk-2.4.3/trame_vtk/widgets/vtk/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:04:12.004878 trame-vtk-2.4.3/trame_vtk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13038 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2295 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-07 19:04:11.000000 trame-vtk-2.4.3/trame_vtk.egg-info/top_level.txt
```

### Comparing `trame-vtk-2.4.2/LICENSE` & `trame-vtk-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/PKG-INFO` & `trame-vtk-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.4.2
+Version: 2.4.3
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.4.2/README.rst` & `trame-vtk-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/setup.cfg` & `trame-vtk-2.4.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-vtk
-version = 2.4.2
+version = 2.4.3
 description = VTK widgets for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-vtk-2.4.2/trame_vtk/LICENSE` & `trame-vtk-2.4.3/trame_vtk/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/common/serve/trame-vtk.js` & `trame-vtk-2.4.3/trame_vtk/modules/common/serve/trame-vtk.js`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/paraview/__init__.py` & `trame-vtk-2.4.3/trame_vtk/modules/paraview/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,22 @@
             "viewport.geometry.view.get.state",
             self.id(view_proxy),
             new_state,
             widgets=widgets,
             orientation_axis=orientation_axis,
         )
 
+    def export(self, render_window, widgets=None, orientation_axis=0, **kwargs):
+        return self._trame_server.protocol_call(
+            "viewport.geometry.view.get.export",
+            self.id(render_window),
+            widgets=widgets,
+            orientation_axis=orientation_axis,
+        )
+
     def push_image(self, view_proxy, reset_camera=False):
         if view_proxy.EnableRenderOnInteraction:
             view_proxy.EnableRenderOnInteraction = 0
 
         if reset_camera:
             self._trame_server.protocol_call(
                 "viewport.camera.reset", self.id(view_proxy)
@@ -211,14 +219,20 @@
 def scene(render_window, reset_camera=False, new_state=True):
     scene_state = HELPER.scene(render_window, new_state)
     if reset_camera:
         scene_state.setdefault("extra", {})["resetCamera"] = 1
     return scene_state
 
 
+def export(render_window, widgets=None, orientation_axis=0):
+    return HELPER.export(
+        render_window, widgets=widgets, orientation_axis=orientation_axis
+    )
+
+
 def push_image(render_window, reset_camera=False):
     return HELPER.push_image(render_window, reset_camera)
 
 
 def camera(render_window):
     return HELPER.camera(render_window)
```

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/paraview/core.py` & `trame-vtk-2.4.3/trame_vtk/modules/paraview/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/local_rendering.py` & `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/local_rendering.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from wslink import register as export_rpc
 
 from trame_vtk.modules.vtk.serializers import (
     reference_id,
     initialize_serializers,
     serialize,
     serialize_widget,
+    extract_array_hash,
     SynchronizationContext,
 )
 
 from .web_protocol import ParaViewWebProtocol
 
 
 class ParaViewWebLocalRendering(ParaViewWebProtocol):
@@ -125,7 +126,25 @@
         self.context.set_ignore_last_dependencies(False)
         self.context.check_for_arrays_to_release()
 
         if view_instance:
             return view_instance
 
         return None
+
+    @export_rpc("viewport.geometry.view.get.export")
+    def get_standalone_state(self, view_id, widgets=None, orientation_axis=0, **kwargs):
+        scene_description = self.get_view_state(
+            view_id,
+            new_subscription=True,
+            widgets=widgets,
+            orientation_axis=orientation_axis,
+            **kwargs,
+        )
+        hashes = {}
+        for entry in extract_array_hash(scene_description):
+            data_hash = entry.get("hash")
+            hashes[data_hash] = dict(
+                **entry, content=self.context.get_cached_data_array(data_hash, False)
+            )
+
+        return dict(hashes=hashes, scene=scene_description)
```

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/mouse_handler.py` & `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/publish_image_delivery.py` & `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/view_port.py` & `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/paraview/protocols/web_protocol.py` & `trame-vtk-2.4.3/trame_vtk/modules/paraview/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/__init__.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,14 +70,22 @@
             "viewport.geometry.view.get.state",
             self.id(render_window),
             new_state,
             widgets=widgets,
             orientation_axis=orientation_axis,
         )
 
+    def export(self, render_window, widgets=None, orientation_axis=0, **kwargs):
+        return self._trame_server.protocol_call(
+            "viewport.geometry.view.get.export",
+            self.id(render_window),
+            widgets=widgets,
+            orientation_axis=orientation_axis,
+        )
+
     def push_image(self, render_window, reset_camera=False):
         # Disable any double render...
         render_window.GetInteractor().EnableRenderOff()
 
         if reset_camera:
             self._trame_server.protocol_call(
                 "viewport.camera.reset", self.id(render_window)
@@ -214,14 +222,20 @@
         render_window, new_state, widgets=widgets, orientation_axis=orientation_axis
     )
     if reset_camera:
         scene_state.setdefault("extra", {})["resetCamera"] = 1
     return scene_state
 
 
+def export(render_window, widgets=None, orientation_axis=0):
+    return HELPER.export(
+        render_window, widgets=widgets, orientation_axis=orientation_axis
+    )
+
+
 def push_image(render_window, reset_camera=False):
     return HELPER.push_image(render_window, reset_camera)
 
 
 def camera(render_window):
     return HELPER.camera(render_window)
```

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/core.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/local_rendering.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/local_rendering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from wslink import register as export_rpc
 
 from ..serializers import (
     reference_id,
     initialize_serializers,
     serialize,
     serialize_widget,
+    extract_array_hash,
     SynchronizationContext,
 )
 from .web_protocol import vtkWebProtocol
 
 
 class vtkWebLocalRendering(vtkWebProtocol):
     """Improved geometry delivery for client-side rendering
@@ -130,7 +131,25 @@
         self.context.set_ignore_last_dependencies(False)
         self.context.check_for_arrays_to_release()
 
         if view_instance:
             return view_instance
 
         return None
+
+    @export_rpc("viewport.geometry.view.get.export")
+    def get_standalone_state(self, view_id, widgets=None, orientation_axis=0, **kwargs):
+        scene_description = self.get_view_state(
+            view_id,
+            new_subscription=True,
+            widgets=widgets,
+            orientation_axis=orientation_axis,
+            **kwargs,
+        )
+        hashes = {}
+        for entry in extract_array_hash(scene_description):
+            data_hash = entry.get("hash")
+            hashes[data_hash] = dict(
+                **entry, content=self.context.get_cached_data_array(data_hash, False)
+            )
+
+        return dict(hashes=hashes, scene=scene_description)
```

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/mouse_handler.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/publish_image_delivery.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/view_port.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/protocols/web_protocol.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/__init__.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 
 from .mesh import mesh
 from .initialize import initialize_serializers
 from .serialize import serialize, serialize_widget
+from .export import extract_array_hash
 from .synchronization_context import SynchronizationContext
 from .utils import reference_id
 
 logger = logging.getLogger(__name__)
 # By default, only show critical messages for serializers
 logger.setLevel(logging.CRITICAL)
 
@@ -18,8 +19,9 @@
 __all__ = [
     "reference_id",
     "initialize_serializers",
     "mesh",
     "serialize",
     "SynchronizationContext",
     "serialize_widget",
+    "extract_array_hash",
 ]
```

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/actors.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/actors.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/data.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/data.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/helpers.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/helpers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/initialize.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/initialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/lights.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/lights.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/lookup_tables.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/mappers.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/mappers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/mesh.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/mesh.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/properties.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/properties.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/render_windows.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/render_windows.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/serialize.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/serialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 
 from .registry import class_name, SERIALIZERS
 from .widgets import handle_widget
 
+__all__ = ["serialize", "serialize_widget"]
+
 logger = logging.getLogger(__name__)
 
 # Keep track of which warnings have been printed
 NO_SERIALIZER_FOR_INSTANCE = {}
 
 
 def serialize(parent, instance, instance_id, context, depth):
```

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/synchronization_context.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/synchronization_context.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/textures.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/textures.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/utils.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/serializers/widgets.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/serializers/widgets.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/modules/vtk/widget.py` & `trame-vtk-2.4.3/trame_vtk/modules/vtk/widget.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/widgets/vtk/__init__.py` & `trame-vtk-2.4.3/trame_vtk/widgets/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.4.2/trame_vtk/widgets/vtk/common.py` & `trame-vtk-2.4.3/trame_vtk/widgets/vtk/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,22 @@
+import io
+import json
+import zipfile
+
 from trame_client.widgets.core import AbstractElement
+
 from trame_vtk.modules import common
 
+try:
+    import zlib  # noqa
+
+    ZIP_COMPRESSION = zipfile.ZIP_DEFLATED
+except ImportError:
+    ZIP_COMPRESSION = zipfile.ZIP_STORED
+
 MODULE = None
 
 
 def use_module(m):
     global MODULE
     MODULE = m
 
@@ -484,14 +496,42 @@
             self.__view,
             new_state=True,
             widgets=widgets,
             orientation_axis=orientation_axis,
         )
         self.server.state[self.__scene_id] = full_state
 
+    def export_geometry(self, widgets=None, orientation_axis=0, format="zip", **kwargs):
+        """Export standalone scene for OfflineViewer
+
+        :param format: Can be either be "zip" or "json".
+        """
+        encoded_data = None
+
+        if widgets is None:
+            widgets = self._widgets
+
+        if self.server.protocol:
+            encoded_data = MODULE.export(
+                self.__view,
+                widgets=widgets,
+                orientation_axis=orientation_axis,
+            )
+
+        if encoded_data:
+            json_out = json.dumps(encoded_data)
+            if format == "json":
+                return json_out.encode(encoding="UTF-8", errors="strict")
+
+            zip_buffer = io.BytesIO()
+            with zipfile.ZipFile(zip_buffer, "a") as zfile:
+                zfile.writestr("index.json", json_out, compress_type=ZIP_COMPRESSION)
+
+            return zip_buffer.getvalue()
+
     def update_image(self, reset_camera=False):
         """
         Force update to image
         """
         MODULE.push_image(self.__view, reset_camera)
 
     def set_local_rendering(self, local=True, **kwargs):
@@ -833,14 +873,42 @@
             self.__view,
             new_state=True,
             widgets=widgets,
             orientation_axis=orientation_axis,
         )
         self.server.state[self.__scene_id] = full_state
 
+    def export(self, widgets=None, orientation_axis=0, format="zip", **kwargs):
+        """Export standalone scene for OfflineViewer
+
+        :param format: Can be either be "zip" or "json".
+        """
+        encoded_data = None
+
+        if widgets is None:
+            widgets = self._widgets
+
+        if self.server.protocol:
+            encoded_data = MODULE.export(
+                self.__view,
+                widgets=widgets,
+                orientation_axis=orientation_axis,
+            )
+
+        if encoded_data:
+            json_out = json.dumps(encoded_data)
+            if format == "json":
+                return json_out.encode(encoding="UTF-8", errors="strict")
+
+            zip_buffer = io.BytesIO()
+            with zipfile.ZipFile(zip_buffer, "a") as zfile:
+                zfile.writestr("index.json", json_out, compress_type=ZIP_COMPRESSION)
+
+            return zip_buffer.getvalue()
+
     def reset_camera(self, **kwargs):
         """
         Move camera to center actors within the frame
         """
         self.server.js_call(ref=self.__ref, method="resetCamera")
 
     def replace_view(self, new_view, **kwargs):
```

### Comparing `trame-vtk-2.4.2/trame_vtk.egg-info/PKG-INFO` & `trame-vtk-2.4.3/trame_vtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.4.2
+Version: 2.4.3
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.4.2/trame_vtk.egg-info/SOURCES.txt` & `trame-vtk-2.4.3/trame_vtk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 trame_vtk/modules/vtk/protocols/mouse_handler.py
 trame_vtk/modules/vtk/protocols/publish_image_delivery.py
 trame_vtk/modules/vtk/protocols/view_port.py
 trame_vtk/modules/vtk/protocols/web_protocol.py
 trame_vtk/modules/vtk/serializers/__init__.py
 trame_vtk/modules/vtk/serializers/actors.py
 trame_vtk/modules/vtk/serializers/data.py
+trame_vtk/modules/vtk/serializers/export.py
 trame_vtk/modules/vtk/serializers/helpers.py
 trame_vtk/modules/vtk/serializers/initialize.py
 trame_vtk/modules/vtk/serializers/lights.py
 trame_vtk/modules/vtk/serializers/lookup_tables.py
 trame_vtk/modules/vtk/serializers/mappers.py
 trame_vtk/modules/vtk/serializers/mesh.py
 trame_vtk/modules/vtk/serializers/properties.py
```

