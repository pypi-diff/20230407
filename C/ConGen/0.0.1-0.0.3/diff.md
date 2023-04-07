# Comparing `tmp/ConGen-0.0.1.tar.gz` & `tmp/ConGen-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConGen-0.0.1.tar", last modified: Fri Mar 31 18:25:51 2023, max compression
+gzip compressed data, was "ConGen-0.0.3.tar", last modified: Fri Apr  7 18:55:04 2023, max compression
```

## Comparing `ConGen-0.0.1.tar` & `ConGen-0.0.3.tar`

### file list

```diff
@@ -1,66 +1,179 @@
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/
--rw-r--r--   0 lukas     (1000) lukas     (1000)    34462 2023-03-31 17:20:48.000000 ConGen-0.0.1/LICENSE
--rw-r--r--   0 lukas     (1000) lukas     (1000)    45726 2023-03-31 18:25:51.180529 ConGen-0.0.1/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4855 2023-03-31 18:06:58.000000 ConGen-0.0.1/README.md
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1357 2023-03-31 18:25:39.000000 ConGen-0.0.1/pyproject.toml
--rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-03-31 18:25:51.180529 ConGen-0.0.1/setup.cfg
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.177196 ConGen-0.0.1/src/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/ConGen.egg-info/
--rw-r--r--   0 lukas     (1000) lukas     (1000)    45726 2023-03-31 18:25:51.000000 ConGen-0.0.1/src/ConGen.egg-info/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1984 2023-03-31 18:25:51.000000 ConGen-0.0.1/src/ConGen.egg-info/SOURCES.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-03-31 18:25:51.000000 ConGen-0.0.1/src/ConGen.egg-info/dependency_links.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       44 2023-03-31 18:25:51.000000 ConGen-0.0.1/src/ConGen.egg-info/entry_points.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       36 2023-03-31 18:25:51.000000 ConGen-0.0.1/src/ConGen.egg-info/requires.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2023-03-31 18:25:51.000000 ConGen-0.0.1/src/ConGen.egg-info/top_level.txt
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/congen/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2022-12-16 23:20:51.000000 ConGen-0.0.1/src/congen/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/congen/exporters/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2760 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/exporters/CocoplanExporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-03-31 13:07:50.000000 ConGen-0.0.1/src/congen/exporters/CustomJSONDecoder.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-03-31 13:07:50.000000 ConGen-0.0.1/src/congen/exporters/CustomJSONEncoder.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1221 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/exporters/Exporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2242 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/exporters/GeoTIFFExporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      212 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/exporters/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/congen/importers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2814 2023-03-31 18:16:50.000000 ConGen-0.0.1/src/congen/importers/GeoTIFFImporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1365 2023-03-31 18:16:50.000000 ConGen-0.0.1/src/congen/importers/Importer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-03-31 13:08:31.000000 ConGen-0.0.1/src/congen/importers/ImporterType.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      130 2023-03-31 18:16:50.000000 ConGen-0.0.1/src/congen/importers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/congen/layers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      684 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/DependentLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3884 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/Layer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-03-28 19:02:40.000000 ConGen-0.0.1/src/congen/layers/LayerType.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-03-28 19:02:40.000000 ConGen-0.0.1/src/congen/layers/LayerUsage.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3839 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/Parameter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1912 2023-03-31 18:16:50.000000 ConGen-0.0.1/src/congen/layers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/congen/layers/graphLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      247 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/graphLayers/FullGraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      242 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/graphLayers/GraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      812 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/graphLayers/RandomGraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-03-31 13:15:36.000000 ConGen-0.0.1/src/congen/layers/graphLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/congen/layers/pointLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      660 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/pointLayers/PointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1614 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/pointLayers/RasterPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      683 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/pointLayers/SimpleRandomPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3353 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-03-31 13:14:41.000000 ConGen-0.0.1/src/congen/layers/pointLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/congen/layers/pointLayers/clustered/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      734 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1595 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-03-31 13:16:28.000000 ConGen-0.0.1/src/congen/layers/pointLayers/clustered/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/congen/layers/rasterLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      953 2023-03-31 18:16:50.000000 ConGen-0.0.1/src/congen/layers/rasterLayers/ImportedRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1723 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/rasterLayers/NoiseRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      302 2023-03-31 18:16:50.000000 ConGen-0.0.1/src/congen/layers/rasterLayers/PerlinNoiseLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2205 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/rasterLayers/PointRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1017 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/layers/rasterLayers/RasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      304 2023-03-31 18:16:50.000000 ConGen-0.0.1/src/congen/layers/rasterLayers/SimplexNoiseLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-03-31 13:14:28.000000 ConGen-0.0.1/src/congen/layers/rasterLayers/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      136 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/main.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-03-31 18:25:51.180529 ConGen-0.0.1/src/congen/ui/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4031 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/ui/LayerListCtrl.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      179 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/ui/MainApp.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     6701 2023-03-31 16:49:40.000000 ConGen-0.0.1/src/congen/ui/MainCanvasPanel.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3668 2023-03-31 18:16:50.000000 ConGen-0.0.1/src/congen/ui/MainFrame.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-03-31 13:00:28.000000 ConGen-0.0.1/src/congen/ui/ValueChoice.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-03-31 13:00:44.000000 ConGen-0.0.1/src/congen/ui/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    34462 2023-03-31 17:20:48.000000 ConGen-0.0.3/LICENSE
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    45962 2023-04-07 18:55:04.403020 ConGen-0.0.3/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5091 2023-03-31 18:42:02.000000 ConGen-0.0.3/README.md
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1501 2023-04-07 18:51:44.000000 ConGen-0.0.3/pyproject.toml
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-04-07 18:55:04.403020 ConGen-0.0.3/setup.cfg
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       36 2023-03-31 18:46:29.000000 ConGen-0.0.3/setup.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.396353 ConGen-0.0.3/src/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/ConGen.egg-info/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    45962 2023-04-07 18:55:04.000000 ConGen-0.0.3/src/ConGen.egg-info/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     7798 2023-04-07 18:55:04.000000 ConGen-0.0.3/src/ConGen.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-04-07 18:55:04.000000 ConGen-0.0.3/src/ConGen.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       44 2023-04-07 18:55:04.000000 ConGen-0.0.3/src/ConGen.egg-info/entry_points.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       46 2023-04-07 18:55:04.000000 ConGen-0.0.3/src/ConGen.egg-info/requires.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       25 2023-04-07 18:55:04.000000 ConGen-0.0.3/src/ConGen.egg-info/top_level.txt
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/congen/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 17:24:35.000000 ConGen-0.0.3/src/congen/__main__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/congen/exporters/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2753 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/exporters/CocoplanExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/exporters/CustomJSONDecoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/exporters/CustomJSONEncoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1200 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/exporters/Exporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2235 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/exporters/GeoTIFFExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      198 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/exporters/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/congen/importers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2812 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/importers/GeoTIFFImporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1360 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/importers/Importer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/importers/ImporterType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      149 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/importers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/congen/layers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      670 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/DependentLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3870 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/Layer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/LayerType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/LayerUsage.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3824 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/Parameter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1801 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/congen/layers/graphLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      240 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/graphLayers/FullGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      235 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/graphLayers/GraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      825 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/graphLayers/RandomGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/graphLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/congen/layers/pointLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      646 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/pointLayers/PointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/pointLayers/RasterPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      669 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/pointLayers/SimpleRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3339 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/pointLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/congen/layers/pointLayers/clustered/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      713 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1574 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/pointLayers/clustered/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/congen/layers/rasterLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      939 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/rasterLayers/ImportedRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1709 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/rasterLayers/NoiseRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      291 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/rasterLayers/PerlinNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2191 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/rasterLayers/PointRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      996 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/rasterLayers/RasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      293 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/rasterLayers/SimplexNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/layers/rasterLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/congen/ui/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4017 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/ui/LayerListCtrl.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      172 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/ui/MainApp.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6659 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/ui/MainCanvasPanel.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3646 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/ui/MainFrame.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/ui/ValueChoice.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.3/src/congen/ui/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/python-congen-git/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.396353 ConGen-0.0.3/src/python-congen-git/build/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.396353 ConGen-0.0.3/src/python-congen-git/build/lib/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/python-congen-git/build/lib/congen/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 18:29:49.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/__main__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/python-congen-git/build/lib/congen/exporters/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2753 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/exporters/CocoplanExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/exporters/CustomJSONDecoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/exporters/CustomJSONEncoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1200 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/exporters/Exporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2235 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/exporters/GeoTIFFExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      198 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/exporters/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/python-congen-git/build/lib/congen/importers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2812 2023-04-07 17:21:19.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/importers/GeoTIFFImporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1360 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/importers/Importer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/importers/ImporterType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      149 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/importers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      670 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/DependentLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3870 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/Layer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/LayerType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/LayerUsage.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3824 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/Parameter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1801 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/graphLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      240 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/graphLayers/FullGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      235 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/graphLayers/GraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      825 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/graphLayers/RandomGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/graphLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      646 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/PointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/RasterPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      669 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/SimpleRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3339 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/StratifiedRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.399686 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      713 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1574 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/rasterLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      939 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/rasterLayers/ImportedRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1709 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/rasterLayers/NoiseRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      291 2023-04-07 17:21:19.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/rasterLayers/PerlinNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2191 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/rasterLayers/PointRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      996 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/rasterLayers/RasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      293 2023-04-07 17:21:19.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/rasterLayers/SimplexNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/layers/rasterLayers/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 17:21:19.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/main.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/build/lib/congen/ui/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4017 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/ui/LayerListCtrl.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      172 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/ui/MainApp.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6659 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/ui/MainCanvasPanel.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3646 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/ui/MainFrame.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/ui/ValueChoice.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/build/lib/congen/ui/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      858 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/gb_output.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     9351 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/parse_output.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       36 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/setup.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.396353 ConGen-0.0.3/src/python-congen-git/src/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/src/congen/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 18:29:49.000000 ConGen-0.0.3/src/python-congen-git/src/congen/__main__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/src/congen/exporters/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2753 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/exporters/CocoplanExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/exporters/CustomJSONDecoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/exporters/CustomJSONEncoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1200 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/exporters/Exporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2235 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/exporters/GeoTIFFExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      198 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/exporters/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/src/congen/importers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2812 2023-04-07 17:21:19.000000 ConGen-0.0.3/src/python-congen-git/src/congen/importers/GeoTIFFImporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1360 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/importers/Importer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/importers/ImporterType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      149 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/importers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/src/congen/layers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      670 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/DependentLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3870 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/Layer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/LayerType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/LayerUsage.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3824 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/Parameter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1801 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/src/congen/layers/graphLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      240 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/graphLayers/FullGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      235 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/graphLayers/GraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      825 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/graphLayers/RandomGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/graphLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      646 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/PointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/RasterPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      669 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/SimpleRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3339 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/clustered/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      713 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1574 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/pointLayers/clustered/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/src/congen/layers/rasterLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      939 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/rasterLayers/ImportedRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1709 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/rasterLayers/NoiseRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      291 2023-04-07 17:21:19.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/rasterLayers/PerlinNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2191 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/rasterLayers/PointRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      996 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/rasterLayers/RasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      293 2023-04-07 17:21:19.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/rasterLayers/SimplexNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/layers/rasterLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 18:55:04.403020 ConGen-0.0.3/src/python-congen-git/src/congen/ui/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4017 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/ui/LayerListCtrl.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      172 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/ui/MainApp.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6659 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/ui/MainCanvasPanel.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3646 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/ui/MainFrame.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/ui/ValueChoice.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.3/src/python-congen-git/src/congen/ui/__init__.py
```

### Comparing `ConGen-0.0.1/LICENSE` & `ConGen-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.1/PKG-INFO` & `ConGen-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConGen
-Version: 0.0.1
+Version: 0.0.3
 Summary: Creating conservation planning datasets intuitively by playing with parameters and getting instant visualized feedback
 Author-email: Lukas Rose <public@lrose.de>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,14 +681,20 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ConGen: Creating conservation planning datasets intuitively by playing with parameters and getting instant visualized feedback
 
+## Requirements
+For python library requirements, see pyproject.toml. Additionally, the following system libraries and development headers are required:
+- basic build tools (gcc, make etc.)
+- 
+- gdal for building the Python GDAL module
+
 ## TODOs
 - [ ] Fix WardClusteredPointLayer
 - [ ] CLI Interface
 - [ ] Benchmark different conservation planning software
 - [ ] Improve UI / UX
   - [ ] Onboarding / Instructions
   - [ ] Project creation wizard with predefined templates?
```

### Comparing `ConGen-0.0.1/README.md` & `ConGen-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # ConGen: Creating conservation planning datasets intuitively by playing with parameters and getting instant visualized feedback
 
+## Requirements
+For python library requirements, see pyproject.toml. Additionally, the following system libraries and development headers are required:
+- basic build tools (gcc, make etc.)
+- 
+- gdal for building the Python GDAL module
+
 ## TODOs
 - [ ] Fix WardClusteredPointLayer
 - [ ] CLI Interface
 - [ ] Benchmark different conservation planning software
 - [ ] Improve UI / UX
   - [ ] Onboarding / Instructions
   - [ ] Project creation wizard with predefined templates?
```

### Comparing `ConGen-0.0.1/src/ConGen.egg-info/PKG-INFO` & `ConGen-0.0.3/src/ConGen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConGen
-Version: 0.0.1
+Version: 0.0.3
 Summary: Creating conservation planning datasets intuitively by playing with parameters and getting instant visualized feedback
 Author-email: Lukas Rose <public@lrose.de>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,14 +681,20 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ConGen: Creating conservation planning datasets intuitively by playing with parameters and getting instant visualized feedback
 
+## Requirements
+For python library requirements, see pyproject.toml. Additionally, the following system libraries and development headers are required:
+- basic build tools (gcc, make etc.)
+- 
+- gdal for building the Python GDAL module
+
 ## TODOs
 - [ ] Fix WardClusteredPointLayer
 - [ ] CLI Interface
 - [ ] Benchmark different conservation planning software
 - [ ] Improve UI / UX
   - [ ] Onboarding / Instructions
   - [ ] Project creation wizard with predefined templates?
```

### Comparing `ConGen-0.0.1/src/congen/exporters/CocoplanExporter.py` & `ConGen-0.0.3/src/congen/exporters/CocoplanExporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import csv
 import math
 import os
 
 import wx
 
-from congen.exporters.Exporter import Exporter
+from exporters.Exporter import Exporter
 
 
 class CocoplanExporter(Exporter):
     def export(self):
         self.export_pu()
 
     def export_pu(self):
```

### Comparing `ConGen-0.0.1/src/congen/exporters/CustomJSONDecoder.py` & `ConGen-0.0.3/src/congen/exporters/CustomJSONDecoder.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.1/src/congen/exporters/CustomJSONEncoder.py` & `ConGen-0.0.3/src/congen/exporters/CustomJSONEncoder.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.1/src/congen/exporters/Exporter.py` & `ConGen-0.0.3/src/congen/exporters/Exporter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import wx
 
-from congen.layers import GraphLayer
-from congen.layers.LayerUsage import LayerUsage
-from congen.layers.rasterLayers.RasterLayer import RasterLayer
+from layers import GraphLayer
+from layers.LayerUsage import LayerUsage
+from layers.rasterLayers.RasterLayer import RasterLayer
 
 
 class Exporter:
     def __init__(self, event: wx.CommandEvent):
         self.event = event
         self.get_layers()
```

### Comparing `ConGen-0.0.1/src/congen/exporters/GeoTIFFExporter.py` & `ConGen-0.0.3/src/congen/exporters/GeoTIFFExporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os, re, unicodedata
 
 import numpy as np
 
-from congen.exporters.Exporter import Exporter
+from exporters.Exporter import Exporter
 from osgeo import gdal, gdal_array
 
 
 class GeoTIFFExporter(Exporter):
     def export(self):
         self.export_raster_layers()
```

### Comparing `ConGen-0.0.1/src/congen/importers/GeoTIFFImporter.py` & `ConGen-0.0.3/src/congen/importers/GeoTIFFImporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import numpy as np
 import wx
 from osgeo import gdal
 
-from src.congen.importers import Importer
+from importers.Importer import Importer
 
 
 class GeoTIFFImporter(Importer):
     def __init__(self, event: wx.CommandEvent = None, wildcard="*.tif", layer=None):
         super().__init__(event, wildcard=wildcard, layer=layer)
 
     def import_file(self):
```

### Comparing `ConGen-0.0.1/src/congen/importers/Importer.py` & `ConGen-0.0.3/src/congen/importers/Importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
 
 import wx
 
-from src.congen.importers import ImporterType
+from importers.ImporterType import ImporterType
 
 
 class Importer(metaclass=ImporterType):
     def __init__(self, event: wx.CommandEvent = None, wildcard="*.*", layer = None):
         self.event = event
         self.layer = layer
 
         if self.layer is None:
             self.layer_list = self.event.GetEventObject().GetWindow().GetPanel().GetLayerList()
             file_dialog = wx.FileDialog(parent=event.GetEventObject().GetWindow(), message="",
                                         defaultDir="/home/lukas/Downloads", defaultFile="project.json",
                                         wildcard=wildcard, style=wx.FD_OPEN | wx.FD_FILE_MUST_EXIST | wx.FD_MULTIPLE)
 
             if file_dialog.ShowModal() == wx.ID_OK:
-                from congen.layers.rasterLayers.ImportedRasterLayer import ImportedRasterLayer
+                from layers.rasterLayers.ImportedRasterLayer import ImportedRasterLayer
                 self.paths = file_dialog.GetPaths()
 
                 for path in self.paths:
                     layer = ImportedRasterLayer(importer_type = self.__class__.__name__,
                                                 name=os.path.basename(path),
                                                 abs_file_path=os.path.abspath(path),
                                                 rel_file_path=os.path.relpath(path))
```

### Comparing `ConGen-0.0.1/src/congen/layers/DependentLayer.py` & `ConGen-0.0.3/src/congen/layers/DependentLayer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from congen.layers.Parameter import Parameter
-from congen.layers.Layer import Layer
+from layers.Parameter import Parameter
+from layers.Layer import Layer
 
 
 class DependentLayer(Layer):
     def __init__(self, **kwargs):
         super().__init__()
         self.parameters.append(Parameter(name="dependingLayer", desc="Layer this layer depends on",
                                          parameterType=Layer, min=None, max=None, default=None, invalidates_cache=True))
```

### Comparing `ConGen-0.0.1/src/congen/layers/Layer.py` & `ConGen-0.0.3/src/congen/layers/Layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
-from congen.layers.LayerUsage import LayerUsage
-from congen.layers.Parameter import ParameterDict, Parameter
+from layers.LayerUsage import LayerUsage
+from layers.Parameter import ParameterDict, Parameter
 
 
 class Layer:
     def __init__(self, enabled=True, **kwargs):
         if not hasattr(self, "parameters"):
             self.parameters = ParameterDict()
         if not hasattr(self, "dependentLayers"):
```

### Comparing `ConGen-0.0.1/src/congen/layers/Parameter.py` & `ConGen-0.0.3/src/congen/layers/Parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import sys
 
-import congen
-
 
 class TypeDefaults(dict):
     def __init__(self, default, min, max):
         super().__init__(default = default, min = min, max = max)
 
 
 class Parameter(dict):
```

### Comparing `ConGen-0.0.1/src/congen/layers/__init__.py` & `ConGen-0.0.3/src/congen/layers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from congen.layers.rasterLayers import SimplexNoiseLayer
-from congen.layers.graphLayers.FullGraphLayer import FullGraphLayer
-from congen.layers.graphLayers.GraphLayer import GraphLayer
-from congen.layers.pointLayers.clustered.KMeansClusteredPointLayer import KMeansClusteredPointLayer
-from src.congen.layers.graphLayers.RandomGraphLayer import RandomGraphLayer
-from congen.layers.rasterLayers.SimplexNoiseLayer import SimplexNoiseLayer
-from congen.layers.rasterLayers.PerlinNoiseLayer import PerlinNoiseLayer
-from congen.layers.rasterLayers.PointRasterLayer import PointRasterLayer
-from congen.layers.pointLayers.RasterPointLayer import RasterPointLayer
-from congen.layers.pointLayers.SimpleRandomPointLayer import SimpleRandomPointLayer
-from congen.layers.pointLayers.StratifiedRandomPointLayer import StratifiedRandomPointLayer
-from congen.layers.rasterLayers.ImportedRasterLayer import ImportedRasterLayer
+from layers.rasterLayers import SimplexNoiseLayer
+from layers.graphLayers.FullGraphLayer import FullGraphLayer
+from layers.graphLayers.GraphLayer import GraphLayer
+from layers.pointLayers.clustered.KMeansClusteredPointLayer import KMeansClusteredPointLayer
+from layers.graphLayers.RandomGraphLayer import RandomGraphLayer
+import layers.rasterLayers.SimplexNoiseLayer
+from layers.rasterLayers.PerlinNoiseLayer import PerlinNoiseLayer
+from layers.rasterLayers.PointRasterLayer import PointRasterLayer
+from layers.pointLayers.RasterPointLayer import RasterPointLayer
+from layers.pointLayers.SimpleRandomPointLayer import SimpleRandomPointLayer
+from layers.pointLayers.StratifiedRandomPointLayer import StratifiedRandomPointLayer
+from layers.rasterLayers.ImportedRasterLayer import ImportedRasterLayer
 
 
 def create_multilayer_class(*superclasses):
     class MultilayerClass(*superclasses):
         def __init__(self, **kwargs):
             for superclass in superclasses:
                 superclass.__init__(self, **kwargs)
```

### Comparing `ConGen-0.0.1/src/congen/layers/graphLayers/RandomGraphLayer.py` & `ConGen-0.0.3/src/congen/layers/graphLayers/RandomGraphLayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from congen.layers.Parameter import Parameter
-from congen.layers import FullGraphLayer
+from layers.graphLayers.FullGraphLayer import FullGraphLayer
+from layers.Parameter import Parameter
 
 
 class RandomGraphLayer(FullGraphLayer):
     def __init__(self, **kwargs):
         super().__init__()
         self.parameters.extend([
             Parameter(name="edge_count", desc="Number of edges that are randomly drawn from the full graph",
```

### Comparing `ConGen-0.0.1/src/congen/layers/pointLayers/PointLayer.py` & `ConGen-0.0.3/src/congen/layers/pointLayers/PointLayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from matplotlib import colors as mcolors
 
-from congen.layers.LayerType import LayerType
-from congen.layers.Layer import Layer
+from layers.LayerType import LayerType
+from layers.Layer import Layer
 
 
 class PointLayer(Layer):
     colors = list(mcolors.TABLEAU_COLORS.values())
     def __init__(self, points = None, layerType = LayerType.LAYER_TYPE_POINTS, color = None, **kwargs):
         if color is None:
             color = self.colors.pop(0)
```

### Comparing `ConGen-0.0.1/src/congen/layers/pointLayers/RasterPointLayer.py` & `ConGen-0.0.3/src/congen/layers/pointLayers/RasterPointLayer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from congen.layers.Parameter import Parameter
-from congen.layers.DependentLayer import DependentLayer
-from congen.layers.pointLayers.PointLayer import PointLayer
+from layers.Parameter import Parameter
+from layers.DependentLayer import DependentLayer
+from layers.pointLayers.PointLayer import PointLayer
 import numpy as np
 
 
 class RasterPointLayer(PointLayer, DependentLayer):
     def __init__(self, **kwargs):
         super().__init__()
         self.parameters.append(Parameter(name="lowerThreshold", desc="Place points in cells with at least this value",
```

### Comparing `ConGen-0.0.1/src/congen/layers/pointLayers/SimpleRandomPointLayer.py` & `ConGen-0.0.3/src/congen/layers/pointLayers/SimpleRandomPointLayer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from congen.layers.Parameter import Parameter
-from congen.layers.pointLayers.PointLayer import PointLayer
+from layers.Parameter import Parameter
+from layers.pointLayers.PointLayer import PointLayer
 
 
 class SimpleRandomPointLayer(PointLayer):
     def __init__(self, type = "Simple Random Points", **kwargs):
         super().__init__()
         self.parameters.append(Parameter(name = "nPoints", desc = "Number of points",
                                          parameterType=int, min=1, max=200, default=25, invalidates_cache=True))
```

### Comparing `ConGen-0.0.1/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py` & `ConGen-0.0.3/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
-from congen.layers.Parameter import Parameter
-from congen.layers.pointLayers.PointLayer import PointLayer
+from layers.Parameter import Parameter
+from layers.pointLayers.PointLayer import PointLayer
 
 
 class StratifiedRandomPointLayer(PointLayer):
     def __init__(self, type="Stratified Random Points", **kwargs):
         super().__init__()
         self.parameters.append(Parameter(name="xCells", desc="Number of horizontal cells",
                                          parameterType=int, min=1, max=50, default=10, invalidates_cache=True))
```

### Comparing `ConGen-0.0.1/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py` & `ConGen-0.0.3/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from congen.layers.Parameter import Parameter
-from congen.layers.DependentLayer import DependentLayer
-from congen.layers.pointLayers.PointLayer import PointLayer
+from layers.Parameter import Parameter
+from layers.DependentLayer import DependentLayer
+from layers.pointLayers.PointLayer import PointLayer
 from sklearn.cluster import AgglomerativeClustering
 import numpy as np
 
 
 
 """
 TODO: Fix this class
```

### Comparing `ConGen-0.0.1/src/congen/layers/rasterLayers/ImportedRasterLayer.py` & `ConGen-0.0.3/src/congen/layers/rasterLayers/ImportedRasterLayer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os.path
 
-from congen.layers.Parameter import Parameter
-from congen.layers.rasterLayers.RasterLayer import RasterLayer
+from layers.Parameter import Parameter
+from layers.rasterLayers.RasterLayer import RasterLayer
 
 
 class ImportedRasterLayer(RasterLayer):
     def __init__(self, **kwargs):
         super().__init__()
         self.parameters.extend([
             Parameter(name='importer_type', desc='Type of the imported data', parameterType=str),
```

### Comparing `ConGen-0.0.1/src/congen/layers/rasterLayers/NoiseRasterLayer.py` & `ConGen-0.0.3/src/congen/layers/rasterLayers/NoiseRasterLayer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import noise_randomized
 import numpy as np
 
-from congen.layers.Parameter import Parameter
-from congen.layers.rasterLayers.RasterLayer import RasterLayer
+from layers.Parameter import Parameter
+from layers.rasterLayers.RasterLayer import RasterLayer
 
 
 class NoiseRasterLayer(RasterLayer):
     def __init__(self, **kwargs):
         super().__init__()
         self.parameters.append(Parameter(name="frequency", desc="Frequency of the perlin noise layer",
                                          parameterType=int, min=1, max=100, default=1, invalidates_cache=True))
```

### Comparing `ConGen-0.0.1/src/congen/layers/rasterLayers/PointRasterLayer.py` & `ConGen-0.0.3/src/congen/layers/rasterLayers/PointRasterLayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from matplotlib.patches import FancyBboxPatch, BoxStyle
 
-from congen.layers.Parameter import Parameter
-from congen.layers.rasterLayers.RasterLayer import RasterLayer
+from layers.Parameter import Parameter
+from layers.rasterLayers.RasterLayer import RasterLayer
 
 
 class PointRasterLayer(RasterLayer):
     def __init__(self, **kwargs):
         super().__init__()
         self.parameters.append(Parameter(name="fullradius", desc="corner radius for the full box",
                                          parameterType=int, min=1, max=100, default=1, invalidates_cache=True))
```

### Comparing `ConGen-0.0.1/src/congen/layers/rasterLayers/RasterLayer.py` & `ConGen-0.0.3/src/congen/layers/rasterLayers/RasterLayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
-from congen.layers.LayerType import LayerType
-from congen.layers.Parameter import Parameter
-from congen.layers.Layer import Layer
+from layers.LayerType import LayerType
+from layers.Parameter import Parameter
+from layers.Layer import Layer
 
 
 class RasterLayer(Layer):
     def __init__(self, pixels = None, layerType = LayerType.LAYER_TYPE_RASTER, **kwargs):
         super().__init__()
         self.parameters.extend([
             Parameter(name="min_value", desc="Minimum value of each pixel",
```

### Comparing `ConGen-0.0.1/src/congen/ui/LayerListCtrl.py` & `ConGen-0.0.3/src/congen/ui/LayerListCtrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import wx
 from wx.lib import newevent
 
-import congen.layers
+import layers
 from collections import defaultdict
 
-from congen.layers.Parameter import ParameterDict
+from layers.Parameter import ParameterDict
 
 
 class LayerListCtrl(wx.ListCtrl):
     EventListUpdate, EVT_LIST_UPDATE = newevent.NewEvent()
     current_instance = None
 
     def __init__(self, *args, **kwargs):
```

### Comparing `ConGen-0.0.1/src/congen/ui/MainCanvasPanel.py` & `ConGen-0.0.3/src/congen/ui/MainCanvasPanel.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import numpy as np
 import wx
 from matplotlib.backends.backend_wx import NavigationToolbar2Wx as NavigationToolbar2Wx
 from matplotlib.backends.backend_wxagg import FigureCanvasWxAgg as FigureCanvas
 from matplotlib.figure import Figure
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
-import congen.layers
-from congen.ui.LayerListCtrl import LayerListCtrl
-from congen.ui.ValueChoice import ValueChoice
-from congen.layers.Layer import Layer
-from congen.layers.rasterLayers.RasterLayer import RasterLayer
+import layers
+from ui.LayerListCtrl import LayerListCtrl
+from ui.ValueChoice import ValueChoice
+from layers.Layer import Layer
+from layers.rasterLayers.RasterLayer import RasterLayer
 
 
 class MainCanvasPanel(wx.Panel):
     def __init__(self, parent):
         super().__init__(parent)
 
         self.figure = Figure()
@@ -37,15 +37,15 @@
         layer_sizer = wx.BoxSizer(wx.VERTICAL)
         self.layer_list = LayerListCtrl(self, style=wx.LC_REPORT)
 
         self.Bind(wx.EVT_LIST_ITEM_SELECTED, self.display_current_layer)
         self.layer_list.Bind(LayerListCtrl.EVT_LIST_UPDATE, self.render_noise)
 
         layer_button_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        layer_add_choice = wx.Choice(self, choices=["Add...", *congen.layers.layer_names.keys()])
+        layer_add_choice = wx.Choice(self, choices=["Add...", *layers.layer_names.keys()])
         layer_add_choice.Select(0)
         layer_rem_button = wx.Button(self, -1, label="Remove")
         layer_button_sizer.Add(layer_add_choice)
         layer_button_sizer.AddStretchSpacer()
         layer_button_sizer.Add(layer_rem_button)
         layer_sizer.Add(self.layer_list, 1, wx.EXPAND)
         layer_sizer.Add(layer_button_sizer)
```

### Comparing `ConGen-0.0.1/src/congen/ui/MainFrame.py` & `ConGen-0.0.3/src/congen/ui/MainFrame.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import jsonpickle, wx
 
-from congen import exporters
-from congen.layers import ImportedRasterLayer
-from congen.ui.MainCanvasPanel import MainCanvasPanel
+import exporters, importers
+from layers import ImportedRasterLayer
+from ui.MainCanvasPanel import MainCanvasPanel
 
 
 class MainFrame(wx.Frame):
     def __init__(self, title):
         super().__init__(parent=None, id=-1, title=title)
         self.panel = MainCanvasPanel(self)
 
@@ -26,15 +26,15 @@
         file_menu.Bind(wx.EVT_MENU, self.open_project, open_item)
 
         for exporter_name, exporter_class in exporters.exporter_names.items():
             exporter_item = wx.MenuItem(export_menu, wx.ID_CONVERT, exporter_name, f"Export data for {exporter_name}", wx.ITEM_NORMAL, None)
             export_menu.Append(exporter_item)
             export_menu.Bind(wx.EVT_MENU, exporter_class, exporter_item)
 
-        for importer_name, importer_class in congen.importers.importer_names.items():
+        for importer_name, importer_class in importers.importer_names.items():
             print(importer_name, ":", importer_class)
             importer_item = wx.MenuItem(import_menu, -1, importer_name, f"Import data from {importer_name}", wx.ITEM_NORMAL, None)
             import_menu.Append(importer_item)
             import_menu.Bind(wx.EVT_MENU, importer_class, importer_item)
 
         menubar.Append(file_menu, "&File")
         file_menu.Append(save_item)
```

### Comparing `ConGen-0.0.1/src/congen/ui/ValueChoice.py` & `ConGen-0.0.3/src/congen/ui/ValueChoice.py`

 * *Files identical despite different names*

