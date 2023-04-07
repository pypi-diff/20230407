# Comparing `tmp/ConGen-0.0.4.tar.gz` & `tmp/ConGen-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConGen-0.0.4.tar", last modified: Fri Apr  7 19:45:18 2023, max compression
+gzip compressed data, was "ConGen-0.0.5.tar", last modified: Fri Apr  7 19:55:40 2023, max compression
```

## Comparing `ConGen-0.0.4.tar` & `ConGen-0.0.5.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/
--rw-r--r--   0 lukas     (1000) lukas     (1000)    34462 2023-03-31 17:20:48.000000 ConGen-0.0.4/LICENSE
--rw-r--r--   0 lukas     (1000) lukas     (1000)    45962 2023-04-07 19:45:18.274589 ConGen-0.0.4/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5091 2023-03-31 18:42:02.000000 ConGen-0.0.4/README.md
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1501 2023-04-07 18:51:44.000000 ConGen-0.0.4/pyproject.toml
--rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-04-07 19:45:18.274589 ConGen-0.0.4/setup.cfg
--rw-r--r--   0 lukas     (1000) lukas     (1000)       36 2023-03-31 18:46:29.000000 ConGen-0.0.4/setup.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.264590 ConGen-0.0.4/src/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.267923 ConGen-0.0.4/src/ConGen.egg-info/
--rw-r--r--   0 lukas     (1000) lukas     (1000)    45962 2023-04-07 19:45:18.000000 ConGen-0.0.4/src/ConGen.egg-info/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     7798 2023-04-07 19:45:18.000000 ConGen-0.0.4/src/ConGen.egg-info/SOURCES.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-04-07 19:45:18.000000 ConGen-0.0.4/src/ConGen.egg-info/dependency_links.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       44 2023-04-07 19:45:18.000000 ConGen-0.0.4/src/ConGen.egg-info/entry_points.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       46 2023-04-07 19:45:18.000000 ConGen-0.0.4/src/ConGen.egg-info/requires.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       25 2023-04-07 19:45:18.000000 ConGen-0.0.4/src/ConGen.egg-info/top_level.txt
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.267923 ConGen-0.0.4/src/congen/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      135 2023-04-07 19:44:31.000000 ConGen-0.0.4/src/congen/__main__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.267923 ConGen-0.0.4/src/congen/exporters/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2753 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/exporters/CocoplanExporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/exporters/CustomJSONDecoder.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/exporters/CustomJSONEncoder.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1200 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/exporters/Exporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2235 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/exporters/GeoTIFFExporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      198 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/exporters/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.267923 ConGen-0.0.4/src/congen/importers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2812 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/importers/GeoTIFFImporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1360 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/importers/Importer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/importers/ImporterType.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      149 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/importers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.267923 ConGen-0.0.4/src/congen/layers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      670 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/DependentLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3870 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/Layer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/LayerType.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/LayerUsage.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3824 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/Parameter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1801 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.267923 ConGen-0.0.4/src/congen/layers/graphLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      240 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/graphLayers/FullGraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      235 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/graphLayers/GraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      825 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/graphLayers/RandomGraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/graphLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/congen/layers/pointLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      646 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/pointLayers/PointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/pointLayers/RasterPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      669 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/pointLayers/SimpleRandomPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3339 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/pointLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/congen/layers/pointLayers/clustered/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      713 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1574 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/pointLayers/clustered/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/congen/layers/rasterLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      939 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/rasterLayers/ImportedRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1709 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/rasterLayers/NoiseRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      291 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/rasterLayers/PerlinNoiseLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2191 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/rasterLayers/PointRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      996 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/rasterLayers/RasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      293 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/rasterLayers/SimplexNoiseLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/layers/rasterLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/congen/ui/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4017 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/ui/LayerListCtrl.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      172 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/ui/MainApp.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     6659 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/ui/MainCanvasPanel.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3646 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/ui/MainFrame.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/ui/ValueChoice.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.4/src/congen/ui/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/python-congen-git/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.264590 ConGen-0.0.4/src/python-congen-git/build/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.264590 ConGen-0.0.4/src/python-congen-git/build/lib/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/python-congen-git/build/lib/congen/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 18:29:49.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/__main__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2753 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/CocoplanExporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/CustomJSONDecoder.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/CustomJSONEncoder.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1200 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/Exporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2235 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/GeoTIFFExporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      198 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/python-congen-git/build/lib/congen/importers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2812 2023-04-07 17:21:19.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/importers/GeoTIFFImporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1360 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/importers/Importer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/importers/ImporterType.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      149 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/importers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      670 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/DependentLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3870 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/Layer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/LayerType.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/LayerUsage.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3824 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/Parameter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1801 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/graphLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      240 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/graphLayers/FullGraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      235 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/graphLayers/GraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      825 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/graphLayers/RandomGraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/graphLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      646 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/PointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/RasterPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      669 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/SimpleRandomPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3339 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/StratifiedRandomPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      713 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1574 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.271256 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      939 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/ImportedRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1709 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/NoiseRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      291 2023-04-07 17:21:19.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/PerlinNoiseLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2191 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/PointRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      996 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/RasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      293 2023-04-07 17:21:19.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/SimplexNoiseLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 17:21:19.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/main.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4017 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/LayerListCtrl.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      172 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/MainApp.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     6659 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/MainCanvasPanel.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3646 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/MainFrame.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/ValueChoice.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      858 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/gb_output.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     9351 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/parse_output.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       36 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/setup.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.267923 ConGen-0.0.4/src/python-congen-git/src/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/src/congen/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 18:29:49.000000 ConGen-0.0.4/src/python-congen-git/src/congen/__main__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/src/congen/exporters/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2753 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/exporters/CocoplanExporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/exporters/CustomJSONDecoder.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/exporters/CustomJSONEncoder.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1200 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/exporters/Exporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2235 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/exporters/GeoTIFFExporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      198 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/exporters/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/src/congen/importers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2812 2023-04-07 17:21:19.000000 ConGen-0.0.4/src/python-congen-git/src/congen/importers/GeoTIFFImporter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1360 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/importers/Importer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/importers/ImporterType.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      149 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/importers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/src/congen/layers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      670 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/DependentLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3870 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/Layer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/LayerType.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/LayerUsage.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3824 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/Parameter.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1801 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/src/congen/layers/graphLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      240 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/graphLayers/FullGraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      235 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/graphLayers/GraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      825 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/graphLayers/RandomGraphLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/graphLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      646 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/PointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/RasterPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      669 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/SimpleRandomPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3339 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/clustered/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      713 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1574 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/clustered/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      939 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/ImportedRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1709 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/NoiseRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      291 2023-04-07 17:21:19.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/PerlinNoiseLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2191 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/PointRasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      996 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/RasterLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      293 2023-04-07 17:21:19.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/SimplexNoiseLayer.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:45:18.274589 ConGen-0.0.4/src/python-congen-git/src/congen/ui/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4017 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/ui/LayerListCtrl.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      172 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/ui/MainApp.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     6659 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/ui/MainCanvasPanel.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3646 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/ui/MainFrame.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/ui/ValueChoice.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.4/src/python-congen-git/src/congen/ui/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    34462 2023-03-31 17:20:48.000000 ConGen-0.0.5/LICENSE
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    45962 2023-04-07 19:55:40.912153 ConGen-0.0.5/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5091 2023-03-31 18:42:02.000000 ConGen-0.0.5/README.md
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1501 2023-04-07 18:51:44.000000 ConGen-0.0.5/pyproject.toml
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-04-07 19:55:40.912153 ConGen-0.0.5/setup.cfg
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       36 2023-03-31 18:46:29.000000 ConGen-0.0.5/setup.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.902154 ConGen-0.0.5/src/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.905487 ConGen-0.0.5/src/ConGen.egg-info/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    45962 2023-04-07 19:55:40.000000 ConGen-0.0.5/src/ConGen.egg-info/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     7798 2023-04-07 19:55:40.000000 ConGen-0.0.5/src/ConGen.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-04-07 19:55:40.000000 ConGen-0.0.5/src/ConGen.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       44 2023-04-07 19:55:40.000000 ConGen-0.0.5/src/ConGen.egg-info/entry_points.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       46 2023-04-07 19:55:40.000000 ConGen-0.0.5/src/ConGen.egg-info/requires.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       25 2023-04-07 19:55:40.000000 ConGen-0.0.5/src/ConGen.egg-info/top_level.txt
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.905487 ConGen-0.0.5/src/congen/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      163 2023-04-07 19:54:18.000000 ConGen-0.0.5/src/congen/__main__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.905487 ConGen-0.0.5/src/congen/exporters/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2753 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/exporters/CocoplanExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/exporters/CustomJSONDecoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/exporters/CustomJSONEncoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1200 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/exporters/Exporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2235 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/exporters/GeoTIFFExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      198 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/exporters/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.905487 ConGen-0.0.5/src/congen/importers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2812 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/importers/GeoTIFFImporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1360 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/importers/Importer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/importers/ImporterType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      149 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/importers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.905487 ConGen-0.0.5/src/congen/layers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      670 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/DependentLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3870 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/Layer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/LayerType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/LayerUsage.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3824 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/Parameter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1801 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.905487 ConGen-0.0.5/src/congen/layers/graphLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      240 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/graphLayers/FullGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      235 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/graphLayers/GraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      825 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/graphLayers/RandomGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/graphLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/congen/layers/pointLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      646 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/pointLayers/PointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/pointLayers/RasterPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      669 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/pointLayers/SimpleRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3339 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/pointLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/congen/layers/pointLayers/clustered/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      713 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1574 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/pointLayers/clustered/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/congen/layers/rasterLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      939 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/rasterLayers/ImportedRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1709 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/rasterLayers/NoiseRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      291 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/rasterLayers/PerlinNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2191 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/rasterLayers/PointRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      996 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/rasterLayers/RasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      293 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/rasterLayers/SimplexNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/layers/rasterLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/congen/ui/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4017 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/ui/LayerListCtrl.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      172 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/ui/MainApp.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6659 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/ui/MainCanvasPanel.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3646 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/ui/MainFrame.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/ui/ValueChoice.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:12:20.000000 ConGen-0.0.5/src/congen/ui/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/python-congen-git/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.902154 ConGen-0.0.5/src/python-congen-git/build/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.902154 ConGen-0.0.5/src/python-congen-git/build/lib/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/python-congen-git/build/lib/congen/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 18:29:49.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/__main__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2753 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/CocoplanExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/CustomJSONDecoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/CustomJSONEncoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1200 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/Exporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2235 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/GeoTIFFExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      198 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/python-congen-git/build/lib/congen/importers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2812 2023-04-07 17:21:19.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/importers/GeoTIFFImporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1360 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/importers/Importer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/importers/ImporterType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      149 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/importers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      670 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/DependentLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3870 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/Layer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/LayerType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/LayerUsage.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3824 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/Parameter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1801 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/graphLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      240 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/graphLayers/FullGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      235 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/graphLayers/GraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      825 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/graphLayers/RandomGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/graphLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      646 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/PointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/RasterPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      669 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/SimpleRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3339 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/StratifiedRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      713 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1574 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.908820 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      939 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/ImportedRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1709 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/NoiseRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      291 2023-04-07 17:21:19.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/PerlinNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2191 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/PointRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      996 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/RasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      293 2023-04-07 17:21:19.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/SimplexNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 17:21:19.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/main.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4017 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/LayerListCtrl.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      172 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/MainApp.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6659 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/MainCanvasPanel.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3646 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/MainFrame.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/ValueChoice.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      858 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/gb_output.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     9351 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/parse_output.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       36 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/setup.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.905487 ConGen-0.0.5/src/python-congen-git/src/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/src/congen/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      129 2023-04-07 18:29:49.000000 ConGen-0.0.5/src/python-congen-git/src/congen/__main__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/src/congen/exporters/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2753 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/exporters/CocoplanExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      565 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/exporters/CustomJSONDecoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      585 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/exporters/CustomJSONEncoder.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1200 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/exporters/Exporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2235 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/exporters/GeoTIFFExporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      198 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/exporters/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/src/congen/importers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2812 2023-04-07 17:21:19.000000 ConGen-0.0.5/src/python-congen-git/src/congen/importers/GeoTIFFImporter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1360 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/importers/Importer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       78 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/importers/ImporterType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      149 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/importers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/src/congen/layers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      670 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/DependentLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3870 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/Layer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       99 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/LayerType.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      164 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/LayerUsage.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3824 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/Parameter.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1801 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/src/congen/layers/graphLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      240 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/graphLayers/FullGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      235 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/graphLayers/GraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      825 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/graphLayers/RandomGraphLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/graphLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      646 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/PointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1593 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/RasterPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      669 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/SimpleRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3339 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/clustered/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      713 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1574 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/clustered/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      939 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/ImportedRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1709 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/NoiseRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      291 2023-04-07 17:21:19.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/PerlinNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2191 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/PointRasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      996 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/RasterLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      293 2023-04-07 17:21:19.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/SimplexNoiseLayer.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-04-07 19:55:40.912153 ConGen-0.0.5/src/python-congen-git/src/congen/ui/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4017 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/ui/LayerListCtrl.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      172 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/ui/MainApp.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     6659 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/ui/MainCanvasPanel.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3646 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/ui/MainFrame.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      529 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/ui/ValueChoice.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        0 2023-04-07 17:21:06.000000 ConGen-0.0.5/src/python-congen-git/src/congen/ui/__init__.py
```

### Comparing `ConGen-0.0.4/LICENSE` & `ConGen-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/PKG-INFO` & `ConGen-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConGen
-Version: 0.0.4
+Version: 0.0.5
 Summary: Creating conservation planning datasets intuitively by playing with parameters and getting instant visualized feedback
 Author-email: Lukas Rose <public@lrose.de>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ConGen-0.0.4/README.md` & `ConGen-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/pyproject.toml` & `ConGen-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/ConGen.egg-info/PKG-INFO` & `ConGen-0.0.5/src/ConGen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConGen
-Version: 0.0.4
+Version: 0.0.5
 Summary: Creating conservation planning datasets intuitively by playing with parameters and getting instant visualized feedback
 Author-email: Lukas Rose <public@lrose.de>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ConGen-0.0.4/src/ConGen.egg-info/SOURCES.txt` & `ConGen-0.0.5/src/ConGen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/exporters/CocoplanExporter.py` & `ConGen-0.0.5/src/congen/exporters/CocoplanExporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/exporters/CustomJSONDecoder.py` & `ConGen-0.0.5/src/congen/exporters/CustomJSONDecoder.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/exporters/CustomJSONEncoder.py` & `ConGen-0.0.5/src/congen/exporters/CustomJSONEncoder.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/exporters/Exporter.py` & `ConGen-0.0.5/src/congen/exporters/Exporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/exporters/GeoTIFFExporter.py` & `ConGen-0.0.5/src/congen/exporters/GeoTIFFExporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/importers/GeoTIFFImporter.py` & `ConGen-0.0.5/src/congen/importers/GeoTIFFImporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/importers/Importer.py` & `ConGen-0.0.5/src/congen/importers/Importer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/DependentLayer.py` & `ConGen-0.0.5/src/congen/layers/DependentLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/Layer.py` & `ConGen-0.0.5/src/congen/layers/Layer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/Parameter.py` & `ConGen-0.0.5/src/congen/layers/Parameter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/__init__.py` & `ConGen-0.0.5/src/congen/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/graphLayers/RandomGraphLayer.py` & `ConGen-0.0.5/src/congen/layers/graphLayers/RandomGraphLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/pointLayers/PointLayer.py` & `ConGen-0.0.5/src/congen/layers/pointLayers/PointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/pointLayers/RasterPointLayer.py` & `ConGen-0.0.5/src/congen/layers/pointLayers/RasterPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/pointLayers/SimpleRandomPointLayer.py` & `ConGen-0.0.5/src/congen/layers/pointLayers/SimpleRandomPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py` & `ConGen-0.0.5/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py` & `ConGen-0.0.5/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py` & `ConGen-0.0.5/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/rasterLayers/ImportedRasterLayer.py` & `ConGen-0.0.5/src/congen/layers/rasterLayers/ImportedRasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/rasterLayers/NoiseRasterLayer.py` & `ConGen-0.0.5/src/congen/layers/rasterLayers/NoiseRasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/rasterLayers/PointRasterLayer.py` & `ConGen-0.0.5/src/congen/layers/rasterLayers/PointRasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/layers/rasterLayers/RasterLayer.py` & `ConGen-0.0.5/src/congen/layers/rasterLayers/RasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/ui/LayerListCtrl.py` & `ConGen-0.0.5/src/congen/ui/LayerListCtrl.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/ui/MainCanvasPanel.py` & `ConGen-0.0.5/src/congen/ui/MainCanvasPanel.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/ui/MainFrame.py` & `ConGen-0.0.5/src/congen/ui/MainFrame.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/congen/ui/ValueChoice.py` & `ConGen-0.0.5/src/congen/ui/ValueChoice.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/CocoplanExporter.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/CocoplanExporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/CustomJSONDecoder.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/CustomJSONDecoder.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/CustomJSONEncoder.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/CustomJSONEncoder.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/Exporter.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/Exporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/exporters/GeoTIFFExporter.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/exporters/GeoTIFFExporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/importers/GeoTIFFImporter.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/importers/GeoTIFFImporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/importers/Importer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/importers/Importer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/DependentLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/DependentLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/Layer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/Layer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/Parameter.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/Parameter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/__init__.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/graphLayers/RandomGraphLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/graphLayers/RandomGraphLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/PointLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/PointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/RasterPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/RasterPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/SimpleRandomPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/SimpleRandomPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/StratifiedRandomPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/StratifiedRandomPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/ImportedRasterLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/ImportedRasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/NoiseRasterLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/NoiseRasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/PointRasterLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/PointRasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/layers/rasterLayers/RasterLayer.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/layers/rasterLayers/RasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/LayerListCtrl.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/LayerListCtrl.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/MainCanvasPanel.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/MainCanvasPanel.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/MainFrame.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/MainFrame.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/build/lib/congen/ui/ValueChoice.py` & `ConGen-0.0.5/src/python-congen-git/build/lib/congen/ui/ValueChoice.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/gb_output.py` & `ConGen-0.0.5/src/python-congen-git/gb_output.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/parse_output.py` & `ConGen-0.0.5/src/python-congen-git/parse_output.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/exporters/CocoplanExporter.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/exporters/CocoplanExporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/exporters/CustomJSONDecoder.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/exporters/CustomJSONDecoder.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/exporters/CustomJSONEncoder.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/exporters/CustomJSONEncoder.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/exporters/Exporter.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/exporters/Exporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/exporters/GeoTIFFExporter.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/exporters/GeoTIFFExporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/importers/GeoTIFFImporter.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/importers/GeoTIFFImporter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/importers/Importer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/importers/Importer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/DependentLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/DependentLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/Layer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/Layer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/Parameter.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/Parameter.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/__init__.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/graphLayers/RandomGraphLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/graphLayers/RandomGraphLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/PointLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/PointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/RasterPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/RasterPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/SimpleRandomPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/SimpleRandomPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/StratifiedRandomPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/clustered/KMeansClusteredPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/pointLayers/clustered/WardClusteredPointLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/ImportedRasterLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/ImportedRasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/NoiseRasterLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/NoiseRasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/PointRasterLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/PointRasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/layers/rasterLayers/RasterLayer.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/layers/rasterLayers/RasterLayer.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/ui/LayerListCtrl.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/ui/LayerListCtrl.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/ui/MainCanvasPanel.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/ui/MainCanvasPanel.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/ui/MainFrame.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/ui/MainFrame.py`

 * *Files identical despite different names*

### Comparing `ConGen-0.0.4/src/python-congen-git/src/congen/ui/ValueChoice.py` & `ConGen-0.0.5/src/python-congen-git/src/congen/ui/ValueChoice.py`

 * *Files identical despite different names*

