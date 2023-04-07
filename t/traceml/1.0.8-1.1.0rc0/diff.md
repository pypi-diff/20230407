# Comparing `tmp/traceml-1.0.8.tar.gz` & `tmp/traceml-1.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceml-1.0.8.tar", last modified: Wed Feb  1 12:29:44 2023, max compression
+gzip compressed data, was "traceml-1.1.0rc0.tar", last modified: Fri Apr  7 15:21:36 2023, max compression
```

## Comparing `traceml-1.0.8.tar` & `traceml-1.1.0rc0.tar`

### file list

```diff
@@ -1,92 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.910358 traceml-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-01 12:29:26.000000 traceml-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-01 12:29:44.914358 traceml-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-01 12:29:44.914358 traceml-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-02-01 12:29:26.000000 traceml-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.882357 traceml-1.0.8/traceml/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.890357 traceml-1.0.8/traceml/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/artifacts/kinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/artifacts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.890357 traceml-1.0.8/traceml/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/events/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.898357 traceml-1.0.8/traceml/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/fastai_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/ignite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/pytorch_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/scikit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/integrations/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.898357 traceml-1.0.8/traceml/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/logging/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/logging/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/logging/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/logging/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.902357 traceml-1.0.8/traceml/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/df_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.910358 traceml-1.0.8/traceml/processors/events_processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/events_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/events_processors/events_artifacts_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/events_processors/events_audio_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/events_processors/events_charts_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/events_processors/events_image_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/events_processors/events_metrics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/events_processors/events_models_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/events_processors/events_tables_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/events_processors/events_video_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/gpu_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/importance_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/logs_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/psutil_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/processors/units_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.910358 traceml-1.0.8/traceml/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/serialization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/serialization/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.910358 traceml-1.0.8/traceml/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)    26351 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60614 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/tracking/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.910358 traceml-1.0.8/traceml/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.910358 traceml-1.0.8/traceml/vendor/matplotlylib/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.910358 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/_py3k_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.910358 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/mpltools.py
--rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/matplotlylib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)   166500 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/vendor/pynvml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.910358 traceml-1.0.8/traceml/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-02-01 12:29:26.000000 traceml-1.0.8/traceml/visualization/run_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:29:44.886357 traceml-1.0.8/traceml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-01 12:29:44.000000 traceml-1.0.8/traceml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-02-01 12:29:44.000000 traceml-1.0.8/traceml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 12:29:44.000000 traceml-1.0.8/traceml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-01 12:29:44.000000 traceml-1.0.8/traceml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-01 12:29:44.000000 traceml-1.0.8/traceml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.206346 traceml-1.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-07 15:21:36.206346 traceml-1.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-07 15:21:36.206346 traceml-1.1.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.198346 traceml-1.1.0rc0/traceml/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.198346 traceml-1.1.0rc0/traceml/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/artifacts/kinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/artifacts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.198346 traceml-1.1.0rc0/traceml/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/events/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.198346 traceml-1.1.0rc0/traceml/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/fastai_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/ignite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/pytorch_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/scikit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/integrations/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/logging/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/logging/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/logging/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/logging/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/pkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/df_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/processors/events_processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/events_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/events_processors/events_artifacts_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/events_processors/events_audio_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/events_processors/events_charts_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/events_processors/events_image_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/events_processors/events_metrics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/events_processors/events_models_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/events_processors/events_tables_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/events_processors/events_video_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/gpu_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/importance_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/logs_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/psutil_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/processors/units_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/serialization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/serialization/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/summary/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61766 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/tracking/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/vendor/matplotlylib/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/_py3k_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/mpltools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/matplotlylib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166500 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/vendor/pynvml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.202345 traceml-1.1.0rc0/traceml/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-04-07 15:21:28.000000 traceml-1.1.0rc0/traceml/visualization/run_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:21:36.198346 traceml-1.1.0rc0/traceml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-07 15:21:36.000000 traceml-1.1.0rc0/traceml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-07 15:21:36.000000 traceml-1.1.0rc0/traceml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:21:36.000000 traceml-1.1.0rc0/traceml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-07 15:21:36.000000 traceml-1.1.0rc0/traceml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 15:21:36.000000 traceml-1.1.0rc0/traceml.egg-info/top_level.txt
```

### Comparing `traceml-1.0.8/PKG-INFO` & `traceml-1.1.0rc0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: traceml
-Version: 1.0.8
+Version: 1.1.0rc0
 Summary: Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon.
 Home-page: https://github.com/polyaxon/traceml
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
 Keywords: polyaxon,aws,s3,microsoft,azure,google cloud storage,gcs,deep-learning,machine-learning,data-science,neural-networks,artificial-intelligence,ai,reinforcement-learning,kubernetes,aws,microsoft,azure,google cloud,tensorFlow,pytorch,matplotlib,plotly,visualization,analytics
 Platform: any
-Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Typing :: Typed
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: polyaxon
 Provides-Extra: dev
 Provides-Extra: all
 
 UNKNOWN
```

### Comparing `traceml-1.0.8/setup.cfg` & `traceml-1.1.0rc0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 honor_noqa = True
 profile = black
 line_length = 88
 lines_between_sections = 1
 lines_between_types = 1
 order_by_type = true
 known_future_library = future,pies
-extra_standard_library = typing,mock,pytest,factory,faker,flaky,numpy,pandas,requests,websocket,jinja2,yaml,pytz
-known_third_party = rest_framework,scipy,sklearn,datadog,docker,corsheaders,celery,picklefield,sentry_sdk,ujson,marshmallow
-known_first_party = polyaxon_sdk,polyaxon_deploy,polyaxon,traceml
+extra_standard_library = typing,typing_extensions,mock,pytest,factory,faker,flaky,numpy,pandas,requests,websocket,jinja2,yaml,pytz
+known_third_party = rest_framework,scipy,sklearn,datadog,docker,corsheaders,celery,picklefield,sentry_sdk,ujson,pydantic,clipped
+known_first_party = polyaxon,traceml
 indent = '    '
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 known_django = django
 forced_separate = django.contrib,django.utils
@@ -30,14 +30,15 @@
 	processors_mark
 	logging_mark
 	serialization_mark
 	tracking_mark
 
 [mypy]
 python_version = 3.9
+namespace_packages = true
 ignore_missing_imports = True
 show_error_codes = True
 allow_redefinition = True
 exclude = (setup.py$)|(tests/)|(vendor/)
 
 [egg_info]
 tag_build =
```

### Comparing `traceml-1.0.8/setup.py` & `traceml-1.1.0rc0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -103,23 +103,33 @@
         "matplotlib",
         "plotly",
         "visualization",
         "analytics",
     ],
     install_requires=[],
     extras_require=extra,
-    python_requires=">=3.5",
+    python_requires=">=3.7",
     classifiers=[
-        "Programming Language :: Python",
+        "Intended Audience :: Information Technology",
+        "Intended Audience :: System Administrators",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Typing :: Typed",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Operating System :: OS Independent",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Science/Research",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     tests_require=["pytest"],
     cmdclass={"test": PyTest},
 )
```

### Comparing `traceml-1.0.8/traceml/__init__.py` & `traceml-1.1.0rc0/traceml/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/artifacts/__init__.py` & `traceml-1.1.0rc0/traceml/artifacts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from traceml.artifacts.kinds import V1ArtifactKind
-from traceml.artifacts.schemas import RunArtifactSchema, V1RunArtifact
+from traceml.artifacts.schemas import V1RunArtifact, V1RunArtifacts
```

### Comparing `traceml-1.0.8/traceml/events/__init__.py` & `traceml-1.1.0rc0/traceml/events/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,23 +17,14 @@
 from traceml.events.paths import (
     get_asset_path,
     get_event_assets_path,
     get_event_path,
     get_resource_path,
 )
 from traceml.events.schemas import (
-    EventArtifactSchema,
-    EventAudioSchema,
-    EventChartSchema,
-    EventDataframeSchema,
-    EventHistogramSchema,
-    EventImageSchema,
-    EventModelSchema,
-    EventSchema,
-    EventVideoSchema,
     LoggedEventListSpec,
     LoggedEventSpec,
     V1Event,
     V1EventArtifact,
     V1EventAudio,
     V1EventChart,
     V1EventChartKind,
```

### Comparing `traceml-1.0.8/traceml/exceptions.py` & `traceml-1.1.0rc0/traceml/exceptions.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/integrations/__init__.py` & `traceml-1.1.0rc0/traceml/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/integrations/fastai.py` & `traceml-1.1.0rc0/traceml/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/integrations/fastai_v1.py` & `traceml-1.1.0rc0/traceml/integrations/fastai_v1.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/integrations/hugging_face.py` & `traceml-1.1.0rc0/traceml/integrations/hugging_face.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/integrations/ignite.py` & `traceml-1.1.0rc0/traceml/integrations/ignite.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/integrations/keras.py` & `traceml-1.1.0rc0/traceml/integrations/keras.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import operator
 
-from typing import List
+from typing import List, Optional
+
+from clipped.np_utils import sanitize_np_types
 
 from polyaxon.client.decorators import client_handler
-from polyaxon.utils.np_utils import sanitize_np_types
 from traceml import tracking
 from traceml.exceptions import TracemlException
 from traceml.logger import logger
 
 try:
     from tensorflow import keras
 except ImportError:
@@ -33,15 +34,15 @@
 
 
 class Callback(keras.callbacks.Callback):
     @client_handler(check_no_op=True)
     def __init__(
         self,
         run=None,
-        metrics: List[str] = None,
+        metrics: Optional[List[str]] = None,
         log_model: bool = True,
         save_weights_only: bool = False,
         log_best_prefix="best",
         mode: str = "auto",
         monitor: str = "val_loss",
         use_store_path: bool = False,
     ):
```

### Comparing `traceml-1.0.8/traceml/integrations/lightgbm.py` & `traceml-1.1.0rc0/traceml/integrations/lightgbm.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/integrations/pytorch_lightning.py` & `traceml-1.1.0rc0/traceml/integrations/pytorch_lightning.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,29 +58,29 @@
 
 
 class Callback(Logger):
     LOGGER_JOIN_CHAR = "_"
 
     def __init__(
         self,
-        owner: str = None,
-        project: str = None,
-        run_uuid: str = None,
+        owner: Optional[str] = None,
+        project: Optional[str] = None,
+        run_uuid: Optional[str] = None,
         client: RunClient = None,
         track_code: bool = True,
         track_env: bool = True,
         refresh_data: bool = False,
-        artifacts_path: str = None,
-        collect_artifacts: str = None,
-        collect_resources: str = None,
-        is_offline: bool = None,
-        is_new: bool = None,
-        name: str = None,
-        description: str = None,
-        tags: List[str] = None,
+        artifacts_path: Optional[str] = None,
+        collect_artifacts: Optional[str] = None,
+        collect_resources: Optional[str] = None,
+        is_offline: Optional[bool] = None,
+        is_new: Optional[bool] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        tags: Optional[List[str]] = None,
         end_on_finalize: bool = False,
         prefix: str = "",
     ):
         super().__init__()
         self._owner = owner
         self._project = project
         self._run_uuid = run_uuid
@@ -122,44 +122,42 @@
             description=self._description,
             tags=self._tags,
         )
         self._experiment = tracking.TRACKING_RUN
         return self._experiment
 
     @rank_zero_only
-    def log_hyperparams(self, params: Union[Dict[str, Any], Namespace]) -> None:
+    def log_hyperparams(self, params: Union[Dict[str, Any], Namespace]):
         params = _convert_params(params)
         params = _flatten_dict(params)
         params = _sanitize_callable_params(params)
         self.experiment.log_inputs(**params)
 
     @rank_zero_only
-    def log_metrics(
-        self, metrics: Dict[str, float], step: Optional[int] = None
-    ) -> None:
+    def log_metrics(self, metrics: Dict[str, float], step: Optional[int] = None):
         assert rank_zero_only.rank == 0, "experiment tried to log from global_rank != 0"
         metrics = _add_prefix(metrics, self._prefix, self.LOGGER_JOIN_CHAR)
         self.experiment.log_metrics(**metrics, step=step)
 
     @rank_zero_only
-    def log_model_summary(
-        self, model: "pl.LightningModule", max_depth: int = -1
-    ) -> None:
+    def log_model_summary(self, model: "pl.LightningModule", max_depth: int = -1):
         summary = str(ModelSummary(model=model, max_depth=max_depth))
-        rel_path = self.run.get_outputs_path("model_summary.txt")
+        rel_path = self.experiment.get_outputs_path("model_summary.txt")
         with open(rel_path, "w") as f:
             f.write(summary)
-        self.run.log_file_ref(path=rel_path, name="model_summary", is_input=False)
+        self.experiment.log_file_ref(
+            path=rel_path, name="model_summary", is_input=False
+        )
 
     @property
     def save_dir(self) -> Optional[str]:
         return self.experiment.get_outputs_path()
 
     @rank_zero_only
-    def finalize(self, status: str) -> None:
+    def finalize(self, status: str):
         if self._end_on_finalize:
             self.experiment.end()
             self._experiment = None
 
     def _set_run_instance_from_env_vars(self, force: bool = False):
         """Tries to extract run info from canonical env vars"""
         run_instance = os.getenv(EV_KEYS_RUN_INSTANCE)
```

### Comparing `traceml-1.0.8/traceml/integrations/scikit.py` & `traceml-1.1.0rc0/traceml/integrations/scikit.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from polyaxon.utils.np_utils import sanitize_dict
+from clipped.np_utils import sanitize_dict
+
 from traceml import tracking
 from traceml.exceptions import TracemlException
 
 try:
     from sklearn.base import is_classifier, is_regressor
     from sklearn.metrics import (
         accuracy_score,
```

### Comparing `traceml-1.0.8/traceml/integrations/tensorboard.py` & `traceml-1.1.0rc0/traceml/integrations/tensorboard.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Optional
 
+from polyaxon.exceptions import PolyaxonClientException
 from traceml import tracking
 from traceml.exceptions import TracemlException
 from traceml.logger import logger
 
 summary_pb2 = None
 
 try:
@@ -49,15 +50,15 @@
 
 
 class Logger:
     @classmethod
     def process_summary(
         cls,
         summary: Any,
-        global_step: int = None,
+        global_step: Optional[int] = None,
         run: "Run" = None,
         log_image: bool = False,
         log_histo: bool = False,
         log_tensor: bool = False,
     ):
         run = tracking.get_or_create_run(run)
         if not run:
```

### Comparing `traceml-1.0.8/traceml/integrations/tensorflow.py` & `traceml-1.1.0rc0/traceml/integrations/tensorflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,17 @@
 from traceml.integrations.tensorboard import Logger
 
 try:
     import tensorflow as tf
 except ImportError:
     raise TracemlException("tensorflow is required to use the tracking Callback")
 
-SessionRunHook = None
-
 try:
     from tensorflow.train import SessionRunHook  # noqa
 except ImportError:
-    pass
-
-if not SessionRunHook:
     raise TracemlException("tensorflow is required to use the tracking Callback")
 
 
 if TYPE_CHECKING:
     from traceml.tracking import Run
```

### Comparing `traceml-1.0.8/traceml/integrations/xgboost.py` & `traceml-1.1.0rc0/traceml/integrations/xgboost.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 import ujson
 
 from traceml import tracking
 from traceml.exceptions import TracemlException
 from traceml.logger import logger
 
@@ -72,16 +72,16 @@
     else:  # train case
         _save(model, "model")
 
 
 def callback(
     log_model: bool = True,
     log_importance: bool = True,
-    max_num_features: int = None,
-    run: "Run" = None,
+    max_num_features: Optional[int] = None,
+    run: Optional["Run"] = None,
 ):
     run = tracking.get_or_create_run(run)
 
     def callback(env):
         # Log metrics after iteration
         metrics = {}
         for item in env.evaluation_result_list:
@@ -120,17 +120,16 @@
 class Callback(xgb.callback.TrainingCallback):
     def __init__(
         self,
         run: "Run" = None,
         log_model: bool = True,
         log_importance: bool = True,
         importance_type: str = "gain",
-        max_num_features: int = None,
+        max_num_features: Optional[int] = None,
     ):
-
         self.log_model: bool = log_model
         self.log_importance: bool = log_importance
         self.importance_type: str = importance_type
         self.max_num_features: int = max_num_features
         self.run = tracking.get_or_create_run(run)
 
     def after_training(self, model: Booster) -> Booster:
```

### Comparing `traceml-1.0.8/traceml/logger.py` & `traceml-1.1.0rc0/traceml/logger.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/logging/__init__.py` & `traceml-1.1.0rc0/traceml/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/logging/handler.py` & `traceml-1.1.0rc0/traceml/logging/handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os
 import socket
 
+from clipped.date_utils import to_datetime
+from clipped.env import get_user
+
 from polyaxon import settings
 from polyaxon.env_vars.keys import EV_KEYS_K8S_NODE_NAME, EV_KEYS_K8S_POD_ID
-from polyaxon.utils.date_utils import to_datetime
-from polyaxon.utils.env import get_user
-from traceml.logger import logger
 from traceml.logging import V1Log
 
 
-class PolyaxonHandler(logging.Handler):
+class LogStreamHandler(logging.Handler):
     def __init__(self, add_logs, **kwargs):
         self._add_logs = add_logs
         self._container = socket.gethostname()
         self._node = os.environ.get(EV_KEYS_K8S_NODE_NAME, "local")
         self._pod = os.environ.get(EV_KEYS_K8S_POD_ID, get_user())
         log_level = settings.CLIENT_CONFIG.log_level
         if log_level and isinstance(log_level, str):
@@ -41,30 +41,49 @@
 
     def set_add_logs(self, add_logs):
         self._add_logs = add_logs
 
     def can_record(self, record):
         return not (
             record.name == "polyaxon"
+            or record.name == "traceml"
             or record.name == "polyaxon.cli"
             or record.name.startswith("polyaxon")
+            or record.name.startswith("traceml")
         )
 
     def format_record(self, record):
         message = ""
         if record.msg:
-            message = record.msg % record.args
+            message = record.msg
+        if record.args:
+            message %= record.args
         return V1Log.process_log_line(
             value=message,
             timestamp=to_datetime(record.created),
             node=self._node,
             pod=self._pod,
             container=self._container,
         )
 
     def emit(self, record):  # pylint:disable=inconsistent-return-statements
         if not self.can_record(record):
             return
         try:
             return self._add_logs(self.format_record(record))
-        except Exception as e:
-            logger.warning("Polyaxon failed creating log record %e", e)
+        except Exception:  # noqa
+            pass
+
+
+class LogStreamWriter:
+    def __init__(self, logger, log_level, channel):
+        self._logger = logger
+        self._log_level = log_level
+        self._channel = channel
+
+    def write(self, buf):
+        for line in buf.rstrip().splitlines():
+            if line != "\n":
+                self._logger.log(self._log_level, line.rstrip())
+
+    def flush(self):
+        self._channel.flush()
```

### Comparing `traceml-1.0.8/traceml/logging/parser.py` & `traceml-1.1.0rc0/traceml/logging/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 
-from polyaxon.utils.date_utils import parse_datetime
+from clipped.date_utils import parse_datetime
 
 # pylint:disable=anomalous-backslash-in-string
 
 DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S %Z"  # noqa
 ISO_DATETIME_REGEX = re.compile(  # noqa
     r"([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]"
     r"([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)(\.[0-9]+)?"
```

### Comparing `traceml-1.0.8/traceml/logging/streamer.py` & `traceml-1.1.0rc0/traceml/logging/streamer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections import deque
 from typing import Callable
 
+from clipped.formatting import Printer
+from clipped.tz_utils import local_datetime
+
+from polyaxon import settings
 from polyaxon.containers.names import MAIN_JOB_CONTAINER
-from polyaxon.utils.formatting import Printer
-from polyaxon.utils.tz_utils import local_datetime
 from traceml.logging.schemas import V1Log, V1Logs
 
 
 def get_logs_streamer(
     show_timestamp: bool = True, all_containers: bool = False, all_info: bool = False
 ) -> Callable:
     colors = deque(Printer.COLORS)
@@ -31,15 +33,17 @@
     if all_info:
         all_containers = True
 
     def handle_log_line(log: V1Log):
         log_dict = log.to_dict()
         log_line = ""
         if log.timestamp and show_timestamp:
-            date_value = local_datetime(log_dict.get("timestamp"))
+            date_value = local_datetime(
+                log_dict.get("timestamp"), tz=settings.CLIENT_CONFIG.timezone
+            )
             log_line = Printer.add_log_color(date_value, "white") + " | "
 
         def get_container_info():
             if container_info in job_to_color:
                 color = job_to_color[container_info]
             else:
                 color = colors[0]
```

### Comparing `traceml-1.0.8/traceml/pkg.py` & `traceml-1.1.0rc0/traceml/pkg.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 NAME = "traceml"
-VERSION = "1.0.8"
+VERSION = "1.1.0-rc0"
 DESC = (
     "Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon."
 )
 URL = "https://github.com/polyaxon/traceml"
 AUTHOR = "Polyaxon, Inc."
 EMAIL = "contact@polyaxon.com"
 LICENSE = "Apache 2.0"
```

### Comparing `traceml-1.0.8/traceml/processors/__init__.py` & `traceml-1.1.0rc0/traceml/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/processors/df_processors.py` & `traceml-1.1.0rc0/traceml/processors/df_processors.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
+
+from clipped.enums_utils import PEnum
 
 from traceml.processors.errors import NUMPY_ERROR_MESSAGE, PANDAS_ERROR_MESSAGE
 from traceml.processors.units_processors import to_percentage
 
 try:
     import numpy as np
 except ImportError as e:
@@ -27,36 +29,40 @@
 try:
     import pandas as pd
 
     from pandas.api import types as pd_types
 except ImportError as e:
     raise ImportError(PANDAS_ERROR_MESSAGE) from e
 
-DF_TYPE_BOOL = "bool"
-DF_TYPE_NUMERIC = "numeric"
-DF_TYPE_DATE = "date"
-DF_TYPE_CATEGORICAL = "categorical"
-DF_TYPE_CONSTANT = "constant"
-DF_TYPE_UNIQUE = "unique"
-
-EXCLUDE = "exclude"
-INCLUDE = "include"
-RAISE = "raise"
-ALL = "all"
+
+class DFTypes(str, PEnum):
+    BOOL = "bool"
+    NUMERIC = "numeric"
+    DATE = "date"
+    CATEGORICAL = "categorical"
+    CONSTANT = "constant"
+    UNIQUE = "unique"
+
+
+class DFUsage(str, PEnum):
+    EXCLUDE = "exclude"
+    INCLUDE = "include"
+    RAISE = "raise"
+    ALL = "all"
 
 
 def df_has_column(df: pd.DataFrame, column: Union[int, str]):
     if not isinstance(column, (int, str)):
         raise ValueError("{} is not a valid column".format(column))
     return column in df.columns
 
 
 def get_df_columns(
     df: pd.DataFrame,
-    usage: Union[INCLUDE, EXCLUDE, ALL],
+    usage: DFUsage,
     columns: Union[pd.Index, List[str]] = None,
 ):
     """
     Returns a `pd.DataFrame.columns`.
 
     Args:
         df: dataframe to select columns from
@@ -71,67 +77,77 @@
     Returns:
         `pd.DataFrame` columns, excluding `target_column` and `id_column` if given.
         `pd.DataFrame` columns, including/excluding the `columns` depending on `usage`.
     """
     columns_excluded = pd.Index([])
     columns_included = df.columns
 
-    if usage == INCLUDE:
+    if usage == DFUsage.INCLUDE:
         try:
             columns_included = columns_included.intersection(pd.Index(columns))
         except TypeError:
             pass
-    elif usage == EXCLUDE:
+    elif usage == DFUsage.EXCLUDE:
         try:
             columns_excluded = columns_excluded.union(pd.Index(columns))
         except TypeError:
             pass
 
     columns_included = columns_included.difference(columns_excluded)
     return columns_included.intersection(df.columns)
 
 
 def get_df_uniques(df: pd.DataFrame):
     return pd.Series(dict((c, df[c].nunique()) for c in df.columns), name="uniques")
 
 
-def get_df_missing(df: pd.DataFrame, df_length: int = None, df_counts: int = None):
+def get_df_missing(
+    df: pd.DataFrame,
+    df_length: Optional[pd.DataFrame] = None,
+    df_counts: Optional[pd.DataFrame] = None,
+):
     if df_length is None:
         df_length = len(df)
     if df_counts is None:
         df_counts = df.count()
         df_counts.name = "counts"
     count = df_length - df_counts
     count.name = "missing"
     perc = (count / df_length).apply(to_percentage)
     perc.name = "missing_perc"
     return pd.concat([count, perc], axis=1, sort=True)
 
 
-def get_df_column_stats(df: pd.DataFrame, df_counts: int = None) -> pd.DataFrame:
+def get_df_column_stats(
+    df: pd.DataFrame, df_counts: Optional[pd.DataFrame] = None
+) -> pd.DataFrame:
     def get_df_columns_info():
         column_info = {}
-        column_info[DF_TYPE_CONSTANT] = stats["uniques"][stats["uniques"] == 1].index
-        column_info[DF_TYPE_BOOL] = stats["uniques"][stats["uniques"] == 2].index
+        column_info[DFTypes.CONSTANT] = stats["uniques"][stats["uniques"] == 1].index
+        column_info[DFTypes.BOOL] = stats["uniques"][stats["uniques"] == 2].index
         rest_columns = get_df_columns(
-            df, EXCLUDE, column_info["constant"].union(column_info["bool"])
+            df, DFUsage.EXCLUDE, column_info["constant"].union(column_info["bool"])
         )
-        column_info[DF_TYPE_NUMERIC] = pd.Index(
+        column_info[DFTypes.NUMERIC] = pd.Index(
             [c for c in rest_columns if pd_types.is_numeric_dtype(df[c])]
         )
-        rest_columns = get_df_columns(df[rest_columns], EXCLUDE, column_info["numeric"])
-        column_info[DF_TYPE_DATE] = pd.Index(
+        rest_columns = get_df_columns(
+            df[rest_columns], DFUsage.EXCLUDE, column_info["numeric"]
+        )
+        column_info[DFTypes.DATE] = pd.Index(
             [c for c in rest_columns if pd_types.is_datetime64_dtype(df[c])]
         )
-        rest_columns = get_df_columns(df[rest_columns], EXCLUDE, column_info["date"])
+        rest_columns = get_df_columns(
+            df[rest_columns], DFUsage.EXCLUDE, column_info["date"]
+        )
         unique_columns = stats["uniques"][rest_columns] == stats["counts"][rest_columns]
-        column_info[DF_TYPE_UNIQUE] = stats["uniques"][rest_columns][
+        column_info[DFTypes.UNIQUE] = stats["uniques"][rest_columns][
             unique_columns
         ].index
-        column_info[DF_TYPE_CATEGORICAL] = stats["uniques"][rest_columns][
+        column_info[DFTypes.CATEGORICAL] = stats["uniques"][rest_columns][
             ~unique_columns
         ].index
         return column_info
 
     if df_counts is None:
         df_counts = df.count()
         df_counts.name = "counts"
@@ -148,46 +164,58 @@
 
 
 def get_df_columns_types(columns_stats: pd.DataFrame):
     return pd.value_counts(columns_stats.loc["types"])
 
 
 def get_deviation_of_mean(
-    series: pd.Series, multiplier: int = 3, df_length: int = None
-) -> Tuple[int, float]:
+    series: pd.Series, multiplier: int = 3, df_length: Optional[pd.DataFrame] = None
+) -> Tuple[int, str]:
     """
     Returns count of values deviating of the mean, i.e. larger than `multiplier` * `std`.
     Args:
         series: Series to perform operation over.
         multiplier: The value to use as
+        df_length: Optional cached length of the dataframe.
     Returns:
         tuple
     """
     if df_length is None:
         df_length = len(series)
     capped_series = np.minimum(series, series.mean() + multiplier * series.std())
     count = pd.value_counts(series != capped_series)
     count = count[True] if True in count else 0
     return count, to_percentage(count / df_length)
 
 
+def mad(series) -> np.ndarray:
+    """Returns Median Absolute Deviation.
+    https://en.wikipedia.org/wiki/Median_absolute_deviation
+    Args:
+        Union[series, np.ndarray]: Series to perform operation over.
+    Returns:
+        float
+    """
+    return np.median(np.abs(series - np.median(series)))
+
+
 def get_median_absolute_deviation(
-    series, multiplier=3, df_length: int = None
+    series, multiplier=3, df_length: Optional[pd.DataFrame] = None
 ) -> Tuple[int, float]:
     """
     Returns count of values larger than `multiplier` * `mad`
     Args:
         series: Series to perform operation over.
         multiplier: The value to use as
     Returns:
         tuple
     """
     if df_length is None:
         df_length = len(series)
-    capped_series = np.minimum(series, series.median() + multiplier * series.mad())
+    capped_series = np.minimum(series, series.median() + multiplier * mad(series))
     count = pd.value_counts(series != capped_series)
     count = count[True] if True in count else 0
     return count, to_percentage(count / df_length)
 
 
 def get_top_correlations(
     df: pd.DataFrame, column: str, threshold: float = 0.65, top: int = 3, df_corr=None
@@ -220,15 +248,15 @@
     )
 
 
 def get_numeric_summary(
     df: pd.DataFrame,
     column: str,
     columns_stats: pd.DataFrame = None,
-    df_length: int = None,
+    df_length: Optional[pd.DataFrame] = None,
     plot: bool = False,
 ):
     series = df[column]
 
     if plot:
         try:
             series.hist()
@@ -253,15 +281,15 @@
     for x in np.array([0.05, 0.25, 0.5, 0.75, 0.95]):
         stats[to_percentage(x)] = series.quantile(x)
 
     stats["iqr"] = stats["75%"] - stats["25%"]
     stats["kurtosis"] = series.kurt()
     stats["skewness"] = series.skew()
     stats["sum"] = series.sum()
-    stats["mad"] = series.mad()
+    stats["mad"] = mad(series)
     stats["cv"] = stats["std"] / stats["mean"] if stats["mean"] else np.nan
     stats["zeros_num"] = df_length - np.count_nonzero(series)
     stats["zeros_perc"] = to_percentage(stats["zeros_num"] / df_length)
     deviation_of_mean, deviation_of_mean_perc = get_deviation_of_mean(
         series, df_length=df_length
     )
     stats["deviating_of_mean"] = deviation_of_mean
@@ -305,15 +333,15 @@
     return "This is a constant value: {}".format(df[column][0])
 
 
 def get_bool_summary(
     df: pd.DataFrame,
     column: str,
     columns_stats: pd.DataFrame = None,
-    df_length: int = None,
+    df_length: Optional[pd.DataFrame] = None,
 ):
     series = df[column]
 
     if columns_stats is None:
         columns_stats = get_df_column_stats(df[[column]])
 
     if df_length is None:
@@ -338,39 +366,39 @@
     return columns_stats[column]
 
 
 def get_df_column_summary(
     df: pd.DataFrame,
     column: str,
     columns_stats: pd.DataFrame = None,
-    df_length: int = None,
+    df_length: Optional[pd.DataFrame] = None,
     plot: bool = False,
 ):
     if columns_stats is None:
         columns_stats = get_df_column_stats(df[[column]])
 
     if df_length is None:
         df_length = len(df)
 
     column_type = columns_stats.loc["types"][column]
-    if column_type == DF_TYPE_NUMERIC:
+    if column_type == DFTypes.NUMERIC:
         return get_numeric_summary(
             df=df,
             column=column,
             columns_stats=columns_stats,
             df_length=df_length,
             plot=plot,
         )
-    if column_type == DF_TYPE_CATEGORICAL:
+    if column_type == DFTypes.CATEGORICAL:
         return get_categorical_summary(
             df=df, column=column, columns_stats=columns_stats
         )
-    if column_type == DF_TYPE_BOOL:
+    if column_type == DFTypes.BOOL:
         return get_bool_summary(
             df=df, column=column, columns_stats=columns_stats, df_length=df_length
         )
-    if column_type == DF_TYPE_UNIQUE:
+    if column_type == DFTypes.UNIQUE:
         return get_unique_summary(df=df, column=column, columns_stats=columns_stats)
-    if column_type == DF_TYPE_DATE:
+    if column_type == DFTypes.DATE:
         return get_date_summary(df=df, column=column, columns_stats=columns_stats)
-    if column_type == DF_TYPE_CONSTANT:
+    if column_type == DFTypes.CONSTANT:
         return get_constant_summary(df=df, column=column)
```

### Comparing `traceml-1.0.8/traceml/processors/errors.py` & `traceml-1.1.0rc0/traceml/processors/errors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/processors/events_processors/__init__.py` & `traceml-1.1.0rc0/traceml/processors/events_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/processors/events_processors/events_artifacts_processors.py` & `traceml-1.1.0rc0/traceml/processors/events_processors/events_artifacts_processors.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Optional
 
+from clipped.path_utils import copy_file_or_dir_path
 
-from polyaxon.utils.path_utils import copy_file_or_dir_path
 from traceml.events import V1EventArtifact
 
 try:
     import numpy as np
 except ImportError:
     np = None
 
 
 def artifact_path(
-    from_path: str, asset_path: str, kind: str, asset_rel_path: str = None
+    from_path: str, asset_path: str, kind: str, asset_rel_path: Optional[str] = None
 ) -> V1EventArtifact:
     copy_file_or_dir_path(from_path, asset_path)
     return V1EventArtifact(kind=kind, path=asset_rel_path or asset_path)
```

### Comparing `traceml-1.0.8/traceml/processors/events_processors/events_audio_processors.py` & `traceml-1.1.0rc0/traceml/processors/events_processors/events_audio_processors.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,36 +9,43 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Optional
+
+from clipped.np_utils import to_np
+from clipped.path_utils import check_or_create_path, copy_file_path
 
 from polyaxon.constants.globals import UNKNOWN
-from polyaxon.utils.np_utils import to_np
-from polyaxon.utils.path_utils import check_or_create_path, copy_file_path
 from traceml.events import V1EventAudio
 from traceml.logger import logger
 from traceml.processors.errors import NUMPY_ERROR_MESSAGE
 
 try:
     import numpy as np
 except ImportError:
     np = None
 
 
 def audio_path(
-    from_path: str, asset_path: str, content_type=None, asset_rel_path: str = None
+    from_path: str,
+    asset_path: str,
+    content_type=None,
+    asset_rel_path: Optional[str] = None,
 ) -> V1EventAudio:
     copy_file_path(from_path, asset_path)
     return V1EventAudio(path=asset_rel_path or asset_path, content_type=content_type)
 
 
-def audio(asset_path: str, tensor, sample_rate=44100, asset_rel_path: str = None):
+def audio(
+    asset_path: str, tensor, sample_rate=44100, asset_rel_path: Optional[str] = None
+):
     if not np:
         logger.warning(NUMPY_ERROR_MESSAGE)
         return UNKNOWN
 
     tensor = to_np(tensor)
     tensor = tensor.squeeze()
     if abs(tensor).max() > 1:
```

### Comparing `traceml-1.0.8/traceml/processors/events_processors/events_charts_processors.py` & `traceml-1.1.0rc0/traceml/processors/events_processors/events_charts_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from clipped.path_utils import module_type
+
 from polyaxon.constants.globals import UNKNOWN
-from polyaxon.utils.path_utils import module_type
 from traceml.events import V1EventChart, V1EventChartKind
 from traceml.logger import logger
 from traceml.processors.errors import (
     BOKEH_ERROR_MESSAGE,
     MATPLOTLIB_ERROR_MESSAGE,
     PLOTLY_ERROR_MESSAGE,
 )
```

### Comparing `traceml-1.0.8/traceml/processors/events_processors/events_image_processors.py` & `traceml-1.1.0rc0/traceml/processors/events_processors/events_image_processors.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 
+from typing import Optional
+
+from clipped.np_utils import calculate_scale_factor, to_np
+from clipped.path_utils import check_or_create_path, copy_file_path
+
 from polyaxon.constants.globals import UNKNOWN
-from polyaxon.utils.np_utils import calculate_scale_factor, to_np
-from polyaxon.utils.path_utils import check_or_create_path, copy_file_path
 from traceml.events import V1EventImage
 from traceml.logger import logger
 from traceml.processors.errors import (
     MATPLOTLIB_ERROR_MESSAGE,
     NUMPY_ERROR_MESSAGE,
     PIL_ERROR_MESSAGE,
 )
@@ -29,15 +32,15 @@
 try:
     import numpy as np
 except ImportError:
     np = None
 
 
 def image_path(
-    from_path: str, asset_path: str, asset_rel_path: str = None
+    from_path: str, asset_path: str, asset_rel_path: Optional[str] = None
 ) -> V1EventImage:
     copy_file_path(from_path, asset_path)
     return V1EventImage(path=asset_rel_path or asset_path)
 
 
 def _draw_single_box(
     image,
@@ -85,15 +88,15 @@
             display_str,
             fill=color_text,
             font=font,
         )
     return image
 
 
-def encoded_image(asset_path: str, data, asset_rel_path: str = None):
+def encoded_image(asset_path: str, data, asset_rel_path: Optional[str] = None):
     try:
         from PIL import Image
     except ImportError:
         logger.warning(PIL_ERROR_MESSAGE)
         return UNKNOWN
 
     image_data = Image.open(io.BytesIO(data.encoded_image_string))
@@ -103,15 +106,19 @@
         height=data.height,
         width=data.width,
         colorspace=data.colorspace,
     )
 
 
 def image(
-    asset_path: str, data, rescale=1, dataformats="CHW", asset_rel_path: str = None
+    asset_path: str,
+    data,
+    rescale=1,
+    dataformats="CHW",
+    asset_rel_path: Optional[str] = None,
 ):
     if not np:
         logger.warning(NUMPY_ERROR_MESSAGE)
         return UNKNOWN
 
     tensor = to_np(data)
     tensor = convert_to_HWC(tensor, dataformats)
@@ -126,15 +133,15 @@
 
 def image_boxes(
     asset_path: str,
     tensor_image,
     tensor_boxes,
     rescale=1,
     dataformats="CHW",
-    asset_rel_path: str = None,
+    asset_rel_path: Optional[str] = None,
 ):
     if not np:
         logger.warning(NUMPY_ERROR_MESSAGE)
         return UNKNOWN
 
     tensor_image = to_np(tensor_image)
     tensor_image = convert_to_HWC(tensor_image, dataformats)
@@ -165,15 +172,15 @@
             display_str=None,
             color="Red",
         )
     return disp_image
 
 
 def make_image(
-    asset_path: str, tensor, rescale=1, rois=None, asset_rel_path: str = None
+    asset_path: str, tensor, rescale=1, rois=None, asset_rel_path: Optional[str] = None
 ):
     try:
         from PIL import Image
     except ImportError:
         logger.warning(PIL_ERROR_MESSAGE)
         return UNKNOWN
 
@@ -192,15 +199,20 @@
         width=width,
         colorspace=colorspace,
         asset_rel_path=asset_rel_path,
     )
 
 
 def save_image(
-    asset_path: str, image_data, height, width, colorspace, asset_rel_path: str = None
+    asset_path: str,
+    image_data,
+    height,
+    width,
+    colorspace,
+    asset_rel_path: Optional[str] = None,
 ):
     check_or_create_path(asset_path, is_dir=False)
     image_data.save(asset_path, format="PNG")
     return V1EventImage(
         height=height,
         width=width,
         colorspace=colorspace,
```

### Comparing `traceml-1.0.8/traceml/processors/events_processors/events_metrics_processors.py` & `traceml-1.1.0rc0/traceml/processors/events_processors/events_metrics_processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, List
 
+from clipped.np_utils import to_np
+
 from polyaxon.constants.globals import UNKNOWN
-from polyaxon.utils.np_utils import to_np
 from traceml.artifacts import V1ArtifactKind
 from traceml.events import (
     LoggedEventSpec,
     V1Event,
     V1EventConfusionMatrix,
     V1EventCurve,
     V1EventCurveKind,
```

### Comparing `traceml-1.0.8/traceml/processors/events_processors/events_models_processors.py` & `traceml-1.1.0rc0/traceml/processors/events_processors/events_models_processors.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,32 +10,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Dict
+from typing import Dict, Optional
+
+from clipped.path_utils import copy_file_or_dir_path
 
-from polyaxon.utils.path_utils import copy_file_or_dir_path
 from traceml.events import V1EventModel
 from traceml.logger import logger
 
 try:
     import numpy as np
 except ImportError:
     np = None
 
 
 def model_path(
     from_path: str,
     asset_path: str,
-    framework: str = None,
-    spec: Dict = None,
-    asset_rel_path: str = None,
+    framework: Optional[str] = None,
+    spec: Optional[Dict] = None,
+    asset_rel_path: Optional[str] = None,
 ) -> V1EventModel:
     copy_file_or_dir_path(from_path, asset_path)
     return V1EventModel(
         path=asset_rel_path or asset_path, framework=framework, spec=spec
     )
```

### Comparing `traceml-1.0.8/traceml/processors/events_processors/events_tables_processors.py` & `traceml-1.1.0rc0/traceml/processors/events_processors/events_tables_processors.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Optional
+
+from clipped.path_utils import copy_file_path
 
-from polyaxon.utils.path_utils import copy_file_path
 from traceml.events import V1EventDataframe
 
 try:
     import numpy as np
 except ImportError:
     np = None
 
 
 def dataframe_path(
     from_path: str,
     asset_path: str,
-    content_type: str = None,
-    asset_rel_path: str = None,
+    content_type: Optional[str] = None,
+    asset_rel_path: Optional[str] = None,
 ) -> V1EventDataframe:
     copy_file_path(from_path, asset_path)
     return V1EventDataframe(
         path=asset_rel_path or asset_path, content_type=content_type
     )
```

### Comparing `traceml-1.0.8/traceml/processors/events_processors/events_video_processors.py` & `traceml-1.1.0rc0/traceml/processors/events_processors/events_video_processors.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,37 +9,46 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Optional
+
+from clipped.np_utils import calculate_scale_factor, to_np
+from clipped.path_utils import check_or_create_path, copy_file_path
 
 from polyaxon.constants.globals import UNKNOWN
-from polyaxon.utils.np_utils import calculate_scale_factor, to_np
-from polyaxon.utils.path_utils import check_or_create_path, copy_file_path
 from traceml.events import V1EventVideo
 from traceml.logger import logger
 from traceml.processors.errors import MOVIEPY_ERROR_MESSAGE, NUMPY_ERROR_MESSAGE
 
 try:
     import numpy as np
 except ImportError:
     np = None
 
 
 def video_path(
-    from_path: str, asset_path: str, content_type=None, asset_rel_path: str = None
+    from_path: str,
+    asset_path: str,
+    content_type=None,
+    asset_rel_path: Optional[str] = None,
 ) -> V1EventVideo:
     copy_file_path(from_path, asset_path)
     return V1EventVideo(path=asset_rel_path or asset_path, content_type=content_type)
 
 
 def video(
-    asset_path: str, tensor, fps=4, content_type="gif", asset_rel_path: str = None
+    asset_path: str,
+    tensor,
+    fps=4,
+    content_type="gif",
+    asset_rel_path: Optional[str] = None,
 ):
     if not np:
         logger.warning(NUMPY_ERROR_MESSAGE)
         return UNKNOWN
 
     tensor = to_np(tensor)
     tensor = prepare_video(tensor)
@@ -49,15 +58,19 @@
     tensor = (tensor * scale_factor).astype(np.uint8)
     return make_video(
         asset_path, tensor, fps, content_type, asset_rel_path=asset_rel_path
     )
 
 
 def make_video(
-    asset_path: str, tensor, fps, content_type="gif", asset_rel_path: str = None
+    asset_path: str,
+    tensor,
+    fps,
+    content_type="gif",
+    asset_rel_path: Optional[str] = None,
 ):
     try:
         import moviepy  # noqa: F401
     except ImportError:
         logger.warning(MOVIEPY_ERROR_MESSAGE)
         return UNKNOWN
     try:
```

### Comparing `traceml-1.0.8/traceml/processors/gpu_processor.py` & `traceml-1.1.0rc0/traceml/processors/gpu_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/processors/importance_processors.py` & `traceml-1.1.0rc0/traceml/processors/importance_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 import math
 import numpy as np
 import pandas as pd
 
 from typing import Dict, List, Optional, Tuple, Union
 
-from polyaxon.utils.np_utils import sanitize_np_types
+from clipped.np_utils import sanitize_np_types
 
 
 def clean_duplicates(
     params: pd.DataFrame, metrics: pd.DataFrame
 ) -> Optional[Tuple[pd.DataFrame, pd.DataFrame]]:
     duplicate_ids = metrics.duplicated()
     params_df = params[~duplicate_ids]
```

### Comparing `traceml-1.0.8/traceml/processors/logs_processor.py` & `traceml-1.1.0rc0/traceml/processors/logs_processor.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,32 +11,39 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import sys
 
-from traceml.logging.handler import PolyaxonHandler
+from traceml.logging.handler import LogStreamHandler, LogStreamWriter
 
-EXCLUDE_DEFAULT_LOGGERS = ("polyaxon.client", "polyaxon.cli")
+EXCLUDE_DEFAULT_LOGGERS = ("polyaxon.client", "polyaxon.cli", "traceml")
 
 
-def setup_logging(add_logs, exclude=EXCLUDE_DEFAULT_LOGGERS):
-    plx_logger = logging.getLogger()
+def start_log_processor(add_logs, exclude=EXCLUDE_DEFAULT_LOGGERS):
+    plx_logger = logging.getLogger("__plx__")
     plx_logger.setLevel(logging.INFO)
-    if logging.StreamHandler not in map(type, plx_logger.handlers):
-        plx_logger.addHandler(logging.StreamHandler())
-        plx_logger.propagate = False
-    if PolyaxonHandler in map(type, plx_logger.handlers):
+    if LogStreamHandler in map(type, plx_logger.handlers):
         for handler in plx_logger.handlers:
-            if isinstance(handler, PolyaxonHandler):
+            if isinstance(handler, LogStreamHandler):
                 handler.set_add_logs(add_logs=add_logs)
     else:
-        handler = PolyaxonHandler(add_logs=add_logs)
+        handler = LogStreamHandler(add_logs=add_logs)
         plx_logger.addHandler(handler)
 
+    exclude = ("__plx__",) + (exclude or ())
     for logger_name in exclude:
-        plx_logger = logging.getLogger(logger_name)
-        if logging.StreamHandler not in map(type, plx_logger.handlers):
-            plx_logger.addHandler(logging.StreamHandler())
-            plx_logger.propagate = False
+        logger = logging.getLogger(logger_name)
+        if logging.StreamHandler not in map(type, logger.handlers):
+            logger.addHandler(logging.StreamHandler())
+            logger.propagate = False
+
+    sys.stdout = LogStreamWriter(plx_logger, logging.INFO, sys.__stdout__)
+    sys.stderr = LogStreamWriter(plx_logger, logging.ERROR, sys.__stderr__)
+
+
+def end_log_processor():
+    sys.stdout = sys.__stdout__
+    sys.stderr = sys.__stderr__
```

### Comparing `traceml-1.0.8/traceml/processors/psutil_processor.py` & `traceml-1.1.0rc0/traceml/processors/psutil_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/processors/units_processors.py` & `traceml-1.1.0rc0/traceml/processors/units_processors.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,40 +9,40 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Union
+from typing import Optional, Union
 
 
 def _sanitize_value(value: Union[str, int, float]) -> Union[int, float]:
     fvalue = float(value)
     ivalue = int(fvalue)
     return ivalue if ivalue == fvalue else fvalue
 
 
 def to_cpu_value(cpu_definition: Union[str, int, float]) -> float:
     try:
         return float(cpu_definition)
     except (ValueError, TypeError):
         pass
 
-    cpu_definition = cpu_definition.lower()
+    cpu_definition = cpu_definition.lower()  # type: ignore[union-attr]
     cpu_unit = cpu_definition[-1]
     cpu_value = cpu_definition[:-1]
     if cpu_unit == "m":
         cpu = _sanitize_value(cpu_value) / 1000
     elif cpu_unit == "u":
         cpu = _sanitize_value(cpu_value) / 1000**2
     elif cpu_unit == "n":
         cpu = _sanitize_value(cpu_value) / 1000**3
     else:
-        cpu = cpu_definition
+        cpu = cpu_definition  # type: ignore[assignment]
     return _sanitize_value(cpu)
 
 
 def to_memory_bytes(mem_definition: Union[str, int, float]) -> int:
     try:
         return int(float(mem_definition))
     except (ValueError, TypeError):
@@ -66,15 +66,15 @@
         "mi": 1024**2,
         "gi": 1024**3,
         "ti": 1024**4,
         "pi": 1024**5,
         "ei": 1024**6,
     }
 
-    mem_definition = mem_definition.lower()
+    mem_definition = mem_definition.lower()  # type: ignore[union-attr]
 
     mem_unit = mem_definition[-2:]
     mem_value = mem_definition[:-2]
     memory = _get_value(mem_unit, mem_value, power_two_unit_multiplier)
     if memory is not None:
         return memory
 
@@ -83,15 +83,15 @@
     memory = _get_value(mem_unit, mem_value, fixed_point_unit_multiplier)
     if memory is not None:
         return memory
 
     return 0
 
 
-def to_unit_memory(number, precision: int = 2):
+def to_unit_memory(number: Union[int, float], precision: int = 2) -> str:
     """Creates a string representation of memory size given `number`."""
     kb = 1024
 
     number /= kb
 
     if number < 100:
         return "{} Ki".format(round(number, precision))
@@ -112,30 +112,32 @@
     if number < 900:
         return "{} Pi".format(round(number, precision))
 
     number /= kb
     return "{} Ei".format(round(number, precision))
 
 
-def number_percentage_format(x, precision: int = None, use_comma: bool = False):
+def number_percentage_format(
+    x, precision: Optional[int] = None, use_comma: bool = False
+) -> str:
     if precision is None:
         return x
     eps = 0.000000001
     comma = "," if use_comma else ""
     num_format = (
         "{{0:{}.0f}}".format(comma)
         if abs(int(x) - x) < eps
         else "{{0:{}.{}f}}".format(comma, precision)
     )
     return num_format.format(x)
 
 
 def to_percentage(
-    number, rounding: int = 2, precision: int = None, use_comma: bool = False
-):
+    number, rounding: int = 2, precision: Optional[int] = None, use_comma: bool = False
+) -> str:
     """Creates a percentage string representation from the given `number`. The
     number is multiplied by 100 before adding a '%' character.
 
     Raises `ValueError` if `number` cannot be converted to a number.
     """
     number = float(number) * 100
     number_as_int = int(number)
@@ -145,15 +147,15 @@
         if number_as_int == rounded
         else number_percentage_format(rounded, precision, use_comma)
     )
 
     return "{}%".format(value)
 
 
-def format_sizeof(num, suffix="B"):
+def format_sizeof(num: Union[int, float], suffix: str = "B") -> str:
     """
     Print in human friendly format
     """
     for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
         if abs(num) < 1024.0:
             return "%3.1f%s%s" % (num, unit, suffix)
         num /= 1024.0
```

### Comparing `traceml-1.0.8/traceml/serialization/__init__.py` & `traceml-1.1.0rc0/traceml/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/serialization/base.py` & `traceml-1.1.0rc0/traceml/serialization/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from typing import Dict, List
 
-from polyaxon.utils.path_utils import check_or_create_path
+from clipped.enums_utils import get_enum_value
+from clipped.path_utils import check_or_create_path
+
 from traceml.events import LoggedEventSpec
 from traceml.events.schemas import LoggedEventListSpec
 
 
 class EventWriter:
     EVENTS_BACKEND = "events"
     RESOURCES_BACKEND = "resources"
@@ -32,21 +34,29 @@
         self._run_path = run_path
         self._files = {}  # type: Dict[str, LoggedEventListSpec]
         self._closed = False
 
     def _get_event_path(self, kind: str, name: str) -> str:
         if self._events_backend == self.EVENTS_BACKEND:
             return os.path.join(
-                self._run_path, self._events_backend, kind, "{}.plx".format(name)
+                self._run_path,
+                get_enum_value(self._events_backend),
+                kind,
+                "{}.plx".format(name),
             )
         if self._events_backend == self.RESOURCES_BACKEND:
             return os.path.join(
-                self._run_path, self._events_backend, kind, "{}.plx".format(name)
+                self._run_path,
+                get_enum_value(self._events_backend),
+                kind,
+                "{}.plx".format(name),
             )
-        raise ValueError("Unrecognized backend {}".format(self._events_backend))
+        raise ValueError(
+            "Unrecognized backend {}".format(get_enum_value(self._events_backend))
+        )
 
     def _init_events(self, events_spec: LoggedEventListSpec):
         event_path = self._get_event_path(kind=events_spec.kind, name=events_spec.name)
         # Check if the file exists otherwise initialize
         if not os.path.exists(event_path):
             check_or_create_path(event_path, is_dir=False)
             with open(event_path, "w") as event_file:
```

### Comparing `traceml-1.0.8/traceml/serialization/writer.py` & `traceml-1.1.0rc0/traceml/serialization/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 import queue
 import threading
 import time
 
 from typing import List, Union
 
-from polyaxon.utils.path_utils import check_or_create_path
+from clipped.path_utils import check_or_create_path
+
 from traceml.events import LoggedEventSpec, get_asset_path, get_event_path
 from traceml.events.paths import get_resource_path
 from traceml.processors.gpu_processor import can_log_gpu_resources, get_gpu_metrics
 from traceml.processors.psutil_processor import (
     can_log_psutil_resources,
     get_psutils_metrics,
 )
```

### Comparing `traceml-1.0.8/traceml/tracking/__init__.py` & `traceml-1.1.0rc0/traceml/tracking/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,36 +13,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Sequence, Union
 
 from polyaxon.client import RunClient
+from polyaxon.schemas.responses.v1_run import V1Run
 from traceml.artifacts import V1ArtifactKind, V1RunArtifact
 from traceml.tracking.run import Run
 
 TRACKING_RUN: Run = None
 
 
 def init(
-    owner: str = None,
-    project: str = None,
-    run_uuid: str = None,
+    owner: Optional[str] = None,
+    project: Optional[str] = None,
+    run_uuid: Optional[str] = None,
     client: RunClient = None,
     track_code: bool = True,
     track_env: bool = True,
+    track_logs: bool = True,
     refresh_data: bool = False,
-    artifacts_path: str = None,
-    collect_artifacts: str = None,
-    collect_resources: str = None,
-    is_offline: bool = None,
-    is_new: bool = None,
-    name: str = None,
-    description: str = None,
-    tags: List[str] = None,
+    artifacts_path: Optional[str] = None,
+    collect_artifacts: Optional[str] = None,
+    collect_resources: Optional[str] = None,
+    is_offline: Optional[bool] = None,
+    is_new: Optional[bool] = None,
+    name: Optional[str] = None,
+    description: Optional[str] = None,
+    tags: Optional[List[str]] = None,
 ) -> Optional[Run]:
     """Tracking module is similar to the tracking client without the need to create a run instance.
 
     The tracking module allows you to call all tracking methods directly from the top level module.
 
     This could be very convenient especially if you are running in-cluster experiments:
 
@@ -68,14 +70,15 @@
             client: [PolyaxonClient](/docs/core/python-library/polyaxon-client/), optional,
                  an instance of a configured client, if not passed,
                  a new instance will be created based on the available environment.
             track_code: bool, optional, default True, to track code version.
                  Polyaxon will try to track information about any repo
                  configured in the context where this client is instantiated.
             track_env: bool, optional, default True, to track information about the environment.
+            track_logs: bool, optional, default True, to track logs for manually managed runs.
             refresh_data: bool, optional, default False, to refresh the run data at instantiation.
             refresh_data: bool, optional, default False, to instruct the run to resume,
                  only useful when the run is not managed by Polyaxon.
             artifacts_path: str, optional, for in-cluster runs it will be set automatically.
             collect_artifacts: bool, optional,
                  similar to the env var flag `POLYAXON_COLLECT_ARTIFACTS`, this env var is `True`
                  by default for managed runs and is controlled by the plugins section.
@@ -107,14 +110,15 @@
         owner=owner,
         project=project,
         run_uuid=run_uuid,
         client=client,
         track_code=track_code,
         refresh_data=refresh_data,
         track_env=track_env,
+        track_logs=track_logs,
         artifacts_path=artifacts_path,
         collect_artifacts=collect_artifacts,
         collect_resources=collect_resources,
         is_offline=is_offline,
         is_new=is_new,
         name=name,
         description=description,
@@ -137,16 +141,24 @@
     if TRACKING_RUN:
         return TRACKING_RUN
 
     init()
     return TRACKING_RUN
 
 
+def update(data: Union[Dict, V1Run], async_req: bool = False):
+    global TRACKING_RUN
+    TRACKING_RUN.update(data=data, async_req=async_req)
+
+
+update.__doc__ = Run.update.__doc__
+
+
 def get_artifacts_path(
-    rel_path: str = None,
+    rel_path: Optional[str] = None,
     ensure_path: bool = False,
     is_dir: bool = False,
     use_store_path: bool = False,
 ):
     global TRACKING_RUN
     return TRACKING_RUN.get_artifacts_path(
         rel_path=rel_path,
@@ -156,15 +168,15 @@
     )
 
 
 get_artifacts_path.__doc__ = Run.get_artifacts_path.__doc__
 
 
 def get_outputs_path(
-    rel_path: str = None,
+    rel_path: Optional[str] = None,
     ensure_path: bool = True,
     is_dir: bool = False,
     use_store_path: bool = False,
 ):
     global TRACKING_RUN
     return TRACKING_RUN.get_outputs_path(
         rel_path=rel_path,
@@ -218,37 +230,49 @@
     global TRACKING_RUN
     TRACKING_RUN.set_run_process_sidecar()
 
 
 set_run_process_sidecar.__doc__ = Run.set_run_process_sidecar.__doc__
 
 
-def log_metric(name: str, value: float, step: int = None, timestamp: datetime = None):
+def log_metric(
+    name: str,
+    value: float,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
+):
     global TRACKING_RUN
     TRACKING_RUN.log_metric(
         name=name,
         value=value,
         step=step,
         timestamp=timestamp,
     )
 
 
 log_metric.__doc__ = Run.log_metric.__doc__
 
 
-def log_metrics(step: int = None, timestamp: datetime = None, **metrics):
+def log_metrics(
+    step: Optional[int] = None, timestamp: Optional[datetime] = None, **metrics
+):
     global TRACKING_RUN
     TRACKING_RUN.log_metrics(step=step, timestamp=timestamp, **metrics)
 
 
 log_metrics.__doc__ = Run.log_metrics.__doc__
 
 
 def log_roc_auc_curve(
-    name: str, fpr, tpr, auc: float = None, step: int = None, timestamp: datetime = None
+    name: str,
+    fpr,
+    tpr,
+    auc: float = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_roc_auc_curve(
         name=name,
         fpr=fpr,
         tpr=tpr,
         auc=auc,
@@ -260,16 +284,16 @@
 log_roc_auc_curve.__doc__ = Run.log_roc_auc_curve.__doc__
 
 
 def log_sklearn_roc_auc_curve(
     name: str,
     y_preds,
     y_targets,
-    step: int = None,
-    timestamp: datetime = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
     is_multi_class: bool = False,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_sklearn_roc_auc_curve(
         name=name,
         y_preds=y_preds,
         y_targets=y_targets,
@@ -283,16 +307,16 @@
 
 
 def log_pr_curve(
     name: str,
     precision,
     recall,
     average_precision=None,
-    step: int = None,
-    timestamp: datetime = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_pr_curve(
         name=name,
         precision=precision,
         recall=recall,
         average_precision=average_precision,
@@ -304,16 +328,16 @@
 log_pr_curve.__doc__ = Run.log_pr_curve.__doc__
 
 
 def log_sklearn_pr_curve(
     name: str,
     y_preds,
     y_targets,
-    step: int = None,
-    timestamp: datetime = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
     is_multi_class: bool = False,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_sklearn_pr_curve(
         name=name,
         y_preds=y_preds,
         y_targets=y_targets,
@@ -326,17 +350,17 @@
 log_sklearn_pr_curve.__doc__ = Run.log_sklearn_pr_curve.__doc__
 
 
 def log_curve(
     name: str,
     x,
     y,
-    annotation: str = None,
-    step: int = None,
-    timestamp: datetime = None,
+    annotation: Optional[str] = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_curve(
         name=name,
         x=x,
         y=y,
         annotation=annotation,
@@ -349,16 +373,16 @@
 
 
 def log_confusion_matrix(
     name: str,
     x,
     y,
     z=None,
-    step: int = None,
-    timestamp: datetime = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_confusion_matrix(
         name=name,
         x=x,
         y=y,
         z=z,
@@ -368,20 +392,20 @@
 
 
 log_confusion_matrix.__doc__ = Run.log_confusion_matrix.__doc__
 
 
 def log_image(
     data: Any,
-    name: str = None,
-    step: int = None,
-    timestamp: datetime = None,
+    name: Optional[str] = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
     rescale=1,
     dataformats: str = "CHW",
-    ext: str = None,
+    ext: Optional[str] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_image(
         data=data,
         name=name,
         step=step,
         timestamp=timestamp,
@@ -393,17 +417,17 @@
 
 log_image.__doc__ = Run.log_image.__doc__
 
 
 def log_image_with_boxes(
     tensor_image,
     tensor_boxes,
-    name: str = None,
-    step: int = None,
-    timestamp: datetime = None,
+    name: Optional[str] = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
     rescale: int = 1,
     dataformats: str = "CHW",
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_image_with_boxes(
         tensor_image=tensor_image,
         tensor_boxes=tensor_boxes,
@@ -416,18 +440,18 @@
 
 
 log_image_with_boxes.__doc__ = Run.log_image_with_boxes.__doc__
 
 
 def log_mpl_image(
     data,
-    name: str = None,
+    name: Optional[str] = None,
     close: bool = True,
-    step: int = None,
-    timestamp: datetime = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_mpl_image(
         data=data,
         name=name,
         close=close,
         step=step,
@@ -436,19 +460,19 @@
 
 
 log_mpl_image.__doc__ = Run.log_mpl_image.__doc__
 
 
 def log_video(
     data,
-    name: str = None,
+    name: Optional[str] = None,
     fps: int = 4,
-    step: int = None,
-    timestamp: datetime = None,
-    content_type: str = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
+    content_type: Optional[str] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_video(
         data=data,
         name=name,
         fps=fps,
         step=step,
@@ -458,19 +482,19 @@
 
 
 log_video.__doc__ = Run.log_video.__doc__
 
 
 def log_audio(
     data,
-    name: str = None,
+    name: Optional[str] = None,
     sample_rate: int = 44100,
-    step: int = None,
-    timestamp: datetime = None,
-    content_type: str = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
+    content_type: Optional[str] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_audio(
         data=data,
         name=name,
         sample_rate=sample_rate,
         step=step,
@@ -478,42 +502,56 @@
         content_type=content_type,
     )
 
 
 log_audio.__doc__ = Run.log_audio.__doc__
 
 
-def log_text(name: str, text: str, step: int = None, timestamp: datetime = None):
+def log_text(
+    name: str,
+    text: str,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
+):
     global TRACKING_RUN
     TRACKING_RUN.log_text(
         name=name,
         text=text,
         step=step,
         timestamp=timestamp,
     )
 
 
 log_text.__doc__ = Run.log_text.__doc__
 
 
-def log_html(name: str, html: str, step: int = None, timestamp: datetime = None):
+def log_html(
+    name: str,
+    html: str,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
+):
     global TRACKING_RUN
     TRACKING_RUN.log_html(
         name=name,
         html=html,
         step=step,
         timestamp=timestamp,
     )
 
 
 log_html.__doc__ = Run.log_html.__doc__
 
 
 def log_np_histogram(
-    name: str, values, counts, step: int = None, timestamp: datetime = None
+    name: str,
+    values,
+    counts,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_np_histogram(
         name=name,
         values=values,
         counts=counts,
         step=step,
@@ -521,15 +559,20 @@
     )
 
 
 log_np_histogram.__doc__ = Run.log_np_histogram.__doc__
 
 
 def log_histogram(
-    name: str, values, bins, max_bins=None, step: int = None, timestamp: datetime = None
+    name: str,
+    values,
+    bins,
+    max_bins=None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_histogram(
         name=name,
         values=values,
         bins=bins,
         max_bins=max_bins,
@@ -539,20 +582,20 @@
 
 
 log_histogram.__doc__ = Run.log_histogram.__doc__
 
 
 def log_model(
     path: str,
-    name: str = None,
-    framework: str = None,
-    summary: Dict = None,
-    step: int = None,
-    timestamp: datetime = None,
-    rel_path: str = None,
+    name: Optional[str] = None,
+    framework: Optional[str] = None,
+    summary: Optional[Dict] = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
+    rel_path: Optional[str] = None,
     skip_hash_calculation: bool = False,
     **kwargs,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_model(
         path=path,
         name=name,
@@ -567,20 +610,20 @@
 
 
 log_model.__doc__ = Run.log_model.__doc__
 
 
 def log_artifact(
     path: str,
-    name: str = None,
-    kind: str = None,
-    summary: Dict = None,
-    step: int = None,
-    timestamp: datetime = None,
-    rel_path: str = None,
+    name: Optional[str] = None,
+    kind: Optional[str] = None,
+    summary: Optional[Dict] = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
+    rel_path: Optional[str] = None,
     skip_hash_calculation: bool = False,
     **kwargs,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_artifact(
         path=path,
         name=name,
@@ -597,57 +640,63 @@
 log_artifact.__doc__ = Run.log_artifact.__doc__
 
 
 def log_dataframe(
     df,
     name: str,
     content_type: str = V1ArtifactKind.CSV,
-    step: int = None,
-    timestamp: datetime = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_dataframe(
         df=df,
         name=name,
         content_type=content_type,
         step=step,
         timestamp=timestamp,
     )
 
 
 log_dataframe.__doc__ = Run.log_dataframe.__doc__
 
 
-def log_plotly_chart(name: str, figure, step: int = None, timestamp: datetime = None):
+def log_plotly_chart(
+    name: str, figure, step: Optional[int] = None, timestamp: Optional[datetime] = None
+):
     global TRACKING_RUN
     TRACKING_RUN.log_plotly_chart(
         name=name,
         figure=figure,
         step=step,
         timestamp=timestamp,
     )
 
 
 log_plotly_chart.__doc__ = Run.log_plotly_chart.__doc__
 
 
-def log_bokeh_chart(name: str, figure, step: int = None, timestamp: datetime = None):
+def log_bokeh_chart(
+    name: str, figure, step: Optional[int] = None, timestamp: Optional[datetime] = None
+):
     global TRACKING_RUN
     TRACKING_RUN.log_bokeh_chart(
         name=name,
         figure=figure,
         step=step,
         timestamp=timestamp,
     )
 
 
 log_bokeh_chart.__doc__ = Run.log_bokeh_chart.__doc__
 
 
-def log_altair_chart(name: str, figure, step: int = None, timestamp: datetime = None):
+def log_altair_chart(
+    name: str, figure, step: Optional[int] = None, timestamp: Optional[datetime] = None
+):
     global TRACKING_RUN
     TRACKING_RUN.log_altair_chart(
         name=name,
         figure=figure,
         step=step,
         timestamp=timestamp,
     )
@@ -655,16 +704,16 @@
 
 log_altair_chart.__doc__ = Run.log_altair_chart.__doc__
 
 
 def log_mpl_plotly_chart(
     name: str,
     figure,
-    step: int = None,
-    timestamp: datetime = None,
+    step: Optional[int] = None,
+    timestamp: Optional[datetime] = None,
     close: bool = True,
     fallback_to_image: bool = True,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_mpl_plotly_chart(
         name=name,
         figure=figure,
@@ -682,14 +731,22 @@
     global TRACKING_RUN
     return TRACKING_RUN.get_log_level()
 
 
 get_log_level.__doc__ = Run.get_log_level.__doc__
 
 
+def set_readme(readme: str, async_req: bool = True):
+    global TRACKING_RUN
+    TRACKING_RUN.set_readme(readme=readme, async_req=async_req)
+
+
+set_readme.__doc__ = Run.set_readme.__doc__
+
+
 def set_description(description: str, async_req: bool = True):
     global TRACKING_RUN
     TRACKING_RUN.set_description(description=description, async_req=async_req)
 
 
 set_description.__doc__ = Run.set_description.__doc__
 
@@ -708,18 +765,18 @@
 
 
 end.__doc__ = Run.end.__doc__
 
 
 def log_status(
     status: str,
-    reason: str = None,
-    message: str = None,
-    last_transition_time: datetime = None,
-    last_update_time: datetime = None,
+    reason: Optional[str] = None,
+    message: Optional[str] = None,
+    last_transition_time: Optional[datetime] = None,
+    last_update_time: Optional[datetime] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_status(
         status=status,
         reason=reason,
         message=message,
         last_transition_time=last_transition_time,
@@ -786,31 +843,31 @@
     global TRACKING_RUN
     TRACKING_RUN.log_stopped()
 
 
 log_stopped.__doc__ = Run.log_stopped.__doc__
 
 
-def log_failed(reason: str = None, message: str = None):
+def log_failed(reason: Optional[str] = None, message: Optional[str] = None):
     global TRACKING_RUN
     TRACKING_RUN.log_failed(reason=reason, message=message)
 
 
 log_failed.__doc__ = Run.log_failed.__doc__
 
 
 def log_artifact_ref(
     path: str,
     kind: V1ArtifactKind,
-    name: str = None,
-    hash: str = None,
+    name: Optional[str] = None,
+    hash: Optional[str] = None,
     content=None,
-    summary: Dict = None,
+    summary: Optional[Dict] = None,
     is_input: bool = False,
-    rel_path: str = None,
+    rel_path: Optional[str] = None,
     skip_hash_calculation: bool = False,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_artifact_ref(
         path=path,
         kind=kind,
         name=name,
@@ -826,15 +883,15 @@
 log_artifact_ref.__doc__ = Run.log_artifact_ref.__doc__
 
 
 def log_tensorboard_ref(
     path: str,
     name: str = "tensorboard",
     is_input: bool = False,
-    rel_path: str = None,
+    rel_path: Optional[str] = None,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_tensorboard_ref(
         path=path,
         name=name,
         is_input=is_input,
         rel_path=rel_path,
@@ -842,19 +899,19 @@
 
 
 log_tensorboard_ref.__doc__ = Run.log_tensorboard_ref.__doc__
 
 
 def log_model_ref(
     path: str,
-    name: str = None,
-    framework: str = None,
-    summary: Dict = None,
+    name: Optional[str] = None,
+    framework: Optional[str] = None,
+    summary: Optional[Dict] = None,
     is_input: bool = False,
-    rel_path: str = None,
+    rel_path: Optional[str] = None,
     skip_hash_calculation: bool = False,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_model_ref(
         path=path,
         name=name,
         framework=framework,
@@ -864,28 +921,28 @@
         skip_hash_calculation=skip_hash_calculation,
     )
 
 
 log_model_ref.__doc__ = Run.log_model_ref.__doc__
 
 
-def log_code_ref(code_ref: Dict = None, is_input: bool = True):
+def log_code_ref(code_ref: Optional[Dict] = None, is_input: bool = True):
     global TRACKING_RUN
     TRACKING_RUN.log_code_ref(code_ref=code_ref, is_input=is_input)
 
 
 log_code_ref.__doc__ = Run.log_code_ref.__doc__
 
 
 def log_data_ref(
     name: str,
-    hash: str = None,
-    path: str = None,
+    hash: Optional[str] = None,
+    path: Optional[str] = None,
     content=None,
-    summary: Dict = None,
+    summary: Optional[Dict] = None,
     is_input: bool = True,
     skip_hash_calculation: bool = False,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_data_ref(
         name=name,
         content=content,
@@ -898,20 +955,20 @@
 
 
 log_data_ref.__doc__ = Run.log_data_ref.__doc__
 
 
 def log_file_ref(
     path: str,
-    name: str = None,
-    hash: str = None,
+    name: Optional[str] = None,
+    hash: Optional[str] = None,
     content=None,
-    summary: Dict = None,
+    summary: Optional[Dict] = None,
     is_input: bool = False,
-    rel_path: str = None,
+    rel_path: Optional[str] = None,
     skip_hash_calculation: bool = False,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_file_ref(
         path=path,
         name=name,
         hash=hash,
@@ -924,19 +981,19 @@
 
 
 log_file_ref.__doc__ = Run.log_file_ref.__doc__
 
 
 def log_dir_ref(
     path: str,
-    name: str = None,
-    hash: str = None,
-    summary: Dict = None,
+    name: Optional[str] = None,
+    hash: Optional[str] = None,
+    summary: Optional[Dict] = None,
     is_input: bool = False,
-    rel_path: str = None,
+    rel_path: Optional[str] = None,
     skip_hash_calculation: bool = False,
 ):
     global TRACKING_RUN
     TRACKING_RUN.log_dir_ref(
         path=path,
         name=name,
         hash=hash,
@@ -954,15 +1011,15 @@
     global TRACKING_RUN
     TRACKING_RUN.log_artifact_lineage(body)
 
 
 log_artifact_lineage.__doc__ = Run.log_artifact_lineage.__doc__
 
 
-def log_env(rel_path: str = None, content: Dict = None):
+def log_env(rel_path: Optional[str] = None, content: Optional[Dict] = None):
     global TRACKING_RUN
     return TRACKING_RUN.log_env(rel_path=rel_path, content=content)
 
 
 log_env.__doc__ = Run.log_env.__doc__
 
 
@@ -979,15 +1036,15 @@
     TRACKING_RUN.sync_system_events_summaries()
 
 
 sync_system_events_summaries.__doc__ = Run.sync_system_events_summaries.__doc__
 
 
 def pull_remote_run(
-    path: str = None,
+    path: Optional[str] = None,
     download_artifacts: bool = True,
 ):
     global TRACKING_RUN
     return TRACKING_RUN.pull_remote_run(
         path=path,
         download_artifacts=download_artifacts,
     )
@@ -1010,19 +1067,19 @@
 
 
 push_offline_run.__doc__ = Run.push_offline_run.__doc__
 
 
 def promote_to_model_version(
     version: str,
-    description: str = None,
-    tags: Union[str, List[str]] = None,
-    content: Union[str, Dict] = None,
-    connection: str = None,
-    artifacts: List[str] = None,
+    description: Optional[str] = None,
+    tags: Optional[Union[str, List[str]]] = None,
+    content: Optional[Union[str, Dict]] = None,
+    connection: Optional[str] = None,
+    artifacts: Optional[List[str]] = None,
     force: bool = False,
 ):
     global TRACKING_RUN
     return TRACKING_RUN.promote_to_model_version(
         version=version,
         description=description,
         tags=tags,
@@ -1034,19 +1091,19 @@
 
 
 promote_to_model_version.__doc__ = Run.promote_to_model_version.__doc__
 
 
 def promote_to_artifact_version(
     version: str,
-    description: str = None,
-    tags: Union[str, List[str]] = None,
-    content: Union[str, Dict] = None,
-    connection: str = None,
-    artifacts: List[str] = None,
+    description: Optional[str] = None,
+    tags: Optional[Union[str, List[str]]] = None,
+    content: Optional[Union[str, Dict]] = None,
+    connection: Optional[str] = None,
+    artifacts: Optional[List[str]] = None,
     force: bool = False,
 ):
     global TRACKING_RUN
     return TRACKING_RUN.promote_to_artifact_version(
         version=version,
         description=description,
         tags=tags,
@@ -1062,14 +1119,15 @@
 
 __all__ = [
     "V1ArtifactKind",
     "V1RunArtifact",
     "Run",
     "init",
     "get_or_create_run",
+    "update",
     "get_artifacts_path",
     "get_outputs_path",
     "get_tensorboard_path",
     "set_artifacts_path",
     "set_run_event_logger",
     "set_run_resource_logger",
     "set_run_process_sidecar",
@@ -1094,14 +1152,15 @@
     "log_artifact",
     "log_dataframe",
     "log_plotly_chart",
     "log_bokeh_chart",
     "log_altair_chart",
     "log_mpl_plotly_chart",
     "get_log_level",
+    "set_readme",
     "set_description",
     "set_name",
     "end",
     "log_status",
     "log_inputs",
     "log_outputs",
     "log_tags",
```

### Comparing `traceml-1.0.8/traceml/tracking/run.py` & `traceml-1.1.0rc0/traceml/tracking/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,49 +17,48 @@
 import atexit
 import os
 import sys
 import tempfile
 import time
 
 from datetime import datetime
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 import ujson
 
-import polyaxon_sdk
+from clipped.env import get_run_env
+from clipped.hashing import hash_value
+from clipped.path_utils import (
+    check_or_create_path,
+    copy_file_or_dir_path,
+    get_base_filename,
+    get_path_extension,
+)
 
 from polyaxon import settings
 from polyaxon.client import PolyaxonClient, RunClient
 from polyaxon.client.decorators import client_handler
 from polyaxon.connections.reader import get_connection_type
 from polyaxon.constants.globals import UNKNOWN
 from polyaxon.contexts import paths as ctx_paths
 from polyaxon.env_vars.getters import (
     get_artifacts_store_name,
     get_collect_artifacts,
     get_collect_resources,
     get_log_level,
 )
-from polyaxon.lifecycle import LifeCycle, V1ProjectFeature
+from polyaxon.lifecycle import LifeCycle, V1ProjectFeature, V1Statuses
 from polyaxon.sidecar.processor import SidecarThread
-from polyaxon.utils.env import get_run_env
 from polyaxon.utils.fqn_utils import to_fqn_name
-from polyaxon.utils.hashing import hash_value
-from polyaxon.utils.path_utils import (
-    check_or_create_path,
-    copy_file_or_dir_path,
-    get_base_filename,
-    get_path_extension,
-)
 from traceml.artifacts import V1ArtifactKind
 from traceml.events import LoggedEventSpec, V1Event, get_asset_path
 from traceml.logger import logger
 from traceml.logging import V1Log, V1Logs
 from traceml.processors import events_processors
-from traceml.processors.logs_processor import setup_logging
+from traceml.processors.logs_processor import end_log_processor, start_log_processor
 from traceml.serialization.writer import EventFileWriter, ResourceFileWriter
 
 
 class Run(RunClient):
     """Run tracking is client to instrument your machine learning model and track experiments.
 
     If no values are passed to this class,
@@ -89,14 +88,15 @@
         client: [PolyaxonClient](/docs/core/python-library/polyaxon-client/), optional,
              an instance of a configured client, if not passed,
              a new instance will be created based on the available environment.
         track_code: bool, optional, default True, to track code version.
              Polyaxon will try to track information about any repo
              configured in the context where this client is instantiated.
         track_env: bool, optional, default True, to track information about the environment.
+        track_logs: bool, optional, default True, to track logs for manually managed runs.
         refresh_data: bool, optional, default False, to refresh the run data at instantiation.
         artifacts_path: str, optional, for in-cluster runs it will be set automatically.
         collect_artifacts: bool, optional,
              similar to the env var flag `POLYAXON_COLLECT_ARTIFACTS`, this env var is `True`
              by default for managed runs and is controlled by the plugins section.
         collect_resources: bool, optional,
              similar to the env var flag `POLYAXON_COLLECT_RESOURCES`, this env var is `True`
@@ -122,31 +122,31 @@
         PolyaxonClientException: If no owner and/or project are passed and Polyaxon cannot
              resolve the values from the environment.
     """
 
     @client_handler(check_no_op=True)
     def __init__(
         self,
-        owner: str = None,
-        project: str = None,
-        run_uuid: str = None,
-        client: PolyaxonClient = None,
+        owner: Optional[str] = None,
+        project: Optional[str] = None,
+        run_uuid: Optional[str] = None,
+        client: Optional[PolyaxonClient] = None,
         track_code: bool = True,
         track_env: bool = True,
         track_logs: bool = True,
         refresh_data: bool = False,
-        artifacts_path: str = None,
-        collect_artifacts: bool = None,
-        collect_resources: bool = None,
-        is_new: bool = None,
-        is_offline: bool = None,
-        no_op: bool = None,
-        name: str = None,
-        description: str = None,
-        tags: List[str] = None,
+        artifacts_path: Optional[str] = None,
+        collect_artifacts: Optional[bool] = None,
+        collect_resources: Optional[bool] = None,
+        is_new: Optional[bool] = None,
+        is_offline: Optional[bool] = None,
+        no_op: Optional[bool] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        tags: Optional[List[str]] = None,
         auto_create: bool = True,
     ):
         super().__init__(
             owner=owner,
             project=project,
             run_uuid=run_uuid,
             client=client,
@@ -189,24 +189,24 @@
             self.log_env()
 
         # Track code
         if is_new and track_code:
             self.log_code_ref()
 
         if is_new and self._artifacts_path and track_logs:
-            setup_logging(add_logs=self._add_logs)
+            start_log_processor(add_logs=self._add_logs)
 
         self._set_exit_handler(is_new=is_new)
 
     def _init_artifacts_tracking(
         self,
-        artifacts_path: str = None,
-        collect_artifacts: bool = None,
-        collect_resources: bool = None,
-        is_new: bool = None,
+        artifacts_path: Optional[str] = None,
+        collect_artifacts: Optional[bool] = None,
+        collect_resources: Optional[bool] = None,
+        is_new: Optional[bool] = None,
     ):
         if (settings.CLIENT_CONFIG.is_managed and self.run_uuid) or artifacts_path:
             self.set_artifacts_path(artifacts_path, is_related=is_new)
         if not self._artifacts_path and self._is_offline:
             self.set_artifacts_path(artifacts_path)
 
         # no artifacts path is set, we use the temp path
@@ -244,27 +244,23 @@
             )
 
     def _persist_logs_history(self):
         if self._logs_history.logs and len(self._logs_history.logs) > 0:
             logs_path = os.path.join(
                 self._artifacts_path,
                 "plxlogs",
-                "{}.plx".format(
-                    datetime.timestamp(self._logs_history.logs[-1].timestamp)
-                ),
+                "{}".format(datetime.timestamp(self._logs_history.logs[-1].timestamp)),
             )
             check_or_create_path(logs_path, is_dir=False)
             with open(logs_path, "w") as logs_file:
-                logs_file.write(
-                    "{}\n{}".format(
-                        self._logs_history.get_csv_header(), self._logs_history.to_csv()
-                    )
-                )
+                logs_file.write(self._logs_history.to_json())
 
     def _add_logs(self, log: V1Log):
+        if not log:
+            return
         self._logs_history.logs.append(log)
         if V1Logs.should_chunk(self._logs_history.logs):
             self._persist_logs_history()
             # Reset
             self._logs_history = V1Logs(logs=[])
 
     def create(self, **kwargs):
@@ -282,15 +278,15 @@
             return None
         self._store_path = os.path.join(connection.store_path, self.run_uuid)
         return self._store_path
 
     @client_handler(check_no_op=True)
     def get_artifacts_path(
         self,
-        rel_path: str = None,
+        rel_path: Optional[str] = None,
         ensure_path: bool = False,
         is_dir: bool = False,
         use_store_path: bool = False,
     ):
         """Get the absolute path of the specified artifact in the currently active run.
 
         If `rel_path` is specified, the artifact root path of the currently active
@@ -327,15 +323,15 @@
                     logger.debug("Failed ensuring paths {}. Error {}", path, e)
             return path
         return artifacts_path
 
     @client_handler(check_no_op=True)
     def get_outputs_path(
         self,
-        rel_path: str = None,
+        rel_path: Optional[str] = None,
         ensure_path: bool = True,
         is_dir: bool = False,
         use_store_path: bool = False,
     ):
         """Get the absolute outputs path of the specified artifact in the currently active run.
 
         If `rel_path` is specified, the outputs artifact root path of the currently active
@@ -396,15 +392,17 @@
             str, outputs_path/rel_path
         """
         path = self.get_outputs_path(rel_path, use_store_path=use_store_path)
         self.log_tensorboard_ref(path)
         return path
 
     @client_handler(check_no_op=True)
-    def set_artifacts_path(self, artifacts_path: str = None, is_related: bool = False):
+    def set_artifacts_path(
+        self, artifacts_path: Optional[str] = None, is_related: bool = False
+    ):
         """Sets the root artifacts_path.
 
         > **Note**: Both `in-cluster` and `offline` modes will call this method automatically.
         > Be careful, this method is called automatically. Polyaxon has some processes
         > to automatically sync your run's artifacts and outputs.
 
         Args:
@@ -456,15 +454,15 @@
         > Be careful, this method is called automatically. Polyaxon has some processes
         > to automatically sync your run's artifacts and outputs.
         """
         self._resource_logger = ResourceFileWriter(run_path=self._artifacts_path)
 
     @client_handler(check_no_op=True)
     def set_run_process_sidecar(self):
-        """Sets an sidecar process to sync artifacts.
+        """Sets a sidecar process to sync artifacts.
 
         > **Note**: Both `in-cluster` and `offline` modes will call this method automatically.
         > Be careful, this method is called automatically. Polyaxon has some processes
         > to automatically sync your run's artifacts and outputs.
         """
         self._sidecar = SidecarThread(client=self, run_path=self._artifacts_path)
         self._sidecar.start()
@@ -473,15 +471,19 @@
         if self._is_offline or is_new:
             self._start()
         elif settings.CLIENT_CONFIG.is_managed:
             self._register_exit_handler(self._wait)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_metric(
-        self, name: str, value: float, step: int = None, timestamp: datetime = None
+        self,
+        name: str,
+        value: float,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a metric datapoint.
 
         ```python
         >>> log_metric(name="loss", value=0.01, step=10)
         ```
 
@@ -512,15 +514,20 @@
             )
         )
         if events:
             self._add_events(events)
             self._results[name] = event_value
 
     @client_handler(check_no_op=True, can_log_events=True)
-    def log_metrics(self, step: int = None, timestamp: datetime = None, **metrics):
+    def log_metrics(
+        self,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
+        **metrics,
+    ):
         """Logs multiple metrics.
 
         ```python
         >>> log_metrics(step=123, loss=0.023, accuracy=0.91)
         ```
 
         > **Note**: It's very important to log `step` as one of your metrics
@@ -555,16 +562,16 @@
     @client_handler(check_no_op=True, can_log_events=True)
     def log_roc_auc_curve(
         self,
         name: str,
         fpr,
         tpr,
         auc=None,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs ROC/AUC curve. This method expects an already processed values.
 
         ```python
         >>> log_roc_auc_curve("roc_value", fpr, tpr, auc=0.6, step=1)
         ```
         Args:
@@ -592,16 +599,16 @@
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_sklearn_roc_auc_curve(
         self,
         name: str,
         y_preds,
         y_targets,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
         is_multi_class: bool = False,
     ):
         """Calculates and logs ROC/AUC curve using sklearn.
 
         ```python
         >>> log_sklearn_roc_auc_curve("roc_value", y_preds, y_targets, step=10)
         ```
@@ -647,16 +654,16 @@
     @client_handler(check_no_op=True, can_log_events=True)
     def log_pr_curve(
         self,
         name: str,
         precision,
         recall,
         average_precision=None,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs PR curve. This method expects an already processed values.
 
         ```python
         >>> log_pr_curve("pr_value", precision, recall, step=10)
         ```
 
@@ -684,16 +691,16 @@
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_sklearn_pr_curve(
         self,
         name: str,
         y_preds,
         y_targets,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
         is_multi_class: bool = False,
     ):
         """Calculates and logs PR curve using sklearn.
 
         ```python
         >>> log_sklearn_pr_curve("pr_value", y_preds, y_targets, step=10)
         ```
@@ -739,16 +746,16 @@
     @client_handler(check_no_op=True, can_log_events=True)
     def log_curve(
         self,
         name: str,
         x,
         y,
         annotation=None,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a custom curve.
 
         ```python
         >>> log_curve("pr_value", x, y, annotation="more=info", step=10)
         ```
 
@@ -778,16 +785,16 @@
     @client_handler(check_no_op=True, can_log_events=True)
     def log_confusion_matrix(
         self,
         name: str,
         x,
         y,
         z,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a custom curve.
 
         ```python
         >>> z = [[0.1, 0.3, 0.5, 0.2],
         >>>      [1.0, 0.8, 0.6, 0.1],
         >>>      [0.1, 0.3, 0.6, 0.9],
@@ -832,20 +839,20 @@
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_image(
         self,
         data,
-        name: str = None,
-        step: int = None,
-        timestamp: datetime = None,
+        name: Optional[str] = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
         rescale: int = 1,
         dataformats: str = "CHW",
-        ext: str = None,
+        ext: Optional[str] = None,
     ):
         """Logs an image.
 
         ```python
         >>> log_image(data="path/to/image.png", step=10)
         >>> log_image(data=np_array, name="generated_image", step=10)
         ```
@@ -913,17 +920,17 @@
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_image_with_boxes(
         self,
         tensor_image,
         tensor_boxes,
-        name: str = None,
-        step: int = None,
-        timestamp: datetime = None,
+        name: Optional[str] = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
         rescale: int = 1,
         dataformats: str = "CHW",
     ):
         """Logs an image with bounding boxes.
 
         ```python
         >>> log_image_with_boxes(
@@ -971,18 +978,18 @@
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_mpl_image(
         self,
         data,
-        name: str = None,
+        name: Optional[str] = None,
         close: bool = True,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a matplotlib image.
 
         ```python
         >>> log_mpl_image(name="figure", data=figure, step=1, close=False)
         ```
 
@@ -1018,19 +1025,19 @@
                 dataformats="CHW",
             )
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_video(
         self,
         data,
-        name: str = None,
+        name: Optional[str] = None,
         fps: int = 4,
-        step: int = None,
-        timestamp: datetime = None,
-        content_type: str = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
+        content_type: Optional[str] = None,
     ):
         """Logs a video.
 
         ```python
         >>> log_video("path/to/my_video1"),
         >>> log_video(
         >>>     name="my_vide2",
@@ -1091,19 +1098,19 @@
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_audio(
         self,
         data,
-        name: str = None,
+        name: Optional[str] = None,
         sample_rate: int = 44100,
-        step: int = None,
-        timestamp: datetime = None,
-        content_type: str = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
+        content_type: Optional[str] = None,
     ):
         """Logs a audio.
 
         ```python
         >>> log_audio("path/to/my_audio1"),
         >>> log_audio(name="my_audio2", data=np.arange(np.prod((42,)), dtype=float).reshape((42,)))
         ```
@@ -1159,15 +1166,19 @@
             kind=V1ArtifactKind.AUDIO,
             event=V1Event.make(timestamp=timestamp, step=step, audio=event_value),
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_text(
-        self, name: str, text: str, step: int = None, timestamp: datetime = None
+        self,
+        name: str,
+        text: str,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a text.
 
         ```python
         >>> log_text(name="text", text="value")
         ```
 
@@ -1185,15 +1196,19 @@
             kind=V1ArtifactKind.TEXT,
             event=V1Event.make(timestamp=timestamp, step=step, text=text),
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_html(
-        self, name: str, html: str, step: int = None, timestamp: datetime = None
+        self,
+        name: str,
+        html: str,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs an html.
 
         ```python
         >>> log_html(name="text", html="<p>value</p>")
         ```
 
@@ -1211,15 +1226,20 @@
             kind=V1ArtifactKind.HTML,
             event=V1Event.make(timestamp=timestamp, step=step, html=html),
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_np_histogram(
-        self, name: str, values, counts, step: int = None, timestamp: datetime = None
+        self,
+        name: str,
+        values,
+        counts,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a numpy histogram.
 
         ```python
         >>> values, counts = np.histogram(np.random.randint(255, size=(1000,)))
         >>> log_np_histogram(name="histo1", values=values, counts=counts, step=1)
         ```
@@ -1249,16 +1269,16 @@
     @client_handler(check_no_op=True, can_log_events=True)
     def log_histogram(
         self,
         name: str,
         values,
         bins,
         max_bins=None,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a histogram.
 
         ```python
         >>> log_histogram(
         >>>     name="histo",
         >>>     values=np.arange(np.prod((1024,)), dtype=float).reshape((1024,)),
@@ -1292,20 +1312,20 @@
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_model(
         self,
         path: str,
-        name: str = None,
-        framework: str = None,
-        summary: Dict = None,
-        step: int = None,
-        timestamp: datetime = None,
-        rel_path: str = None,
+        name: Optional[str] = None,
+        framework: Optional[str] = None,
+        summary: Optional[Dict] = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
+        rel_path: Optional[str] = None,
         skip_hash_calculation: bool = False,
         **kwargs,
     ):
         """Logs a model or a versioned model if a step value is provided.
 
         This method will:
          * save the model
@@ -1375,20 +1395,20 @@
                 skip_hash_calculation=skip_hash_calculation,
             )
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_artifact(
         self,
         path: str,
-        name: str = None,
-        kind: str = None,
-        summary: Dict = None,
-        step: int = None,
-        timestamp: datetime = None,
-        rel_path: str = None,
+        name: Optional[str] = None,
+        kind: Optional[str] = None,
+        summary: Optional[Dict] = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
+        rel_path: Optional[str] = None,
         skip_hash_calculation: bool = False,
         **kwargs,
     ):
         """Logs a generic artifact or a versioned generic artifact if a step value is provided.
 
         This method will:
          * save the artifact
@@ -1461,16 +1481,16 @@
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_dataframe(
         self,
         df,
         name: str,
         content_type: str = V1ArtifactKind.CSV,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a dataframe.
 
         Args:
             df: the dataframe to save
             name: str, optional, if not provided the name of the file will be used.
             content_type: str, optional, csv or html.
@@ -1512,15 +1532,19 @@
             kind=V1ArtifactKind.DATAFRAME,
             event=V1Event.make(timestamp=timestamp, step=step, dataframe=df),
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_plotly_chart(
-        self, name: str, figure, step: int = None, timestamp: datetime = None
+        self,
+        name: str,
+        figure,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a plotly chart/figure.
 
         Args:
             name: str, name of the figure
             figure: plotly.figure
             step: int, optional
@@ -1535,15 +1559,19 @@
             kind=V1ArtifactKind.CHART,
             event=V1Event.make(timestamp=timestamp, step=step, chart=chart),
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_bokeh_chart(
-        self, name: str, figure, step: int = None, timestamp: datetime = None
+        self,
+        name: str,
+        figure,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a bokeh chart/figure.
 
         Args:
             name: str, name of the figure
             figure: bokeh.figure
             step: int, optional
@@ -1558,15 +1586,19 @@
             kind=V1ArtifactKind.CHART,
             event=V1Event.make(timestamp=timestamp, step=step, chart=chart),
         )
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_altair_chart(
-        self, name: str, figure, step: int = None, timestamp: datetime = None
+        self,
+        name: str,
+        figure,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
     ):
         """Logs a vega/altair chart/figure.
 
         Args:
             name: str, name of the figure
             figure: figure
             step: int, optional
@@ -1584,16 +1616,16 @@
         self._add_event(logged_event)
 
     @client_handler(check_no_op=True, can_log_events=True)
     def log_mpl_plotly_chart(
         self,
         name: str,
         figure,
-        step: int = None,
-        timestamp: datetime = None,
+        step: Optional[int] = None,
+        timestamp: Optional[datetime] = None,
         close: bool = True,
         fallback_to_image: bool = True,
     ):
         """Logs a matplotlib figure to plotly figure.
 
         Args:
             name: str, name of the figure
@@ -1643,15 +1675,15 @@
     def _start(self):
         if self._is_offline:
             self.load_offline_run(path=self._artifacts_path, run_client=self)
             if self.run_data.status:
                 logger.info(f"An offline run was found: {self._artifacts_path}")
             else:
                 self.log_status(
-                    polyaxon_sdk.V1Statuses.CREATED,
+                    V1Statuses.CREATED,
                     reason="OfflineOperation",
                     message="Operation is starting",
                 )
                 logger.info(f"A new offline run started: {self._artifacts_path}")
         if LifeCycle.is_pending(self.status):
             self.start()
         self._register_exit_handler(self._end)
@@ -1665,14 +1697,15 @@
             # Resume normal work
             sys.__excepthook__(exception, value, tb)
 
         sys.excepthook = excepthook
 
     def _end(self):
         self.log_succeeded()
+        end_log_processor()
         self._persist_logs_history()
         self._wait(sync_artifacts=True)
         if self._is_offline:
             self.persist_run(path=self._artifacts_path)
 
     def _wait(self, sync_artifacts: bool = False):
         if self._event_logger:
@@ -1695,29 +1728,29 @@
                 events_path=ctx_paths.CONTEXTS_SYSTEM_RESOURCES_EVENTS_SUBPATH_FORMAT.format(
                     self._artifacts_path
                 ),
             )
         time.sleep(settings.CLIENT_CONFIG.tracking_timeout)
 
     @client_handler(check_no_op=True, can_log_outputs=True)
-    def log_env(self, rel_path: str = None, content: Dict = None):
+    def log_env(self, rel_path: Optional[str] = None, content: Optional[Dict] = None):
         """Logs information about the environment.
 
         Called automatically if track_env is set to True.
 
         Can be called manually, and can accept a custom content as a form of a dictionary.
 
         Args:
             rel_path: str, optional, default "env.json".
             content: Dict, optional, default to current system information.
         """
         if not os.path.exists(self._outputs_path):
             return
         if not content:
-            content = get_run_env()
+            content = get_run_env(["polyaxon", "traceml"])
 
         rel_path = rel_path or "env.json"
         path = self._outputs_path
         if rel_path:
             path = os.path.join(path, rel_path)
 
         with open(os.path.join(path), "w") as env_file:
```

### Comparing `traceml-1.0.8/traceml/vendor/__init__.py` & `traceml-1.1.0rc0/traceml/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/exporter.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/exporter.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/base.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,20 @@
 import itertools
 from contextlib import contextmanager
 
 import numpy as np
 import matplotlib as mpl
 from matplotlib import transforms
 
+from clipped.versions import get_loose_version
+
 from .. import utils
 from .. import _py3k_compat as py3k
 
 
-def get_loose_version(vstring: str):
-    try:
-        from setuptools._distutils.version import LooseVersion
-    except ImportError:
-        from distutils.version import LooseVersion
-    return LooseVersion(vstring)
-
-
 class Renderer(object):
     @staticmethod
     def ax_zoomable(ax):
         return bool(ax and ax.get_navigate())
 
     @staticmethod
     def ax_has_xgrid(ax):
```

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/tools.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/tools.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/mplexporter/utils.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/mplexporter/utils.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/mpltools.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/mpltools.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/renderer.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/matplotlylib/tools.py` & `traceml-1.1.0rc0/traceml/vendor/matplotlylib/tools.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/vendor/pynvml.py` & `traceml-1.1.0rc0/traceml/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml/visualization/__init__.py` & `traceml-1.1.0rc0/traceml/vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.0.8/traceml.egg-info/PKG-INFO` & `traceml-1.1.0rc0/traceml.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: traceml
-Version: 1.0.8
+Version: 1.1.0rc0
 Summary: Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon.
 Home-page: https://github.com/polyaxon/traceml
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
 Keywords: polyaxon,aws,s3,microsoft,azure,google cloud storage,gcs,deep-learning,machine-learning,data-science,neural-networks,artificial-intelligence,ai,reinforcement-learning,kubernetes,aws,microsoft,azure,google cloud,tensorFlow,pytorch,matplotlib,plotly,visualization,analytics
 Platform: any
-Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Typing :: Typed
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: polyaxon
 Provides-Extra: dev
 Provides-Extra: all
 
 UNKNOWN
```

### Comparing `traceml-1.0.8/traceml.egg-info/SOURCES.txt` & `traceml-1.1.0rc0/traceml.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MANIFEST.in
 setup.cfg
 setup.py
-../CONTRIBUTING.md
+../LICENSE
 ../README.md
 traceml/__init__.py
 traceml/exceptions.py
 traceml/logger.py
 traceml/pkg.py
 traceml.egg-info/PKG-INFO
 traceml.egg-info/SOURCES.txt
@@ -51,14 +51,16 @@
 traceml/processors/events_processors/events_metrics_processors.py
 traceml/processors/events_processors/events_models_processors.py
 traceml/processors/events_processors/events_tables_processors.py
 traceml/processors/events_processors/events_video_processors.py
 traceml/serialization/__init__.py
 traceml/serialization/base.py
 traceml/serialization/writer.py
+traceml/summary/__init__.py
+traceml/summary/df.py
 traceml/tracking/__init__.py
 traceml/tracking/run.py
 traceml/vendor/__init__.py
 traceml/vendor/pynvml.py
 traceml/vendor/matplotlylib/__init__.py
 traceml/vendor/matplotlylib/mpltools.py
 traceml/vendor/matplotlylib/renderer.py
```

