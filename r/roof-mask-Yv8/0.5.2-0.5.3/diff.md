# Comparing `tmp/roof_mask_Yv8-0.5.2.tar.gz` & `tmp/roof_mask_Yv8-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roof_mask_Yv8-0.5.2.tar", last modified: Thu Apr  6 17:58:59 2023, max compression
+gzip compressed data, was "roof_mask_Yv8-0.5.3.tar", last modified: Fri Apr  7 17:38:27 2023, max compression
```

## Comparing `roof_mask_Yv8-0.5.2.tar` & `roof_mask_Yv8-0.5.3.tar`

### file list

```diff
@@ -1,14 +1,182 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-06 17:58:58.006351 roof_mask_Yv8-0.5.2/
--rwxrwxrwx   0 root         (0) root         (0)      429 2023-04-06 17:58:59.476546 roof_mask_Yv8-0.5.2/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-06 17:58:58.048326 roof_mask_Yv8-0.5.2/roof_mask_Yv8.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      429 2023-04-06 17:58:57.000000 roof_mask_Yv8-0.5.2/roof_mask_Yv8.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      265 2023-04-06 17:58:57.000000 roof_mask_Yv8-0.5.2/roof_mask_Yv8.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-06 17:58:57.000000 roof_mask_Yv8-0.5.2/roof_mask_Yv8.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2023-04-06 17:58:57.000000 roof_mask_Yv8-0.5.2/roof_mask_Yv8.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-06 17:58:59.552547 roof_mask_Yv8-0.5.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      604 2023-04-06 17:47:41.000000 roof_mask_Yv8-0.5.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-06 17:58:58.122284 roof_mask_Yv8-0.5.2/yolo_roof/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.2/yolo_roof/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    26220 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.2/yolo_roof/detect_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    21374 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.2/yolo_roof/geo_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    45837 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.2/yolo_roof/report_functions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.684330 roof_mask_Yv8-0.5.3/
+-rwxrwxrwx   0 root         (0) root         (0)      429 2023-04-07 17:38:26.946950 roof_mask_Yv8-0.5.3/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.728304 roof_mask_Yv8-0.5.3/detectron2/
+-rwxrwxrwx   0 root         (0) root         (0)      258 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.786271 roof_mask_Yv8-0.5.3/detectron2/checkpoint/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/checkpoint/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17782 2023-04-07 16:23:15.000000 roof_mask_Yv8-0.5.3/detectron2/checkpoint/c2_model_loading.py
+-rwxrwxrwx   0 root         (0) root         (0)     5685 2023-04-07 16:23:15.000000 roof_mask_Yv8-0.5.3/detectron2/checkpoint/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     5258 2023-04-07 16:23:15.000000 roof_mask_Yv8-0.5.3/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.839241 roof_mask_Yv8-0.5.3/detectron2/config/
+-rwxrwxrwx   0 root         (0) root         (0)      599 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7890 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/compat.py
+-rwxrwxrwx   0 root         (0) root         (0)     9211 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    29512 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)     2719 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/instantiate.py
+-rwxrwxrwx   0 root         (0) root         (0)    14944 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/config/lazy.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.887214 roof_mask_Yv8-0.5.3/detectron2/data/
+-rwxrwxrwx   0 root         (0) root         (0)      644 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7378 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/benchmark.py
+-rwxrwxrwx   0 root         (0) root         (0)    20605 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     7224 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     9164 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/common.py
+-rwxrwxrwx   0 root         (0) root         (0)     8169 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/dataset_mapper.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.944181 roof_mask_Yv8-0.5.3/detectron2/data/datasets/
+-rwxrwxrwx   0 root         (0) root         (0)      523 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10174 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/builtin.py
+-rwxrwxrwx   0 root         (0) root         (0)    21841 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/builtin_meta.py
+-rwxrwxrwx   0 root         (0) root         (0)    13167 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/cityscapes.py
+-rwxrwxrwx   0 root         (0) root         (0)     7821 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/cityscapes_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)    23465 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/coco.py
+-rwxrwxrwx   0 root         (0) root         (0)     8977 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/coco_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)     9623 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis.py
+-rwxrwxrwx   0 root         (0) root         (0)   223757 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis_v0_5_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)   219177 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis_v1_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)    39414 2023-04-07 16:23:16.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/pascal_voc.py
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/datasets/register_coco.py
+-rwxrwxrwx   0 root         (0) root         (0)    22841 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/detection_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:05.999150 roof_mask_Yv8-0.5.3/detectron2/data/samplers/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/samplers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11789 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/samplers/distributed_sampler.py
+-rwxrwxrwx   0 root         (0) root         (0)     1944 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.065112 roof_mask_Yv8-0.5.3/detectron2/data/transforms/
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/transforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14117 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/transforms/augmentation.py
+-rwxrwxrwx   0 root         (0) root         (0)    23069 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/transforms/augmentation_impl.py
+-rwxrwxrwx   0 root         (0) root         (0)    12629 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/data/transforms/transform.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.104090 roof_mask_Yv8-0.5.3/detectron2/engine/
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26868 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)    25497 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     4089 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/launch.py
+-rwxrwxrwx   0 root         (0) root         (0)    14104 2023-04-07 16:23:17.000000 roof_mask_Yv8-0.5.3/detectron2/engine/train_loop.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.160057 roof_mask_Yv8-0.5.3/detectron2/evaluation/
+-rwxrwxrwx   0 root         (0) root         (0)      671 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8369 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/cityscapes_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    30423 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8156 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/evaluator.py
+-rwxrwxrwx   0 root         (0) root         (0)     5078 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/fast_eval_api.py
+-rwxrwxrwx   0 root         (0) root         (0)    15018 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/lvis_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7500 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/panoptic_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    10862 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/pascal_voc_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7608 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/rotated_coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8191 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/sem_seg_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     2614 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/evaluation/testing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.216026 roof_mask_Yv8-0.5.3/detectron2/export/
+-rwxrwxrwx   0 root         (0) root         (0)      336 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9280 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/api.py
+-rwxrwxrwx   0 root         (0) root         (0)    21035 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/c10.py
+-rwxrwxrwx   0 root         (0) root         (0)     7803 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/caffe2_export.py
+-rwxrwxrwx   0 root         (0) root         (0)     6674 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/caffe2_inference.py
+-rwxrwxrwx   0 root         (0) root         (0)    17034 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/caffe2_modeling.py
+-rwxrwxrwx   0 root         (0) root         (0)     5033 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/caffe2_patch.py
+-rwxrwxrwx   0 root         (0) root         (0)    11807 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/flatten.py
+-rwxrwxrwx   0 root         (0) root         (0)    38071 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/shared.py
+-rwxrwxrwx   0 root         (0) root         (0)     5008 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/torchscript.py
+-rwxrwxrwx   0 root         (0) root         (0)    11526 2023-04-07 16:23:18.000000 roof_mask_Yv8-0.5.3/detectron2/export/torchscript_patch.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.270995 roof_mask_Yv8-0.5.3/detectron2/layers/
+-rwxrwxrwx   0 root         (0) root         (0)      839 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5764 2023-04-07 16:23:19.000000 roof_mask_Yv8-0.5.3/detectron2/layers/aspp.py
+-rwxrwxrwx   0 root         (0) root         (0)    12131 2023-04-07 16:23:19.000000 roof_mask_Yv8-0.5.3/detectron2/layers/batch_norm.py
+-rwxrwxrwx   0 root         (0) root         (0)     3024 2023-04-07 16:23:19.000000 roof_mask_Yv8-0.5.3/detectron2/layers/blocks.py
+-rwxrwxrwx   0 root         (0) root         (0)    16978 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/deform_conv.py
+-rwxrwxrwx   0 root         (0) root         (0)     4204 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/losses.py
+-rwxrwxrwx   0 root         (0) root         (0)    10881 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/mask_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     6490 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/nms.py
+-rwxrwxrwx   0 root         (0) root         (0)     3098 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/roi_align.py
+-rwxrwxrwx   0 root         (0) root         (0)     3302 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/roi_align_rotated.py
+-rwxrwxrwx   0 root         (0) root         (0)      652 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/rotated_boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/shape_spec.py
+-rwxrwxrwx   0 root         (0) root         (0)     4893 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/layers/wrappers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.325963 roof_mask_Yv8-0.5.3/detectron2/modeling/
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15443 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/anchor_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.379932 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/
+-rwxrwxrwx   0 root         (0) root         (0)      475 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1543 2023-04-07 16:23:20.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/backbone.py
+-rwxrwxrwx   0 root         (0) root         (0)     1015 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    10055 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    16656 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/regnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    23658 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/backbone/resnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    15123 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/box_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     6264 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/matcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.429904 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/
+-rwxrwxrwx   0 root         (0) root         (0)      508 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      814 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    11550 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/dense_detector.py
+-rwxrwxrwx   0 root         (0) root         (0)    13213 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/fcos.py
+-rwxrwxrwx   0 root         (0) root         (0)    10335 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    13710 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    18265 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/retinanet.py
+-rwxrwxrwx   0 root         (0) root         (0)     9720 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/meta_arch/semantic_seg.py
+-rwxrwxrwx   0 root         (0) root         (0)    10832 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/mmdet_wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)    11316 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/poolers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4046 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/postprocessing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.489869 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/
+-rwxrwxrwx   0 root         (0) root         (0)      231 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      836 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8128 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/proposal_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    23814 2023-04-07 16:23:21.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/rpn.py
+-rwxrwxrwx   0 root         (0) root         (0)     8807 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.544838 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/
+-rwxrwxrwx   0 root         (0) root         (0)      768 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4077 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/box_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12990 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    25274 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    11156 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/keypoint_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12169 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/mask_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    37701 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/roi_heads.py
+-rwxrwxrwx   0 root         (0) root         (0)    11158 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)     2334 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/sampling.py
+-rwxrwxrwx   0 root         (0) root         (0)    12416 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/modeling/test_time_augmentation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.588813 roof_mask_Yv8-0.5.3/detectron2/solver/
+-rwxrwxrwx   0 root         (0) root         (0)      298 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/solver/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11127 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/solver/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8648 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/solver/lr_scheduler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.642782 roof_mask_Yv8-0.5.3/detectron2/structures/
+-rwxrwxrwx   0 root         (0) root         (0)      645 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14429 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/structures/boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)     4557 2023-04-07 16:23:22.000000 roof_mask_Yv8-0.5.3/detectron2/structures/image_list.py
+-rwxrwxrwx   0 root         (0) root         (0)     6542 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/instances.py
+-rwxrwxrwx   0 root         (0) root         (0)     9030 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/keypoints.py
+-rwxrwxrwx   0 root         (0) root         (0)    19802 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/masks.py
+-rwxrwxrwx   0 root         (0) root         (0)    18853 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/structures/rotated_boxes.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.694752 roof_mask_Yv8-0.5.3/detectron2/tracking/
+-rwxrwxrwx   0 root         (0) root         (0)      580 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/base_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)    11858 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     7486 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/hungarian_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     4142 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     1106 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     5288 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.750720 roof_mask_Yv8-0.5.3/detectron2/utils/
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6017 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)     8391 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/collect_env.py
+-rwxrwxrwx   0 root         (0) root         (0)     4096 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/colormap.py
+-rwxrwxrwx   0 root         (0) root         (0)     5610 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/comm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1838 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/develop.py
+-rwxrwxrwx   0 root         (0) root         (0)     5644 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/env.py
+-rwxrwxrwx   0 root         (0) root         (0)    17024 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/events.py
+-rwxrwxrwx   0 root         (0) root         (0)     1189 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/file_io.py
+-rwxrwxrwx   0 root         (0) root         (0)     7807 2023-04-07 16:23:23.000000 roof_mask_Yv8-0.5.3/detectron2/utils/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2583 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/memory.py
+-rwxrwxrwx   0 root         (0) root         (0)     1874 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/registry.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/serialize.py
+-rwxrwxrwx   0 root         (0) root         (0)     4833 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/testing.py
+-rwxrwxrwx   0 root         (0) root         (0)    11319 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/video_visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    51159 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    52915 2023-04-07 16:23:24.000000 roof_mask_Yv8-0.5.3/detectron2/utils/visualizer_new.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.789698 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      429 2023-04-07 17:38:04.000000 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5655 2023-04-07 17:38:05.000000 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-07 17:38:04.000000 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-04-07 17:38:05.000000 roof_mask_Yv8-0.5.3/roof_mask_Yv8.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-07 17:38:27.030951 roof_mask_Yv8-0.5.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      604 2023-04-07 17:37:51.000000 roof_mask_Yv8-0.5.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:38:06.841668 roof_mask_Yv8-0.5.3/yolo_roof/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.3/yolo_roof/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26220 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.3/yolo_roof/detect_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    21374 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.3/yolo_roof/geo_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    45837 2023-04-06 16:59:40.000000 roof_mask_Yv8-0.5.3/yolo_roof/report_functions.py
```

### Comparing `roof_mask_Yv8-0.5.2/setup.py` & `roof_mask_Yv8-0.5.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## test upload
 import setuptools
 
 setuptools.setup(
     name = "roof_mask_Yv8",
-    version = "0.5.2",
+    version = "0.5.3",
     author = "Ruixu",
     author_email = "lrxjason@gmail.com",
     description = "upload pip package test",
     long_description = 'package supporting Yolo_v8 roof model deployment',
     long_description_content_type="text/markdown",
     url="https://github.com/lrxjason/roof_model_test/",
     packages=setuptools.find_packages(),
```

### Comparing `roof_mask_Yv8-0.5.2/yolo_roof/detect_functions.py` & `roof_mask_Yv8-0.5.3/yolo_roof/detect_functions.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.2/yolo_roof/geo_functions.py` & `roof_mask_Yv8-0.5.3/yolo_roof/geo_functions.py`

 * *Files identical despite different names*

### Comparing `roof_mask_Yv8-0.5.2/yolo_roof/report_functions.py` & `roof_mask_Yv8-0.5.3/yolo_roof/report_functions.py`

 * *Files identical despite different names*

