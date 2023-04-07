# Comparing `tmp/neuralogic-0.7.4.tar.gz` & `tmp/neuralogic-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralogic-0.7.4.tar", last modified: Fri Mar  3 22:14:54 2023, max compression
+gzip compressed data, was "neuralogic-0.7.5.tar", last modified: Fri Apr  7 19:40:36 2023, max compression
```

## Comparing `neuralogic-0.7.4.tar` & `neuralogic-0.7.5.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.579422 neuralogic-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-03 22:14:45.000000 neuralogic-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-03-03 22:14:54.579422 neuralogic-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-03-03 22:14:45.000000 neuralogic-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.563422 neuralogic-0.7.4/neuralogic/
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-03 22:14:53.000000 neuralogic-0.7.4/neuralogic/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.563422 neuralogic-0.7.4/neuralogic/core/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.567422 neuralogic-0.7.4/neuralogic/core/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/builder/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/builder/dataset_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.567422 neuralogic-0.7.4/neuralogic/core/constructs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.567422 neuralogic-0.7.4/neuralogic/core/constructs/function/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/function/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/function/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/function/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/function/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/function/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/java_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/constructs/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.567422 neuralogic-0.7.4/neuralogic/core/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/settings/settings_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/core/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.567422 neuralogic-0.7.4/neuralogic/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/dataset/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/dataset/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/dataset/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/dataset/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/dataset/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.567422 neuralogic-0.7.4/neuralogic/db/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/db/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.567422 neuralogic-0.7.4/neuralogic/db/pg/
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/db/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/db/pg/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.567422 neuralogic-0.7.4/neuralogic/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/inference/evaluation_inference_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/inference/inference_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.571422 neuralogic-0.7.4/neuralogic/jar/
--rw-r--r--   0 runner    (1001) docker     (123)  2001165 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/jar/NeuraLogic.jar
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/jar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.571422 neuralogic-0.7.4/neuralogic/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.571422 neuralogic-0.7.4/neuralogic/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.571422 neuralogic-0.7.4/neuralogic/nn/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/evaluator/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/java.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.571422 neuralogic-0.7.4/neuralogic/nn/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.571422 neuralogic-0.7.4/neuralogic/nn/module/general/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/gru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/rvnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/general/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.571422 neuralogic-0.7.4/neuralogic/nn/module/gnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/appnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/gatv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/gin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/gsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/res_gated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/rgcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/sg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/gnn/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.571422 neuralogic-0.7.4/neuralogic/nn/module/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/meta/magnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/meta/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/module/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/nn/torch_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/optim/adam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/optim/lr_scheduler/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/optim/lr_scheduler/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/optim/lr_scheduler/lr_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/optim/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.563422 neuralogic-0.7.4/neuralogic/utils/data/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/bondEmbeddings3.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/
--rw-r--r--   0 runner    (1001) docker     (123)   402216 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/queries.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/embeddings.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_crosssum.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_elementProduct.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_gnn.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_graphlets.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_partial.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_product.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/data/datasets/nations/
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/nations/embeddings.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/nations/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)   205423 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/nations/queries.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/nations/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.563422 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/family/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/family/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/family/queries.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/family/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/trains/
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/trains/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/trains/queries.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/trains/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.563422 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/generalized/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/generalized/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/generalized/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/generalized/texamples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/generalized/ztexamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.575422 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/naive/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/naive/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/naive/trainExamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.579422 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/solution/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/solution/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/solution/testExamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.579422 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/vectorized/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/vectorized/template.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/xor/vectorized/trainExamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.579422 neuralogic-0.7.4/neuralogic/utils/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-03-03 22:14:45.000000 neuralogic-0.7.4/neuralogic/utils/visualize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 22:14:54.563422 neuralogic-0.7.4/neuralogic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-03-03 22:14:54.000000 neuralogic-0.7.4/neuralogic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-03-03 22:14:54.000000 neuralogic-0.7.4/neuralogic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 22:14:54.000000 neuralogic-0.7.4/neuralogic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-03 22:14:54.000000 neuralogic-0.7.4/neuralogic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-03 22:14:54.000000 neuralogic-0.7.4/neuralogic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-03 22:14:45.000000 neuralogic-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 22:14:54.579422 neuralogic-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-03 22:14:45.000000 neuralogic-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-07 19:40:25.000000 neuralogic-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-07 19:40:36.401836 neuralogic-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-07 19:40:25.000000 neuralogic-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 19:40:34.000000 neuralogic-0.7.5/neuralogic/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/core/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/builder/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/builder/dataset_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/core/constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/core/constructs/function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/function/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/java_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/constructs/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/core/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/settings/settings_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/core/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/dataset/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/db/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/db/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/db/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/db/pg/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/inference/evaluation_inference_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/inference/inference_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/jar/
+-rw-r--r--   0 runner    (1001) docker     (123)  2007653 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/jar/NeuraLogic.jar
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/jar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.393835 neuralogic-0.7.5/neuralogic/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/evaluator/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/module/general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/gru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/rvnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/general/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/module/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/appnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/gatv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/gin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/gsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/res_gated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/rgcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/sg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/gnn/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/nn/module/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/meta/magnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/meta/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/module/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/nn/torch_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/adam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/lr_scheduler/lr_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/optim/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/utils/data/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/bondEmbeddings3.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.397836 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/
+-rw-r--r--   0 runner    (1001) docker     (123)   402216 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/embeddings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_crosssum.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_elementProduct.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_gnn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_graphlets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_partial.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_product.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/embeddings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   205423 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/family/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/family/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/family/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/family/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/texamples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/generalized/ztexamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/naive/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/naive/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/naive/trainExamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/solution/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/solution/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/solution/testExamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/vectorized/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/vectorized/template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/xor/vectorized/trainExamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.401836 neuralogic-0.7.5/neuralogic/utils/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-07 19:40:25.000000 neuralogic-0.7.5/neuralogic/utils/visualize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:40:36.389835 neuralogic-0.7.5/neuralogic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 19:40:36.000000 neuralogic-0.7.5/neuralogic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 19:40:25.000000 neuralogic-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:40:36.401836 neuralogic-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-07 19:40:25.000000 neuralogic-0.7.5/setup.py
```

### Comparing `neuralogic-0.7.4/LICENSE` & `neuralogic-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/PKG-INFO` & `neuralogic-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralogic
-Version: 0.7.4
+Version: 0.7.5
 Summary: PyNeuraLogic lets you use Python to create Differentiable Logic Programs.
 Home-page: https://github.com/LukasZahradnik/PyNeuraLogic
 Author: Lukáš Zahradník
 Author-email: lukaszahradnik96@seznam.cz
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuralogic Version: 0.7.4 Summary: PyNeuraLogic
+Metadata-Version: 2.1 Name: neuralogic Version: 0.7.5 Summary: PyNeuraLogic
 lets you use Python to create Differentiable Logic Programs. Home-page: https:/
 /github.com/LukasZahradnik/PyNeuraLogic Author: LukÃ¡Å¡ ZahradnÃ­k Author-
 email: lukaszahradnik96@seznam.cz License: MIT Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `neuralogic-0.7.4/README.md` & `neuralogic-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/__init__.py` & `neuralogic-0.7.5/neuralogic/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/__init__.py` & `neuralogic-0.7.5/neuralogic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/builder/builder.py` & `neuralogic-0.7.5/neuralogic/core/builder/builder.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/builder/components.py` & `neuralogic-0.7.5/neuralogic/core/builder/components.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/builder/dataset_builder.py` & `neuralogic-0.7.5/neuralogic/core/builder/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/factories.py` & `neuralogic-0.7.5/neuralogic/core/constructs/factories.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/function/__init__.py` & `neuralogic-0.7.5/neuralogic/core/constructs/function/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/function/concat.py` & `neuralogic-0.7.5/neuralogic/core/constructs/function/concat.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/function/function.py` & `neuralogic-0.7.5/neuralogic/core/constructs/function/function.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/function/reshape.py` & `neuralogic-0.7.5/neuralogic/core/constructs/function/reshape.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/function/slice.py` & `neuralogic-0.7.5/neuralogic/core/constructs/function/slice.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/function/softmax.py` & `neuralogic-0.7.5/neuralogic/core/constructs/function/softmax.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/java_objects.py` & `neuralogic-0.7.5/neuralogic/core/constructs/java_objects.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/metadata.py` & `neuralogic-0.7.5/neuralogic/core/constructs/metadata.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/predicate.py` & `neuralogic-0.7.5/neuralogic/core/constructs/predicate.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/relation.py` & `neuralogic-0.7.5/neuralogic/core/constructs/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     def to_str(self, end=False) -> str:
         end = "." if end else ""
 
         if self.terms:
             terms = ", ".join([str(term) for term in self.terms])
 
             if self.negated:
-                return f"~{self.predicate.to_str()}({terms}){end}"
+                return f"!{self.predicate.to_str()}({terms}){end}"
             if self.function:
                 literal = f"{self.predicate.to_str()}({terms})"
                 return f"{self.function.wrap(literal)}{end}"
             return f"{self.predicate.to_str()}({terms}){end}"
 
         if self.negated:
             return f"!{self.predicate.to_str()}{end}"
```

### Comparing `neuralogic-0.7.4/neuralogic/core/constructs/rule.py` & `neuralogic-0.7.5/neuralogic/core/constructs/rule.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/settings/__init__.py` & `neuralogic-0.7.5/neuralogic/core/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/settings/settings_proxy.py` & `neuralogic-0.7.5/neuralogic/core/settings/settings_proxy.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/sources.py` & `neuralogic-0.7.5/neuralogic/core/sources.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/core/template.py` & `neuralogic-0.7.5/neuralogic/core/template.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/dataset/__init__.py` & `neuralogic-0.7.5/neuralogic/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/dataset/base.py` & `neuralogic-0.7.5/neuralogic/dataset/base.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/dataset/csv.py` & `neuralogic-0.7.5/neuralogic/dataset/csv.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/dataset/db.py` & `neuralogic-0.7.5/neuralogic/dataset/db.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/dataset/file.py` & `neuralogic-0.7.5/neuralogic/dataset/file.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/dataset/logic.py` & `neuralogic-0.7.5/neuralogic/dataset/logic.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/dataset/tensor.py` & `neuralogic-0.7.5/neuralogic/dataset/tensor.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/db/converter.py` & `neuralogic-0.7.5/neuralogic/db/converter.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/db/pg/__init__.py` & `neuralogic-0.7.5/neuralogic/db/pg/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/db/pg/helpers.py` & `neuralogic-0.7.5/neuralogic/db/pg/helpers.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/inference/evaluation_inference_engine.py` & `neuralogic-0.7.5/neuralogic/inference/evaluation_inference_engine.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/inference/inference_engine.py` & `neuralogic-0.7.5/neuralogic/inference/inference_engine.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/jar/NeuraLogic.jar` & `neuralogic-0.7.5/neuralogic/jar/NeuraLogic.jar`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,56 +1,56 @@
-Zip file size: 2001165 bytes, number of entries: 1478
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:06 META-INF/
--rw-r--r--  2.0 unx      172 b- defN 23-Mar-03 23:06 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 generated/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/neuralogic/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-28 21:51 cz/cvut/fel/ida/neuralogic/cli/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/neuralogic/cli/utils/
--rw-r--r--  2.0 unx     1733 b- defN 23-Jan-28 21:51 cz/cvut/fel/ida/neuralogic/cli/Main.class
--rw-r--r--  2.0 unx     6196 b- defN 23-Jan-12 20:15 cz/cvut/fel/ida/neuralogic/cli/utils/Runner.class
--rw-r--r--  2.0 unx    17210 b- defN 23-Jan-12 20:15 cz/cvut/fel/ida/neuralogic/cli/utils/CommandLineHandler.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/setup/
--rw-r--r--  2.0 unx     1282 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$ResultsType.class
--rw-r--r--  2.0 unx      776 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$1.class
--rw-r--r--  2.0 unx     1222 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$DataSelection.class
--rw-r--r--  2.0 unx     1319 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$ModelSelection.class
--rw-r--r--  2.0 unx     1191 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$HitsClashes.class
--rw-r--r--  2.0 unx     1243 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$ErrorFcn.class
--rw-r--r--  2.0 unx     1269 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$IterationMode.class
--rw-r--r--  2.0 unx     1176 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$Optimize.class
--rw-r--r--  2.0 unx     2005 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$TransformationFcn.class
--rw-r--r--  2.0 unx     1133 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$DecaySet.class
--rw-r--r--  2.0 unx    19348 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/SourceFiles.class
--rw-r--r--  2.0 unx     1227 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$GroundingMode.class
--rw-r--r--  2.0 unx     1285 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$InitDistribution.class
--rw-r--r--  2.0 unx    28968 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings.class
--rw-r--r--  2.0 unx     1266 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$NeuralState.class
--rw-r--r--  2.0 unx     1211 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$ExportFileType.class
--rw-r--r--  2.0 unx     1201 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$NeuronSearch.class
--rw-r--r--  2.0 unx     1206 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$GroundingAlgo.class
--rw-r--r--  2.0 unx     1133 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$OS.class
--rw-r--r--  2.0 unx     8553 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Sources.class
--rw-r--r--  2.0 unx      665 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$Inferred.class
--rw-r--r--  2.0 unx     1156 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$Detail.class
--rw-r--r--  2.0 unx     1498 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Source.class
--rw-r--r--  2.0 unx     1672 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$CombinationFcn.class
--rw-r--r--  2.0 unx     1195 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$MainMode.class
--rw-r--r--  2.0 unx     1164 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$InitSet.class
--rw-r--r--  2.0 unx     1149 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$OptimizerSet.class
--rw-r--r--  2.0 unx     1248 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$HitsPreservation.class
--rw-r--r--  2.0 unx     1231 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$HitsCorruption.class
--rw-r--r--  2.0 unx     1058 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/SourceFiles$1.class
--rw-r--r--  2.0 unx     1222 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/setup/Settings$DropoutMode.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 20:14 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 20:14 META-INF/maven/io.github.gustiks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 20:14 META-INF/maven/io.github.gustiks/NeuraLogic-Settings/
+Zip file size: 2007653 bytes, number of entries: 1481
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:24 META-INF/
+-rw-r--r--  2.0 unx      172 b- defN 23-Apr-07 21:24 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/neuralogic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/neuralogic/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/neuralogic/cli/utils/
+-rw-r--r--  2.0 unx     1733 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/neuralogic/cli/Main.class
+-rw-r--r--  2.0 unx     6196 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/neuralogic/cli/utils/Runner.class
+-rw-r--r--  2.0 unx    17210 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/neuralogic/cli/utils/CommandLineHandler.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 generated/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/setup/
+-rw-r--r--  2.0 unx     1282 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$ResultsType.class
+-rw-r--r--  2.0 unx      776 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$1.class
+-rw-r--r--  2.0 unx     1222 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$DataSelection.class
+-rw-r--r--  2.0 unx     1319 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$ModelSelection.class
+-rw-r--r--  2.0 unx     1191 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$HitsClashes.class
+-rw-r--r--  2.0 unx     1243 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$ErrorFcn.class
+-rw-r--r--  2.0 unx     1269 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$IterationMode.class
+-rw-r--r--  2.0 unx     1176 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$Optimize.class
+-rw-r--r--  2.0 unx     2005 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$TransformationFcn.class
+-rw-r--r--  2.0 unx     1133 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$DecaySet.class
+-rw-r--r--  2.0 unx    19348 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/SourceFiles.class
+-rw-r--r--  2.0 unx     1227 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$GroundingMode.class
+-rw-r--r--  2.0 unx     1285 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$InitDistribution.class
+-rw-r--r--  2.0 unx    29017 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings.class
+-rw-r--r--  2.0 unx     1266 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$NeuralState.class
+-rw-r--r--  2.0 unx     1211 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$ExportFileType.class
+-rw-r--r--  2.0 unx     1201 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$NeuronSearch.class
+-rw-r--r--  2.0 unx     1206 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$GroundingAlgo.class
+-rw-r--r--  2.0 unx     1133 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$OS.class
+-rw-r--r--  2.0 unx     9988 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Sources.class
+-rw-r--r--  2.0 unx      665 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$Inferred.class
+-rw-r--r--  2.0 unx     1156 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$Detail.class
+-rw-r--r--  2.0 unx     1498 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Source.class
+-rw-r--r--  2.0 unx     1672 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$CombinationFcn.class
+-rw-r--r--  2.0 unx     1195 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$MainMode.class
+-rw-r--r--  2.0 unx     1164 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$InitSet.class
+-rw-r--r--  2.0 unx     1149 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$OptimizerSet.class
+-rw-r--r--  2.0 unx     1248 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$HitsPreservation.class
+-rw-r--r--  2.0 unx     1231 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$HitsCorruption.class
+-rw-r--r--  2.0 unx     1058 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/SourceFiles$1.class
+-rw-r--r--  2.0 unx     1222 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$DropoutMode.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/NeuraLogic-Settings/
 -rw-r--r--  2.0 unx     1091 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/NeuraLogic-Settings/pom.xml
 -rw-r--r--  2.0 unx      122 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/NeuraLogic-Settings/pom.properties
 drwxr-xr-x  2.0 unx        0 b- stor 21-Oct-29 12:59 com/
 drwxr-xr-x  2.0 unx        0 b- stor 21-Oct-29 12:59 com/google/
 drwxr-xr-x  2.0 unx        0 b- stor 21-Oct-29 12:59 com/google/gson/
 drwxr-xr-x  2.0 unx        0 b- stor 21-Oct-29 12:59 com/google/gson/stream/
 drwxr-xr-x  2.0 unx        0 b- stor 21-Oct-29 12:59 com/google/gson/reflect/
@@ -293,475 +293,478 @@
 -rw-r--r--  2.0 unx     9632 b- defN 17-Mar-09 14:01 org/apache/commons/cli/DefaultParser.class
 -rw-r--r--  2.0 unx     1685 b- defN 17-Mar-09 14:01 org/apache/commons/cli/MissingOptionException.class
 -rw-r--r--  2.0 unx     9245 b- defN 17-Mar-09 14:01 org/apache/commons/cli/Option.class
 -rw-r--r--  2.0 unx     3784 b- defN 17-Mar-09 14:01 org/apache/commons/cli/OptionBuilder.class
 -rw-r--r--  2.0 unx      444 b- defN 17-Mar-09 14:01 org/apache/commons/cli/ParseException.class
 -rw-r--r--  2.0 unx     3752 b- defN 17-Mar-09 14:01 org/apache/commons/cli/TypeHandler.class
 -rw-r--r--  2.0 unx      116 b- defN 17-Mar-09 14:01 META-INF/maven/commons-cli/commons-cli/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/exporting/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/python/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/metacentrum/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/random/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/hypergraphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/tuples/
--rw-r--r--  2.0 unx     4777 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/exporting/JsonExporter.class
--rw-r--r--  2.0 unx     2888 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/exporting/TextExporter.class
--rw-r--r--  2.0 unx     1275 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/exporting/Exportable.class
--rw-r--r--  2.0 unx     3350 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/exporting/Exporter.class
--rw-r--r--  2.0 unx     4078 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/exporting/JavaExporter.class
--rw-r--r--  2.0 unx      300 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/python/PythonOutputStream$TextIOWrapper.class
--rw-r--r--  2.0 unx     1108 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/python/PythonOutputStream.class
--rw-r--r--  2.0 unx      332 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/metacentrum/AutoEvaluator.class
--rw-r--r--  2.0 unx      497 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$1.class
--rw-r--r--  2.0 unx     1586 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/MutableDouble.class
--rw-r--r--  2.0 unx     2227 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/random/BinomialGenerator.class
--rw-r--r--  2.0 unx     1867 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/random/CustomRandomGenerator.class
--rw-r--r--  2.0 unx      876 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$3.class
--rw-r--r--  2.0 unx      510 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Parallel$Int.class
--rw-r--r--  2.0 unx     2542 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/StringUtils.class
--rw-r--r--  2.0 unx      365 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$MyComparator.class
--rw-r--r--  2.0 unx      356 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$Fun.class
--rw-r--r--  2.0 unx     1106 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Statistics$5.class
--rw-r--r--  2.0 unx      817 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/IntegerFunction$Exponential.class
--rw-r--r--  2.0 unx     2530 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/hypergraphs/HypergraphUtils.class
--rw-r--r--  2.0 unx     7437 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/hypergraphs/Hypergraph.class
--rw-r--r--  2.0 unx     1959 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/CommandLine.class
--rw-r--r--  2.0 unx      607 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$Int.class
--rw-r--r--  2.0 unx    11177 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Statistics.class
--rw-r--r--  2.0 unx    43565 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar.class
--rw-r--r--  2.0 unx     1344 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Combinatorics$1.class
--rw-r--r--  2.0 unx     3154 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Parallel.class
--rw-r--r--  2.0 unx      764 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/IntegerFunction.class
--rw-r--r--  2.0 unx     1503 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Statistics$3.class
--rw-r--r--  2.0 unx      394 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$MultiFun.class
--rw-r--r--  2.0 unx    10615 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Combinatorics.class
--rw-r--r--  2.0 unx      325 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$VoidFun.class
--rw-r--r--  2.0 unx      683 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/LinearFunction.class
--rw-r--r--  2.0 unx      156 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/DoubleFunction.class
--rw-r--r--  2.0 unx      580 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/IntegerFunction$ConstantFunction.class
--rw-r--r--  2.0 unx     1503 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Statistics$4.class
--rw-r--r--  2.0 unx     1140 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$4.class
--rw-r--r--  2.0 unx     1290 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$2.class
--rw-r--r--  2.0 unx      697 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/IntegerFunction$Cubic.class
--rw-r--r--  2.0 unx      501 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/IntegerFunction$Identity.class
--rw-r--r--  2.0 unx     1269 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$4$1.class
--rw-r--r--  2.0 unx     1504 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Statistics$2.class
--rw-r--r--  2.0 unx     1658 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Cache.class
--rw-r--r--  2.0 unx      452 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$MultiFunWithParams.class
--rw-r--r--  2.0 unx    11149 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/DoubleMultiSet.class
--rw-r--r--  2.0 unx     4828 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/BigIntegerCounters.class
--rw-r--r--  2.0 unx      253 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/DoubleSet$1.class
--rw-r--r--  2.0 unx     7073 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/MultiMap.class
--rw-r--r--  2.0 unx     4609 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/ValueToIndex.class
--rw-r--r--  2.0 unx     3447 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/VectorSet.class
--rw-r--r--  2.0 unx    18752 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/IntegerSet.class
--rw-r--r--  2.0 unx    13346 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/TupleSet.class
--rw-r--r--  2.0 unx     1629 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/DoubleMultiSet$1.class
--rw-r--r--  2.0 unx     4769 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/IntegerMultiMap.class
--rw-r--r--  2.0 unx     1036 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/TupleSet$1.class
--rw-r--r--  2.0 unx    16759 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/LongSet.class
--rw-r--r--  2.0 unx     7034 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/Counters.class
--rw-r--r--  2.0 unx     5490 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/NaturalNumbersList.class
--rw-r--r--  2.0 unx      247 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/LongSet$1.class
--rw-r--r--  2.0 unx     6774 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/MultiList.class
--rw-r--r--  2.0 unx     1135 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/IntegerSet$1.class
--rw-r--r--  2.0 unx     1541 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/DoubleMultiSet$EmptySet.class
--rw-r--r--  2.0 unx     2635 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/NaturalNumbersList$Iter.class
--rw-r--r--  2.0 unx     1711 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/IntegerSet$EmptySet.class
--rw-r--r--  2.0 unx     2651 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/FakeMap.class
--rw-r--r--  2.0 unx     1901 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/LongSet$EmptySet.class
--rw-r--r--  2.0 unx     7337 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/Heap.class
--rw-r--r--  2.0 unx     1045 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/TupleSet$2.class
--rw-r--r--  2.0 unx     4503 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/BigIntegerVector.class
--rw-r--r--  2.0 unx     1701 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/DoubleSet$EmptySet.class
--rw-r--r--  2.0 unx     7120 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/DoubleCounters.class
--rw-r--r--  2.0 unx    14306 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/DoubleSet.class
--rw-r--r--  2.0 unx     2306 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/collections/TupleSet$EmptySet.class
--rw-r--r--  2.0 unx    10013 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/MatrixUtils.class
--rw-r--r--  2.0 unx     1455 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/MutableInteger.class
--rw-r--r--  2.0 unx      414 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$FunWithParams.class
--rw-r--r--  2.0 unx    28127 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/VectorUtils.class
--rw-r--r--  2.0 unx     1504 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Statistics$1.class
--rw-r--r--  2.0 unx     1227 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/AttributedObject.class
--rw-r--r--  2.0 unx      670 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/UniqueIDs.class
--rw-r--r--  2.0 unx      860 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$IdentityFun.class
--rw-r--r--  2.0 unx     1885 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Parallel$WorkerThread.class
--rw-r--r--  2.0 unx     1588 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$MapBasedComparator.class
--rw-r--r--  2.0 unx      655 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/IntegerFunction$Quadratic.class
--rw-r--r--  2.0 unx     1316 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/math/Sugar$3$1.class
--rw-r--r--  2.0 unx     2899 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/Utilities$BatchSpliterator.class
--rw-r--r--  2.0 unx     1811 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/Pair.class
--rw-r--r--  2.0 unx     2095 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/Timing.class
--rw-r--r--  2.0 unx     1676 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/Utilities$1.class
--rw-r--r--  2.0 unx    12053 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/Utilities.class
--rw-r--r--  2.0 unx     1787 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/tuples/Pair.class
--rw-r--r--  2.0 unx     8226 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/tuples/Tuple.class
--rw-r--r--  2.0 unx     2174 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/tuples/Quintuple.class
--rw-r--r--  2.0 unx     2000 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/tuples/Quadruple.class
--rw-r--r--  2.0 unx     1999 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/utils/generic/tuples/Triple.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 META-INF/maven/io.github.gustiks/Utilities/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/utils/exporting/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/utils/python/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/utils/metacentrum/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/random/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/hypergraphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/
+-rw-r--r--  2.0 unx     4777 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/exporting/JsonExporter.class
+-rw-r--r--  2.0 unx     2888 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/exporting/TextExporter.class
+-rw-r--r--  2.0 unx     2958 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/exporting/Exportable.class
+-rw-r--r--  2.0 unx     3350 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/exporting/Exporter.class
+-rw-r--r--  2.0 unx     4078 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/exporting/JavaExporter.class
+-rw-r--r--  2.0 unx      300 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/python/PythonOutputStream$TextIOWrapper.class
+-rw-r--r--  2.0 unx     1108 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/python/PythonOutputStream.class
+-rw-r--r--  2.0 unx      332 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/metacentrum/AutoEvaluator.class
+-rw-r--r--  2.0 unx      497 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$1.class
+-rw-r--r--  2.0 unx     1586 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/MutableDouble.class
+-rw-r--r--  2.0 unx     2227 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/random/BinomialGenerator.class
+-rw-r--r--  2.0 unx     1867 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/random/CustomRandomGenerator.class
+-rw-r--r--  2.0 unx      876 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$3.class
+-rw-r--r--  2.0 unx      510 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Parallel$Int.class
+-rw-r--r--  2.0 unx     2542 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/StringUtils.class
+-rw-r--r--  2.0 unx      365 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$MyComparator.class
+-rw-r--r--  2.0 unx      356 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$Fun.class
+-rw-r--r--  2.0 unx     1106 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Statistics$5.class
+-rw-r--r--  2.0 unx      817 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/IntegerFunction$Exponential.class
+-rw-r--r--  2.0 unx     2530 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/hypergraphs/HypergraphUtils.class
+-rw-r--r--  2.0 unx     7437 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/hypergraphs/Hypergraph.class
+-rw-r--r--  2.0 unx     1959 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/CommandLine.class
+-rw-r--r--  2.0 unx      607 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$Int.class
+-rw-r--r--  2.0 unx    11177 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Statistics.class
+-rw-r--r--  2.0 unx    43565 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar.class
+-rw-r--r--  2.0 unx     1344 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Combinatorics$1.class
+-rw-r--r--  2.0 unx     3154 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Parallel.class
+-rw-r--r--  2.0 unx      764 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/IntegerFunction.class
+-rw-r--r--  2.0 unx     1503 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Statistics$3.class
+-rw-r--r--  2.0 unx      394 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$MultiFun.class
+-rw-r--r--  2.0 unx    10615 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Combinatorics.class
+-rw-r--r--  2.0 unx      325 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$VoidFun.class
+-rw-r--r--  2.0 unx      683 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/LinearFunction.class
+-rw-r--r--  2.0 unx      156 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/DoubleFunction.class
+-rw-r--r--  2.0 unx      580 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/IntegerFunction$ConstantFunction.class
+-rw-r--r--  2.0 unx     1503 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Statistics$4.class
+-rw-r--r--  2.0 unx     1140 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$4.class
+-rw-r--r--  2.0 unx     1290 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$2.class
+-rw-r--r--  2.0 unx      697 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/IntegerFunction$Cubic.class
+-rw-r--r--  2.0 unx      501 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/IntegerFunction$Identity.class
+-rw-r--r--  2.0 unx     1269 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$4$1.class
+-rw-r--r--  2.0 unx     1504 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Statistics$2.class
+-rw-r--r--  2.0 unx     1658 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Cache.class
+-rw-r--r--  2.0 unx      452 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$MultiFunWithParams.class
+-rw-r--r--  2.0 unx    11149 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/DoubleMultiSet.class
+-rw-r--r--  2.0 unx     4828 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/BigIntegerCounters.class
+-rw-r--r--  2.0 unx      253 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/DoubleSet$1.class
+-rw-r--r--  2.0 unx     7073 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/MultiMap.class
+-rw-r--r--  2.0 unx     4609 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/ValueToIndex.class
+-rw-r--r--  2.0 unx     3447 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/VectorSet.class
+-rw-r--r--  2.0 unx    18752 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/IntegerSet.class
+-rw-r--r--  2.0 unx    13346 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/TupleSet.class
+-rw-r--r--  2.0 unx     1629 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/DoubleMultiSet$1.class
+-rw-r--r--  2.0 unx     4769 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/IntegerMultiMap.class
+-rw-r--r--  2.0 unx     1036 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/TupleSet$1.class
+-rw-r--r--  2.0 unx    16759 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/LongSet.class
+-rw-r--r--  2.0 unx     7034 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/Counters.class
+-rw-r--r--  2.0 unx     5490 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/NaturalNumbersList.class
+-rw-r--r--  2.0 unx      247 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/LongSet$1.class
+-rw-r--r--  2.0 unx     6774 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/MultiList.class
+-rw-r--r--  2.0 unx     1135 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/IntegerSet$1.class
+-rw-r--r--  2.0 unx     1541 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/DoubleMultiSet$EmptySet.class
+-rw-r--r--  2.0 unx     2635 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/NaturalNumbersList$Iter.class
+-rw-r--r--  2.0 unx     1711 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/IntegerSet$EmptySet.class
+-rw-r--r--  2.0 unx     2651 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/FakeMap.class
+-rw-r--r--  2.0 unx     1901 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/LongSet$EmptySet.class
+-rw-r--r--  2.0 unx     7337 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/Heap.class
+-rw-r--r--  2.0 unx     1045 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/TupleSet$2.class
+-rw-r--r--  2.0 unx     4503 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/BigIntegerVector.class
+-rw-r--r--  2.0 unx     1701 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/DoubleSet$EmptySet.class
+-rw-r--r--  2.0 unx     7120 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/DoubleCounters.class
+-rw-r--r--  2.0 unx    14306 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/DoubleSet.class
+-rw-r--r--  2.0 unx     2306 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/collections/TupleSet$EmptySet.class
+-rw-r--r--  2.0 unx    10013 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/MatrixUtils.class
+-rw-r--r--  2.0 unx     1455 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/MutableInteger.class
+-rw-r--r--  2.0 unx      414 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$FunWithParams.class
+-rw-r--r--  2.0 unx    28127 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/VectorUtils.class
+-rw-r--r--  2.0 unx     1504 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Statistics$1.class
+-rw-r--r--  2.0 unx     1227 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/AttributedObject.class
+-rw-r--r--  2.0 unx      670 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/UniqueIDs.class
+-rw-r--r--  2.0 unx      860 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$IdentityFun.class
+-rw-r--r--  2.0 unx     1885 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Parallel$WorkerThread.class
+-rw-r--r--  2.0 unx     1588 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$MapBasedComparator.class
+-rw-r--r--  2.0 unx      655 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/IntegerFunction$Quadratic.class
+-rw-r--r--  2.0 unx     1316 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/math/Sugar$3$1.class
+-rw-r--r--  2.0 unx     2899 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/Utilities$BatchSpliterator.class
+-rw-r--r--  2.0 unx     1811 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/Pair.class
+-rw-r--r--  2.0 unx     2095 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/Timing.class
+-rw-r--r--  2.0 unx     1676 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/Utilities$1.class
+-rw-r--r--  2.0 unx    12053 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/Utilities.class
+-rw-r--r--  2.0 unx     1787 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/Pair.class
+-rw-r--r--  2.0 unx     8226 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/Tuple.class
+-rw-r--r--  2.0 unx     2174 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/Quintuple.class
+-rw-r--r--  2.0 unx     2000 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/Quadruple.class
+-rw-r--r--  2.0 unx     1999 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/Triple.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Utilities/
 -rw-r--r--  2.0 unx     1017 b- defN 23-Feb-13 21:15 META-INF/maven/io.github.gustiks/Utilities/pom.xml
 -rw-r--r--  2.0 unx      112 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Utilities/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/bulding/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debuging/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debuging/drawing/
--rw-r--r--  2.0 unx     4682 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/MultiMerge.class
--rw-r--r--  2.0 unx     7115 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Pipe.class
--rw-r--r--  2.0 unx     3163 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/ParallelPipe.class
--rw-r--r--  2.0 unx      958 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Pipe$1.class
--rw-r--r--  2.0 unx      375 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/CheckedSupplier.class
--rw-r--r--  2.0 unx      992 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Branch$1.class
--rw-r--r--  2.0 unx      380 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/CheckedConsumer.class
--rw-r--r--  2.0 unx      986 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/ParallelPipe$1.class
--rw-r--r--  2.0 unx     2012 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/bulding/AbstractPipelineBuilder.class
--rw-r--r--  2.0 unx     6601 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Branch.class
--rw-r--r--  2.0 unx     1109 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Merge$3.class
--rw-r--r--  2.0 unx     1100 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Merge$1.class
--rw-r--r--  2.0 unx     6552 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Merge.class
--rw-r--r--  2.0 unx     1389 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/RecurrentPipe.class
--rw-r--r--  2.0 unx      231 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Executable.class
--rw-r--r--  2.0 unx     1609 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/StreamifyPipe.class
--rw-r--r--  2.0 unx     1562 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/StreamParallelizationPipe.class
--rw-r--r--  2.0 unx     1612 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/DuplicateListBranch.class
--rw-r--r--  2.0 unx     1416 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/ListMerge.class
--rw-r--r--  2.0 unx     3053 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/ExportingPipe.class
--rw-r--r--  2.0 unx     1811 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/SecondFromPairExtractionBranch.class
--rw-r--r--  2.0 unx     1612 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/LambdaPipe.class
--rw-r--r--  2.0 unx     1664 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/SecondFromPairPipe.class
--rw-r--r--  2.0 unx     1208 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/IdentityGenPipe.class
--rw-r--r--  2.0 unx     1927 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/FirstFromPairExtractionBranch.class
--rw-r--r--  2.0 unx     1650 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/PairBranch.class
--rw-r--r--  2.0 unx     1460 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/ListBranch.class
--rw-r--r--  2.0 unx     1659 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/FirstFromPairPipe.class
--rw-r--r--  2.0 unx     1387 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/DuplicateBranch.class
--rw-r--r--  2.0 unx     1683 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/generic/PairMerge.class
--rw-r--r--  2.0 unx     3706 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/MultiBranch.class
--rw-r--r--  2.0 unx    14169 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Pipeline.class
--rw-r--r--  2.0 unx     1676 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/ConnectBefore.class
--rw-r--r--  2.0 unx     1134 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/MultiMerge$1.class
--rw-r--r--  2.0 unx     1423 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Block$PipelineTiming.class
--rw-r--r--  2.0 unx     2863 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDrawer$GenericTypeGetter.class
--rw-r--r--  2.0 unx     1277 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDebugger.class
--rw-r--r--  2.0 unx    10019 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDrawer.class
--rw-r--r--  2.0 unx      418 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/CheckedFunction.class
--rw-r--r--  2.0 unx     3089 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Block.class
--rw-r--r--  2.0 unx     2125 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/ConnectAfter.class
--rw-r--r--  2.0 unx     1100 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/Merge$2.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 20:14 META-INF/maven/io.github.gustiks/Pipelines/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/bulding/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/drawing/
+-rw-r--r--  2.0 unx     4682 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/MultiMerge.class
+-rw-r--r--  2.0 unx     7115 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Pipe.class
+-rw-r--r--  2.0 unx     3163 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/ParallelPipe.class
+-rw-r--r--  2.0 unx      958 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Pipe$1.class
+-rw-r--r--  2.0 unx      375 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/CheckedSupplier.class
+-rw-r--r--  2.0 unx      992 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Branch$1.class
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/CheckedConsumer.class
+-rw-r--r--  2.0 unx      986 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/ParallelPipe$1.class
+-rw-r--r--  2.0 unx     2012 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/bulding/AbstractPipelineBuilder.class
+-rw-r--r--  2.0 unx     6601 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Branch.class
+-rw-r--r--  2.0 unx     1109 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Merge$3.class
+-rw-r--r--  2.0 unx     1100 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Merge$1.class
+-rw-r--r--  2.0 unx     6552 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Merge.class
+-rw-r--r--  2.0 unx     1389 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/RecurrentPipe.class
+-rw-r--r--  2.0 unx      231 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Executable.class
+-rw-r--r--  2.0 unx     1609 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/StreamifyPipe.class
+-rw-r--r--  2.0 unx     1562 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/StreamParallelizationPipe.class
+-rw-r--r--  2.0 unx     1612 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/DuplicateListBranch.class
+-rw-r--r--  2.0 unx     1416 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/ListMerge.class
+-rw-r--r--  2.0 unx     3053 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/ExportingPipe.class
+-rw-r--r--  2.0 unx     1811 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/SecondFromPairExtractionBranch.class
+-rw-r--r--  2.0 unx     1612 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/LambdaPipe.class
+-rw-r--r--  2.0 unx     1664 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/SecondFromPairPipe.class
+-rw-r--r--  2.0 unx     1208 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/IdentityGenPipe.class
+-rw-r--r--  2.0 unx     1927 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/FirstFromPairExtractionBranch.class
+-rw-r--r--  2.0 unx     1650 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/PairBranch.class
+-rw-r--r--  2.0 unx     1460 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/ListBranch.class
+-rw-r--r--  2.0 unx     1659 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/FirstFromPairPipe.class
+-rw-r--r--  2.0 unx     1387 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/DuplicateBranch.class
+-rw-r--r--  2.0 unx     1683 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/PairMerge.class
+-rw-r--r--  2.0 unx     3706 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/MultiBranch.class
+-rw-r--r--  2.0 unx    14169 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Pipeline.class
+-rw-r--r--  2.0 unx     1676 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/ConnectBefore.class
+-rw-r--r--  2.0 unx     1134 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/MultiMerge$1.class
+-rw-r--r--  2.0 unx     1423 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Block$PipelineTiming.class
+-rw-r--r--  2.0 unx     2863 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDrawer$GenericTypeGetter.class
+-rw-r--r--  2.0 unx     1277 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDebugger.class
+-rw-r--r--  2.0 unx    10019 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDrawer.class
+-rw-r--r--  2.0 unx      418 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/CheckedFunction.class
+-rw-r--r--  2.0 unx     3089 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Block.class
+-rw-r--r--  2.0 unx     2125 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/ConnectAfter.class
+-rw-r--r--  2.0 unx     1100 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Merge$2.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Pipelines/
 -rw-r--r--  2.0 unx     1228 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Pipelines/pom.xml
 -rw-r--r--  2.0 unx      112 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Pipelines/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/drawing/
--rw-r--r--  2.0 unx     5124 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/drawing/DrawWindow.class
--rw-r--r--  2.0 unx     2614 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/drawing/DrawWindow$ImagePanel$MouseListener.class
--rw-r--r--  2.0 unx    11843 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/drawing/GraphViz.class
--rw-r--r--  2.0 unx     3976 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/drawing/DrawWindow$ImagePanel.class
--rw-r--r--  2.0 unx     1087 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/drawing/DrawWindow$1.class
--rw-r--r--  2.0 unx     4717 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/drawing/Drawer.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 20:14 META-INF/maven/io.github.gustiks/Drawing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/
+-rw-r--r--  2.0 unx     5124 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/DrawWindow.class
+-rw-r--r--  2.0 unx     2614 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/DrawWindow$ImagePanel$MouseListener.class
+-rw-r--r--  2.0 unx    11843 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/GraphViz.class
+-rw-r--r--  2.0 unx     3976 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/DrawWindow$ImagePanel.class
+-rw-r--r--  2.0 unx     1087 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/DrawWindow$1.class
+-rw-r--r--  2.0 unx     4717 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/Drawer.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Drawing/
 -rw-r--r--  2.0 unx      806 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Drawing/pom.xml
 -rw-r--r--  2.0 unx      110 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Drawing/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logging/
--rw-r--r--  2.0 unx     1416 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logging/HtmlFormatter.class
--rw-r--r--  2.0 unx     2938 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logging/NormalFormatter.class
--rw-r--r--  2.0 unx     5562 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logging/Logging.class
--rw-r--r--  2.0 unx     1098 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logging/FlushStreamHandler.class
--rw-r--r--  2.0 unx     3344 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logging/ColoredFormatter.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 20:14 META-INF/maven/io.github.gustiks/Logging/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logging/
+-rw-r--r--  2.0 unx     1416 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logging/HtmlFormatter.class
+-rw-r--r--  2.0 unx     2938 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logging/NormalFormatter.class
+-rw-r--r--  2.0 unx     5562 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logging/Logging.class
+-rw-r--r--  2.0 unx     1098 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logging/FlushStreamHandler.class
+-rw-r--r--  2.0 unx     3344 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logging/ColoredFormatter.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Logging/
 -rw-r--r--  2.0 unx     1017 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Logging/pom.xml
 -rw-r--r--  2.0 unx      110 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Logging/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-02 20:37 cz/cvut/fel/ida/pipelines/debugging/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 22:51 cz/cvut/fel/ida/pipelines/debugging/drawing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/utils/
--rw-r--r--  2.0 unx     1558 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$2.class
--rw-r--r--  2.0 unx     1406 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$3.class
--rw-r--r--  2.0 unx     3793 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$LogicLearningBuilder$1.class
--rw-r--r--  2.0 unx     2616 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$8.class
--rw-r--r--  2.0 unx     1791 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$StructureLearningBuilder.class
--rw-r--r--  2.0 unx     1757 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$6.class
--rw-r--r--  2.0 unx     2558 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$NeuralLearningBuilder.class
--rw-r--r--  2.0 unx     7192 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$LogicTrainTestBuilder.class
--rw-r--r--  2.0 unx     1346 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TestingBuilder$1.class
--rw-r--r--  2.0 unx     3186 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateSamplesBuilder$1.class
--rw-r--r--  2.0 unx     3003 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$1.class
--rw-r--r--  2.0 unx     2042 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$7.class
--rw-r--r--  2.0 unx     6818 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$NeuralTrainTestBuilder.class
--rw-r--r--  2.0 unx     1822 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$1.class
--rw-r--r--  2.0 unx     2939 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$10.class
--rw-r--r--  2.0 unx     2596 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$1.class
--rw-r--r--  2.0 unx     1395 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$4.class
--rw-r--r--  2.0 unx     5327 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder$1.class
--rw-r--r--  2.0 unx     7466 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$LogicLearningBuilder.class
--rw-r--r--  2.0 unx     1510 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$3.class
--rw-r--r--  2.0 unx     1720 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$7.class
--rw-r--r--  2.0 unx     1819 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$4.class
--rw-r--r--  2.0 unx     7849 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder.class
--rw-r--r--  2.0 unx    27709 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder.class
--rw-r--r--  2.0 unx     2430 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TestingBuilder$NeuralTestingBuilder.class
--rw-r--r--  2.0 unx     3078 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TestingBuilder$LogicTestingBuilder$1.class
--rw-r--r--  2.0 unx     6077 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/GroundingBuilder.class
--rw-r--r--  2.0 unx     7236 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder.class
--rw-r--r--  2.0 unx     6105 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TestingBuilder$LogicTestingBuilder.class
--rw-r--r--  2.0 unx     1025 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$StructureLearningBuilder$1.class
--rw-r--r--  2.0 unx     2970 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$9.class
--rw-r--r--  2.0 unx     6351 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TestingBuilder.class
--rw-r--r--  2.0 unx     7794 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder.class
--rw-r--r--  2.0 unx     2383 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$2.class
--rw-r--r--  2.0 unx     2455 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$5.class
--rw-r--r--  2.0 unx     2105 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$6.class
--rw-r--r--  2.0 unx     8748 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/LearningSchemeBuilder.class
--rw-r--r--  2.0 unx     5986 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$StructureTrainTestBuilder.class
--rw-r--r--  2.0 unx     2190 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$4.class
--rw-r--r--  2.0 unx     7030 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainingBuilder.class
--rw-r--r--  2.0 unx    17171 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/PythonBuilder.class
--rw-r--r--  2.0 unx     8874 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateSamplesBuilder.class
--rw-r--r--  2.0 unx     1358 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$2.class
--rw-r--r--  2.0 unx     7508 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder.class
--rw-r--r--  2.0 unx     1511 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$2.class
--rw-r--r--  2.0 unx     2385 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$3.class
--rw-r--r--  2.0 unx     3801 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$5.class
--rw-r--r--  2.0 unx     1847 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$1.class
--rw-r--r--  2.0 unx     8130 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/End2endTrainigBuilder$End2endNNBuilder.class
--rw-r--r--  2.0 unx     9130 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/End2endTrainigBuilder.class
--rw-r--r--  2.0 unx     1518 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/LearningSchemeBuilder$1.class
--rw-r--r--  2.0 unx     1841 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$5.class
--rw-r--r--  2.0 unx     1524 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$3$1.class
--rw-r--r--  2.0 unx     4125 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/GroundingDebugger.class
--rw-r--r--  2.0 unx     1462 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$1.class
--rw-r--r--  2.0 unx     6572 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger.class
--rw-r--r--  2.0 unx     2427 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$2.class
--rw-r--r--  2.0 unx     5603 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/TrainingDebugger.class
--rw-r--r--  2.0 unx    12872 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer$NeuronDrawer.class
--rw-r--r--  2.0 unx     7340 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/pipelines/debugging/drawing/GroundingDrawer.class
--rw-r--r--  2.0 unx     9185 b- defN 23-Mar-03 22:51 cz/cvut/fel/ida/pipelines/debugging/drawing/TemplateDrawer.class
--rw-r--r--  2.0 unx     4996 b- defN 23-Mar-02 20:37 cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer.class
--rw-r--r--  2.0 unx     1699 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$3.class
--rw-r--r--  2.0 unx     4938 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/NeuralDebugger.class
--rw-r--r--  2.0 unx     3091 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/SampleDebugger.class
--rw-r--r--  2.0 unx     3637 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/debugging/TemplateDebugger.class
--rw-r--r--  2.0 unx     3630 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/CycleBreakingPipe.class
--rw-r--r--  2.0 unx     5816 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/GroundingSampleWrappingPipe.class
--rw-r--r--  2.0 unx     6781 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/NetworkFinalizationPipe.class
--rw-r--r--  2.0 unx     4329 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralTrainingPipe.class
--rw-r--r--  2.0 unx     7867 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralEvaluationPipe.class
--rw-r--r--  2.0 unx     2222 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/GlobalSharingGroundingPipe.class
--rw-r--r--  2.0 unx     3760 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/EdgeMergerPipe.class
--rw-r--r--  2.0 unx     4052 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/SequentiallySharedGroundingPipe.class
--rw-r--r--  2.0 unx     2838 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/TrainingResultTemplateMerge.class
--rw-r--r--  2.0 unx     6896 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/PruningPipe.class
--rw-r--r--  2.0 unx     6763 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/CompressionPipe.class
--rw-r--r--  2.0 unx     3146 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedGroundTemplatePruningPipe.class
--rw-r--r--  2.0 unx     2830 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/TemplateToNeuralPipe.class
--rw-r--r--  2.0 unx     5881 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedNeuralizationPipe.class
--rw-r--r--  2.0 unx     3931 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/StandardGroundingPipe.class
--rw-r--r--  2.0 unx     1712 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/ResultsFromProgressPipe.class
--rw-r--r--  2.0 unx     4576 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralSerializerPipe.class
--rw-r--r--  2.0 unx     2944 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedTemplateReducingPipe.class
--rw-r--r--  2.0 unx     1742 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/pipelines/utils/WorkflowUtils.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/drawing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/utils/
+-rw-r--r--  2.0 unx     1558 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$2.class
+-rw-r--r--  2.0 unx     1406 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$3.class
+-rw-r--r--  2.0 unx     3793 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$LogicLearningBuilder$1.class
+-rw-r--r--  2.0 unx     2616 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$8.class
+-rw-r--r--  2.0 unx     1791 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$StructureLearningBuilder.class
+-rw-r--r--  2.0 unx     1841 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$6.class
+-rw-r--r--  2.0 unx     2558 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$NeuralLearningBuilder.class
+-rw-r--r--  2.0 unx     7192 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$LogicTrainTestBuilder.class
+-rw-r--r--  2.0 unx     1346 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TestingBuilder$1.class
+-rw-r--r--  2.0 unx     3186 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateSamplesBuilder$1.class
+-rw-r--r--  2.0 unx     3003 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$1.class
+-rw-r--r--  2.0 unx     2042 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$7.class
+-rw-r--r--  2.0 unx     6818 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$NeuralTrainTestBuilder.class
+-rw-r--r--  2.0 unx     1822 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$1.class
+-rw-r--r--  2.0 unx     2939 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$10.class
+-rw-r--r--  2.0 unx     2596 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$1.class
+-rw-r--r--  2.0 unx     1395 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$4.class
+-rw-r--r--  2.0 unx     5327 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder$1.class
+-rw-r--r--  2.0 unx     7466 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$LogicLearningBuilder.class
+-rw-r--r--  2.0 unx     2122 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$3.class
+-rw-r--r--  2.0 unx     1757 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$7.class
+-rw-r--r--  2.0 unx     1510 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$4.class
+-rw-r--r--  2.0 unx     7849 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder.class
+-rw-r--r--  2.0 unx    27709 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder.class
+-rw-r--r--  2.0 unx     2430 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TestingBuilder$NeuralTestingBuilder.class
+-rw-r--r--  2.0 unx     3078 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TestingBuilder$LogicTestingBuilder$1.class
+-rw-r--r--  2.0 unx     6077 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/GroundingBuilder.class
+-rw-r--r--  2.0 unx     7579 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder.class
+-rw-r--r--  2.0 unx     6105 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TestingBuilder$LogicTestingBuilder.class
+-rw-r--r--  2.0 unx     1025 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$StructureLearningBuilder$1.class
+-rw-r--r--  2.0 unx     2970 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$9.class
+-rw-r--r--  2.0 unx     6351 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TestingBuilder.class
+-rw-r--r--  2.0 unx     7794 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder.class
+-rw-r--r--  2.0 unx     2383 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$2.class
+-rw-r--r--  2.0 unx     2455 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$5.class
+-rw-r--r--  2.0 unx     2105 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$6.class
+-rw-r--r--  2.0 unx     8748 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/LearningSchemeBuilder.class
+-rw-r--r--  2.0 unx     5986 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$StructureTrainTestBuilder.class
+-rw-r--r--  2.0 unx     2190 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$4.class
+-rw-r--r--  2.0 unx     7030 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainingBuilder.class
+-rw-r--r--  2.0 unx    17171 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/PythonBuilder.class
+-rw-r--r--  2.0 unx     8874 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateSamplesBuilder.class
+-rw-r--r--  2.0 unx     1720 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$8.class
+-rw-r--r--  2.0 unx     1358 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$2.class
+-rw-r--r--  2.0 unx     7508 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder.class
+-rw-r--r--  2.0 unx     1511 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$2.class
+-rw-r--r--  2.0 unx     2385 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$3.class
+-rw-r--r--  2.0 unx     3801 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$5.class
+-rw-r--r--  2.0 unx     1847 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$1.class
+-rw-r--r--  2.0 unx     8130 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/End2endTrainigBuilder$End2endNNBuilder.class
+-rw-r--r--  2.0 unx     9130 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/End2endTrainigBuilder.class
+-rw-r--r--  2.0 unx     1518 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/LearningSchemeBuilder$1.class
+-rw-r--r--  2.0 unx     1819 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$5.class
+-rw-r--r--  2.0 unx     1524 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$3$1.class
+-rw-r--r--  2.0 unx     4125 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/GroundingDebugger.class
+-rw-r--r--  2.0 unx     1462 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$1.class
+-rw-r--r--  2.0 unx     6572 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger.class
+-rw-r--r--  2.0 unx     2427 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$2.class
+-rw-r--r--  2.0 unx     5603 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/TrainingDebugger.class
+-rw-r--r--  2.0 unx    12872 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer$NeuronDrawer.class
+-rw-r--r--  2.0 unx     7340 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/drawing/GroundingDrawer.class
+-rw-r--r--  2.0 unx     9294 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/drawing/TemplateDrawer.class
+-rw-r--r--  2.0 unx     4996 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer.class
+-rw-r--r--  2.0 unx     1699 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$3.class
+-rw-r--r--  2.0 unx     4938 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/NeuralDebugger.class
+-rw-r--r--  2.0 unx     3091 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/SampleDebugger.class
+-rw-r--r--  2.0 unx     3637 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debugging/TemplateDebugger.class
+-rw-r--r--  2.0 unx     3630 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/CycleBreakingPipe.class
+-rw-r--r--  2.0 unx     5816 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/GroundingSampleWrappingPipe.class
+-rw-r--r--  2.0 unx     6781 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/NetworkFinalizationPipe.class
+-rw-r--r--  2.0 unx     4329 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralTrainingPipe.class
+-rw-r--r--  2.0 unx     7867 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralEvaluationPipe.class
+-rw-r--r--  2.0 unx     2222 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/GlobalSharingGroundingPipe.class
+-rw-r--r--  2.0 unx     3760 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/EdgeMergerPipe.class
+-rw-r--r--  2.0 unx     4052 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/SequentiallySharedGroundingPipe.class
+-rw-r--r--  2.0 unx     2838 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/TrainingResultTemplateMerge.class
+-rw-r--r--  2.0 unx     6896 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/PruningPipe.class
+-rw-r--r--  2.0 unx     6763 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/CompressionPipe.class
+-rw-r--r--  2.0 unx     3146 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedGroundTemplatePruningPipe.class
+-rw-r--r--  2.0 unx     2830 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/TemplateToNeuralPipe.class
+-rw-r--r--  2.0 unx     5881 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedNeuralizationPipe.class
+-rw-r--r--  2.0 unx     3931 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/StandardGroundingPipe.class
+-rw-r--r--  2.0 unx     1712 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/ResultsFromProgressPipe.class
+-rw-r--r--  2.0 unx     4576 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralSerializerPipe.class
+-rw-r--r--  2.0 unx     2944 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedTemplateReducingPipe.class
+-rw-r--r--  2.0 unx     1742 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/utils/WorkflowUtils.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/
 -rw-r--r--  2.0 unx     1857 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/pom.xml
 -rw-r--r--  2.0 unx      122 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logic/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logic/constructs/building/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/building/factories/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/example/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/transforming/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/metadata/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/template/components/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/types/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 00:05 cz/cvut/fel/ida/logic/grounding/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 00:05 cz/cvut/fel/ida/logic/grounding/bottomUp/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 00:05 cz/cvut/fel/ida/logic/grounding/topDown/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/constructs/
--rw-r--r--  2.0 unx     3021 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/building/factories/ConstantFactory.class
--rw-r--r--  2.0 unx     3015 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/building/factories/VariableFactory.class
--rw-r--r--  2.0 unx     5412 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/building/factories/WeightedPredicateFactory.class
--rw-r--r--  2.0 unx     5579 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/building/factories/WeightFactory.class
--rw-r--r--  2.0 unx     1548 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/Conjunction.class
--rw-r--r--  2.0 unx     1919 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/WeightedPredicate.class
--rw-r--r--  2.0 unx     4180 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/Atom.class
--rw-r--r--  2.0 unx     3603 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/example/QueryAtom.class
--rw-r--r--  2.0 unx     2101 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/example/LiftedExample.class
--rw-r--r--  2.0 unx     2171 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/example/CompositeQuery.class
--rw-r--r--  2.0 unx     2623 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/example/ValuedFact.class
--rw-r--r--  2.0 unx     1937 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/example/LogicSample.class
--rw-r--r--  2.0 unx     3245 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/example/GroundExample.class
--rw-r--r--  2.0 unx     2627 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/transforming/SupervisedReducer.class
--rw-r--r--  2.0 unx     3730 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/transforming/MetadataProcessor.class
--rw-r--r--  2.0 unx     1162 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/transforming/SimpleTemplateMerger.class
--rw-r--r--  2.0 unx     1723 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/transforming/TemplateChainReducer.class
--rw-r--r--  2.0 unx      343 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/transforming/TemplateMerging.class
--rw-r--r--  2.0 unx     1095 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/transforming/TemplateReducing.class
--rw-r--r--  2.0 unx     1729 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/metadata/TemplateMetadata.class
--rw-r--r--  2.0 unx     5785 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/metadata/RuleMetadata.class
--rw-r--r--  2.0 unx     6331 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/metadata/PredicateMetadata.class
--rw-r--r--  2.0 unx     2992 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/components/GroundRule.class
--rw-r--r--  2.0 unx     1664 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/template/components/HeadAtom.class
--rw-r--r--  2.0 unx     2452 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/template/components/BodyAtom.class
--rw-r--r--  2.0 unx     9930 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/constructs/template/components/WeightedRule.class
--rw-r--r--  2.0 unx     2414 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/components/GroundHeadRule.class
--rw-r--r--  2.0 unx    10064 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/Template.class
--rw-r--r--  2.0 unx     1737 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/types/ParsedTemplate.class
--rw-r--r--  2.0 unx     1016 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/types/RichLogicTemplate.class
--rw-r--r--  2.0 unx     7825 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate.class
--rw-r--r--  2.0 unx    14044 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/Grounder.class
--rw-r--r--  2.0 unx    17813 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/grounding/bottomUp/BottomUp.class
--rw-r--r--  2.0 unx    21335 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/grounding/topDown/Gringo.class
--rw-r--r--  2.0 unx     1196 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/topDown/TopDown.class
--rw-r--r--  2.0 unx      297 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection$1.class
--rw-r--r--  2.0 unx     1974 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection.class
--rw-r--r--  2.0 unx     1112 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection$GroundRulesCollectionDuplicit.class
--rw-r--r--  2.0 unx     1109 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection$GroundRulesCollectionUnique.class
--rw-r--r--  2.0 unx     1610 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/GroundingSample.class
--rw-r--r--  2.0 unx    10533 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/GroundTemplate.class
--rw-r--r--  2.0 unx     1529 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/GroundingSample$Wrap.class
--rw-r--r--  2.0 unx      885 b- defN 23-Jan-12 21:48 cz/cvut/fel/ida/logic/grounding/Grounder$1.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 16:36 META-INF/maven/io.github.gustiks/Logical/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/factories/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/example/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/transforming/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/metadata/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/components/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/types/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/bottomUp/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/topDown/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/constructs/
+-rw-r--r--  2.0 unx     3021 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/factories/ConstantFactory.class
+-rw-r--r--  2.0 unx     3015 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/factories/VariableFactory.class
+-rw-r--r--  2.0 unx     5412 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/factories/WeightedPredicateFactory.class
+-rw-r--r--  2.0 unx     5579 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/factories/WeightFactory.class
+-rw-r--r--  2.0 unx     1548 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/Conjunction.class
+-rw-r--r--  2.0 unx     1919 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/WeightedPredicate.class
+-rw-r--r--  2.0 unx     4180 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/Atom.class
+-rw-r--r--  2.0 unx     3603 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/example/QueryAtom.class
+-rw-r--r--  2.0 unx     2101 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/example/LiftedExample.class
+-rw-r--r--  2.0 unx     2171 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/example/CompositeQuery.class
+-rw-r--r--  2.0 unx     2623 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/example/ValuedFact.class
+-rw-r--r--  2.0 unx     1937 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/example/LogicSample.class
+-rw-r--r--  2.0 unx     3245 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/example/GroundExample.class
+-rw-r--r--  2.0 unx     2627 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/transforming/SupervisedReducer.class
+-rw-r--r--  2.0 unx     3730 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/transforming/MetadataProcessor.class
+-rw-r--r--  2.0 unx     1162 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/transforming/SimpleTemplateMerger.class
+-rw-r--r--  2.0 unx     1723 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/transforming/TemplateChainReducer.class
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/transforming/TemplateMerging.class
+-rw-r--r--  2.0 unx     1095 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/transforming/TemplateReducing.class
+-rw-r--r--  2.0 unx     1729 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/metadata/TemplateMetadata.class
+-rw-r--r--  2.0 unx     5785 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/metadata/RuleMetadata.class
+-rw-r--r--  2.0 unx     6331 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/metadata/PredicateMetadata.class
+-rw-r--r--  2.0 unx     2992 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/components/GroundRule.class
+-rw-r--r--  2.0 unx     1664 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/components/HeadAtom.class
+-rw-r--r--  2.0 unx     2452 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/components/BodyAtom.class
+-rw-r--r--  2.0 unx     9930 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/components/WeightedRule.class
+-rw-r--r--  2.0 unx     2414 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/components/GroundHeadRule.class
+-rw-r--r--  2.0 unx    10131 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/Template.class
+-rw-r--r--  2.0 unx     4812 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate$Stratification.class
+-rw-r--r--  2.0 unx     1737 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/types/ParsedTemplate.class
+-rw-r--r--  2.0 unx     1016 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/types/RichLogicTemplate.class
+-rw-r--r--  2.0 unx     8405 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate.class
+-rw-r--r--  2.0 unx     2092 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate$UnsignedLiteral.class
+-rw-r--r--  2.0 unx    14044 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/Grounder.class
+-rw-r--r--  2.0 unx    17813 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/bottomUp/BottomUp.class
+-rw-r--r--  2.0 unx    21335 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/topDown/Gringo.class
+-rw-r--r--  2.0 unx     1196 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/topDown/TopDown.class
+-rw-r--r--  2.0 unx      297 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection$1.class
+-rw-r--r--  2.0 unx     1974 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection.class
+-rw-r--r--  2.0 unx     1112 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection$GroundRulesCollectionDuplicit.class
+-rw-r--r--  2.0 unx     1109 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection$GroundRulesCollectionUnique.class
+-rw-r--r--  2.0 unx     1610 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/GroundingSample.class
+-rw-r--r--  2.0 unx    10533 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/GroundTemplate.class
+-rw-r--r--  2.0 unx     1529 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/GroundingSample$Wrap.class
+-rw-r--r--  2.0 unx      885 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/grounding/Grounder$1.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Logical/
 -rw-r--r--  2.0 unx     1422 b- defN 22-Sep-14 19:24 META-INF/maven/io.github.gustiks/Logical/pom.xml
 -rw-r--r--  2.0 unx      110 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Logical/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/algebra/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/weights/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/utils/metadata/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-28 21:51 cz/cvut/fel/ida/algebra/values/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/inits/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/distributions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/algebra/functions/transformation/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/error/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/
--rw-r--r--  2.0 unx      978 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/weights/ScalarWeight.class
--rw-r--r--  2.0 unx     3795 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/weights/Weight.class
--rw-r--r--  2.0 unx     1304 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/weights/StatefulWeight.class
--rw-r--r--  2.0 unx     2059 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/utils/metadata/Parameter.class
--rw-r--r--  2.0 unx     1573 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/utils/metadata/Parameter$Type.class
--rw-r--r--  2.0 unx     2994 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/utils/metadata/ParameterValue.class
--rw-r--r--  2.0 unx     3813 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/utils/metadata/Metadata.class
--rw-r--r--  2.0 unx     1512 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/utils/metadata/ParameterValue$Type.class
--rw-r--r--  2.0 unx     4379 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/utils/metadata/WeightMetadata.class
--rw-r--r--  2.0 unx     4509 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/utils/MathUtils.class
--rw-r--r--  2.0 unx    14886 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/ScalarValue.class
--rw-r--r--  2.0 unx     4553 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/Value.class
--rw-r--r--  2.0 unx    20912 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/MatrixValue.class
--rw-r--r--  2.0 unx     7790 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/StringValue.class
--rw-r--r--  2.0 unx     9025 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/TensorValue.class
--rw-r--r--  2.0 unx     2060 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/inits/SimpleInitializer.class
--rw-r--r--  2.0 unx     1609 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/inits/HeUniformInitializer.class
--rw-r--r--  2.0 unx     1285 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/inits/ValueInitializer.class
--rw-r--r--  2.0 unx     2726 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/inits/GlorotUniformInitializer.class
--rw-r--r--  2.0 unx     9459 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/Zero.class
--rw-r--r--  2.0 unx      990 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/distributions/Constant.class
--rw-r--r--  2.0 unx     1172 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/distributions/Longtail.class
--rw-r--r--  2.0 unx     1142 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/distributions/Uniform.class
--rw-r--r--  2.0 unx      978 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/distributions/Normal.class
--rw-r--r--  2.0 unx     2045 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/distributions/Distribution.class
--rw-r--r--  2.0 unx     1214 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/MatrixValue$ValueIterator.class
--rw-r--r--  2.0 unx     1137 b- defN 23-Jan-28 21:51 cz/cvut/fel/ida/algebra/values/VectorValue$ValueIterator.class
--rw-r--r--  2.0 unx     1129 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/ScalarValue$ValueIterator.class
--rw-r--r--  2.0 unx    23137 b- defN 23-Jan-28 21:51 cz/cvut/fel/ida/algebra/values/VectorValue.class
--rw-r--r--  2.0 unx     1415 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/Tensor.class
--rw-r--r--  2.0 unx     9847 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/values/One.class
--rw-r--r--  2.0 unx     2071 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/AtIndex$State.class
--rw-r--r--  2.0 unx     2351 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Reshape.class
--rw-r--r--  2.0 unx     4051 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Normalization.class
--rw-r--r--  2.0 unx     2178 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Reshape$State.class
--rw-r--r--  2.0 unx     3344 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Normalization$State.class
--rw-r--r--  2.0 unx     2620 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/AtIndex.class
--rw-r--r--  2.0 unx     2692 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Transposition.class
--rw-r--r--  2.0 unx     2799 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Slice.class
--rw-r--r--  2.0 unx     1072 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Identity$State.class
--rw-r--r--  2.0 unx     1142 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/ConstantOne$State.class
--rw-r--r--  2.0 unx     2630 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Slice$State.class
--rw-r--r--  2.0 unx     1767 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Identity.class
--rw-r--r--  2.0 unx     1074 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/Transposition$State.class
--rw-r--r--  2.0 unx      316 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/XMax.class
--rw-r--r--  2.0 unx     1925 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/joint/ConstantOne.class
--rw-r--r--  2.0 unx     2447 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/ReLu.class
--rw-r--r--  2.0 unx     2617 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/LeakyReLu.class
--rw-r--r--  2.0 unx     2431 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Tanh.class
--rw-r--r--  2.0 unx     2421 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Inverse.class
--rw-r--r--  2.0 unx     2283 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Exponentiation.class
--rw-r--r--  2.0 unx     2505 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Reverse.class
--rw-r--r--  2.0 unx     2395 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/SquareRoot.class
--rw-r--r--  2.0 unx     2020 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Signum.class
--rw-r--r--  2.0 unx     2668 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/LukasiewiczSigmoid.class
--rw-r--r--  2.0 unx     2374 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Logarithm.class
--rw-r--r--  2.0 unx     2597 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Sigmoid.class
--rw-r--r--  2.0 unx     1466 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Aggregation$Singletons.class
--rw-r--r--  2.0 unx     2558 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/ActivationFcn$SimpleValueState.class
--rw-r--r--  2.0 unx     3079 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Combination.class
--rw-r--r--  2.0 unx     2232 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/error/SquaredDiff.class
--rw-r--r--  2.0 unx     3780 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/error/Crossentropy.class
--rw-r--r--  2.0 unx     3423 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/error/SoftEntropy.class
--rw-r--r--  2.0 unx     1029 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Transformation$1.class
--rw-r--r--  2.0 unx     1191 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Aggregation$State.class
--rw-r--r--  2.0 unx     3432 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/ActivationFcn$State.class
--rw-r--r--  2.0 unx     3235 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Transformation$State.class
--rw-r--r--  2.0 unx      733 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Average$TransformationState.class
--rw-r--r--  2.0 unx     2280 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum$TransformationState.class
--rw-r--r--  2.0 unx     3693 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Average.class
--rw-r--r--  2.0 unx     1877 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Count$AggregationState.class
--rw-r--r--  2.0 unx     4628 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum.class
--rw-r--r--  2.0 unx     1011 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Count$TransformationState.class
--rw-r--r--  2.0 unx      942 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Sum$TransformationState.class
--rw-r--r--  2.0 unx     4628 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum.class
--rw-r--r--  2.0 unx     2279 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum$TransformationState.class
--rw-r--r--  2.0 unx     2228 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Average$AggregationState.class
--rw-r--r--  2.0 unx     1410 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Sum$AggregationState.class
--rw-r--r--  2.0 unx     3373 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Count.class
--rw-r--r--  2.0 unx     1811 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum$AggregationState.class
--rw-r--r--  2.0 unx     1811 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum$AggregationState.class
--rw-r--r--  2.0 unx     3517 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/aggregation/Sum.class
--rw-r--r--  2.0 unx     1079 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/CrossSum$State$Mapping.class
--rw-r--r--  2.0 unx     2382 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/Product$State.class
--rw-r--r--  2.0 unx     4343 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/Sparsemax.class
--rw-r--r--  2.0 unx     4078 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/CosineSim$State.class
--rw-r--r--  2.0 unx     2480 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/Concatenation$State.class
--rw-r--r--  2.0 unx     2213 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/Softmax$CombinationState.class
--rw-r--r--  2.0 unx     5670 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/Concatenation.class
--rw-r--r--  2.0 unx     1632 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct$TransformationState.class
--rw-r--r--  2.0 unx     1959 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct$AggregationState.class
--rw-r--r--  2.0 unx     1596 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/Softmax$TransformationState.class
--rw-r--r--  2.0 unx     4064 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct.class
--rw-r--r--  2.0 unx     2491 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/Product.class
--rw-r--r--  2.0 unx     4103 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/CosineSim.class
--rw-r--r--  2.0 unx     6081 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/Softmax.class
--rw-r--r--  2.0 unx     3474 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/CrossSum.class
--rw-r--r--  2.0 unx     4817 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/combination/CrossSum$State.class
--rw-r--r--  2.0 unx     1521 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Combination$Singletons.class
--rw-r--r--  2.0 unx     1191 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/ElementWise$State.class
--rw-r--r--  2.0 unx     2671 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/ElementWise$Singletons.class
--rw-r--r--  2.0 unx      365 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/ErrorFcn.class
--rw-r--r--  2.0 unx     1247 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Combination$State.class
--rw-r--r--  2.0 unx     1614 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Transformation$Singletons.class
--rw-r--r--  2.0 unx     1036 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Aggregation$1.class
--rw-r--r--  2.0 unx     1695 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Combination$InputArrayState.class
--rw-r--r--  2.0 unx     3830 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/CompoundState.class
--rw-r--r--  2.0 unx     2482 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Transformation.class
--rw-r--r--  2.0 unx     1319 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/ActivationFcn.class
--rw-r--r--  2.0 unx     2363 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Aggregation.class
--rw-r--r--  2.0 unx     1309 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/ElementWise$1.class
--rw-r--r--  2.0 unx     3856 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/ElementWise.class
--rw-r--r--  2.0 unx     1107 b- defN 23-Jan-22 15:51 cz/cvut/fel/ida/algebra/functions/Combination$1.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-28 23:11 META-INF/maven/io.github.gustiks/Algebra/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/weights/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/utils/metadata/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/inits/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/distributions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/error/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/
+-rw-r--r--  2.0 unx      978 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/weights/ScalarWeight.class
+-rw-r--r--  2.0 unx     3795 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/weights/Weight.class
+-rw-r--r--  2.0 unx     1304 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/weights/StatefulWeight.class
+-rw-r--r--  2.0 unx     2059 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/utils/metadata/Parameter.class
+-rw-r--r--  2.0 unx     1573 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/utils/metadata/Parameter$Type.class
+-rw-r--r--  2.0 unx     2994 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/utils/metadata/ParameterValue.class
+-rw-r--r--  2.0 unx     3813 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/utils/metadata/Metadata.class
+-rw-r--r--  2.0 unx     1512 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/utils/metadata/ParameterValue$Type.class
+-rw-r--r--  2.0 unx     4379 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/utils/metadata/WeightMetadata.class
+-rw-r--r--  2.0 unx     4509 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/utils/MathUtils.class
+-rw-r--r--  2.0 unx    14886 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/ScalarValue.class
+-rw-r--r--  2.0 unx     4553 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/Value.class
+-rw-r--r--  2.0 unx    20912 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/MatrixValue.class
+-rw-r--r--  2.0 unx     7790 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/StringValue.class
+-rw-r--r--  2.0 unx     9025 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/TensorValue.class
+-rw-r--r--  2.0 unx     2060 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/inits/SimpleInitializer.class
+-rw-r--r--  2.0 unx     1609 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/inits/HeUniformInitializer.class
+-rw-r--r--  2.0 unx     1285 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/inits/ValueInitializer.class
+-rw-r--r--  2.0 unx     2726 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/inits/GlorotUniformInitializer.class
+-rw-r--r--  2.0 unx     9459 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/Zero.class
+-rw-r--r--  2.0 unx      990 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/distributions/Constant.class
+-rw-r--r--  2.0 unx     1172 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/distributions/Longtail.class
+-rw-r--r--  2.0 unx     1142 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/distributions/Uniform.class
+-rw-r--r--  2.0 unx      978 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/distributions/Normal.class
+-rw-r--r--  2.0 unx     2045 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/distributions/Distribution.class
+-rw-r--r--  2.0 unx     1214 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/MatrixValue$ValueIterator.class
+-rw-r--r--  2.0 unx     1137 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/VectorValue$ValueIterator.class
+-rw-r--r--  2.0 unx     1129 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/ScalarValue$ValueIterator.class
+-rw-r--r--  2.0 unx    23137 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/VectorValue.class
+-rw-r--r--  2.0 unx     1415 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/Tensor.class
+-rw-r--r--  2.0 unx     9847 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/values/One.class
+-rw-r--r--  2.0 unx     2071 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/AtIndex$State.class
+-rw-r--r--  2.0 unx     2351 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Reshape.class
+-rw-r--r--  2.0 unx     4051 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Normalization.class
+-rw-r--r--  2.0 unx     2178 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Reshape$State.class
+-rw-r--r--  2.0 unx     3344 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Normalization$State.class
+-rw-r--r--  2.0 unx     2620 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/AtIndex.class
+-rw-r--r--  2.0 unx     2692 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Transposition.class
+-rw-r--r--  2.0 unx     2799 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Slice.class
+-rw-r--r--  2.0 unx     1072 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Identity$State.class
+-rw-r--r--  2.0 unx     1142 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/ConstantOne$State.class
+-rw-r--r--  2.0 unx     2630 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Slice$State.class
+-rw-r--r--  2.0 unx     1767 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Identity.class
+-rw-r--r--  2.0 unx     1074 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/Transposition$State.class
+-rw-r--r--  2.0 unx      316 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/XMax.class
+-rw-r--r--  2.0 unx     1925 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/joint/ConstantOne.class
+-rw-r--r--  2.0 unx     2447 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/ReLu.class
+-rw-r--r--  2.0 unx     2617 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/LeakyReLu.class
+-rw-r--r--  2.0 unx     2431 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Tanh.class
+-rw-r--r--  2.0 unx     2421 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Inverse.class
+-rw-r--r--  2.0 unx     2283 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Exponentiation.class
+-rw-r--r--  2.0 unx     2505 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Reverse.class
+-rw-r--r--  2.0 unx     2395 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/SquareRoot.class
+-rw-r--r--  2.0 unx     2020 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Signum.class
+-rw-r--r--  2.0 unx     2668 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/LukasiewiczSigmoid.class
+-rw-r--r--  2.0 unx     2374 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Logarithm.class
+-rw-r--r--  2.0 unx     2597 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Sigmoid.class
+-rw-r--r--  2.0 unx     1466 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Aggregation$Singletons.class
+-rw-r--r--  2.0 unx     2558 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/ActivationFcn$SimpleValueState.class
+-rw-r--r--  2.0 unx     3079 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Combination.class
+-rw-r--r--  2.0 unx     2232 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/error/SquaredDiff.class
+-rw-r--r--  2.0 unx     3780 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/error/Crossentropy.class
+-rw-r--r--  2.0 unx     3423 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/error/SoftEntropy.class
+-rw-r--r--  2.0 unx     1029 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Transformation$1.class
+-rw-r--r--  2.0 unx     1191 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Aggregation$State.class
+-rw-r--r--  2.0 unx     3432 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/ActivationFcn$State.class
+-rw-r--r--  2.0 unx     3235 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Transformation$State.class
+-rw-r--r--  2.0 unx      733 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Average$TransformationState.class
+-rw-r--r--  2.0 unx     2280 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum$TransformationState.class
+-rw-r--r--  2.0 unx     3693 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Average.class
+-rw-r--r--  2.0 unx     1877 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Count$AggregationState.class
+-rw-r--r--  2.0 unx     4628 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum.class
+-rw-r--r--  2.0 unx     1011 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Count$TransformationState.class
+-rw-r--r--  2.0 unx      942 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Sum$TransformationState.class
+-rw-r--r--  2.0 unx     4628 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum.class
+-rw-r--r--  2.0 unx     2279 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum$TransformationState.class
+-rw-r--r--  2.0 unx     2228 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Average$AggregationState.class
+-rw-r--r--  2.0 unx     1410 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Sum$AggregationState.class
+-rw-r--r--  2.0 unx     3373 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Count.class
+-rw-r--r--  2.0 unx     1811 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum$AggregationState.class
+-rw-r--r--  2.0 unx     1811 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum$AggregationState.class
+-rw-r--r--  2.0 unx     3517 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/aggregation/Sum.class
+-rw-r--r--  2.0 unx     1079 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/CrossSum$State$Mapping.class
+-rw-r--r--  2.0 unx     2382 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/Product$State.class
+-rw-r--r--  2.0 unx     4343 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/Sparsemax.class
+-rw-r--r--  2.0 unx     4078 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/CosineSim$State.class
+-rw-r--r--  2.0 unx     2480 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/Concatenation$State.class
+-rw-r--r--  2.0 unx     2213 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/Softmax$CombinationState.class
+-rw-r--r--  2.0 unx     5670 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/Concatenation.class
+-rw-r--r--  2.0 unx     1632 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct$TransformationState.class
+-rw-r--r--  2.0 unx     1959 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct$AggregationState.class
+-rw-r--r--  2.0 unx     1596 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/Softmax$TransformationState.class
+-rw-r--r--  2.0 unx     4064 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct.class
+-rw-r--r--  2.0 unx     2491 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/Product.class
+-rw-r--r--  2.0 unx     4103 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/CosineSim.class
+-rw-r--r--  2.0 unx     6081 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/Softmax.class
+-rw-r--r--  2.0 unx     3474 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/CrossSum.class
+-rw-r--r--  2.0 unx     4817 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/combination/CrossSum$State.class
+-rw-r--r--  2.0 unx     1521 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Combination$Singletons.class
+-rw-r--r--  2.0 unx     1191 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/ElementWise$State.class
+-rw-r--r--  2.0 unx     2671 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/ElementWise$Singletons.class
+-rw-r--r--  2.0 unx      365 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/ErrorFcn.class
+-rw-r--r--  2.0 unx     1247 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Combination$State.class
+-rw-r--r--  2.0 unx     1614 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Transformation$Singletons.class
+-rw-r--r--  2.0 unx     1036 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Aggregation$1.class
+-rw-r--r--  2.0 unx     1695 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Combination$InputArrayState.class
+-rw-r--r--  2.0 unx     3830 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/CompoundState.class
+-rw-r--r--  2.0 unx     2482 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Transformation.class
+-rw-r--r--  2.0 unx     1319 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/ActivationFcn.class
+-rw-r--r--  2.0 unx     2363 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Aggregation.class
+-rw-r--r--  2.0 unx     1309 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/ElementWise$1.class
+-rw-r--r--  2.0 unx     3856 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/ElementWise.class
+-rw-r--r--  2.0 unx     1107 b- defN 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/Combination$1.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 META-INF/maven/io.github.gustiks/Algebra/
 -rw-r--r--  2.0 unx     1658 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Algebra/pom.xml
--rw-r--r--  2.0 unx      110 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Algebra/pom.properties
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-07 21:22 META-INF/maven/io.github.gustiks/Algebra/pom.properties
 drwxr-xr-x  2.0 unx        0 b- stor 20-Feb-14 14:23 org/jetbrains/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Feb-14 14:23 org/jetbrains/annotations/
 -rw-r--r--  2.0 unx     1220 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Nls$Capitalization.class
 -rw-r--r--  2.0 unx      787 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Nls.class
 -rw-r--r--  2.0 unx      703 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/NotNull.class
 -rw-r--r--  2.0 unx      564 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Nullable.class
 -rw-r--r--  2.0 unx      463 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Range.class
@@ -809,443 +812,443 @@
 -rw-r--r--  2.0 unx      443 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Async.class
 -rw-r--r--  2.0 unx      577 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Contract.class
 -rw-r--r--  2.0 unx      931 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Debug$Renderer.class
 -rw-r--r--  2.0 unx      380 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Debug.class
 -rw-r--r--  2.0 unx      508 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/NonNls.class
 -rw-r--r--  2.0 unx      525 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/PropertyKey.class
 -rw-r--r--  2.0 unx      478 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/TestOnly.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/logic/io/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/logic/special/
--rw-r--r--  2.0 unx     4849 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/ParserUtils.class
--rw-r--r--  2.0 unx     1447 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/Matching$1.class
--rw-r--r--  2.0 unx     7011 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionUtils.class
--rw-r--r--  2.0 unx     9526 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$ClauseE.class
--rw-r--r--  2.0 unx      419 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SymmetricPredicates.class
--rw-r--r--  2.0 unx      230 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SolutionConsumer.class
--rw-r--r--  2.0 unx     7696 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/MaxCardXorConstraint.class
--rw-r--r--  2.0 unx      829 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$HerbrandMap.class
--rw-r--r--  2.0 unx      255 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$1.class
--rw-r--r--  2.0 unx     1633 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$HighArityLiterals$2.class
--rw-r--r--  2.0 unx    20139 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/ApproximateSubsetCounter.class
--rw-r--r--  2.0 unx     3022 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$LowArityLiterals.class
--rw-r--r--  2.0 unx     1683 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$TupleNotIn.class
--rw-r--r--  2.0 unx     1889 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$PredicateSolutionConsumer.class
--rw-r--r--  2.0 unx      242 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/CustomPredicate.class
--rw-r--r--  2.0 unx     2592 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SpecialBinaryPredicates.class
--rw-r--r--  2.0 unx    35709 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2.class
--rw-r--r--  2.0 unx     2851 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SpecialVarargPredicates.class
--rw-r--r--  2.0 unx      559 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$ClauseStructure.class
--rw-r--r--  2.0 unx    10978 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/HerbrandModel.class
--rw-r--r--  2.0 unx     1447 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/Matching$2.class
--rw-r--r--  2.0 unx     4726 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$CompletelySymmetricLiterals.class
--rw-r--r--  2.0 unx    31343 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/Matching.class
--rw-r--r--  2.0 unx      347 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/GlobalConstraint.class
--rw-r--r--  2.0 unx     5595 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$HighArityLiterals.class
--rw-r--r--  2.0 unx    16949 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$ClauseC.class
--rw-r--r--  2.0 unx     1633 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$HighArityLiterals$1.class
--rw-r--r--  2.0 unx      286 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$LiteralPrunning.class
--rw-r--r--  2.0 unx    29526 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LogicUtils.class
--rw-r--r--  2.0 unx     4012 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/Constant.class
--rw-r--r--  2.0 unx     3022 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$TemplateBasedLiteralFilter.class
--rw-r--r--  2.0 unx     4854 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/PrologList.class
--rw-r--r--  2.0 unx     4143 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$BasicTermLGG.class
--rw-r--r--  2.0 unx     3114 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/Predicate.class
--rw-r--r--  2.0 unx      628 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$BasicLiteralFilter.class
--rw-r--r--  2.0 unx     1594 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$BasicLiteralLGG.class
--rw-r--r--  2.0 unx      399 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$LiteralLGG.class
--rw-r--r--  2.0 unx    14896 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/Clause.class
--rw-r--r--  2.0 unx     3591 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/Function.class
--rw-r--r--  2.0 unx     3229 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/Variable.class
--rw-r--r--  2.0 unx     1314 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/io/PrologParser$2.class
--rw-r--r--  2.0 unx     2812 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/io/Prolog2PseudoPrologReader.class
--rw-r--r--  2.0 unx     1314 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/io/PrologParser$1.class
--rw-r--r--  2.0 unx     2043 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/io/PseudoPrologParser.class
--rw-r--r--  2.0 unx     4403 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/io/PrologParser.class
--rw-r--r--  2.0 unx     3181 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$Lgg.class
--rw-r--r--  2.0 unx      499 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$TermLGG.class
--rw-r--r--  2.0 unx    12111 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/Literal.class
--rw-r--r--  2.0 unx    10537 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/special/IsoClauseWrapper.class
--rw-r--r--  2.0 unx      255 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$LiteralFilter.class
--rw-r--r--  2.0 unx     3717 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG.class
--rw-r--r--  2.0 unx      117 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/Formula.class
--rw-r--r--  2.0 unx      480 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/Term.class
--rw-r--r--  2.0 unx      201 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/LGG$1.class
--rw-r--r--  2.0 unx     7149 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/logic/HornClause.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 META-INF/maven/io.github.gustiks/Logic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/io/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/special/
+-rw-r--r--  2.0 unx     4849 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/ParserUtils.class
+-rw-r--r--  2.0 unx     1447 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/Matching$1.class
+-rw-r--r--  2.0 unx     7011 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionUtils.class
+-rw-r--r--  2.0 unx     9526 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$ClauseE.class
+-rw-r--r--  2.0 unx      419 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SymmetricPredicates.class
+-rw-r--r--  2.0 unx      230 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SolutionConsumer.class
+-rw-r--r--  2.0 unx     7696 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/MaxCardXorConstraint.class
+-rw-r--r--  2.0 unx      829 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$HerbrandMap.class
+-rw-r--r--  2.0 unx      255 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$1.class
+-rw-r--r--  2.0 unx     1633 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$HighArityLiterals$2.class
+-rw-r--r--  2.0 unx    20139 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/ApproximateSubsetCounter.class
+-rw-r--r--  2.0 unx     3022 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$LowArityLiterals.class
+-rw-r--r--  2.0 unx     1696 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$TupleNotIn.class
+-rw-r--r--  2.0 unx     1889 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$PredicateSolutionConsumer.class
+-rw-r--r--  2.0 unx      242 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/CustomPredicate.class
+-rw-r--r--  2.0 unx     2592 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SpecialBinaryPredicates.class
+-rw-r--r--  2.0 unx    35709 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2.class
+-rw-r--r--  2.0 unx     2851 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SpecialVarargPredicates.class
+-rw-r--r--  2.0 unx      559 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$ClauseStructure.class
+-rw-r--r--  2.0 unx    11255 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/HerbrandModel.class
+-rw-r--r--  2.0 unx     1447 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/Matching$2.class
+-rw-r--r--  2.0 unx     4726 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$CompletelySymmetricLiterals.class
+-rw-r--r--  2.0 unx    31343 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/Matching.class
+-rw-r--r--  2.0 unx      347 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/GlobalConstraint.class
+-rw-r--r--  2.0 unx     5595 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$HighArityLiterals.class
+-rw-r--r--  2.0 unx    16949 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$ClauseC.class
+-rw-r--r--  2.0 unx     1633 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$HighArityLiterals$1.class
+-rw-r--r--  2.0 unx      286 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$LiteralPrunning.class
+-rw-r--r--  2.0 unx    29526 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LogicUtils.class
+-rw-r--r--  2.0 unx     4012 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/Constant.class
+-rw-r--r--  2.0 unx     3022 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$TemplateBasedLiteralFilter.class
+-rw-r--r--  2.0 unx     4854 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/PrologList.class
+-rw-r--r--  2.0 unx     4143 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$BasicTermLGG.class
+-rw-r--r--  2.0 unx     3114 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/Predicate.class
+-rw-r--r--  2.0 unx      628 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$BasicLiteralFilter.class
+-rw-r--r--  2.0 unx     1594 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$BasicLiteralLGG.class
+-rw-r--r--  2.0 unx      399 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$LiteralLGG.class
+-rw-r--r--  2.0 unx    14896 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/Clause.class
+-rw-r--r--  2.0 unx     3591 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/Function.class
+-rw-r--r--  2.0 unx     3229 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/Variable.class
+-rw-r--r--  2.0 unx     1314 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/io/PrologParser$2.class
+-rw-r--r--  2.0 unx     2812 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/io/Prolog2PseudoPrologReader.class
+-rw-r--r--  2.0 unx     1314 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/io/PrologParser$1.class
+-rw-r--r--  2.0 unx     2043 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/io/PseudoPrologParser.class
+-rw-r--r--  2.0 unx     4403 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/io/PrologParser.class
+-rw-r--r--  2.0 unx     3181 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$Lgg.class
+-rw-r--r--  2.0 unx      499 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$TermLGG.class
+-rw-r--r--  2.0 unx    12077 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/Literal.class
+-rw-r--r--  2.0 unx    10537 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/special/IsoClauseWrapper.class
+-rw-r--r--  2.0 unx      255 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$LiteralFilter.class
+-rw-r--r--  2.0 unx     3717 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG.class
+-rw-r--r--  2.0 unx      117 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/Formula.class
+-rw-r--r--  2.0 unx      480 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/Term.class
+-rw-r--r--  2.0 unx      201 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/LGG$1.class
+-rw-r--r--  2.0 unx     6976 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/HornClause.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Logic/
 -rw-r--r--  2.0 unx      799 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Logic/pom.xml
 -rw-r--r--  2.0 unx      108 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Logic/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/learning/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/metrics/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/metrics/Jesse/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/splitting/
--rw-r--r--  2.0 unx      380 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/Learner.class
--rw-r--r--  2.0 unx     1409 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/Query.class
--rw-r--r--  2.0 unx      498 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/Model.class
--rw-r--r--  2.0 unx      258 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/Example.class
--rw-r--r--  2.0 unx     1668 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/LearningSample.class
--rw-r--r--  2.0 unx     2298 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Results$Factory.class
--rw-r--r--  2.0 unx     1403 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Results$RegressionFactory.class
--rw-r--r--  2.0 unx     2737 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Progress.class
--rw-r--r--  2.0 unx     1781 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Progress$TrainVal.class
--rw-r--r--  2.0 unx     1747 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/VoidResults.class
--rw-r--r--  2.0 unx     7754 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/DetailedClassificationResults.class
--rw-r--r--  2.0 unx      950 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Results$2.class
--rw-r--r--  2.0 unx    11974 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/ClassificationResults.class
--rw-r--r--  2.0 unx     2235 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/metrics/HITS$Stats.class
--rw-r--r--  2.0 unx     1383 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/metrics/Jesse/ROCpoint.class
--rw-r--r--  2.0 unx     5038 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/metrics/Jesse/Confusions.class
--rw-r--r--  2.0 unx     3959 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/metrics/AUC.class
--rw-r--r--  2.0 unx    15712 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/metrics/HITS.class
--rw-r--r--  2.0 unx     1748 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/metrics/HITS$1.class
--rw-r--r--  2.0 unx     1487 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Results$DetailedClassificationFactory.class
--rw-r--r--  2.0 unx     2354 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Results$KBCFactory.class
--rw-r--r--  2.0 unx     3282 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Result.class
--rw-r--r--  2.0 unx     1011 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/DetailedClassificationResults$1.class
--rw-r--r--  2.0 unx     3922 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/RegressionResults.class
--rw-r--r--  2.0 unx     1213 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Results$1.class
--rw-r--r--  2.0 unx     2207 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Result$Factory.class
--rw-r--r--  2.0 unx      232 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Result$1.class
--rw-r--r--  2.0 unx     1431 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Results$ClassificationFactory.class
--rw-r--r--  2.0 unx      869 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Progress$Restart.class
--rw-r--r--  2.0 unx     5463 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Results.class
--rw-r--r--  2.0 unx     1214 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/Results$VoidFactory.class
--rw-r--r--  2.0 unx     2411 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/results/KBCResults.class
--rw-r--r--  2.0 unx      855 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/MeanStdResults$TrainValTest.class
--rw-r--r--  2.0 unx     1329 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/TrainTestResults.class
--rw-r--r--  2.0 unx    11471 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/Crossvalidation.class
--rw-r--r--  2.0 unx     1138 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/Fold.class
--rw-r--r--  2.0 unx      974 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/MeanStdResults.class
--rw-r--r--  2.0 unx     8100 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/splitting/StratifiedSplitter.class
--rw-r--r--  2.0 unx     4275 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/splitting/Splitter.class
--rw-r--r--  2.0 unx     2737 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/crossvalidation/splitting/LinearSplitter.class
--rw-r--r--  2.0 unx      446 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/Classifier.class
--rw-r--r--  2.0 unx      402 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/Regressor.class
--rw-r--r--  2.0 unx     1274 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/learning/LearningSample$Split.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 20:14 META-INF/maven/io.github.gustiks/Learning/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/Jesse/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/splitting/
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/Learner.class
+-rw-r--r--  2.0 unx     1409 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/Query.class
+-rw-r--r--  2.0 unx      498 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/Model.class
+-rw-r--r--  2.0 unx      258 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/Example.class
+-rw-r--r--  2.0 unx     1668 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/LearningSample.class
+-rw-r--r--  2.0 unx     2298 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Results$Factory.class
+-rw-r--r--  2.0 unx     1403 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Results$RegressionFactory.class
+-rw-r--r--  2.0 unx     2737 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Progress.class
+-rw-r--r--  2.0 unx     1781 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Progress$TrainVal.class
+-rw-r--r--  2.0 unx     1747 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/VoidResults.class
+-rw-r--r--  2.0 unx     7754 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/DetailedClassificationResults.class
+-rw-r--r--  2.0 unx      950 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Results$2.class
+-rw-r--r--  2.0 unx    11974 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/ClassificationResults.class
+-rw-r--r--  2.0 unx     2235 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/HITS$Stats.class
+-rw-r--r--  2.0 unx     1383 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/Jesse/ROCpoint.class
+-rw-r--r--  2.0 unx     5038 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/Jesse/Confusions.class
+-rw-r--r--  2.0 unx     3959 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/AUC.class
+-rw-r--r--  2.0 unx    15712 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/HITS.class
+-rw-r--r--  2.0 unx     1748 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/HITS$1.class
+-rw-r--r--  2.0 unx     1487 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Results$DetailedClassificationFactory.class
+-rw-r--r--  2.0 unx     2354 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Results$KBCFactory.class
+-rw-r--r--  2.0 unx     3282 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Result.class
+-rw-r--r--  2.0 unx     1011 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/DetailedClassificationResults$1.class
+-rw-r--r--  2.0 unx     3922 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/RegressionResults.class
+-rw-r--r--  2.0 unx     1213 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Results$1.class
+-rw-r--r--  2.0 unx     2207 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Result$Factory.class
+-rw-r--r--  2.0 unx      232 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Result$1.class
+-rw-r--r--  2.0 unx     1431 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Results$ClassificationFactory.class
+-rw-r--r--  2.0 unx      869 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Progress$Restart.class
+-rw-r--r--  2.0 unx     5463 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Results.class
+-rw-r--r--  2.0 unx     1214 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/Results$VoidFactory.class
+-rw-r--r--  2.0 unx     2411 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/KBCResults.class
+-rw-r--r--  2.0 unx      855 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/MeanStdResults$TrainValTest.class
+-rw-r--r--  2.0 unx     1329 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/TrainTestResults.class
+-rw-r--r--  2.0 unx    11471 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/Crossvalidation.class
+-rw-r--r--  2.0 unx     1138 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/Fold.class
+-rw-r--r--  2.0 unx      974 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/MeanStdResults.class
+-rw-r--r--  2.0 unx     8100 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/splitting/StratifiedSplitter.class
+-rw-r--r--  2.0 unx     4275 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/splitting/Splitter.class
+-rw-r--r--  2.0 unx     2737 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/splitting/LinearSplitter.class
+-rw-r--r--  2.0 unx      446 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/Classifier.class
+-rw-r--r--  2.0 unx      402 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/Regressor.class
+-rw-r--r--  2.0 unx     1274 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/learning/LearningSample$Split.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Learning/
 -rw-r--r--  2.0 unx     1439 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Learning/pom.xml
 -rw-r--r--  2.0 unx      111 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Learning/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/neural/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/computation/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/weights/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/optimizers/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/debugging/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/structure/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/structure/building/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/building/builders/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/building/factories/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/export/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/types/
--rw-r--r--  2.0 unx     2266 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/NeuronVisiting.class
--rw-r--r--  2.0 unx     1921 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/NeuronVisiting$Weighted.class
--rw-r--r--  2.0 unx     3123 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/NeuronIterating.class
--rw-r--r--  2.0 unx     1352 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/BFS.class
--rw-r--r--  2.0 unx     8499 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack$TDownVisitor.class
--rw-r--r--  2.0 unx     6547 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack$BUpIterator.class
--rw-r--r--  2.0 unx     4139 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic$BUpIterator.class
--rw-r--r--  2.0 unx     4252 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic$TDownVisitor.class
--rw-r--r--  2.0 unx     5486 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/BFS$TDownIterator.class
--rw-r--r--  2.0 unx     3113 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic$TDownIterator.class
--rw-r--r--  2.0 unx     6813 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSrecursion$BUpVisitor.class
--rw-r--r--  2.0 unx     2010 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic.class
--rw-r--r--  2.0 unx     5615 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic$BUpVisitor.class
--rw-r--r--  2.0 unx     8437 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/BFS$TDownVisitor.class
--rw-r--r--  2.0 unx     5650 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack$TDownIterator.class
--rw-r--r--  2.0 unx     6526 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack$BUpVisitor.class
--rw-r--r--  2.0 unx     7519 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSrecursion$TDownVisitor.class
--rw-r--r--  2.0 unx     1972 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack.class
--rw-r--r--  2.0 unx      907 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSrecursion.class
--rw-r--r--  2.0 unx     7900 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/Accumulating.class
--rw-r--r--  2.0 unx     7980 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/Evaluation.class
--rw-r--r--  2.0 unx      240 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/PythonHookHandler.class
--rw-r--r--  2.0 unx     7735 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/PythonEvaluation.class
--rw-r--r--  2.0 unx     4789 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/IndependentNeuronProcessing.class
--rw-r--r--  2.0 unx     7015 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/PythonEvaluation$PythonUp.class
--rw-r--r--  2.0 unx     9314 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/Backpropagation.class
--rw-r--r--  2.0 unx     4808 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Accumulator.class
--rw-r--r--  2.0 unx     3204 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted.class
--rw-r--r--  2.0 unx     2353 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor.class
--rw-r--r--  2.0 unx     6105 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Up.class
--rw-r--r--  2.0 unx     8143 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/StateInitializer.class
--rw-r--r--  2.0 unx     3060 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted$Indexed.class
--rw-r--r--  2.0 unx     4156 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted$Detailed.class
--rw-r--r--  2.0 unx     3493 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Independent.class
--rw-r--r--  2.0 unx     6912 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Down.class
--rw-r--r--  2.0 unx     3217 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/weights/WeightUpdater.class
--rw-r--r--  2.0 unx      278 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/weights/WeightVisitor.class
--rw-r--r--  2.0 unx     1584 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Invalidator.class
--rw-r--r--  2.0 unx     3408 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Dropouter.class
--rw-r--r--  2.0 unx     3266 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Backproper.class
--rw-r--r--  2.0 unx      546 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Evaluator$one.class
--rw-r--r--  2.0 unx     2960 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Evaluator.class
--rw-r--r--  2.0 unx     2688 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/SaturationChecker.class
--rw-r--r--  2.0 unx     1002 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/BackproperWithWeightUpdates.class
--rw-r--r--  2.0 unx     3360 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/ParentsTransfer.class
--rw-r--r--  2.0 unx     2248 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/OutputsGetter.class
--rw-r--r--  2.0 unx     2381 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/InputsGetter$Weighted.class
--rw-r--r--  2.0 unx     1518 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/ParentsGetter.class
--rw-r--r--  2.0 unx     2364 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/InputsGetter.class
--rw-r--r--  2.0 unx     1692 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/StateVisiting$Structure.class
--rw-r--r--  2.0 unx     2405 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/StateVisiting$Computation.class
--rw-r--r--  2.0 unx     1443 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/StateVisiting.class
--rw-r--r--  2.0 unx     2136 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/StateVisiting$Computation$Detailed.class
--rw-r--r--  2.0 unx      193 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/DirectedIteration.class
--rw-r--r--  2.0 unx     1255 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/NeuronIterator.class
--rw-r--r--  2.0 unx      458 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/TopDown.class
--rw-r--r--  2.0 unx     1804 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/IterationStrategy.class
--rw-r--r--  2.0 unx      753 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/iteration/BottomUp.class
--rw-r--r--  2.0 unx     1249 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/NeuralSample.class
--rw-r--r--  2.0 unx     3118 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/optimizers/Adam.class
--rw-r--r--  2.0 unx     2184 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/optimizers/Optimizer.class
--rw-r--r--  2.0 unx     2162 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/optimizers/SGD.class
--rw-r--r--  2.0 unx     8243 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/NeuralModel.class
--rw-r--r--  2.0 unx    21171 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/IterativeTrainingStrategy.class
--rw-r--r--  2.0 unx     6058 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/StreamTrainingStrategy.class
--rw-r--r--  2.0 unx      302 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/debugging/NeuralDebugging.class
--rw-r--r--  2.0 unx     1594 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/RestartingStrategy.class
--rw-r--r--  2.0 unx     4379 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/DynamicRestartingStrategy.class
--rw-r--r--  2.0 unx     1269 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/StaticRestartingStrategy.class
--rw-r--r--  2.0 unx     1965 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/GeometricDecay.class
--rw-r--r--  2.0 unx     1492 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/ArithmeticDecay.class
--rw-r--r--  2.0 unx     1048 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/DynamicRestartingStrategy$1.class
--rw-r--r--  2.0 unx     2626 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/LearnRateDecayStrategy.class
--rw-r--r--  2.0 unx      962 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/LearnRateDecayStrategy$1.class
--rw-r--r--  2.0 unx     2950 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/DropoutRateStrategy.class
--rw-r--r--  2.0 unx     7416 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/TrainingStrategy.class
--rw-r--r--  2.0 unx    11280 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/PythonTrainingStrategy.class
--rw-r--r--  2.0 unx      341 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/Training.class
--rw-r--r--  2.0 unx    10439 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/MiniBatchTrainer.class
--rw-r--r--  2.0 unx     4344 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/SequentialTrainer$SequentialStreamTrainer.class
--rw-r--r--  2.0 unx     4528 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/MiniBatchTrainer$MinibatchStreamTrainer.class
--rw-r--r--  2.0 unx     1607 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/AsyncParallelTrainer.class
--rw-r--r--  2.0 unx     4098 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/MiniBatchTrainer$MinibatchListTrainer.class
--rw-r--r--  2.0 unx     4330 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/SequentialTrainer.class
--rw-r--r--  2.0 unx      893 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/ListTrainer.class
--rw-r--r--  2.0 unx     4408 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/AsyncParallelTrainer$AsyncStreamTrainer.class
--rw-r--r--  2.0 unx     6503 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/Trainer.class
--rw-r--r--  2.0 unx     6402 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/SequentialTrainer$SequentialListTrainer.class
--rw-r--r--  2.0 unx      664 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/StreamTrainer.class
--rw-r--r--  2.0 unx     2031 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/MiniBatchTrainer$MiniBatchIterator.class
--rw-r--r--  2.0 unx     5738 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/AsyncParallelTrainer$AsyncListTrainer.class
--rw-r--r--  2.0 unx     1204 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/computation/training/strategies/TrainingStrategy$TrainVal.class
--rw-r--r--  2.0 unx    19204 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/building/builders/StatesBuilder.class
--rw-r--r--  2.0 unx     7527 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/building/factories/NeuralNetFactory.class
--rw-r--r--  2.0 unx     2667 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/IsoValueNetworkCompressor$ValueList.class
--rw-r--r--  2.0 unx    10554 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/LinearChainReducer.class
--rw-r--r--  2.0 unx     4582 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/ParallelEdgeMerger.class
--rw-r--r--  2.0 unx    24438 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/IsoValueNetworkCompressor.class
--rw-r--r--  2.0 unx      705 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/CycleBreaking.class
--rw-r--r--  2.0 unx     3823 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/ParentsExtractor.class
--rw-r--r--  2.0 unx     8563 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/ParallelEdgeMerger$MergingVisitor.class
--rw-r--r--  2.0 unx      677 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/IsoGradientCompressor.class
--rw-r--r--  2.0 unx      766 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/SimpleCycleBreaker.class
--rw-r--r--  2.0 unx     3754 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/NetworkReducing.class
--rw-r--r--  2.0 unx      389 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/transforming/NetworkMerging.class
--rw-r--r--  2.0 unx      802 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/NetworkMetadata.class
--rw-r--r--  2.0 unx     3335 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/WeightedNeuronMapping.class
--rw-r--r--  2.0 unx      623 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/LinkedMapping.class
--rw-r--r--  2.0 unx     2524 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/WeightedNeuronMapping$WeightIterator.class
--rw-r--r--  2.0 unx     5321 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/NeuronMapping.class
--rw-r--r--  2.0 unx     2254 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/NeuronMapping$InputIterator.class
--rw-r--r--  2.0 unx      520 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/LinkedMapping$WeightMapping.class
--rw-r--r--  2.0 unx      696 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/metadata/NeuronMetadata.class
--rw-r--r--  2.0 unx     1402 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/export/NeuralSerializer$SerializedWeight.class
--rw-r--r--  2.0 unx     7631 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/export/NeuralSerializer$SerializedNeuron.class
--rw-r--r--  2.0 unx     6202 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/export/NeuralSerializer.class
--rw-r--r--  2.0 unx     2378 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/export/NeuralSerializer$SerializedSample.class
--rw-r--r--  2.0 unx     6985 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/BaseNeuron.class
--rw-r--r--  2.0 unx     2423 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/Neurons.class
--rw-r--r--  2.0 unx     3676 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/QueryNeuron.class
--rw-r--r--  2.0 unx     6164 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/WeightedNeuron.class
--rw-r--r--  2.0 unx     2355 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/WeightedNeuron$WeightedInputsIterator.class
--rw-r--r--  2.0 unx      833 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure$Parents.class
--rw-r--r--  2.0 unx     1915 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$WeightedInputs.class
--rw-r--r--  2.0 unx     1451 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache$DirectCache.class
--rw-r--r--  2.0 unx     1239 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural$Computation$HasDropout.class
--rw-r--r--  2.0 unx     1598 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure.class
--rw-r--r--  2.0 unx      839 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural.class
--rw-r--r--  2.0 unx     1834 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$Inputs.class
--rw-r--r--  2.0 unx     1011 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure$WeightedInputsMap.class
--rw-r--r--  2.0 unx     1523 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$Outputs.class
--rw-r--r--  2.0 unx     4711 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$ComputationStateStandard.class
--rw-r--r--  2.0 unx     5426 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State.class
--rw-r--r--  2.0 unx     1928 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States.class
--rw-r--r--  2.0 unx     1621 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache$HeapCache.class
--rw-r--r--  2.0 unx     1774 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache$HashCache.class
--rw-r--r--  2.0 unx      802 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural$Computation$HasParents.class
--rw-r--r--  2.0 unx      998 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$1.class
--rw-r--r--  2.0 unx     5235 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$DropoutStore$ParentsDropoutStore.class
--rw-r--r--  2.0 unx      978 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure$InputNeuronMap.class
--rw-r--r--  2.0 unx     1583 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache$LinearCache.class
--rw-r--r--  2.0 unx     5422 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache.class
--rw-r--r--  2.0 unx      981 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure$OutputNeuronMap.class
--rw-r--r--  2.0 unx     3202 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$NetworkParents$WeightedInputsParents.class
--rw-r--r--  2.0 unx     3203 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$ComputationStateComposite.class
--rw-r--r--  2.0 unx     4866 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$ParentCounter.class
--rw-r--r--  2.0 unx     3238 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$NetworkParents.class
--rw-r--r--  2.0 unx     2411 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural$Computation.class
--rw-r--r--  2.0 unx     4438 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$DropoutStore.class
--rw-r--r--  2.0 unx      769 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural$Computation$Detailed.class
--rw-r--r--  2.0 unx     3839 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$SimpleValue.class
--rw-r--r--  2.0 unx     3103 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$NetworkParents$InputsParents.class
--rw-r--r--  2.0 unx     2552 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/AtomNeuron.class
--rw-r--r--  2.0 unx      754 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/AtomNeurons.class
--rw-r--r--  2.0 unx     2840 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/WeightedAtomNeuron.class
--rw-r--r--  2.0 unx     2277 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/AggregationNeuron.class
--rw-r--r--  2.0 unx     3168 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/NegationNeuron.class
--rw-r--r--  2.0 unx     2384 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/SplittableAggregationNeuron.class
--rw-r--r--  2.0 unx      789 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/AtomFact.class
--rw-r--r--  2.0 unx     3003 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/WeightedRuleNeuron.class
--rw-r--r--  2.0 unx      730 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/RuleNeurons.class
--rw-r--r--  2.0 unx     3724 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/FactNeuron.class
--rw-r--r--  2.0 unx     2487 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/RuleNeuron.class
--rw-r--r--  2.0 unx    13927 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/NeuralNetwork.class
--rw-r--r--  2.0 unx     5493 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/NeuralSets.class
--rw-r--r--  2.0 unx      597 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/NeuralLayer.class
--rw-r--r--  2.0 unx     1404 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/NeuralSets$NeuronCounter.class
--rw-r--r--  2.0 unx     6209 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/types/TopologicNetwork.class
--rw-r--r--  2.0 unx    14189 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/types/DetailedNetwork.class
--rw-r--r--  2.0 unx     5981 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/types/TopologicNetwork$TopoSorting.class
--rw-r--r--  2.0 unx     1037 b- defN 23-Mar-03 23:03 cz/cvut/fel/ida/neural/networks/structure/components/types/LayeredNetwork.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-03 23:03 META-INF/maven/io.github.gustiks/Neural/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/weights/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/optimizers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/debugging/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/builders/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/factories/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/export/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/types/
+-rw-r--r--  2.0 unx     2266 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/NeuronVisiting.class
+-rw-r--r--  2.0 unx     1921 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/NeuronVisiting$Weighted.class
+-rw-r--r--  2.0 unx     3123 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/NeuronIterating.class
+-rw-r--r--  2.0 unx     1352 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/BFS.class
+-rw-r--r--  2.0 unx     8499 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack$TDownVisitor.class
+-rw-r--r--  2.0 unx     6547 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack$BUpIterator.class
+-rw-r--r--  2.0 unx     4139 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic$BUpIterator.class
+-rw-r--r--  2.0 unx     4252 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic$TDownVisitor.class
+-rw-r--r--  2.0 unx     5486 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/BFS$TDownIterator.class
+-rw-r--r--  2.0 unx     3113 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic$TDownIterator.class
+-rw-r--r--  2.0 unx     6813 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSrecursion$BUpVisitor.class
+-rw-r--r--  2.0 unx     2010 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic.class
+-rw-r--r--  2.0 unx     5615 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/Topologic$BUpVisitor.class
+-rw-r--r--  2.0 unx     8437 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/BFS$TDownVisitor.class
+-rw-r--r--  2.0 unx     5650 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack$TDownIterator.class
+-rw-r--r--  2.0 unx     6526 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack$BUpVisitor.class
+-rw-r--r--  2.0 unx     7519 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSrecursion$TDownVisitor.class
+-rw-r--r--  2.0 unx     1972 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSstack.class
+-rw-r--r--  2.0 unx      907 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/DFSrecursion.class
+-rw-r--r--  2.0 unx     7900 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/Accumulating.class
+-rw-r--r--  2.0 unx     7980 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/Evaluation.class
+-rw-r--r--  2.0 unx      240 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/PythonHookHandler.class
+-rw-r--r--  2.0 unx     7735 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/PythonEvaluation.class
+-rw-r--r--  2.0 unx     4789 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/IndependentNeuronProcessing.class
+-rw-r--r--  2.0 unx     7015 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/PythonEvaluation$PythonUp.class
+-rw-r--r--  2.0 unx     9314 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/Backpropagation.class
+-rw-r--r--  2.0 unx     4808 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Accumulator.class
+-rw-r--r--  2.0 unx     3204 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted.class
+-rw-r--r--  2.0 unx     2353 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor.class
+-rw-r--r--  2.0 unx     6105 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Up.class
+-rw-r--r--  2.0 unx     8143 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/StateInitializer.class
+-rw-r--r--  2.0 unx     3060 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted$Indexed.class
+-rw-r--r--  2.0 unx     4156 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted$Detailed.class
+-rw-r--r--  2.0 unx     3493 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Independent.class
+-rw-r--r--  2.0 unx     6912 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Down.class
+-rw-r--r--  2.0 unx     3217 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/weights/WeightUpdater.class
+-rw-r--r--  2.0 unx      278 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/weights/WeightVisitor.class
+-rw-r--r--  2.0 unx     1584 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Invalidator.class
+-rw-r--r--  2.0 unx     3408 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Dropouter.class
+-rw-r--r--  2.0 unx     3266 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Backproper.class
+-rw-r--r--  2.0 unx      546 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Evaluator$one.class
+-rw-r--r--  2.0 unx     2960 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Evaluator.class
+-rw-r--r--  2.0 unx     2688 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/SaturationChecker.class
+-rw-r--r--  2.0 unx     1002 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/BackproperWithWeightUpdates.class
+-rw-r--r--  2.0 unx     3360 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/ParentsTransfer.class
+-rw-r--r--  2.0 unx     2248 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/OutputsGetter.class
+-rw-r--r--  2.0 unx     2381 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/InputsGetter$Weighted.class
+-rw-r--r--  2.0 unx     1518 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/ParentsGetter.class
+-rw-r--r--  2.0 unx     2364 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/InputsGetter.class
+-rw-r--r--  2.0 unx     1692 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/StateVisiting$Structure.class
+-rw-r--r--  2.0 unx     2405 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/StateVisiting$Computation.class
+-rw-r--r--  2.0 unx     1443 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/StateVisiting.class
+-rw-r--r--  2.0 unx     2136 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/StateVisiting$Computation$Detailed.class
+-rw-r--r--  2.0 unx      193 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/DirectedIteration.class
+-rw-r--r--  2.0 unx     1255 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/NeuronIterator.class
+-rw-r--r--  2.0 unx      458 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/TopDown.class
+-rw-r--r--  2.0 unx     1804 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/IterationStrategy.class
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/BottomUp.class
+-rw-r--r--  2.0 unx     1249 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/NeuralSample.class
+-rw-r--r--  2.0 unx     3118 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/optimizers/Adam.class
+-rw-r--r--  2.0 unx     2184 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/optimizers/Optimizer.class
+-rw-r--r--  2.0 unx     2162 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/optimizers/SGD.class
+-rw-r--r--  2.0 unx     8243 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/NeuralModel.class
+-rw-r--r--  2.0 unx    21171 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/IterativeTrainingStrategy.class
+-rw-r--r--  2.0 unx     6058 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/StreamTrainingStrategy.class
+-rw-r--r--  2.0 unx      302 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/debugging/NeuralDebugging.class
+-rw-r--r--  2.0 unx     1594 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/RestartingStrategy.class
+-rw-r--r--  2.0 unx     4379 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/DynamicRestartingStrategy.class
+-rw-r--r--  2.0 unx     1269 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/StaticRestartingStrategy.class
+-rw-r--r--  2.0 unx     1965 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/GeometricDecay.class
+-rw-r--r--  2.0 unx     1492 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/ArithmeticDecay.class
+-rw-r--r--  2.0 unx     1048 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/DynamicRestartingStrategy$1.class
+-rw-r--r--  2.0 unx     2626 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/LearnRateDecayStrategy.class
+-rw-r--r--  2.0 unx      962 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/LearnRateDecayStrategy$1.class
+-rw-r--r--  2.0 unx     2950 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/Hyperparameters/DropoutRateStrategy.class
+-rw-r--r--  2.0 unx     7416 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/TrainingStrategy.class
+-rw-r--r--  2.0 unx    11280 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/PythonTrainingStrategy.class
+-rw-r--r--  2.0 unx      341 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/Training.class
+-rw-r--r--  2.0 unx    10439 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/MiniBatchTrainer.class
+-rw-r--r--  2.0 unx     4344 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/SequentialTrainer$SequentialStreamTrainer.class
+-rw-r--r--  2.0 unx     4528 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/MiniBatchTrainer$MinibatchStreamTrainer.class
+-rw-r--r--  2.0 unx     1607 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/AsyncParallelTrainer.class
+-rw-r--r--  2.0 unx     4098 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/MiniBatchTrainer$MinibatchListTrainer.class
+-rw-r--r--  2.0 unx     4330 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/SequentialTrainer.class
+-rw-r--r--  2.0 unx      893 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/ListTrainer.class
+-rw-r--r--  2.0 unx     4408 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/AsyncParallelTrainer$AsyncStreamTrainer.class
+-rw-r--r--  2.0 unx     6503 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/Trainer.class
+-rw-r--r--  2.0 unx     6402 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/SequentialTrainer$SequentialListTrainer.class
+-rw-r--r--  2.0 unx      664 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/StreamTrainer.class
+-rw-r--r--  2.0 unx     2031 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/MiniBatchTrainer$MiniBatchIterator.class
+-rw-r--r--  2.0 unx     5738 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/trainers/AsyncParallelTrainer$AsyncListTrainer.class
+-rw-r--r--  2.0 unx     1204 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/training/strategies/TrainingStrategy$TrainVal.class
+-rw-r--r--  2.0 unx    19204 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/builders/StatesBuilder.class
+-rw-r--r--  2.0 unx     7527 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/factories/NeuralNetFactory.class
+-rw-r--r--  2.0 unx     2667 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/IsoValueNetworkCompressor$ValueList.class
+-rw-r--r--  2.0 unx    10554 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/LinearChainReducer.class
+-rw-r--r--  2.0 unx     4582 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/ParallelEdgeMerger.class
+-rw-r--r--  2.0 unx    24438 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/IsoValueNetworkCompressor.class
+-rw-r--r--  2.0 unx      705 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/CycleBreaking.class
+-rw-r--r--  2.0 unx     3823 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/ParentsExtractor.class
+-rw-r--r--  2.0 unx     8563 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/ParallelEdgeMerger$MergingVisitor.class
+-rw-r--r--  2.0 unx      677 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/IsoGradientCompressor.class
+-rw-r--r--  2.0 unx      766 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/SimpleCycleBreaker.class
+-rw-r--r--  2.0 unx     3754 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/NetworkReducing.class
+-rw-r--r--  2.0 unx      389 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/transforming/NetworkMerging.class
+-rw-r--r--  2.0 unx      802 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/NetworkMetadata.class
+-rw-r--r--  2.0 unx     3335 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/WeightedNeuronMapping.class
+-rw-r--r--  2.0 unx      623 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/LinkedMapping.class
+-rw-r--r--  2.0 unx     2524 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/WeightedNeuronMapping$WeightIterator.class
+-rw-r--r--  2.0 unx     5321 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/NeuronMapping.class
+-rw-r--r--  2.0 unx     2254 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/NeuronMapping$InputIterator.class
+-rw-r--r--  2.0 unx      520 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/inputMappings/LinkedMapping$WeightMapping.class
+-rw-r--r--  2.0 unx      696 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/metadata/NeuronMetadata.class
+-rw-r--r--  2.0 unx     1402 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/export/NeuralSerializer$SerializedWeight.class
+-rw-r--r--  2.0 unx     7631 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/export/NeuralSerializer$SerializedNeuron.class
+-rw-r--r--  2.0 unx     6202 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/export/NeuralSerializer.class
+-rw-r--r--  2.0 unx     2378 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/export/NeuralSerializer$SerializedSample.class
+-rw-r--r--  2.0 unx     7425 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/BaseNeuron.class
+-rw-r--r--  2.0 unx     2423 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/Neurons.class
+-rw-r--r--  2.0 unx     3676 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/QueryNeuron.class
+-rw-r--r--  2.0 unx     6164 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/WeightedNeuron.class
+-rw-r--r--  2.0 unx     2355 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/WeightedNeuron$WeightedInputsIterator.class
+-rw-r--r--  2.0 unx      833 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure$Parents.class
+-rw-r--r--  2.0 unx     1915 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$WeightedInputs.class
+-rw-r--r--  2.0 unx     1451 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache$DirectCache.class
+-rw-r--r--  2.0 unx     1239 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural$Computation$HasDropout.class
+-rw-r--r--  2.0 unx     1598 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure.class
+-rw-r--r--  2.0 unx      839 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural.class
+-rw-r--r--  2.0 unx     1834 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$Inputs.class
+-rw-r--r--  2.0 unx     1011 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure$WeightedInputsMap.class
+-rw-r--r--  2.0 unx     1523 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$Outputs.class
+-rw-r--r--  2.0 unx     4711 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$ComputationStateStandard.class
+-rw-r--r--  2.0 unx     5426 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State.class
+-rw-r--r--  2.0 unx     1928 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States.class
+-rw-r--r--  2.0 unx     1621 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache$HeapCache.class
+-rw-r--r--  2.0 unx     1774 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache$HashCache.class
+-rw-r--r--  2.0 unx      802 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural$Computation$HasParents.class
+-rw-r--r--  2.0 unx      998 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$1.class
+-rw-r--r--  2.0 unx     5235 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$DropoutStore$ParentsDropoutStore.class
+-rw-r--r--  2.0 unx      978 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure$InputNeuronMap.class
+-rw-r--r--  2.0 unx     1583 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache$LinearCache.class
+-rw-r--r--  2.0 unx     5422 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/StatesCache.class
+-rw-r--r--  2.0 unx      981 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Structure$OutputNeuronMap.class
+-rw-r--r--  2.0 unx     3202 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$NetworkParents$WeightedInputsParents.class
+-rw-r--r--  2.0 unx     3203 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$ComputationStateComposite.class
+-rw-r--r--  2.0 unx     4866 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$ParentCounter.class
+-rw-r--r--  2.0 unx     3238 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$NetworkParents.class
+-rw-r--r--  2.0 unx     2411 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural$Computation.class
+-rw-r--r--  2.0 unx     4438 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$DropoutStore.class
+-rw-r--r--  2.0 unx      769 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/State$Neural$Computation$Detailed.class
+-rw-r--r--  2.0 unx     3839 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$SimpleValue.class
+-rw-r--r--  2.0 unx     3103 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/states/States$NetworkParents$InputsParents.class
+-rw-r--r--  2.0 unx     2552 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/AtomNeuron.class
+-rw-r--r--  2.0 unx      754 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/AtomNeurons.class
+-rw-r--r--  2.0 unx     2840 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/WeightedAtomNeuron.class
+-rw-r--r--  2.0 unx     2277 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/AggregationNeuron.class
+-rw-r--r--  2.0 unx     3168 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/NegationNeuron.class
+-rw-r--r--  2.0 unx     2384 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/SplittableAggregationNeuron.class
+-rw-r--r--  2.0 unx      789 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/AtomFact.class
+-rw-r--r--  2.0 unx     3003 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/WeightedRuleNeuron.class
+-rw-r--r--  2.0 unx      730 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/RuleNeurons.class
+-rw-r--r--  2.0 unx     3724 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/FactNeuron.class
+-rw-r--r--  2.0 unx     2487 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/neurons/types/RuleNeuron.class
+-rw-r--r--  2.0 unx    13927 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/NeuralNetwork.class
+-rw-r--r--  2.0 unx     5493 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/NeuralSets.class
+-rw-r--r--  2.0 unx      597 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/NeuralLayer.class
+-rw-r--r--  2.0 unx     1404 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/NeuralSets$NeuronCounter.class
+-rw-r--r--  2.0 unx     6209 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/types/TopologicNetwork.class
+-rw-r--r--  2.0 unx    14189 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/types/DetailedNetwork.class
+-rw-r--r--  2.0 unx     5981 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/types/TopologicNetwork$TopoSorting.class
+-rw-r--r--  2.0 unx     1037 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/components/types/LayeredNetwork.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Neural/
 -rw-r--r--  2.0 unx     1390 b- defN 22-Nov-29 16:47 META-INF/maven/io.github.gustiks/Neural/pom.xml
 -rw-r--r--  2.0 unx      109 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Neural/pom.properties
--rw-r--r--  2.0 unx    19407 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/structure/building/NeuronFactory.class
--rw-r--r--  2.0 unx    27873 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/structure/building/NeuralNetBuilder.class
--rw-r--r--  2.0 unx     2247 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/structure/building/NeuralBuilder.class
--rw-r--r--  2.0 unx     5365 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/structure/building/NeuralProcessingSample.class
--rw-r--r--  2.0 unx     4259 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/neural/networks/structure/building/NeuronMaps.class
--rw-r--r--  2.0 unx    22653 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/neural/networks/structure/building/Neuralizer.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 16:36 META-INF/maven/io.github.gustiks/Neuralization/
+-rw-r--r--  2.0 unx    19407 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuronFactory.class
+-rw-r--r--  2.0 unx    27873 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuralNetBuilder.class
+-rw-r--r--  2.0 unx     2247 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuralBuilder.class
+-rw-r--r--  2.0 unx     5365 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuralProcessingSample.class
+-rw-r--r--  2.0 unx     4259 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuronMaps.class
+-rw-r--r--  2.0 unx    22653 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/Neuralizer.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Neuralization/
 -rw-r--r--  2.0 unx     1008 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Neuralization/pom.xml
 -rw-r--r--  2.0 unx      116 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Neuralization/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/queries/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/
--rw-r--r--  2.0 unx     1504 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTree.class
--rw-r--r--  2.0 unx     1985 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/examples/ExamplesParseTreeExtractor.class
--rw-r--r--  2.0 unx     8650 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTreeExtractor.class
--rw-r--r--  2.0 unx     1494 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/queries/PlainQueriesParseTree.class
--rw-r--r--  2.0 unx     7281 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/queries/PlainQueriesParseTreeExtractor.class
--rw-r--r--  2.0 unx     1740 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/queries/QueriesParseTreeExtractor.class
--rw-r--r--  2.0 unx     2261 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor.class
--rw-r--r--  2.0 unx     3078 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor.class
--rw-r--r--  2.0 unx     5099 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor.class
--rw-r--r--  2.0 unx     4804 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor.class
--rw-r--r--  2.0 unx     3983 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor.class
--rw-r--r--  2.0 unx     2712 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainParseTree.class
--rw-r--r--  2.0 unx      541 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/grammarParsing/GrammarVisitor.class
--rw-r--r--  2.0 unx      295 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$1.class
--rw-r--r--  2.0 unx     7836 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor.class
--rw-r--r--  2.0 unx    11022 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor.class
--rw-r--r--  2.0 unx     4449 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor.class
--rw-r--r--  2.0 unx     2795 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor.class
--rw-r--r--  2.0 unx     7294 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomVisitor.class
--rw-r--r--  2.0 unx     1617 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/grammarParsing/ParseTree.class
--rw-r--r--  2.0 unx     6462 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor.class
--rw-r--r--  2.0 unx     3608 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor.class
--rw-r--r--  2.0 unx     3785 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor.class
--rw-r--r--  2.0 unx     6585 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$RuleLineVisitor.class
--rw-r--r--  2.0 unx     5042 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor.class
--rw-r--r--  2.0 unx     4569 b- defN 23-Jan-29 00:05 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomConjunctionVisitor.class
--rw-r--r--  2.0 unx    38187 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser.class
--rw-r--r--  2.0 unx     4008 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateLineContext.class
--rw-r--r--  2.0 unx     2330 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext.class
--rw-r--r--  2.0 unx     2276 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ImpliedByContext.class
--rw-r--r--  2.0 unx     3345 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$SparseVectorContext.class
--rw-r--r--  2.0 unx     3091 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LiftedExampleContext.class
--rw-r--r--  2.0 unx     2237 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext.class
--rw-r--r--  2.0 unx     2951 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataValContext.class
--rw-r--r--  2.0 unx     2688 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateMetadataContext.class
--rw-r--r--  2.0 unx     2606 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FixedValueContext.class
--rw-r--r--  2.0 unx     3548 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LrnnRuleContext.class
--rw-r--r--  2.0 unx     3435 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$SparseMatrixContext.class
--rw-r--r--  2.0 unx     3488 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$QueriesFileContext.class
--rw-r--r--  2.0 unx     2331 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConstantContext.class
--rw-r--r--  2.0 unx     2267 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NegationContext.class
--rw-r--r--  2.0 unx     2295 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FactContext.class
--rw-r--r--  2.0 unx     3154 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermListContext.class
--rw-r--r--  2.0 unx     2648 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateOffsetContext.class
--rw-r--r--  2.0 unx     2987 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext.class
--rw-r--r--  2.0 unx     3225 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataListContext.class
--rw-r--r--  2.0 unx    11229 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicVisitor.class
--rw-r--r--  2.0 unx     2655 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ElementContext.class
--rw-r--r--  2.0 unx     2913 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightContext.class
--rw-r--r--  2.0 unx     3511 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ExamplesFileContext.class
--rw-r--r--  2.0 unx     2660 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateFileContext.class
--rw-r--r--  2.0 unx     3600 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ValueContext.class
--rw-r--r--  2.0 unx     2187 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$VariableContext.class
--rw-r--r--  2.0 unx     2846 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MatrixContext.class
--rw-r--r--  2.0 unx     2488 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateContext.class
--rw-r--r--  2.0 unx     2319 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$OffsetContext.class
--rw-r--r--  2.0 unx     3152 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$VectorContext.class
--rw-r--r--  2.0 unx     3178 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$DimensionsContext.class
--rw-r--r--  2.0 unx    17205 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor.class
--rw-r--r--  2.0 unx     2564 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermContext.class
--rw-r--r--  2.0 unx     8320 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicListener.class
--rw-r--r--  2.0 unx     3066 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext.class
--rw-r--r--  2.0 unx     8056 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicLexer.class
--rw-r--r--  2.0 unx     3001 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$Element2dContext.class
--rw-r--r--  2.0 unx     2671 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightMetadataContext.class
--rw-r--r--  2.0 unx    15880 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseListener.class
--rw-r--r--  2.0 unx     2423 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateMetadataContext.class
--rw-r--r--  2.0 unx      862 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/SQLdumpExampleParser.class
--rw-r--r--  2.0 unx      259 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextTemplateParser.class
--rw-r--r--  2.0 unx     1285 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/Parser.class
--rw-r--r--  2.0 unx      164 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/TemplateParser.class
--rw-r--r--  2.0 unx      868 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextExampleParser.class
--rw-r--r--  2.0 unx      376 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/ExampleParser.class
--rw-r--r--  2.0 unx      466 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/JsonTemplateParser.class
--rw-r--r--  2.0 unx     1188 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/DefaultQueryExampleParser.class
--rw-r--r--  2.0 unx     3314 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextQueryParser.class
--rw-r--r--  2.0 unx      435 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/QueryParser.class
--rw-r--r--  2.0 unx     8550 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$PredicatesMetadataVisitor.class
--rw-r--r--  2.0 unx     5530 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$ConjunctionsVisitor.class
--rw-r--r--  2.0 unx     7466 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$WeightsMetadataVisitor.class
--rw-r--r--  2.0 unx     1504 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTree.class
--rw-r--r--  2.0 unx     5043 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor.class
--rw-r--r--  2.0 unx     5586 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$RuleLinesVisitor.class
--rw-r--r--  2.0 unx     5450 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$FactsVisitor.class
--rw-r--r--  2.0 unx     2773 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/TemplateParseTreeExtractor.class
--rw-r--r--  2.0 unx     1325 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/XmlPlainParseTree.class
--rw-r--r--  2.0 unx     3069 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/XmlTemplateParseTreeExtractor.class
--rw-r--r--  2.0 unx     6080 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$TemplateMetadataVisitor.class
--rw-r--r--  2.0 unx     9008 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/constructs/building/QueriesBuilder.class
--rw-r--r--  2.0 unx    10432 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/constructs/building/ExamplesBuilder.class
--rw-r--r--  2.0 unx     8662 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/constructs/building/TemplateBuilder.class
--rw-r--r--  2.0 unx    13362 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/constructs/building/SamplesBuilder.class
--rw-r--r--  2.0 unx     2540 b- defN 23-Jan-12 18:08 cz/cvut/fel/ida/logic/constructs/building/LogicSourceBuilder.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jan-29 16:36 META-INF/maven/io.github.gustiks/Parsing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/examples/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/queries/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/
+-rw-r--r--  2.0 unx     1504 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTree.class
+-rw-r--r--  2.0 unx     1985 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/examples/ExamplesParseTreeExtractor.class
+-rw-r--r--  2.0 unx     8650 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTreeExtractor.class
+-rw-r--r--  2.0 unx     1494 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/queries/PlainQueriesParseTree.class
+-rw-r--r--  2.0 unx     7281 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/queries/PlainQueriesParseTreeExtractor.class
+-rw-r--r--  2.0 unx     1740 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/queries/QueriesParseTreeExtractor.class
+-rw-r--r--  2.0 unx     2261 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor.class
+-rw-r--r--  2.0 unx     3078 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor.class
+-rw-r--r--  2.0 unx     5099 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor.class
+-rw-r--r--  2.0 unx     4804 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor.class
+-rw-r--r--  2.0 unx     3983 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor.class
+-rw-r--r--  2.0 unx     2712 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainParseTree.class
+-rw-r--r--  2.0 unx      541 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/GrammarVisitor.class
+-rw-r--r--  2.0 unx      295 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$1.class
+-rw-r--r--  2.0 unx     7836 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor.class
+-rw-r--r--  2.0 unx    11022 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor.class
+-rw-r--r--  2.0 unx     4449 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor.class
+-rw-r--r--  2.0 unx     2795 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor.class
+-rw-r--r--  2.0 unx     7338 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomVisitor.class
+-rw-r--r--  2.0 unx     1617 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/ParseTree.class
+-rw-r--r--  2.0 unx     6462 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor.class
+-rw-r--r--  2.0 unx     3608 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor.class
+-rw-r--r--  2.0 unx     3785 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor.class
+-rw-r--r--  2.0 unx     6585 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$RuleLineVisitor.class
+-rw-r--r--  2.0 unx     5042 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor.class
+-rw-r--r--  2.0 unx     4569 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomConjunctionVisitor.class
+-rw-r--r--  2.0 unx    38187 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser.class
+-rw-r--r--  2.0 unx     4008 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateLineContext.class
+-rw-r--r--  2.0 unx     2330 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext.class
+-rw-r--r--  2.0 unx     2276 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ImpliedByContext.class
+-rw-r--r--  2.0 unx     3345 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$SparseVectorContext.class
+-rw-r--r--  2.0 unx     3091 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LiftedExampleContext.class
+-rw-r--r--  2.0 unx     2237 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext.class
+-rw-r--r--  2.0 unx     2951 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataValContext.class
+-rw-r--r--  2.0 unx     2688 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateMetadataContext.class
+-rw-r--r--  2.0 unx     2606 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FixedValueContext.class
+-rw-r--r--  2.0 unx     3548 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LrnnRuleContext.class
+-rw-r--r--  2.0 unx     3435 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$SparseMatrixContext.class
+-rw-r--r--  2.0 unx     3488 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$QueriesFileContext.class
+-rw-r--r--  2.0 unx     2331 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConstantContext.class
+-rw-r--r--  2.0 unx     2267 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NegationContext.class
+-rw-r--r--  2.0 unx     2295 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FactContext.class
+-rw-r--r--  2.0 unx     3154 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermListContext.class
+-rw-r--r--  2.0 unx     2648 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateOffsetContext.class
+-rw-r--r--  2.0 unx     2987 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext.class
+-rw-r--r--  2.0 unx     3225 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataListContext.class
+-rw-r--r--  2.0 unx    11229 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicVisitor.class
+-rw-r--r--  2.0 unx     2655 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ElementContext.class
+-rw-r--r--  2.0 unx     2913 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightContext.class
+-rw-r--r--  2.0 unx     3511 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ExamplesFileContext.class
+-rw-r--r--  2.0 unx     2660 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateFileContext.class
+-rw-r--r--  2.0 unx     3600 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ValueContext.class
+-rw-r--r--  2.0 unx     2187 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$VariableContext.class
+-rw-r--r--  2.0 unx     2846 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MatrixContext.class
+-rw-r--r--  2.0 unx     2488 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateContext.class
+-rw-r--r--  2.0 unx     2319 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$OffsetContext.class
+-rw-r--r--  2.0 unx     3152 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$VectorContext.class
+-rw-r--r--  2.0 unx     3178 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$DimensionsContext.class
+-rw-r--r--  2.0 unx    17205 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor.class
+-rw-r--r--  2.0 unx     2564 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermContext.class
+-rw-r--r--  2.0 unx     8320 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicListener.class
+-rw-r--r--  2.0 unx     3066 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext.class
+-rw-r--r--  2.0 unx     8056 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicLexer.class
+-rw-r--r--  2.0 unx     3001 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$Element2dContext.class
+-rw-r--r--  2.0 unx     2671 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightMetadataContext.class
+-rw-r--r--  2.0 unx    15880 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseListener.class
+-rw-r--r--  2.0 unx     2423 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateMetadataContext.class
+-rw-r--r--  2.0 unx      862 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/SQLdumpExampleParser.class
+-rw-r--r--  2.0 unx      259 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextTemplateParser.class
+-rw-r--r--  2.0 unx     1285 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/Parser.class
+-rw-r--r--  2.0 unx      164 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/TemplateParser.class
+-rw-r--r--  2.0 unx      868 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextExampleParser.class
+-rw-r--r--  2.0 unx      376 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/ExampleParser.class
+-rw-r--r--  2.0 unx      466 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/JsonTemplateParser.class
+-rw-r--r--  2.0 unx     1188 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/DefaultQueryExampleParser.class
+-rw-r--r--  2.0 unx     3314 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextQueryParser.class
+-rw-r--r--  2.0 unx      435 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/QueryParser.class
+-rw-r--r--  2.0 unx     8550 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$PredicatesMetadataVisitor.class
+-rw-r--r--  2.0 unx     5530 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$ConjunctionsVisitor.class
+-rw-r--r--  2.0 unx     7466 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$WeightsMetadataVisitor.class
+-rw-r--r--  2.0 unx     1504 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTree.class
+-rw-r--r--  2.0 unx     5043 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor.class
+-rw-r--r--  2.0 unx     5586 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$RuleLinesVisitor.class
+-rw-r--r--  2.0 unx     5450 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$FactsVisitor.class
+-rw-r--r--  2.0 unx     2773 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/TemplateParseTreeExtractor.class
+-rw-r--r--  2.0 unx     1325 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/XmlPlainParseTree.class
+-rw-r--r--  2.0 unx     3069 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/XmlTemplateParseTreeExtractor.class
+-rw-r--r--  2.0 unx     6080 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$TemplateMetadataVisitor.class
+-rw-r--r--  2.0 unx     9008 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/QueriesBuilder.class
+-rw-r--r--  2.0 unx    10432 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/ExamplesBuilder.class
+-rw-r--r--  2.0 unx     8733 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/TemplateBuilder.class
+-rw-r--r--  2.0 unx    13362 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/SamplesBuilder.class
+-rw-r--r--  2.0 unx     2590 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/LogicSourceBuilder.class
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Parsing/
 -rw-r--r--  2.0 unx     1212 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Parsing/pom.xml
 -rw-r--r--  2.0 unx      110 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Parsing/pom.properties
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/v4/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/v4/runtime/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/v4/runtime/misc/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/v4/runtime/tree/
@@ -1473,8 +1476,8 @@
 -rw-r--r--  2.0 unx     1175 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/AtomTransition.class
 -rw-r--r--  2.0 unx      510 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/RuleStartState.class
 -rw-r--r--  2.0 unx     1799 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/LexerTypeAction.class
 -rw-r--r--  2.0 unx      425 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/TokensStartState.class
 -rw-r--r--  2.0 unx     1026 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/ATNSerializer$2.class
 -rw-r--r--  2.0 unx      506 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/PlusBlockStartState.class
 -rw-r--r--  2.0 unx     4467 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/ANTLRInputStream.class
-1478 files, 4423685 bytes uncompressed, 1718849 bytes compressed:  61.2%
+1481 files, 4437665 bytes uncompressed, 1724643 bytes compressed:  61.1%
```

#### zipnote «TEMP»/diffoscope_291dxby7_074075/tmp0r5fikm1_.zip

```diff
@@ -1,16 +1,13 @@
 Filename: META-INF/
 Comment: 
 
 Filename: META-INF/MANIFEST.MF
 Comment: 
 
-Filename: generated/
-Comment: 
-
 Filename: cz/
 Comment: 
 
 Filename: cz/cvut/
 Comment: 
 
 Filename: cz/cvut/fel/
@@ -33,14 +30,17 @@
 
 Filename: cz/cvut/fel/ida/neuralogic/cli/utils/Runner.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/neuralogic/cli/utils/CommandLineHandler.class
 Comment: 
 
+Filename: generated/
+Comment: 
+
 Filename: cz/cvut/fel/ida/setup/
 Comment: 
 
 Filename: cz/cvut/fel/ida/setup/Settings$ResultsType.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/setup/Settings$1.class
@@ -1563,14 +1563,17 @@
 
 Filename: cz/cvut/fel/ida/pipelines/building/PythonBuilder.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/building/TemplateSamplesBuilder.class
 Comment: 
 
+Filename: cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$8.class
+Comment: 
+
 Filename: cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$2.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$2.class
@@ -1827,23 +1830,29 @@
 
 Filename: cz/cvut/fel/ida/logic/constructs/template/components/GroundHeadRule.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/constructs/template/Template.class
 Comment: 
 
+Filename: cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate$Stratification.class
+Comment: 
+
 Filename: cz/cvut/fel/ida/logic/constructs/template/types/ParsedTemplate.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/constructs/template/types/RichLogicTemplate.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate.class
 Comment: 
 
+Filename: cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate$UnsignedLiteral.class
+Comment: 
+
 Filename: cz/cvut/fel/ida/logic/grounding/Grounder.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/grounding/bottomUp/BottomUp.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/grounding/topDown/Gringo.class
```

#### cz/cvut/fel/ida/setup/Settings.class

##### procyon -ec {}

```diff
@@ -190,14 +190,15 @@
     public String queryExampleSeparator;
     public boolean crossvalidation;
     public boolean shuffleBeforeFoldSplit;
     public int foldsCount;
     public boolean stratification;
     public boolean exportFolds;
     public boolean trainFoldsIsolation;
+    public boolean checkStratification;
     public boolean processMetadata;
     public boolean graphTemplate;
     public boolean reduceTemplate;
     public boolean inferTemplateFacts;
     public boolean supervisedTemplateGraphPruning;
     public boolean oneQueryPerExample;
     public boolean queriesAlignedWithExamples;
@@ -739,14 +740,15 @@
         this.foldsPrefix = "fold_";
         this.queryExampleSeparator = ":-";
         this.shuffleBeforeFoldSplit = true;
         this.foldsCount = 5;
         this.stratification = true;
         this.exportFolds = true;
         this.trainFoldsIsolation = false;
+        this.checkStratification = true;
         this.processMetadata = true;
         this.graphTemplate = true;
         this.reduceTemplate = false;
         this.inferTemplateFacts = true;
         this.supervisedTemplateGraphPruning = false;
         this.oneQueryPerExample = true;
         this.defaultSampleImportance = 1.0;
```

#### cz/cvut/fel/ida/setup/Sources.class

##### procyon -ec {}

```diff
@@ -1,11 +1,17 @@
 
 package cz.cvut.fel.ida.setup;
 
+import com.google.gson.JsonObject;
+import com.google.gson.JsonElement;
+import com.google.gson.JsonSerializationContext;
 import com.google.gson.Gson;
+import com.google.gson.JsonSerializer;
+import java.lang.reflect.Type;
+import java.io.File;
 import com.google.gson.GsonBuilder;
 import java.util.Iterator;
 import org.apache.commons.cli.CommandLine;
 import java.io.FileInputStream;
 import java.io.Reader;
 import java.util.List;
 import java.util.logging.Logger;
@@ -208,15 +214,20 @@
             return this.exportToJson();
         }
         Sources.LOG.warning("Only exporting of Sources to JSON is supported");
         return this.exportToJson();
     }
     
     public String exportToJson() {
-        final Gson gson = new GsonBuilder().setPrettyPrinting().serializeSpecialFloatingPointValues().create();
+        final JsonSerializer<File> serializer = (JsonSerializer<File>)((file, type, jsonSerializationContext) -> {
+            final JsonObject jsonFile = new JsonObject();
+            jsonFile.addProperty("path", file.getPath());
+            return (JsonElement)jsonFile;
+        });
+        final Gson gson = new GsonBuilder().setPrettyPrinting().registerTypeAdapter((Type)File.class, (Object)serializer).serializeSpecialFloatingPointValues().create();
         final String json = gson.toJson((Object)this);
         return json;
     }
     
     public Reader getTemplateReader() {
         return this.templateReader;
     }
```

#### cz/cvut/fel/ida/setup/Settings$Inferred.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 20e464fa897877dcbc22d8699d6780fff27c57db209236feca4de9c3c28186c5
+  SHA-256 checksum 05172c06a674c710635b083341974999f2b6f6c0bda6921f3bdd0d411b4a8a5a
   Compiled from "Settings.java"
 public class cz.cvut.fel.ida.setup.Settings$Inferred
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #6                          // cz/cvut/fel/ida/setup/Settings$Inferred
   super_class: #7                         // java/lang/Object
@@ -64,16 +64,16 @@
         10: new           #3                  // class java/util/concurrent/atomic/AtomicInteger
         13: dup
         14: iconst_0
         15: invokespecial #4                  // Method java/util/concurrent/atomic/AtomicInteger."<init>":(I)V
         18: putfield      #5                  // Field maxWeightCount:Ljava/util/concurrent/atomic/AtomicInteger;
         21: return
       LineNumberTable:
-        line 1053: 0
-        line 1060: 9
+        line 1057: 0
+        line 1064: 9
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      22     0  this   Lcz/cvut/fel/ida/setup/Settings$Inferred;
             0      22     1 this$0   Lcz/cvut/fel/ida/setup/Settings;
 }
 SourceFile: "Settings.java"
 InnerClasses:
```

#### cz/cvut/fel/ida/utils/exporting/Exportable.class

##### procyon -ec {}

```diff
@@ -1,19 +1,31 @@
 
 package cz.cvut.fel.ida.utils.exporting;
 
+import com.google.gson.JsonObject;
+import com.google.gson.JsonElement;
+import com.google.gson.JsonSerializationContext;
 import com.google.gson.Gson;
+import com.google.gson.JsonSerializer;
+import java.lang.reflect.Type;
+import java.time.Duration;
 import com.google.gson.GsonBuilder;
 import java.io.Serializable;
 
 public interface Exportable<I> extends Serializable
 {
     default void export(final Exporter exporter) {
         exporter.export(this);
     }
     
     default String exportToJson() {
-        final Gson gson = new GsonBuilder().setPrettyPrinting().serializeSpecialFloatingPointValues().create();
+        final JsonSerializer<Duration> durationJsonSerializer = (JsonSerializer<Duration>)((duration, type, jsonSerializationContext) -> {
+            final JsonObject jsonDuration = new JsonObject();
+            jsonDuration.addProperty("seconds", (Number)Long.valueOf(duration.getSeconds()));
+            jsonDuration.addProperty("nanos", (Number)Integer.valueOf(duration.getNano()));
+            return (JsonElement)jsonDuration;
+        });
+        final Gson gson = new GsonBuilder().setPrettyPrinting().registerTypeAdapter((Type)Duration.class, (Object)durationJsonSerializer).serializeSpecialFloatingPointValues().create();
         final String json = gson.toJson((Object)this);
         return json;
     }
 }
```

#### cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$6.class

##### procyon -ec {}

```diff
@@ -1,12 +1,12 @@
 
 package cz.cvut.fel.ida.pipelines.building;
 
+import cz.cvut.fel.ida.logic.constructs.template.Template;
 import cz.cvut.fel.ida.logic.constructs.template.types.ParsedTemplate;
-import cz.cvut.fel.ida.setup.Sources;
 import cz.cvut.fel.ida.pipelines.Pipe;
 
-class TemplateProcessingBuilder$6 extends Pipe<Sources, ParsedTemplate> {
-    public ParsedTemplate apply(final Sources sources) {
-        return this.this$0.templateBuilder.buildTemplateFrom(sources.getTemplateReader());
+class TemplateProcessingBuilder$6 extends Pipe<ParsedTemplate, Template> {
+    public Template apply(final ParsedTemplate template) {
+        return (Template)this.this$0.metadataProcessor.processMetadata(template);
     }
 }
```

#### cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$3.class

##### procyon -ec {}

```diff
@@ -1,12 +1,20 @@
 
 package cz.cvut.fel.ida.pipelines.building;
 
+import java.util.Objects;
+import cz.cvut.fel.ida.logic.constructs.template.types.GraphTemplate;
 import cz.cvut.fel.ida.logic.constructs.template.Template;
 import cz.cvut.fel.ida.pipelines.Pipe;
 
 class TemplateProcessingBuilder$3 extends Pipe<Template, Template> {
     public Template apply(final Template template) {
-        template.inferTemplateFacts();
+        if (template.containsNegation) {
+            final GraphTemplate obj;
+            final GraphTemplate graphTemplate = obj = new GraphTemplate(template);
+            Objects.requireNonNull(obj);
+            new GraphTemplate.Stratification(obj, graphTemplate).check();
+            return (Template)graphTemplate;
+        }
         return template;
     }
 }
```

#### cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$7.class

##### procyon -ec {}

```diff
@@ -1,13 +1,12 @@
 
 package cz.cvut.fel.ida.pipelines.building;
 
-import cz.cvut.fel.ida.logic.constructs.template.types.GraphTemplate;
-import cz.cvut.fel.ida.logic.constructs.template.Template;
+import cz.cvut.fel.ida.logic.constructs.template.types.ParsedTemplate;
+import cz.cvut.fel.ida.setup.Sources;
 import cz.cvut.fel.ida.pipelines.Pipe;
 
-class TemplateProcessingBuilder$7 extends Pipe<Template, GraphTemplate> {
-    public GraphTemplate apply(final Template template) {
-        final GraphTemplate graphTemplate = new GraphTemplate(template);
-        return graphTemplate;
+class TemplateProcessingBuilder$7 extends Pipe<Sources, ParsedTemplate> {
+    public ParsedTemplate apply(final Sources sources) {
+        return this.this$0.templateBuilder.buildTemplateFrom(sources.getTemplateReader());
     }
 }
```

#### cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$4.class

##### procyon -ec {}

```diff
@@ -1,12 +1,12 @@
 
 package cz.cvut.fel.ida.pipelines.building;
 
 import cz.cvut.fel.ida.logic.constructs.template.Template;
-import cz.cvut.fel.ida.logic.constructs.template.types.GraphTemplate;
 import cz.cvut.fel.ida.pipelines.Pipe;
 
-class TemplateProcessingBuilder$4 extends Pipe<GraphTemplate, Template> {
-    public Template apply(final GraphTemplate template) {
-        return this.this$0.templateReducer.reduce((Template)template);
+class TemplateProcessingBuilder$4 extends Pipe<Template, Template> {
+    public Template apply(final Template template) {
+        template.inferTemplateFacts();
+        return template;
     }
 }
```

#### cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder.class

##### procyon -ec {}

```diff
@@ -47,14 +47,19 @@
                 sourcesTemplatePipe.connectAfter((Pipe)nextPipe);
             }
             else {
                 nextPipe = (Pipe<ParsedTemplate, Template>)pipeline.registerEnd((Pipe)new TemplateProcessingBuilder.TemplateProcessingBuilder$2(this, "SkippingMetadataPipe"));
                 sourcesTemplatePipe.connectAfter((Pipe)nextPipe);
             }
             Pipe<?, Template> nextPipe2 = nextPipe;
+            if (this.settings.checkStratification) {
+                final Pipe<Template, Template> stratificationPipe = (Pipe<Template, Template>)pipeline.registerEnd((Pipe)this.checkStratificationPipe());
+                nextPipe2.connectAfter((Pipe)stratificationPipe);
+                nextPipe2 = stratificationPipe;
+            }
             if (this.settings.reduceTemplate) {
                 final Pipe<Template, GraphTemplate> graphTemplatePipe = (Pipe<Template, GraphTemplate>)pipeline.register((Pipe)this.buildTemplateGraph());
                 nextPipe.connectAfter((Pipe)graphTemplatePipe);
                 final Pipe<GraphTemplate, Template> reduceTemplatePipe = this.reduceTemplate();
                 graphTemplatePipe.connectAfter(pipeline.registerEnd((Pipe)reduceTemplatePipe));
                 nextPipe2 = reduceTemplatePipe;
             }
@@ -66,38 +71,42 @@
             if (this.settings.debugTemplate) {
                 new TemplateDebugger(this.settings).addDebugElement((Pipeline)pipeline);
             }
         }
         return pipeline;
     }
     
+    private Pipe<Template, Template> checkStratificationPipe() {
+        return (Pipe<Template, Template>)new TemplateProcessingBuilder.TemplateProcessingBuilder$3(this, "CheckStratificationPipe");
+    }
+    
     protected Pipe<Template, Template> inferFacts() {
-        return (Pipe<Template, Template>)new TemplateProcessingBuilder.TemplateProcessingBuilder$3(this, "TemplateInferencePipe");
+        return (Pipe<Template, Template>)new TemplateProcessingBuilder.TemplateProcessingBuilder$4(this, "TemplateInferencePipe");
     }
     
     protected Pipe<GraphTemplate, Template> reduceTemplate() {
         this.templateReducer = TemplateReducing.getReducer(this.settings);
-        return (Pipe<GraphTemplate, Template>)new TemplateProcessingBuilder.TemplateProcessingBuilder$4(this, "TemplateReducingPipe");
+        return (Pipe<GraphTemplate, Template>)new TemplateProcessingBuilder.TemplateProcessingBuilder$5(this, "TemplateReducingPipe");
     }
     
     protected Pipe<ParsedTemplate, Template> processMetadata() {
         this.metadataProcessor = new MetadataProcessor(this.settings);
-        return (Pipe<ParsedTemplate, Template>)new TemplateProcessingBuilder.TemplateProcessingBuilder$5(this, "MetadataProcessingPipe");
+        return (Pipe<ParsedTemplate, Template>)new TemplateProcessingBuilder.TemplateProcessingBuilder$6(this, "MetadataProcessingPipe");
     }
     
     public Pipe<Sources, ParsedTemplate> extractTemplate(final Sources sources) {
         if (!sources.templateProvided) {
             TemplateProcessingBuilder.LOG.severe("No template provided yet required.");
             return null;
         }
-        final Pipe<Sources, ParsedTemplate> pipe = (Pipe<Sources, ParsedTemplate>)new TemplateProcessingBuilder.TemplateProcessingBuilder$6(this, "TemplateExtractionPipe");
+        final Pipe<Sources, ParsedTemplate> pipe = (Pipe<Sources, ParsedTemplate>)new TemplateProcessingBuilder.TemplateProcessingBuilder$7(this, "TemplateExtractionPipe");
         return pipe;
     }
     
     protected Pipe<Template, GraphTemplate> buildTemplateGraph() {
-        return (Pipe<Template, GraphTemplate>)new TemplateProcessingBuilder.TemplateProcessingBuilder$7(this, "BuildTemplateGraphPipe");
+        return (Pipe<Template, GraphTemplate>)new TemplateProcessingBuilder.TemplateProcessingBuilder$8(this, "BuildTemplateGraphPipe");
     }
     
     static {
         LOG = Logger.getLogger(TemplateProcessingBuilder.class.getName());
     }
 }
```

#### cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$5.class

##### procyon -ec {}

```diff
@@ -1,12 +1,12 @@
 
 package cz.cvut.fel.ida.pipelines.building;
 
 import cz.cvut.fel.ida.logic.constructs.template.Template;
-import cz.cvut.fel.ida.logic.constructs.template.types.ParsedTemplate;
+import cz.cvut.fel.ida.logic.constructs.template.types.GraphTemplate;
 import cz.cvut.fel.ida.pipelines.Pipe;
 
-class TemplateProcessingBuilder$5 extends Pipe<ParsedTemplate, Template> {
-    public Template apply(final ParsedTemplate template) {
-        return (Template)this.this$0.metadataProcessor.processMetadata(template);
+class TemplateProcessingBuilder$5 extends Pipe<GraphTemplate, Template> {
+    public Template apply(final GraphTemplate template) {
+        return this.this$0.templateReducer.reduce((Template)template);
     }
 }
```

#### cz/cvut/fel/ida/pipelines/debugging/drawing/TemplateDrawer.class

##### procyon -ec {}

```diff
@@ -98,15 +98,19 @@
     }
     
     private String draw(final BodyAtom bodyAtom, final ValuedFact matchedFact) {
         return matchedFact.literal.liftedHashCode() + " -> " + bodyAtom.literal.liftedHashCode() + "[dir=both, style=dotted, color=blue]";
     }
     
     private String draw(final Literal literal) {
-        return literal.liftedHashCode() + "[label=" + GraphViz.sanitize(literal.toString()) + "]";
+        String name = literal.toString();
+        if (literal.isNegated()) {
+            name = name.substring(1);
+        }
+        return literal.liftedHashCode() + "[label=" + GraphViz.sanitize(name) + "]";
     }
     
     private String draw(final WeightedRule rule) {
         return rule.hashCode() + "[label=" + GraphViz.sanitize(rule.getOriginalString()) + ", shape=larrow, color=green]";
     }
     
     private String draw(final ValuedFact fact) {
```

#### cz/cvut/fel/ida/logic/constructs/template/Template.class

##### procyon -ec {}

```diff
@@ -36,29 +36,33 @@
     static int counter;
     protected String name;
     public LinkedHashSet<WeightedRule> rules;
     public LinkedHashSet<ValuedFact> facts;
     public LinkedHashSet<Conjunction> constraints;
     @Nullable
     public transient Set<Literal> inferredLiterals;
+    public boolean containsNegation;
     @Nullable
     public transient Map<HornClause, List<WeightedRule>> hornClauses;
     
     public Template() {
+        this.containsNegation = false;
         this.name = "template" + Template.counter++;
         this.rules = new LinkedHashSet<WeightedRule>();
         this.facts = new LinkedHashSet<ValuedFact>();
         this.constraints = new LinkedHashSet<Conjunction>();
     }
     
     public Template(final Template other) {
+        this.containsNegation = false;
         this.name = "template" + Template.counter++;
         this.rules = other.rules;
         this.facts = other.facts;
         this.constraints = other.constraints;
+        this.containsNegation = other.containsNegation;
     }
     
     public Template(final List<WeightedRule> rules, final List<ValuedFact> facts) {
         this();
         this.rules.addAll((Collection<?>)rules);
         this.facts.addAll((Collection<?>)facts);
     }
```

#### cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate.class

##### procyon -ec {}

```diff
@@ -26,21 +26,33 @@
 
 public class GraphTemplate extends Template
 {
     private static final Logger LOG;
     public transient Map<Literal, Set<WeightedRule>> atom2rules;
     transient Set<Literal> closedAtoms;
     transient Set<Literal> openAtoms;
+    public boolean isStratified;
     
     public GraphTemplate() {
+        this.isStratified = true;
         this.atom2rules = new LinkedHashMap<Literal, Set<WeightedRule>>();
     }
     
+    public GraphTemplate(final GraphTemplate template) {
+        super((Template)template);
+        this.isStratified = true;
+        this.atom2rules = template.atom2rules;
+        this.closedAtoms = template.closedAtoms;
+        this.openAtoms = template.openAtoms;
+        this.isStratified = template.isStratified;
+    }
+    
     public GraphTemplate(final Template template) {
         super(template);
+        this.isStratified = true;
         final Map<Predicate, List<WeightedRule>> predicate2heads = new LinkedHashMap<Predicate, List<WeightedRule>>();
         this.atom2rules = new LinkedHashMap<Literal, Set<WeightedRule>>();
         this.closedAtoms = (Set)template.facts.stream().map(f -> f.literal).collect(Collectors.toSet());
         if (template.inferredLiterals != null) {
             this.closedAtoms.addAll(template.inferredLiterals);
         }
         this.openAtoms = new HashSet<Literal>();
@@ -51,40 +63,38 @@
             list.add(rule);
             final Set<WeightedRule> list2 = (Set<WeightedRule>)this.atom2rules.computeIfAbsent(rule.getHead().literal, k -> new HashSet());
             list2.add(rule);
         }
         for (final Map.Entry<Predicate, List<WeightedRule>> entry : predicate2heads.entrySet()) {
             for (final WeightedRule anyRule : (List)entry.getValue()) {
                 for (final BodyAtom bodyAtom : anyRule.getBody()) {
-                    final List<WeightedRule> possibleRules = (List<WeightedRule>)predicate2heads.get(bodyAtom.literal.predicate());
+                    Literal bodyLiteral = bodyAtom.literal;
+                    if (bodyLiteral.isNegated()) {
+                        this.containsNegation = true;
+                        bodyLiteral = new Literal(bodyLiteral.predicate(), false, bodyLiteral.termList());
+                    }
+                    final List<WeightedRule> possibleRules = (List<WeightedRule>)predicate2heads.get(bodyLiteral.predicate());
                     boolean hasChildren = false;
                     if (possibleRules != null) {
                         for (final WeightedRule possibleRule : possibleRules) {
-                            if (matching.subsumption(new Clause(new Literal[] { possibleRule.getHead().literal }), new Clause(new Literal[] { bodyAtom.literal })) || matching.subsumption(new Clause(new Literal[] { bodyAtom.literal }), new Clause(new Literal[] { possibleRule.getHead().literal }))) {
+                            if (matching.subsumption(new Clause(new Literal[] { possibleRule.getHead().literal }), new Clause(new Literal[] { bodyLiteral })) || matching.subsumption(new Clause(new Literal[] { bodyLiteral }), new Clause(new Literal[] { possibleRule.getHead().literal }))) {
                                 hasChildren = true;
-                                final Set<WeightedRule> rules4atom = (Set<WeightedRule>)this.atom2rules.computeIfAbsent(bodyAtom.literal, k -> new HashSet());
+                                final Set<WeightedRule> rules4atom = (Set<WeightedRule>)this.atom2rules.computeIfAbsent(bodyLiteral, k -> new HashSet());
                                 rules4atom.add(possibleRule);
                             }
                         }
                     }
-                    if (!hasChildren && !this.closedAtoms.contains(bodyAtom.literal)) {
-                        this.openAtoms.add(bodyAtom.literal);
+                    if (!hasChildren && !this.closedAtoms.contains(bodyLiteral)) {
+                        this.openAtoms.add(bodyLiteral);
                     }
                 }
             }
         }
     }
     
-    public GraphTemplate(final GraphTemplate template) {
-        super((Template)template);
-        this.atom2rules = template.atom2rules;
-        this.closedAtoms = template.closedAtoms;
-        this.openAtoms = template.openAtoms;
-    }
-    
     public GraphTemplate prune(final QueryAtom queryAtom) {
         final GraphTemplate pruned = new GraphTemplate(this);
         pruned.rules = new LinkedHashSet();
         this.recursePrune(queryAtom.headAtom.literal, pruned.rules);
         return pruned;
     }
```

#### cz/cvut/fel/ida/algebra/values/distributions/Distribution.class

##### procyon -ec {}

```diff
@@ -6,15 +6,15 @@
 import java.util.logging.Logger;
 import cz.cvut.fel.ida.utils.exporting.Exportable;
 
 public abstract class Distribution implements Exportable
 {
     private static final Logger LOG;
     transient Settings setting;
-    Random rg;
+    transient Random rg;
     double scale;
     
     public Distribution(final Random rg, final Settings settings) {
         this.rg = rg;
         this.scale = settings.randomInitScale;
         this.setting = settings;
     }
```

#### META-INF/maven/io.github.gustiks/Algebra/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Sat Oct 01 18:09:47 CEST 2022
+#Fri Apr 07 21:21:59 CEST 2023
 groupId=io.github.gustiks
 artifactId=Algebra
 version=0.3.0
```

#### cz/cvut/fel/ida/logic/subsumption/HerbrandModel$HerbrandMap.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 6915795734569f312a8846d1512ec2db945baa298ad826a9ae0043a18ef306e2
+  SHA-256 checksum fbfdeb834fb118d5ceb320b8ddd4fe5af5126eec298a153bfaa361db411e684b
   Compiled from "HerbrandModel.java"
 public class cz.cvut.fel.ida.logic.subsumption.HerbrandModel$HerbrandMap extends cz.cvut.fel.ida.utils.math.collections.MultiMap<cz.cvut.fel.ida.logic.Predicate, cz.cvut.fel.ida.logic.Literal>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #3                          // cz/cvut/fel/ida/logic/subsumption/HerbrandModel$HerbrandMap
   super_class: #4                         // cz/cvut/fel/ida/utils/math/collections/MultiMap
@@ -41,29 +41,29 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method cz/cvut/fel/ida/utils/math/collections/MultiMap."<init>":()V
          4: return
       LineNumberTable:
-        line 235: 0
+        line 252: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcz/cvut/fel/ida/logic/subsumption/HerbrandModel$HerbrandMap;
 
   public java.util.Collection<java.util.Set<cz.cvut.fel.ida.logic.Literal>> getLiterals();
     descriptor: ()Ljava/util/Collection;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #2                  // Method cz/cvut/fel/ida/utils/math/collections/MultiMap.values:()Ljava/util/Collection;
          4: areturn
       LineNumberTable:
-        line 237: 0
+        line 254: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcz/cvut/fel/ida/logic/subsumption/HerbrandModel$HerbrandMap;
     Signature: #17                          // ()Ljava/util/Collection<Ljava/util/Set<Lcz/cvut/fel/ida/logic/Literal;>;>;
 }
 Signature: #18                          // Lcz/cvut/fel/ida/utils/math/collections/MultiMap<Lcz/cvut/fel/ida/logic/Predicate;Lcz/cvut/fel/ida/logic/Literal;>;
 SourceFile: "HerbrandModel.java"
```

#### cz/cvut/fel/ida/logic/subsumption/HerbrandModel$TupleNotIn.class

##### procyon -ec {}

```diff
@@ -10,15 +10,15 @@
 {
     private Set<Literal> literals;
     private String name;
     private String predicate;
     
     TupleNotIn(final Predicate predicate, final Set<Literal> literals) {
         this.predicate = predicate.name;
-        this.name = HerbrandModel.access$100(predicate);
+        this.name = HerbrandModel.tupleNotInPredicateName(predicate);
         this.literals = literals;
     }
     
     public String name() {
         return this.name;
     }
```

#### cz/cvut/fel/ida/logic/subsumption/HerbrandModel$PredicateSolutionConsumer.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 829220bf60110e07d4bdf75e4d8b5b08ea5ee4e9e433433b901ff1ffe9f3bb0f
+  SHA-256 checksum f2547ab7e4dff499b2a9c5d392ed48a533a1707add3adb29b0c9f46cf0c92c64
   Compiled from "HerbrandModel.java"
 class cz.cvut.fel.ida.logic.subsumption.HerbrandModel$PredicateSolutionConsumer implements cz.cvut.fel.ida.logic.subsumption.SolutionConsumer
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #8                          // cz/cvut/fel/ida/logic/subsumption/HerbrandModel$PredicateSolutionConsumer
   super_class: #9                         // java/lang/Object
@@ -99,18 +99,18 @@
          5: aload_1
          6: putfield      #3                  // Field ruleHead:Lcz/cvut/fel/ida/logic/Literal;
          9: aload_0
         10: aload_2
         11: putfield      #4                  // Field headGroundings:Ljava/util/Set;
         14: return
       LineNumberTable:
-        line 187: 0
-        line 188: 4
-        line 189: 9
-        line 190: 14
+        line 194: 0
+        line 195: 4
+        line 196: 9
+        line 197: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lcz/cvut/fel/ida/logic/subsumption/HerbrandModel$PredicateSolutionConsumer;
             0      15     1  head   Lcz/cvut/fel/ida/logic/Literal;
             0      15     2 groundHeads   Ljava/util/Set;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -141,19 +141,19 @@
         28: getfield      #3                  // Field ruleHead:Lcz/cvut/fel/ida/logic/Literal;
         31: aload_2
         32: invokevirtual #6                  // Method cz/cvut/fel/ida/logic/Literal.subsCopy:([Lcz/cvut/fel/ida/logic/Term;)Lcz/cvut/fel/ida/logic/Literal;
         35: invokeinterface #7,  2            // InterfaceMethod java/util/Set.add:(Ljava/lang/Object;)Z
         40: pop
         41: return
       LineNumberTable:
-        line 194: 0
-        line 195: 8
-        line 194: 17
-        line 197: 23
-        line 198: 41
+        line 201: 0
+        line 202: 8
+        line 201: 17
+        line 204: 23
+        line 205: 41
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             2      21     3     i   I
             0      42     0  this   Lcz/cvut/fel/ida/logic/subsumption/HerbrandModel$PredicateSolutionConsumer;
             0      42     1 template   [Lcz/cvut/fel/ida/logic/Term;
             0      42     2 solution   [Lcz/cvut/fel/ida/logic/Term;
       StackMapTable: number_of_entries = 2
@@ -170,15 +170,15 @@
       stack=3, locals=4, args_size=4
          0: aload_0
          1: aload_1
          2: aload_2
          3: invokespecial #1                  // Method "<init>":(Lcz/cvut/fel/ida/logic/Literal;Ljava/util/Set;)V
          6: return
       LineNumberTable:
-        line 182: 0
+        line 189: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcz/cvut/fel/ida/logic/subsumption/HerbrandModel$PredicateSolutionConsumer;
             0       7     1    x0   Lcz/cvut/fel/ida/logic/Literal;
             0       7     2    x1   Ljava/util/Set;
             0       7     3    x2   Lcz/cvut/fel/ida/logic/subsumption/HerbrandModel$1;
 }
```

#### cz/cvut/fel/ida/logic/subsumption/HerbrandModel.class

##### procyon -ec {}

```diff
@@ -68,23 +68,21 @@
             final Iterator<? extends HornClause> iterator = rules.iterator();
             while (iterator.hasNext()) {
                 final HornClause rule2 = (HornClause)iterator.next();
                 final Literal head = rule2.head();
                 final SolutionConsumer solutionConsumer = (SolutionConsumer)new HerbrandModel.PredicateSolutionConsumer(head, this.herbrand.get((Object)head.predicate()), (HerbrandModel.HerbrandModel$1)null);
                 this.matching.getEngine().addSolutionConsumer(solutionConsumer);
                 if (LogicUtils.isGround(head)) {
-                    final Clause query = new Clause((Iterable)rule2.body().literals());
-                    if ((boolean)this.matching.subsumption(query, 0)) {
+                    if ((boolean)this.matching.subsumption(this.prepareClauseForGrounder(rule2, true), 0)) {
                         this.herbrand.put((Object)head.predicate(), (Object)head);
                         iterator.remove();
                     }
                 }
                 else {
-                    final Clause query = new Clause((Iterable)Sugar.union((Collection)rule2.getNegatedLiterals(), (Object[])new Literal[] { new Literal(tupleNotInPredicateName(head.predicate()), false, head.arguments()) }));
-                    this.matching.allSubstitutions(query, 0, Integer.MAX_VALUE);
+                    this.matching.allSubstitutions(this.prepareClauseForGrounder(rule2, false), 0, Integer.MAX_VALUE);
                 }
                 this.matching.getEngine().removeSolutionConsumer(solutionConsumer);
             }
             HerbrandModel.LOG.finest(() -> irules.size() + " rules grounded.");
             final int herbrandSize2 = VectorUtils.sum(this.herbrand.sizes());
             HerbrandModel.LOG.finer("herbrand size after round " + round++ + " = " + herbrandSize2);
             changed = (herbrandSize2 > herbrandSize0);
@@ -123,19 +121,33 @@
                 }
                 rest.add(hc);
             }
         }
         return (Pair<List<HornClause>, List<Literal>>)new Pair((Object)rest, (Object)groundFacts);
     }
     
-    private static String tupleNotInPredicateName(final Predicate predicate) {
-        return "@tuplenotin-" + predicate.name + "/" + predicate.arity;
+    public Clause prepareClauseForGrounder(final HornClause hc, final boolean groundHead) {
+        final Set<Literal> literalSet = new HashSet<Literal>(hc.body().literals());
+        for (final Literal l : hc.body().literals()) {
+            if (l.isNegated()) {
+                literalSet.add(new Literal(tupleNotInPredicateName(l.predicate()), false, l.arguments()));
+            }
+        }
+        if (!groundHead) {
+            literalSet.add(hc.head().negation());
+            literalSet.add(new Literal(tupleNotInPredicateName(hc.head().predicate()), false, hc.head().arguments()));
+        }
+        return new Clause((Iterable)literalSet);
     }
     
     public void clear() {
         this.herbrand.clear();
     }
     
+    public static String tupleNotInPredicateName(final Predicate predicate) {
+        return "@tuplenotin-" + predicate.name + "/" + predicate.arity;
+    }
+    
     static {
         LOG = Logger.getLogger(HerbrandModel.class.getName());
     }
 }
```

#### cz/cvut/fel/ida/logic/Literal.class

##### procyon -ec {}

```diff
@@ -268,15 +268,14 @@
                 varcode = 7L;
             }
             else {
                 varcode = this.terms[i].hashCode();
             }
             hash *= varcode;
         }
-        hash *= (this.negated ? -1 : 1);
         return hash;
     }
     
     public int id() {
         return this.id;
     }
```

#### cz/cvut/fel/ida/logic/HornClause.class

##### procyon -ec {}

```diff
@@ -109,20 +109,14 @@
     
     public Set<Literal> getLiterals() {
         final Set<Literal> literalSet = new HashSet<Literal>(this.body.literals());
         literalSet.add(this.head);
         return literalSet;
     }
     
-    public Set<Literal> getNegatedLiterals() {
-        final Set<Literal> literalSet = new HashSet<Literal>(this.body.literals());
-        literalSet.add(this.head.negation());
-        return literalSet;
-    }
-    
     public Clause toClause() {
         return new Clause((Iterable)Sugar.union((Collection)LogicUtils.flipSigns((Collection)this.body().literals()), (Collection)((this.head() == null) ? Sugar.list() : Sugar.list((Object[])new Literal[] { this.head }))));
     }
     
     @Override
     public String toString() {
         if (this.head == null) {
```

#### cz/cvut/fel/ida/neural/networks/structure/components/neurons/BaseNeuron.class

##### procyon -ec {}

```diff
@@ -38,15 +38,19 @@
     
     public void addInput(final T input) {
         this.inputs.add(input);
     }
     
     @NotNull
     public final ArrayList<T> getInputs() {
-        return this.inputs;
+        final ArrayList<T> inputs = this.inputs;
+        if (inputs == null) {
+            $$$reportNull$$$0(0);
+        }
+        return inputs;
     }
     
     public void invalidate() {
         this.state.invalidate();
     }
     
     public Combination getCombination() {
@@ -117,15 +121,19 @@
         }
         final BaseNeuron obj2 = (BaseNeuron)obj;
         return this.index == obj2.index;
     }
     
     @NotNull
     public String getName() {
-        return this.name;
+        final String name = this.name;
+        if (name == null) {
+            $$$reportNull$$$0(1);
+        }
+        return name;
     }
     
     public final State.Neural.Computation getComputationView(final int index) {
         return this.state.getComputationView(index);
     }
     
     public final S getRawState() {
@@ -140,8 +148,24 @@
     public String toString() {
         return this.getClass().getSimpleName() + " = " + this.name;
     }
     
     static {
         LOG = Logger.getLogger(BaseNeuron.class.getName());
     }
+    
+    private static /* synthetic */ void $$$reportNull$$$0(final int n) {
+        final String format = "@NotNull method %s.%s must not return null";
+        final Object[] args = { "cz/cvut/fel/ida/neural/networks/structure/components/neurons/BaseNeuron", null };
+        switch (n) {
+            default: {
+                args[1] = "getInputs";
+                break;
+            }
+            case 1: {
+                args[1] = "getName";
+                break;
+            }
+        }
+        throw new IllegalStateException(String.format(format, args));
+    }
 }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum c0e6b605c77eac79265b9946c05751bb986d4f490401acee9e2534acf1077187
+  SHA-256 checksum bac9cfafad510b6370968ae0c9493606aa79822e9ac7be2f9dc015bf450242b0
   Compiled from "PlainGrammarVisitor.java"
 public class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$LabelVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.logic.constructs.Conjunction>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #9                          // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor
   super_class: #10                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -87,15 +87,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #2                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 173: 0
+        line 174: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor;
             0      10     1 this$0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
 
   public cz.cvut.fel.ida.logic.constructs.Conjunction visitLabel(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$LabelContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext;)Lcz/cvut/fel/ida/logic/constructs/Conjunction;
@@ -113,17 +113,17 @@
         16: aload_2
         17: invokevirtual #6                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext.accept:(Lorg/antlr/v4/runtime/tree/ParseTreeVisitor;)Ljava/lang/Object;
         20: checkcast     #7                  // class cz/cvut/fel/ida/logic/constructs/Conjunction
         23: astore_3
         24: aload_3
         25: areturn
       LineNumberTable:
-        line 178: 0
-        line 179: 12
-        line 180: 24
+        line 179: 0
+        line 180: 12
+        line 181: 24
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      26     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor;
             0      26     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext;
            12      14     2 factConjunctionVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor;
            24       2     3 label   Lcz/cvut/fel/ida/logic/constructs/Conjunction;
 
@@ -133,15 +133,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #8                  // Method visitLabel:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext;)Lcz/cvut/fel/ida/logic/constructs/Conjunction;
          5: areturn
       LineNumberTable:
-        line 173: 0
+        line 174: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor;
 }
 Signature: #37                          // Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor<Lcz/cvut/fel/ida/logic/constructs/Conjunction;>;
 SourceFile: "PlainGrammarVisitor.java"
 InnerClasses:
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 986147e91c49852cc284185f068a0f37b34077dfa388653143892e0192485a16
+  SHA-256 checksum 1bfe3601220bdeed26cf76b098bc567084d2e5252ff16524d6a5c469b5c3fdf1
   Compiled from "PlainGrammarVisitor.java"
 public class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$TemplateMetadataVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<java.util.Map<java.lang.String, java.lang.Object>>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #9                          // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor
   super_class: #10                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -111,15 +111,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #2                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 446: 0
+        line 447: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor;
             0      10     1 this$0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
 
   public java.util.Map<java.lang.String, java.lang.Object> visitTemplateMetadata(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$TemplateMetadataContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateMetadataContext;)Ljava/util/Map;
@@ -142,16 +142,16 @@
         27: checkcast     #7                  // class java/util/Map
         30: astore_2
         31: aload_2
         32: areturn
       StackMapTable: number_of_entries = 1
         frame_type = 8 /* same */
       LineNumberTable:
-        line 449: 8
-        line 450: 31
+        line 450: 8
+        line 451: 31
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      33     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor;
             0      33     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateMetadataContext;
            31       2     2 metadata   Ljava/util/Map;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -171,15 +171,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #8                  // Method visitTemplateMetadata:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateMetadataContext;)Ljava/util/Map;
          5: areturn
       LineNumberTable:
-        line 446: 0
+        line 447: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #35(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f799b232caf20829670bab30e943388e947895ea6e5c672a41f72c7b51e6344b
+  SHA-256 checksum b8cd4942eca28e349d1c751599bef7e3e72871da51437f0de468388a7e6fa20c
   Compiled from "PlainGrammarVisitor.java"
 public class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$PredicateMetadataVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.utils.generic.Pair<cz.cvut.fel.ida.logic.constructs.WeightedPredicate, java.util.Map<java.lang.String, java.lang.Object>>>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #31                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor
   super_class: #32                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -199,15 +199,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #2                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 377: 0
+        line 378: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor;
             0      10     1 this$0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
 
   public cz.cvut.fel.ida.utils.generic.Pair<cz.cvut.fel.ida.logic.constructs.WeightedPredicate, java.util.Map<java.lang.String, java.lang.Object>> visitPredicateMetadata(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$PredicateMetadataContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateMetadataContext;)Lcz/cvut/fel/ida/utils/generic/Pair;
@@ -306,22 +306,22 @@
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateMetadataContext, int ]
           stack = [ class cz/cvut/fel/ida/logic/constructs/building/factories/WeightedPredicateFactory, class java/lang/String, int, class java/lang/Boolean ]
         frame_type = 255 /* full_frame */
           offset_delta = 0
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateMetadataContext, int ]
           stack = [ class cz/cvut/fel/ida/logic/constructs/building/factories/WeightedPredicateFactory, class java/lang/String, int, class java/lang/Boolean, int ]
       LineNumberTable:
-        line 380: 8
-        line 382: 10
-        line 385: 26
-        line 383: 29
-        line 384: 30
-        line 386: 58
-        line 387: 121
-        line 388: 145
+        line 381: 8
+        line 383: 10
+        line 386: 26
+        line 384: 29
+        line 385: 30
+        line 387: 58
+        line 388: 121
+        line 389: 145
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            30      28     3    ex   Ljava/lang/Exception;
             0     156     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor;
             0     156     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateMetadataContext;
            10     146     2 arity   I
           121      35     3 predicate   Lcz/cvut/fel/ida/logic/constructs/WeightedPredicate;
@@ -344,15 +344,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #30                 // Method visitPredicateMetadata:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateMetadataContext;)Lcz/cvut/fel/ida/utils/generic/Pair;
          5: areturn
       LineNumberTable:
-        line 377: 0
+        line 378: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #67(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum dceb39b8fa9316f1d9f7bb465c8907924b751a9045beb0c294760500df7eb668
+  SHA-256 checksum e6e0387bb91534dbd87ca6d82d034cbf11d96b8b7afac1209a7ce9846d073eb6
   Compiled from "PlainGrammarVisitor.java"
 class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$MetadataListVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<java.util.Map<java.lang.String, java.lang.Object>>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #26                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor
   super_class: #27                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -190,15 +190,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #2                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #3                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 422: 0
+        line 423: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor;
 
   public java.util.Map<java.lang.String, java.lang.Object> visitMetadataList(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$MetadataListContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataListContext;)Ljava/util/Map;
     flags: (0x0001) ACC_PUBLIC
@@ -292,28 +292,28 @@
           offset_delta = 10
           locals = [ class java/lang/Object ]
         frame_type = 255 /* full_frame */
           offset_delta = 13
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataListContext, class java/util/LinkedHashMap, class java/util/Iterator ]
           stack = []
       LineNumberTable:
-        line 425: 8
-        line 426: 16
-        line 427: 46
-        line 428: 59
-        line 429: 62
-        line 430: 71
-        line 433: 84
-        line 434: 92
-        line 435: 112
-        line 436: 120
-        line 438: 148
-        line 440: 159
-        line 441: 170
-        line 442: 173
+        line 426: 8
+        line 427: 16
+        line 428: 46
+        line 429: 59
+        line 430: 62
+        line 431: 71
+        line 434: 84
+        line 435: 92
+        line 436: 112
+        line 437: 120
+        line 439: 148
+        line 441: 159
+        line 442: 170
+        line 443: 173
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           109       3     7 value   Ljava/lang/Object;
           145       3     7 value   Ljava/lang/Object;
            59     111     5 parameter   Ljava/lang/String;
            62     108     6 valueText   Ljava/lang/String;
           159      11     7 value   Ljava/lang/Object;
@@ -339,15 +339,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #25                 // Method visitMetadataList:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataListContext;)Ljava/util/Map;
          5: areturn
       LineNumberTable:
-        line 422: 0
+        line 423: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #65(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
@@ -361,15 +361,15 @@
     Code:
       stack=2, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: invokespecial #1                  // Method "<init>":(Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;)V
          5: return
       LineNumberTable:
-        line 422: 0
+        line 423: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor;
             0       6     1    x0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
             0       6     2    x1   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$1;
 
   private static void $$$reportNull$$$0(int);
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 761100a3947cb5eb8f08b2382c981b8188be3e8267c43840e33e30da97b0a4a8
+  SHA-256 checksum 244a11a2712c476b7031a4f0ff92de904f9b07551348f78bfe17ec7f620590a6
   Compiled from "PlainGrammarVisitor.java"
 public class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$WeightMetadataVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.utils.generic.Pair<cz.cvut.fel.ida.algebra.weights.Weight, java.util.Map<java.lang.String, java.lang.Object>>>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #16                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor
   super_class: #17                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -144,15 +144,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #2                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 392: 0
+        line 393: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor;
             0      10     1 this$0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
 
   public cz.cvut.fel.ida.utils.generic.Pair<cz.cvut.fel.ida.algebra.weights.Weight, java.util.Map<java.lang.String, java.lang.Object>> visitWeightMetadata(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$WeightMetadataContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightMetadataContext;)Lcz/cvut/fel/ida/utils/generic/Pair;
@@ -188,17 +188,17 @@
         58: aload_2
         59: aload_3
         60: invokespecial #14                 // Method cz/cvut/fel/ida/utils/generic/Pair."<init>":(Ljava/lang/Object;Ljava/lang/Object;)V
         63: areturn
       StackMapTable: number_of_entries = 1
         frame_type = 8 /* same */
       LineNumberTable:
-        line 395: 8
-        line 396: 31
-        line 397: 54
+        line 396: 8
+        line 397: 31
+        line 398: 54
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      64     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor;
             0      64     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightMetadataContext;
            31      33     2 weight   Lcz/cvut/fel/ida/algebra/weights/Weight;
            54      10     3 metadata   Ljava/util/Map;
       LocalVariableTypeTable:
@@ -219,15 +219,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #15                 // Method visitWeightMetadata:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightMetadataContext;)Lcz/cvut/fel/ida/utils/generic/Pair;
          5: areturn
       LineNumberTable:
-        line 392: 0
+        line 393: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #44(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f5b52dea74b1f9b4782c024c24e9b22b2f6930edb8a3ab37b9ce833405781151
+  SHA-256 checksum 04b5aed2a376006fe05032045b653f4438e9de172fdb98165bd5f0c868ac13a3
   Compiled from "PlainGrammarVisitor.java"
 public class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$FactVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.logic.constructs.example.ValuedFact>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #47                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor
   super_class: #48                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -294,17 +294,17 @@
          9: aload_0
         10: new           #3                  // class cz/cvut/fel/ida/logic/constructs/building/factories/VariableFactory
         13: dup
         14: invokespecial #4                  // Method cz/cvut/fel/ida/logic/constructs/building/factories/VariableFactory."<init>":()V
         17: putfield      #5                  // Field variableFactory:Lcz/cvut/fel/ida/logic/constructs/building/factories/VariableFactory;
         20: return
       LineNumberTable:
-        line 202: 0
-        line 203: 9
-        line 204: 20
+        line 203: 0
+        line 204: 9
+        line 205: 20
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      21     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor;
             0      21     1 this$0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
 
   public cz.cvut.fel.ida.logic.constructs.example.ValuedFact visitFact(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$FactContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FactContext;)Lcz/cvut/fel/ida/logic/constructs/example/ValuedFact;
@@ -319,15 +319,15 @@
          9: aload_1
         10: invokevirtual #6                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FactContext.atom:()Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext;
         13: invokevirtual #7                  // Method visitAtom:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext;)Lcz/cvut/fel/ida/logic/constructs/example/ValuedFact;
         16: areturn
       StackMapTable: number_of_entries = 1
         frame_type = 8 /* same */
       LineNumberTable:
-        line 208: 8
+        line 209: 8
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      17     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor;
             0      17     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FactContext;
     RuntimeInvisibleTypeAnnotations:
       0: #69(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
@@ -451,31 +451,31 @@
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext, class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor, class java/util/List, class cz/cvut/fel/ida/logic/constructs/WeightedPredicate, class cz/cvut/fel/ida/algebra/weights/Weight ]
           stack = [ uninitialized 178, uninitialized 178, class cz/cvut/fel/ida/logic/constructs/WeightedPredicate, class java/util/List ]
         frame_type = 255 /* full_frame */
           offset_delta = 0
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext, class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor, class java/util/List, class cz/cvut/fel/ida/logic/constructs/WeightedPredicate, class cz/cvut/fel/ida/algebra/weights/Weight ]
           stack = [ uninitialized 178, uninitialized 178, class cz/cvut/fel/ida/logic/constructs/WeightedPredicate, class java/util/List, int ]
       LineNumberTable:
-        line 213: 8
-        line 214: 21
-        line 216: 29
-        line 217: 36
-        line 218: 43
-        line 219: 54
-        line 220: 59
-        line 222: 74
-        line 225: 83
-        line 227: 112
-        line 228: 115
-        line 229: 122
-        line 230: 146
-        line 231: 170
-        line 238: 178
-        line 239: 204
-        line 241: 213
+        line 214: 8
+        line 215: 21
+        line 217: 29
+        line 218: 36
+        line 219: 43
+        line 220: 54
+        line 221: 59
+        line 223: 74
+        line 226: 83
+        line 228: 112
+        line 229: 115
+        line 230: 122
+        line 231: 146
+        line 232: 170
+        line 239: 178
+        line 240: 204
+        line 242: 213
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            71       3     3 terms   Ljava/util/List;
             0     216     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor;
             0     216     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext;
            21     195     2 termVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor;
            83     133     3 terms   Ljava/util/List;
@@ -500,15 +500,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #7                  // Method visitAtom:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext;)Lcz/cvut/fel/ida/logic/constructs/example/ValuedFact;
          5: areturn
       LineNumberTable:
-        line 199: 0
+        line 200: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #69(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
@@ -522,15 +522,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #44                 // Method visitFact:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FactContext;)Lcz/cvut/fel/ida/logic/constructs/example/ValuedFact;
          5: areturn
       LineNumberTable:
-        line 199: 0
+        line 200: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #69(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
@@ -545,15 +545,15 @@
       stack=2, locals=2, args_size=2
          0: aload_1
          1: aload_0
          2: invokevirtual #45                 // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermContext.accept:(Lorg/antlr/v4/runtime/tree/ParseTreeVisitor;)Ljava/lang/Object;
          5: checkcast     #46                 // class cz/cvut/fel/ida/logic/Term
          8: areturn
       LineNumberTable:
-        line 219: 0
+        line 220: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0 termVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor;
             0       9     1  term   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermContext;
 
   private static void $$$reportNull$$$0(int);
     descriptor: (I)V
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum c3f805c567adf055d66c3d175335dea06540610374565e9a25ebe130cd3c39f7
+  SHA-256 checksum cdebe1332c791218b7f62f08cb6ae4d982e659d39bf4ae5a07550ece9cc87719
   Compiled from "PlainGrammarVisitor.java"
 class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$WeightVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.algebra.weights.Weight>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #90                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor
   super_class: #91                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -441,15 +441,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #2                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #3                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 267: 0
+        line 268: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor;
 
   public cz.cvut.fel.ida.algebra.weights.Weight visitWeight(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$WeightContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightContext;)Lcz/cvut/fel/ida/algebra/weights/Weight;
     flags: (0x0001) ACC_PUBLIC
@@ -539,29 +539,29 @@
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightContext, class cz/cvut/fel/ida/utils/generic/Pair, int ]
           stack = []
         frame_type = 55 /* same */
         frame_type = 252 /* append */
           offset_delta = 32
           locals = [ class cz/cvut/fel/ida/algebra/weights/Weight ]
       LineNumberTable:
-        line 270: 8
-        line 271: 10
-        line 272: 12
-        line 273: 19
-        line 274: 21
-        line 275: 36
-        line 276: 43
-        line 277: 45
-        line 279: 57
-        line 282: 65
-        line 283: 72
-        line 284: 83
-        line 285: 118
-        line 286: 121
-        line 288: 154
+        line 271: 8
+        line 272: 10
+        line 273: 12
+        line 274: 19
+        line 275: 21
+        line 276: 36
+        line 277: 43
+        line 278: 45
+        line 280: 57
+        line 283: 65
+        line 284: 72
+        line 285: 83
+        line 286: 118
+        line 287: 121
+        line 289: 154
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            83      35     5  name   Ljava/lang/String;
           118       3     4 weight   Lcz/cvut/fel/ida/algebra/weights/Weight;
             0     157     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor;
             0     157     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightContext;
            10     147     2 value   Lcz/cvut/fel/ida/utils/generic/Pair;
@@ -957,68 +957,68 @@
           stack = []
         frame_type = 255 /* full_frame */
           offset_delta = 27
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ValueContext, class cz/cvut/fel/ida/algebra/values/Value, int ]
           stack = []
         frame_type = 31 /* same */
       LineNumberTable:
-        line 292: 0
-        line 293: 2
-        line 294: 4
-        line 295: 11
-        line 296: 33
-        line 297: 40
-        line 298: 75
-        line 300: 85
-        line 301: 95
-        line 302: 112
-        line 303: 118
-        line 304: 154
-        line 305: 169
-        line 306: 182
-        line 307: 189
-        line 308: 192
-        line 310: 202
-        line 311: 212
-        line 312: 221
-        line 313: 257
-        line 314: 292
-        line 315: 302
-        line 316: 305
-        line 317: 315
-        line 318: 325
-        line 319: 351
-        line 320: 377
-        line 321: 386
-        line 322: 422
-        line 323: 446
-        line 324: 470
-        line 325: 483
-        line 326: 496
-        line 327: 499
-        line 328: 513
-        line 329: 523
-        line 330: 525
-        line 331: 560
-        line 332: 571
-        line 333: 589
-        line 335: 600
-        line 338: 625
-        line 339: 636
-        line 340: 654
-        line 341: 676
-        line 342: 687
-        line 343: 705
-        line 344: 727
-        line 346: 738
-        line 348: 774
-        line 349: 777
-        line 351: 805
-        line 352: 809
-        line 354: 837
+        line 293: 0
+        line 294: 2
+        line 295: 4
+        line 296: 11
+        line 297: 33
+        line 298: 40
+        line 299: 75
+        line 301: 85
+        line 302: 95
+        line 303: 112
+        line 304: 118
+        line 305: 154
+        line 306: 169
+        line 307: 182
+        line 308: 189
+        line 309: 192
+        line 311: 202
+        line 312: 212
+        line 313: 221
+        line 314: 257
+        line 315: 292
+        line 316: 302
+        line 317: 305
+        line 318: 315
+        line 319: 325
+        line 320: 351
+        line 321: 377
+        line 322: 386
+        line 323: 422
+        line 324: 446
+        line 325: 470
+        line 326: 483
+        line 327: 496
+        line 328: 499
+        line 329: 513
+        line 330: 523
+        line 331: 525
+        line 332: 560
+        line 333: 571
+        line 334: 589
+        line 336: 600
+        line 339: 625
+        line 340: 636
+        line 341: 654
+        line 342: 676
+        line 343: 687
+        line 344: 705
+        line 345: 727
+        line 347: 738
+        line 349: 774
+        line 350: 777
+        line 352: 805
+        line 353: 809
+        line 355: 837
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            75      10     4 vector   Ljava/util/List;
           169      20     8     i   I
           182       7     9     v   D
           154      35     7 context   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ElementContext;
           112      90     4 length   I
@@ -1052,15 +1052,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #87                 // Method visitWeight:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightContext;)Lcz/cvut/fel/ida/algebra/weights/Weight;
          5: areturn
       LineNumberTable:
-        line 267: 0
+        line 268: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #122(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
@@ -1075,15 +1075,15 @@
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokevirtual #24                 // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext.getText:()Ljava/lang/String;
          4: invokestatic  #39                 // Method java/lang/Integer.parseInt:(Ljava/lang/String;)I
          7: invokestatic  #88                 // Method java/lang/Integer.valueOf:(I)Ljava/lang/Integer;
         10: areturn
       LineNumberTable:
-        line 330: 0
+        line 331: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0   num   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext;
 
   private static java.lang.Double lambda$parseValue$1(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$NumberContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext;)Ljava/lang/Double;
     flags: (0x100a) ACC_PRIVATE, ACC_STATIC, ACC_SYNTHETIC
@@ -1091,15 +1091,15 @@
       stack=2, locals=1, args_size=1
          0: aload_0
          1: invokevirtual #24                 // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext.getText:()Ljava/lang/String;
          4: invokestatic  #47                 // Method java/lang/Double.parseDouble:(Ljava/lang/String;)D
          7: invokestatic  #89                 // Method java/lang/Double.valueOf:(D)Ljava/lang/Double;
         10: areturn
       LineNumberTable:
-        line 313: 0
+        line 314: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0   num   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext;
 
   private static java.lang.Double lambda$parseValue$0(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$NumberContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext;)Ljava/lang/Double;
     flags: (0x100a) ACC_PRIVATE, ACC_STATIC, ACC_SYNTHETIC
@@ -1107,30 +1107,30 @@
       stack=2, locals=1, args_size=1
          0: aload_0
          1: invokevirtual #24                 // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext.getText:()Ljava/lang/String;
          4: invokestatic  #47                 // Method java/lang/Double.parseDouble:(Ljava/lang/String;)D
          7: invokestatic  #89                 // Method java/lang/Double.valueOf:(D)Ljava/lang/Double;
         10: areturn
       LineNumberTable:
-        line 297: 0
+        line 298: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0   num   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext;
 
   cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$WeightVisitor(cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor, cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$1);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$1;)V
     flags: (0x1000) ACC_SYNTHETIC
     Code:
       stack=2, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: invokespecial #1                  // Method "<init>":(Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;)V
          5: return
       LineNumberTable:
-        line 267: 0
+        line 268: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor;
             0       6     1    x0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
             0       6     2    x1   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$1;
 
   private static void $$$reportNull$$$0(int);
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 868d262cbe8b96bc9f906766fcae32b79dfa13ac834716feda444feeac5c4caa
+  SHA-256 checksum 032d2d2aaf0338e20c33b4211178070f8f2f4e125be177bf06a82cccf6dc7c47
   Compiled from "PlainGrammarVisitor.java"
 public class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$FactConjunctionVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.logic.constructs.Conjunction>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #19                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor
   super_class: #20                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -172,15 +172,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #2                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 184: 0
+        line 185: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor;
             0      10     1 this$0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
 
   public cz.cvut.fel.ida.logic.constructs.Conjunction visitConjunction(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$ConjunctionContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext;)Lcz/cvut/fel/ida/logic/constructs/Conjunction;
@@ -215,21 +215,21 @@
         63: dup
         64: aload_3
         65: invokespecial #15                 // Method cz/cvut/fel/ida/logic/constructs/Conjunction."<init>":(Ljava/util/List;)V
         68: areturn
       StackMapTable: number_of_entries = 1
         frame_type = 8 /* same */
       LineNumberTable:
-        line 189: 8
-        line 190: 20
-        line 191: 28
-        line 192: 32
-        line 193: 43
-        line 194: 48
-        line 195: 60
+        line 190: 8
+        line 191: 20
+        line 192: 28
+        line 193: 32
+        line 194: 43
+        line 195: 48
+        line 196: 60
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      69     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor;
             0      69     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext;
            20      49     2 factVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor;
            60       9     3 conjunction   Ljava/util/List;
       LocalVariableTypeTable:
@@ -249,15 +249,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #16                 // Method visitConjunction:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext;)Lcz/cvut/fel/ida/logic/constructs/Conjunction;
          5: areturn
       LineNumberTable:
-        line 184: 0
+        line 185: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #48(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
@@ -272,15 +272,15 @@
       stack=2, locals=2, args_size=2
          0: aload_1
          1: aload_0
          2: invokevirtual #17                 // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext.accept:(Lorg/antlr/v4/runtime/tree/ParseTreeVisitor;)Ljava/lang/Object;
          5: checkcast     #18                 // class cz/cvut/fel/ida/logic/constructs/example/ValuedFact
          8: areturn
       LineNumberTable:
-        line 193: 0
+        line 194: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0 factVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor;
             0       9     1  atom   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext;
 
   private static void $$$reportNull$$$0(int);
     descriptor: (I)V
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomVisitor.class

##### procyon -ec {}

```diff
@@ -44,14 +44,15 @@
         Transformation softNegation = null;
         if (ctx.negation() != null) {
             if (ctx.negation().SOFTNEGATION() != null) {
                 softNegation = Transformation.getFunction(this.this$0.builder.settings.softNegation);
             }
             else if (ctx.negation().NEGATION() != null) {
                 hardNegation = true;
+                this.this$0.builder.negationDetected = true;
             }
         }
         final BodyAtom bodyAtom = new BodyAtom(predicate, (List)terms, hardNegation, softNegation, weight);
         bodyAtom.originalString = ctx.getText();
         return bodyAtom;
     }
 }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 2a7ef036c4e2d4e000aa2ba26ddaa5e4b67559fdb4d19e92ac0c6b427d461f88
+  SHA-256 checksum 0bcaed00522d68e69b1a135a334fa22811bf219ec7b1a01be44777e352b19a63
   Compiled from "PlainGrammarVisitor.java"
 public class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$LiftedExampleVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.logic.constructs.example.LiftedExample>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #36                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor
   super_class: #37                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -237,16 +237,16 @@
          9: aload_0
         10: new           #3                  // class cz/cvut/fel/ida/logic/constructs/building/factories/VariableFactory
         13: dup
         14: invokespecial #4                  // Method cz/cvut/fel/ida/logic/constructs/building/factories/VariableFactory."<init>":()V
         17: putfield      #5                  // Field variableFactory:Lcz/cvut/fel/ida/logic/constructs/building/factories/VariableFactory;
         20: return
       LineNumberTable:
-        line 147: 0
-        line 148: 9
+        line 148: 0
+        line 149: 9
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      21     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor;
             0      21     1 this$0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
 
   public cz.cvut.fel.ida.logic.constructs.example.LiftedExample visitLiftedExample(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$LiftedExampleContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LiftedExampleContext;)Lcz/cvut/fel/ida/logic/constructs/example/LiftedExample;
@@ -314,29 +314,29 @@
        147: invokevirtual #29                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
        150: invokevirtual #30                 // Method java/util/logging/Logger.info:(Ljava/lang/String;)V
        153: aload         6
        155: areturn
       StackMapTable: number_of_entries = 1
         frame_type = 8 /* same */
       LineNumberTable:
-        line 152: 8
-        line 153: 20
-        line 154: 28
-        line 155: 40
-        line 157: 48
-        line 158: 52
-        line 159: 63
-        line 160: 68
-        line 162: 81
-        line 163: 85
-        line 164: 96
-        line 165: 101
-        line 167: 114
-        line 168: 127
-        line 169: 153
+        line 153: 8
+        line 154: 20
+        line 155: 28
+        line 156: 40
+        line 158: 48
+        line 159: 52
+        line 160: 63
+        line 161: 68
+        line 163: 81
+        line 164: 85
+        line 165: 96
+        line 166: 101
+        line 168: 114
+        line 169: 127
+        line 170: 153
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0     156     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor;
             0     156     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LiftedExampleContext;
            20     136     2 factConjunctionVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor;
            40     116     3 ruleLineVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$RuleLineVisitor;
            81      75     4 conjunctions   Ljava/util/List;
@@ -360,15 +360,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #31                 // Method visitLiftedExample:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LiftedExampleContext;)Lcz/cvut/fel/ida/logic/constructs/example/LiftedExample;
          5: areturn
       LineNumberTable:
-        line 147: 0
+        line 148: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #72(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
@@ -383,15 +383,15 @@
       stack=2, locals=2, args_size=2
          0: aload_1
          1: aload_0
          2: invokevirtual #32                 // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LrnnRuleContext.accept:(Lorg/antlr/v4/runtime/tree/ParseTreeVisitor;)Ljava/lang/Object;
          5: checkcast     #33                 // class cz/cvut/fel/ida/logic/constructs/template/components/WeightedRule
          8: areturn
       LineNumberTable:
-        line 164: 0
+        line 165: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0 ruleLineVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$RuleLineVisitor;
             0       9     1  conj   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LrnnRuleContext;
 
   private static cz.cvut.fel.ida.logic.constructs.Conjunction lambda$visitLiftedExample$0(cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$FactConjunctionVisitor, cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$ConjunctionContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor;Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext;)Lcz/cvut/fel/ida/logic/constructs/Conjunction;
@@ -400,15 +400,15 @@
       stack=2, locals=2, args_size=2
          0: aload_1
          1: aload_0
          2: invokevirtual #34                 // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext.accept:(Lorg/antlr/v4/runtime/tree/ParseTreeVisitor;)Ljava/lang/Object;
          5: checkcast     #35                 // class cz/cvut/fel/ida/logic/constructs/Conjunction
          8: areturn
       LineNumberTable:
-        line 159: 0
+        line 160: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0 factConjunctionVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor;
             0       9     1  conj   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext;
 
   private static void $$$reportNull$$$0(int);
     descriptor: (I)V
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum e547db69ae26a4d95543b8439ffea40b4b51e58bdc5d48861193d251b6795cb1
+  SHA-256 checksum 372205b073b95a29f9bf3e739c1a3847185ecba74feff7cab19561eaddae61c3
   Compiled from "PlainGrammarVisitor.java"
 class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$PredicateVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.logic.constructs.WeightedPredicate>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #24                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor
   super_class: #25                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -174,18 +174,18 @@
         10: iconst_m1
         11: putfield      #3                  // Field arity:I
         14: aload_0
         15: iload_2
         16: putfield      #3                  // Field arity:I
         19: return
       LineNumberTable:
-        line 248: 0
-        line 246: 9
-        line 249: 14
-        line 250: 19
+        line 249: 0
+        line 247: 9
+        line 250: 14
+        line 251: 19
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor;
             0      20     2 arity   I
 
   public cz.cvut.fel.ida.logic.constructs.WeightedPredicate visitPredicate(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$PredicateContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateContext;)Lcz/cvut/fel/ida/logic/constructs/WeightedPredicate;
@@ -266,21 +266,21 @@
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateContext ]
           stack = [ class cz/cvut/fel/ida/logic/constructs/building/factories/WeightedPredicateFactory, class java/lang/String, int, class java/lang/Boolean ]
         frame_type = 255 /* full_frame */
           offset_delta = 0
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateContext ]
           stack = [ class cz/cvut/fel/ida/logic/constructs/building/factories/WeightedPredicateFactory, class java/lang/String, int, class java/lang/Boolean, int ]
       LineNumberTable:
-        line 254: 8
-        line 256: 15
-        line 259: 31
-        line 257: 34
-        line 258: 35
-        line 261: 63
-        line 263: 120
+        line 255: 8
+        line 257: 15
+        line 260: 31
+        line 258: 34
+        line 259: 35
+        line 262: 63
+        line 264: 120
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            35      28     2    ex   Ljava/lang/Exception;
             0     122     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor;
             0     122     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateContext;
           120       2     2 predicate   Lcz/cvut/fel/ida/logic/constructs/WeightedPredicate;
     RuntimeInvisibleTypeAnnotations:
@@ -297,15 +297,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #23                 // Method visitPredicate:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateContext;)Lcz/cvut/fel/ida/logic/constructs/WeightedPredicate;
          5: areturn
       LineNumberTable:
-        line 245: 0
+        line 246: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #54(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 20cb8ec3b1305db056cd8b516b2a4d90cf008b65fe6b5e7c362612f6fd3039a5
+  SHA-256 checksum 6d7c4918d161eb7f39335de76a56b748b410cfeb22d969712a6b7eea84efa050
   Compiled from "PlainGrammarVisitor.java"
 class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$TermVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.logic.Term>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #16                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor
   super_class: #17                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -155,15 +155,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #2                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #3                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 358: 0
+        line 359: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor;
 
   public cz.cvut.fel.ida.logic.Term visitTerm(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$TermContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermContext;)Lcz/cvut/fel/ida/logic/Term;
     flags: (0x0001) ACC_PUBLIC
@@ -206,21 +206,21 @@
         frame_type = 8 /* same */
         frame_type = 27 /* same */
         frame_type = 21 /* same */
         frame_type = 252 /* append */
           offset_delta = 9
           locals = [ class java/lang/Object ]
       LineNumberTable:
-        line 365: 8
-        line 366: 15
-        line 367: 36
-        line 368: 43
-        line 370: 58
-        line 371: 66
-        line 373: 68
+        line 366: 8
+        line 367: 15
+        line 368: 36
+        line 369: 43
+        line 371: 58
+        line 372: 66
+        line 374: 68
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            33       3     2  term   Lcz/cvut/fel/ida/logic/Term;
            55       3     2  term   Lcz/cvut/fel/ida/logic/Term;
             0      70     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor;
             0      70     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermContext;
            68       2     2  term   Lcz/cvut/fel/ida/logic/Term;
@@ -238,15 +238,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #15                 // Method visitTerm:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermContext;)Lcz/cvut/fel/ida/logic/Term;
          5: areturn
       LineNumberTable:
-        line 358: 0
+        line 359: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #42(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
@@ -260,15 +260,15 @@
     Code:
       stack=2, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: invokespecial #1                  // Method "<init>":(Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;)V
          5: return
       LineNumberTable:
-        line 358: 0
+        line 359: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor;
             0       6     1    x0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
             0       6     2    x1   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$1;
 
   private static void $$$reportNull$$$0(int);
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 69c7e438df87558bc86a379730735cb614731a27ed0eb4501e8f3f3e1cf22dcc
+  SHA-256 checksum ee94a3ebfa70dd09bbbbb5db6a10e493362d40e3880688b81912d091d40d5360
   Compiled from "PlainGrammarVisitor.java"
 public class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$PredicateOffsetVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.utils.generic.Pair<cz.cvut.fel.ida.logic.constructs.WeightedPredicate, cz.cvut.fel.ida.algebra.weights.Weight>>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #32                         // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor
   super_class: #33                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -201,15 +201,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #2                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 401: 0
+        line 402: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor;
             0      10     1 this$0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
 
   public cz.cvut.fel.ida.utils.generic.Pair<cz.cvut.fel.ida.logic.constructs.WeightedPredicate, cz.cvut.fel.ida.algebra.weights.Weight> visitPredicateOffset(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$PredicateOffsetContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateOffsetContext;)Lcz/cvut/fel/ida/utils/generic/Pair;
@@ -311,23 +311,23 @@
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateOffsetContext, int ]
           stack = [ class cz/cvut/fel/ida/logic/constructs/building/factories/WeightedPredicateFactory, class java/lang/String, int, class java/lang/Boolean ]
         frame_type = 255 /* full_frame */
           offset_delta = 0
           locals = [ class cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor, class cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateOffsetContext, int ]
           stack = [ class cz/cvut/fel/ida/logic/constructs/building/factories/WeightedPredicateFactory, class java/lang/String, int, class java/lang/Boolean, int ]
       LineNumberTable:
-        line 404: 8
-        line 406: 10
-        line 409: 26
-        line 407: 29
-        line 408: 30
-        line 410: 58
-        line 411: 121
-        line 412: 145
-        line 413: 151
+        line 405: 8
+        line 407: 10
+        line 410: 26
+        line 408: 29
+        line 409: 30
+        line 411: 58
+        line 412: 121
+        line 413: 145
+        line 414: 151
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            30      28     3    ex   Ljava/lang/Exception;
             0     162     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor;
             0     162     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateOffsetContext;
            10     152     2 arity   I
           121      41     3 predicate   Lcz/cvut/fel/ida/logic/constructs/WeightedPredicate;
@@ -347,15 +347,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #31                 // Method visitPredicateOffset:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateOffsetContext;)Lcz/cvut/fel/ida/utils/generic/Pair;
          5: areturn
       LineNumberTable:
-        line 401: 0
+        line 402: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor;
     RuntimeInvisibleTypeAnnotations:
       0: #66(): METHOD_FORMAL_PARAMETER, param_index=0
         org.jetbrains.annotations.NotNull
     RuntimeInvisibleParameterAnnotations:
```

#### cz/cvut/fel/ida/logic/constructs/building/TemplateBuilder.class

##### procyon -ec {}

```diff
@@ -81,14 +81,15 @@
             new Pair((Object)pair.r, (Object)new PredicateMetadata(this.settings, (Map)pair.s));
             return;
         }).collect((Collector<? super Object, ?, List<? super Object>>)Collectors.toList());
         template.weightsMetadata = weightsMetadata.stream().map(pair -> {
             new Pair((Object)pair.r, (Object)new WeightMetadata(this.settings, (Map)pair.s));
             return;
         }).collect((Collector<? super Object, ?, List<? super Object>>)Collectors.toList());
+        template.containsNegation = this.negationDetected;
         TemplateBuilder.LOG.fine("Template has been built : " + template);
         return template;
     }
     
     public Template extendTemplateWith(final Reader reader, final Settings settings) {
         return null;
     }
```

#### cz/cvut/fel/ida/logic/constructs/building/LogicSourceBuilder.class

##### procyon -ec {}

```diff
@@ -11,20 +11,22 @@
 import org.antlr.v4.runtime.ParserRuleContext;
 import cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainParseTree;
 
 public abstract class LogicSourceBuilder<I extends PlainParseTree<? extends ParserRuleContext>, O>
 {
     private static final Logger LOG;
     public Settings settings;
+    public boolean negationDetected;
     public Function<String, Boolean> rebuildCallback;
     public ConstantFactory constantFactory;
     public WeightedPredicateFactory predicateFactory;
     public WeightFactory weightFactory;
     
     public LogicSourceBuilder(final Settings settings, final WeightFactory weightFactory) {
+        this.negationDetected = false;
         this.constantFactory = new ConstantFactory();
         this.predicateFactory = new WeightedPredicateFactory();
         this.settings = settings;
         this.weightFactory = weightFactory;
     }
     
     public void setFactoriesFrom(final LogicSourceBuilder other) {
```

### Comparing `neuralogic-0.7.4/neuralogic/logging/__init__.py` & `neuralogic-0.7.5/neuralogic/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/base.py` & `neuralogic-0.7.5/neuralogic/nn/base.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/evaluator/java.py` & `neuralogic-0.7.5/neuralogic/nn/evaluator/java.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/functional.py` & `neuralogic-0.7.5/neuralogic/nn/functional.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/init.py` & `neuralogic-0.7.5/neuralogic/nn/init.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/java.py` & `neuralogic-0.7.5/neuralogic/nn/java.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/loss.py` & `neuralogic-0.7.5/neuralogic/nn/loss.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/__init__.py` & `neuralogic-0.7.5/neuralogic/nn/module/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/attention.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/attention.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/gru.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/gru.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/linear.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/linear.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/lstm.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/lstm.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/mlp.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/mlp.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/pooling.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/pooling.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/positional_encoding.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/rnn.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/rnn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/rvnn.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/rvnn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/general/transformer.py` & `neuralogic-0.7.5/neuralogic/nn/module/general/transformer.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/gnn/appnp.py` & `neuralogic-0.7.5/neuralogic/nn/module/gnn/appnp.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/gnn/gatv2.py` & `neuralogic-0.7.5/neuralogic/nn/module/gnn/gatv2.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/gnn/gcn.py` & `neuralogic-0.7.5/neuralogic/nn/module/gnn/gcn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/gnn/gin.py` & `neuralogic-0.7.5/neuralogic/nn/module/gnn/gin.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/gnn/gsage.py` & `neuralogic-0.7.5/neuralogic/nn/module/gnn/gsage.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/gnn/res_gated.py` & `neuralogic-0.7.5/neuralogic/nn/module/gnn/res_gated.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/gnn/rgcn.py` & `neuralogic-0.7.5/neuralogic/nn/module/gnn/rgcn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/gnn/sg.py` & `neuralogic-0.7.5/neuralogic/nn/module/gnn/sg.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/gnn/tag.py` & `neuralogic-0.7.5/neuralogic/nn/module/gnn/tag.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/meta/magnn.py` & `neuralogic-0.7.5/neuralogic/nn/module/meta/magnn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/module/meta/meta.py` & `neuralogic-0.7.5/neuralogic/nn/module/meta/meta.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/nn/torch_function.py` & `neuralogic-0.7.5/neuralogic/nn/torch_function.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/optim/adam.py` & `neuralogic-0.7.5/neuralogic/optim/adam.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/optim/lr_scheduler/arithmetic.py` & `neuralogic-0.7.5/neuralogic/optim/lr_scheduler/arithmetic.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/optim/lr_scheduler/geometric.py` & `neuralogic-0.7.5/neuralogic/optim/lr_scheduler/geometric.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/optim/lr_scheduler/lr_decay.py` & `neuralogic-0.7.5/neuralogic/optim/lr_scheduler/lr_decay.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/optim/optimizer.py` & `neuralogic-0.7.5/neuralogic/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/optim/sgd.py` & `neuralogic-0.7.5/neuralogic/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/data/__init__.py` & `neuralogic-0.7.5/neuralogic/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt` & `neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt` & `neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt` & `neuralogic-0.7.5/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/data/datasets/nations/embeddings.txt` & `neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/embeddings.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/data/datasets/nations/examples.txt` & `neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/examples.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/data/datasets/nations/queries.txt` & `neuralogic-0.7.5/neuralogic/utils/data/datasets/nations/queries.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/trains/examples.txt` & `neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/examples.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/data/datasets/simple/trains/template.txt` & `neuralogic-0.7.5/neuralogic/utils/data/datasets/simple/trains/template.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic/utils/visualize/__init__.py` & `neuralogic-0.7.5/neuralogic/utils/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/neuralogic.egg-info/PKG-INFO` & `neuralogic-0.7.5/neuralogic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralogic
-Version: 0.7.4
+Version: 0.7.5
 Summary: PyNeuraLogic lets you use Python to create Differentiable Logic Programs.
 Home-page: https://github.com/LukasZahradnik/PyNeuraLogic
 Author: Lukáš Zahradník
 Author-email: lukaszahradnik96@seznam.cz
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuralogic Version: 0.7.4 Summary: PyNeuraLogic
+Metadata-Version: 2.1 Name: neuralogic Version: 0.7.5 Summary: PyNeuraLogic
 lets you use Python to create Differentiable Logic Programs. Home-page: https:/
 /github.com/LukasZahradnik/PyNeuraLogic Author: LukÃ¡Å¡ ZahradnÃ­k Author-
 email: lukaszahradnik96@seznam.cz License: MIT Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `neuralogic-0.7.4/neuralogic.egg-info/SOURCES.txt` & `neuralogic-0.7.5/neuralogic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.4/setup.py` & `neuralogic-0.7.5/setup.py`

 * *Files identical despite different names*

