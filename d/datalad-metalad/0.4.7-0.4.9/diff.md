# Comparing `tmp/datalad_metalad-0.4.7.tar.gz` & `tmp/datalad_metalad-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_metalad-0.4.7.tar", last modified: Wed Sep 28 15:18:00 2022, max compression
+gzip compressed data, was "datalad_metalad-0.4.9.tar", last modified: Thu Sep 29 08:17:40 2022, max compression
```

## Comparing `datalad_metalad-0.4.7.tar` & `datalad_metalad-0.4.9.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.752961 datalad_metalad-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9316 2022-09-28 15:18:00.752961 datalad_metalad-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8803 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.752961 datalad_metalad-0.4.7/datalad_metalad/
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-28 15:18:00.752961 datalad_metalad-0.4.7/datalad_metalad/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    31603 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/add.py
--rw-r--r--   0 runner    (1001) docker     (121)    22309 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (121)    19425 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/conduct.py
--rw-r--r--   0 runner    (1001) docker     (121)    19950 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/dump.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    32185 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.740960 datalad_metalad-0.4.7/datalad_metalad/extractors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/annex.py
--rw-r--r--   0 runner    (1001) docker     (121)    14091 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    17878 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/custom.py
--rw-r--r--   0 runner    (1001) docker     (121)     4808 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/external.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/external_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/external_file.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.744960 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/annex.py
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3625 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/datacite.py
--rw-r--r--   0 runner    (1001) docker     (121)     4814 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/datalad_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3694 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/datalad_rfc822.py
--rw-r--r--   0 runner    (1001) docker     (121)     5990 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/exif.py
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/frictionless_datapackage.py
--rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/image.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.744960 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.744960 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)     5702 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/data/audio.mp3
--rw-r--r--   0 runner    (1001) docker     (121)    33891 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/data/exif.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    15920 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/data/nifti1.nii.gz
--rw-r--r--   0 runner    (1001) docker     (121)    19350 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/data/xmp.pdf
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_datacite_xml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2822 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_exif.py
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_frictionless_datapackage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_rfc822.py
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_xmp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/xmp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/metalad_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/metalad_example_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     9905 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/runprov.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.744960 datalad_metalad-0.4.7/datalad_metalad/extractors/studyminimeta/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/studyminimeta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16358 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/studyminimeta/ldcreator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4033 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/studyminimeta/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.744960 datalad_metalad-0.4.7/datalad_metalad/extractors/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_annex.py
--rw-r--r--   0 runner    (1001) docker     (121)     5997 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6859 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (121)     4324 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_runprov.py
--rw-r--r--   0 runner    (1001) docker     (121)    19832 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_studyminimeta.py
--rw-r--r--   0 runner    (1001) docker     (121)    11949 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.744960 datalad_metalad-0.4.7/datalad_metalad/filters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/filters/demofilter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/indexers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/indexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/indexers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3854 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/indexers/jsonld.py
--rw-r--r--   0 runner    (1001) docker     (121)     6587 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/indexers/studyminimeta.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/indexers/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/indexers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8635 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/indexers/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     8404 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/indexers/tests/test_jsonld.py
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/indexers/tests/test_studyminimeta.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/metadatatypes/
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/metadatatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4864 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/metadatatypes/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/metadatatypes/result.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/metadatautils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/pathutils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4323 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pathutils/metadataurlparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pathutils/mtreesearch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/pathutils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pathutils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pathutils/tests/test_metadataurlparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4533 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pathutils/tests/test_mtreesearch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/pipeline/consumer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5829 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/consumer/add.py
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/consumer/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/documentedinterface.py
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelinedata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelineelement.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelines/extract_metadata_autoget_autodrop_pipeline.json
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelines/extract_metadata_autoget_pipeline.json
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelines/extract_metadata_consume_pipeline.json
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelines/extract_metadata_pipeline.json
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelines/filter_metadata_pipeline.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/add.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/autodrop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/autoget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.748961 datalad_metalad-0.4.7/datalad_metalad/pipeline/provider/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/provider/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7928 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/provider/datasettraverse.py
--rw-r--r--   0 runner    (1001) docker     (121)     3390 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/pipeline/provider/metadatatraverse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.752961 datalad_metalad-0.4.7/datalad_metalad/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36949 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (121)     9347 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/tests/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (121)     6673 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/tests/test_conduct.py
--rw-r--r--   0 runner    (1001) docker     (121)    20570 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/tests/test_locking.py
--rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/datalad_metalad/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 15:18:00.740960 datalad_metalad-0.4.7/datalad_metalad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9316 2022-09-28 15:18:00.000000 datalad_metalad-0.4.7/datalad_metalad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-09-28 15:18:00.000000 datalad_metalad-0.4.7/datalad_metalad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 15:18:00.000000 datalad_metalad-0.4.7/datalad_metalad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-09-28 15:18:00.000000 datalad_metalad-0.4.7/datalad_metalad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-28 15:18:00.000000 datalad_metalad-0.4.7/datalad_metalad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-28 15:18:00.000000 datalad_metalad-0.4.7/datalad_metalad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-09-28 15:18:00.752961 datalad_metalad-0.4.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3985 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-09-28 15:17:48.000000 datalad_metalad-0.4.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.558696 datalad_metalad-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9316 2022-09-29 08:17:40.558696 datalad_metalad-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8803 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.558696 datalad_metalad-0.4.9/datalad_metalad/
+-rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-09-29 08:17:40.558696 datalad_metalad-0.4.9/datalad_metalad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31603 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/add.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22309 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19425 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/conduct.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19950 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32896 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.550695 datalad_metalad-0.4.9/datalad_metalad/extractors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/annex.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14091 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17878 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7044 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/custom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4808 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/external.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/external_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/external_file.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.550695 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2789 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/annex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3625 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/datacite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4814 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/datalad_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3694 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/datalad_rfc822.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5990 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/exif.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/frictionless_datapackage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3467 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/image.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.550695 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.550695 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     5702 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/data/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (121)    33891 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/data/exif.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    15920 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/data/nifti1.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    19350 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/data/xmp.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_datacite_xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2822 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_exif.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_frictionless_datapackage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_rfc822.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/xmp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/metalad_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/metalad_example_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9905 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/runprov.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.550695 datalad_metalad-0.4.9/datalad_metalad/extractors/studyminimeta/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/studyminimeta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16358 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/studyminimeta/ldcreator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4033 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/studyminimeta/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.550695 datalad_metalad-0.4.9/datalad_metalad/extractors/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_annex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5997 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6859 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4324 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_runprov.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19832 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_studyminimeta.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11949 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.554695 datalad_metalad-0.4.9/datalad_metalad/filters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/filters/demofilter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.554695 datalad_metalad-0.4.9/datalad_metalad/indexers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/indexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/indexers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3854 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/indexers/jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6587 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/indexers/studyminimeta.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.554695 datalad_metalad-0.4.9/datalad_metalad/indexers/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/indexers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8635 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/indexers/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8404 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/indexers/tests/test_jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/indexers/tests/test_studyminimeta.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.554695 datalad_metalad-0.4.9/datalad_metalad/metadatatypes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/metadatatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4864 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/metadatatypes/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/metadatatypes/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/metadatautils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.554695 datalad_metalad-0.4.9/datalad_metalad/pathutils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4323 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pathutils/metadataurlparser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pathutils/mtreesearch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.554695 datalad_metalad-0.4.9/datalad_metalad/pathutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pathutils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pathutils/tests/test_metadataurlparser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4533 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pathutils/tests/test_mtreesearch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.554695 datalad_metalad-0.4.9/datalad_metalad/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.554695 datalad_metalad-0.4.9/datalad_metalad/pipeline/consumer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5829 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/consumer/add.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/consumer/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/documentedinterface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelinedata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelineelement.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.554695 datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelines/extract_metadata_autoget_autodrop_pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelines/extract_metadata_autoget_pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelines/extract_metadata_consume_pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelines/extract_metadata_pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelines/filter_metadata_pipeline.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.558696 datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/add.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/autodrop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/autoget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.558696 datalad_metalad-0.4.9/datalad_metalad/pipeline/provider/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7928 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/provider/datasettraverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3390 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/pipeline/provider/metadatatraverse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.558696 datalad_metalad-0.4.9/datalad_metalad/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36949 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9347 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/tests/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6673 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/tests/test_conduct.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20570 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4078 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/tests/test_locking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/datalad_metalad/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 08:17:40.546695 datalad_metalad-0.4.9/datalad_metalad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9316 2022-09-29 08:17:40.000000 datalad_metalad-0.4.9/datalad_metalad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-09-29 08:17:40.000000 datalad_metalad-0.4.9/datalad_metalad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 08:17:40.000000 datalad_metalad-0.4.9/datalad_metalad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-09-29 08:17:40.000000 datalad_metalad-0.4.9/datalad_metalad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-29 08:17:40.000000 datalad_metalad-0.4.9/datalad_metalad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-29 08:17:40.000000 datalad_metalad-0.4.9/datalad_metalad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      882 2022-09-29 08:17:40.558696 datalad_metalad-0.4.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3985 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-09-29 08:17:25.000000 datalad_metalad-0.4.9/versioneer.py
```

### Comparing `datalad_metalad-0.4.7/COPYING` & `datalad_metalad-0.4.9/COPYING`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/PKG-INFO` & `datalad_metalad-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: datalad_metalad
-Version: 0.4.7
+Version: 0.4.9
 Summary: DataLad extension for semantic metadata handling
 Home-page: https://github.com/datalad/datalad-metalad
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: COPYING
 
 # DataLad extension for semantic metadata handling
 
 [![Build_status](https://ci.appveyor.com/api/projects/status/hlwg6yi008mbmr1m?svg=true)](https://ci.appveyor.com/project/mih/datalad-metalad) [![codecov.io](https://codecov.io/github/datalad/datalad-metalad/coverage.svg?branch=master)](https://codecov.io/github/datalad/datalad-metalad?branch=master) [![GitHub release](https://img.shields.io/github/release/datalad/datalad-metalad.svg)](https://GitHub.com/datalad/datalad-metalad/releases/) [![PyPI version fury.io](https://badge.fury.io/py/datalad-metalad.svg)](https://pypi.python.org/pypi/datalad-metalad/) [![Documentation](https://readthedocs.org/projects/datalad-metalad/badge/?version=latest)](http://docs.datalad.org/projects/metalad/en/latest)
```

### Comparing `datalad_metalad-0.4.7/README.md` & `datalad_metalad-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/__init__.py` & `datalad_metalad-0.4.9/datalad_metalad/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """DataLad MetaLad extension"""
 import os
 import hashlib
 
-from datalad.support.digests import Digester
-
 
 __docformat__ = 'restructuredtext'
 
 
 # defines a datalad command suite
 # this symbol must be identified as a setuptools entrypoint
 # to be found by datalad
@@ -78,14 +76,16 @@
     always around. Identify the GITSHA as such, and in a similar manner
     to git-annex's style.
 
     Any ID string is prefixed with 'datalad:' to identify it as a
     DataLad-recognized ID. This prefix is defined in the main JSON-LD
     context defintion.
     """
+    from datalad.support.digests import Digester
+
     id_ = rec['key'] if 'key' in rec else 'SHA1-s{}--{}'.format(
         rec['bytesize'] if 'bytesize' in rec
         else 0 if rec['type'] == 'symlink'
         else os.stat(rec['path']).st_size,
         rec['gitshasum'] if 'gitshasum' in rec
         else Digester(digests=['sha1'])(rec['path'])['sha1'])
     return 'datalad:{}'.format(id_)
```

### Comparing `datalad_metalad-0.4.7/datalad_metalad/add.py` & `datalad_metalad-0.4.9/datalad_metalad/add.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/aggregate.py` & `datalad_metalad-0.4.9/datalad_metalad/aggregate.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/conduct.py` & `datalad_metalad-0.4.9/datalad_metalad/conduct.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/dump.py` & `datalad_metalad-0.4.9/datalad_metalad/dump.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/exceptions.py` & `datalad_metalad-0.4.9/datalad_metalad/exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extract.py` & `datalad_metalad-0.4.9/datalad_metalad/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,16 +484,37 @@
 def get_extractor_class(extractor_name: str) -> Union[
                                             Type[DatasetMetadataExtractor],
                                             Type[FileMetadataExtractor]]:
 
     """ Get an extractor from its name """
     from pkg_resources import iter_entry_points
 
-    entry_points = list(
-        iter_entry_points("datalad.metadata.extractors", extractor_name))
+    # The extractor class names of the old datalad-contained extractors have
+    # been changed, when the extractors were moved to datalad_metalad.
+    # Therefore, we have to use to extractors in
+    # `datalad_metalad.extractors.legacy` instead of any old extractor code
+    # from datalad core.
+    entry_points = [
+        entry_point
+        for entry_point in iter_entry_points(
+            "datalad.metadata.extractors",
+            extractor_name
+        )
+        if entry_point.dist.project_name != "datalad"
+    ]
+
+    if not entry_points:
+        entry_points = [
+            entry_point
+            for entry_point in iter_entry_points(
+                "datalad.metadata.extractors",
+                extractor_name
+            )
+            if entry_point.dist.project_name == "datalad"
+        ]
 
     if not entry_points:
         raise ExtractorNotFoundError(
             "Requested metadata extractor '{}' not available".format(
                 extractor_name))
 
     entry_point, ignored_entry_points = entry_points[-1], entry_points[:-1]
```

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/annex.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/annex.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/base.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/base.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/core.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/core.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/custom.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/custom.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/external.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/external.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/external_dataset.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/external_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/external_file.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/external_file.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/__init__.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/annex.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/annex.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/audio.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/audio.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/datacite.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/datacite.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/datalad_core.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/datalad_core.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/datalad_rfc822.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/datalad_rfc822.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/definitions.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/definitions.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/exif.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/exif.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/frictionless_datapackage.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/frictionless_datapackage.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/image.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/image.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/data/audio.mp3` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/data/audio.mp3`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/data/exif.jpg` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/data/exif.jpg`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/data/nifti1.nii.gz` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/data/nifti1.nii.gz`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/data/xmp.pdf` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/data/xmp.pdf`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_audio.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_audio.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,32 +8,30 @@
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 """Test audio extractor"""
 
 from pathlib import Path
 
 from datalad.tests.utils_pytest import (
     SkipTest,
-    assert_in,
-    assert_not_in,
     assert_repo_status,
     assert_result_count,
-    assert_status,
     eq_,
     with_tempfile,
 )
 
 try:
     import mutagen
 except ImportError:
     raise SkipTest
 
 from shutil import copy
 
 from datalad.api import Dataset
 
+
 target = {
     "format": "mime:audio/mp3",
     "duration(s)": 1.0,
     "name": "dltracktitle",
     "music:album": "dlalbumtitle",
     "music:artist": "dlartist",
     "music:channels": 1,
```

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_base.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_datacite_xml.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_datacite_xml.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_exif.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_exif.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_frictionless_datapackage.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_frictionless_datapackage.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_image.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_rfc822.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_rfc822.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/tests/test_xmp.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/tests/test_xmp.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/legacy/xmp.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/legacy/xmp.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/metalad_example_dataset.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/metalad_example_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/metalad_example_file.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/metalad_example_file.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/runprov.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/runprov.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/studyminimeta/ldcreator.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/studyminimeta/ldcreator.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/studyminimeta/main.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/studyminimeta/main.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_annex.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_annex.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_base.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_custom.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_runprov.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_runprov.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/extractors/tests/test_studyminimeta.py` & `datalad_metalad-0.4.9/datalad_metalad/extractors/tests/test_studyminimeta.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/filter.py` & `datalad_metalad-0.4.9/datalad_metalad/filter.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/filters/base.py` & `datalad_metalad-0.4.9/datalad_metalad/filters/base.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/filters/demofilter.py` & `datalad_metalad-0.4.9/datalad_metalad/filters/demofilter.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/indexers/base.py` & `datalad_metalad-0.4.9/datalad_metalad/indexers/base.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/indexers/jsonld.py` & `datalad_metalad-0.4.9/datalad_metalad/indexers/jsonld.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/indexers/studyminimeta.py` & `datalad_metalad-0.4.9/datalad_metalad/indexers/studyminimeta.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/indexers/tests/common.py` & `datalad_metalad-0.4.9/datalad_metalad/indexers/tests/common.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/indexers/tests/test_jsonld.py` & `datalad_metalad-0.4.9/datalad_metalad/indexers/tests/test_jsonld.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/indexers/tests/test_studyminimeta.py` & `datalad_metalad-0.4.9/datalad_metalad/indexers/tests/test_studyminimeta.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/metadatatypes/__init__.py` & `datalad_metalad-0.4.9/datalad_metalad/metadatatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/metadatatypes/metadata.py` & `datalad_metalad-0.4.9/datalad_metalad/metadatatypes/metadata.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/metadatatypes/result.py` & `datalad_metalad-0.4.9/datalad_metalad/metadatatypes/result.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/metadatautils.py` & `datalad_metalad-0.4.9/datalad_metalad/metadatautils.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pathutils/metadataurlparser.py` & `datalad_metalad-0.4.9/datalad_metalad/pathutils/metadataurlparser.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pathutils/mtreesearch.py` & `datalad_metalad-0.4.9/datalad_metalad/pathutils/mtreesearch.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pathutils/tests/test_metadataurlparser.py` & `datalad_metalad-0.4.9/datalad_metalad/pathutils/tests/test_metadataurlparser.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pathutils/tests/test_mtreesearch.py` & `datalad_metalad-0.4.9/datalad_metalad/pathutils/tests/test_mtreesearch.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/consumer/add.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/consumer/add.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/consumer/base.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/consumer/base.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/documentedinterface.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/documentedinterface.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelinedata.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelinedata.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelineelement.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelineelement.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelines/extract_metadata_autoget_autodrop_pipeline.json` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelines/extract_metadata_autoget_autodrop_pipeline.json`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/pipelines/extract_metadata_autoget_pipeline.json` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/pipelines/extract_metadata_autoget_pipeline.json`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/add.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/add.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/autodrop.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/autodrop.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/autoget.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/autoget.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/base.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/base.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/extract.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/extract.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/processor/filter.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/processor/filter.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/provider/datasettraverse.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/provider/datasettraverse.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/pipeline/provider/metadatatraverse.py` & `datalad_metalad-0.4.9/datalad_metalad/pipeline/provider/metadatatraverse.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/tests/__init__.py` & `datalad_metalad-0.4.9/datalad_metalad/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/tests/test_add.py` & `datalad_metalad-0.4.9/datalad_metalad/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/tests/test_aggregate.py` & `datalad_metalad-0.4.9/datalad_metalad/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/tests/test_conduct.py` & `datalad_metalad-0.4.9/datalad_metalad/tests/test_conduct.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/tests/test_extract.py` & `datalad_metalad-0.4.9/datalad_metalad/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/tests/test_filter.py` & `datalad_metalad-0.4.9/datalad_metalad/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/tests/test_locking.py` & `datalad_metalad-0.4.9/datalad_metalad/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/tests/utils.py` & `datalad_metalad-0.4.9/datalad_metalad/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad/utils.py` & `datalad_metalad-0.4.9/datalad_metalad/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad.egg-info/PKG-INFO` & `datalad_metalad-0.4.9/datalad_metalad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: datalad-metalad
-Version: 0.4.7
+Version: 0.4.9
 Summary: DataLad extension for semantic metadata handling
 Home-page: https://github.com/datalad/datalad-metalad
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: COPYING
 
 # DataLad extension for semantic metadata handling
 
 [![Build_status](https://ci.appveyor.com/api/projects/status/hlwg6yi008mbmr1m?svg=true)](https://ci.appveyor.com/project/mih/datalad-metalad) [![codecov.io](https://codecov.io/github/datalad/datalad-metalad/coverage.svg?branch=master)](https://codecov.io/github/datalad/datalad-metalad?branch=master) [![GitHub release](https://img.shields.io/github/release/datalad/datalad-metalad.svg)](https://GitHub.com/datalad/datalad-metalad/releases/) [![PyPI version fury.io](https://badge.fury.io/py/datalad-metalad.svg)](https://pypi.python.org/pypi/datalad-metalad/) [![Documentation](https://readthedocs.org/projects/datalad-metalad/badge/?version=latest)](http://docs.datalad.org/projects/metalad/en/latest)
```

### Comparing `datalad_metalad-0.4.7/datalad_metalad.egg-info/SOURCES.txt` & `datalad_metalad-0.4.9/datalad_metalad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/datalad_metalad.egg-info/entry_points.txt` & `datalad_metalad-0.4.9/datalad_metalad.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/setup.cfg` & `datalad_metalad-0.4.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 license = MIT
 classifiers = 
 	Programming Language :: Python
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
 
 [options]
-python_requires = >= 3.5
+python_requires = >= 3.7
 install_requires = 
 	six
+	datalad >= 0.17.6
 	datalad-metadata-model >=0.3.5,<0.4.0
 	pyyaml
 test_requires = 
 	coverage
 	pytest
 	pytest-cov
 packages = find_namespace:
```

### Comparing `datalad_metalad-0.4.7/setup.py` & `datalad_metalad-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_metalad-0.4.7/versioneer.py` & `datalad_metalad-0.4.9/versioneer.py`

 * *Files identical despite different names*

