# Comparing `tmp/dive_into_graphs-1.0.0.tar.gz` & `tmp/dive_into_graphs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/grads/m/mengliu/DIG/dist/tmp2wy4d54i/dive_into_graphs-1.0.0.tar", last modified: Thu Jul 14 06:57:58 2022, max compression
+gzip compressed data, was "dive_into_graphs-1.1.0.tar", last modified: Fri Apr  7 20:06:28 2023, max compression
```

## Comparing `dive_into_graphs-1.0.0.tar` & `dive_into_graphs-1.1.0.tar`

### file list

```diff
@@ -1,217 +1,262 @@
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    35149 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/LICENSE
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      194 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/MANIFEST.in
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10701 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/PKG-INFO
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10144 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/README.md
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/dataset/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    16176 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/dataset/PygDataset.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      180 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/dataset/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1085 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/dataset/config.csv
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11965 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/dataset/ggraph_dataset.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/evaluation/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      168 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/evaluation/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     8836 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/evaluation/metric.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/method/
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       63 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    20501 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/graphaf.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       85 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13280 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/graphaf.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    15460 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/graphflow.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    89964 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/graphflow_con_rl.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    45868 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/graphflow_rl.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7169 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/model_utils.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4689 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/rgcn.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6848 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/st_net.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      966 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/train_utils.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       57 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    20431 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/graphdf.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      133 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7509 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/df_utils.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9258 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/disgraphaf.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    16549 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/graphflow.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    73720 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/graphflow_con_rl.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    41177 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/graphflow_rl.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4670 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/rgcn.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7854 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/st_net.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      937 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/train_utils.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphEBM/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphEBM/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4247 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphEBM/energy_func.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    28487 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphEBM/graphebm.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1251 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/GraphEBM/util.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       53 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      273 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    17307 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/chemutils.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5514 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/datautils.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5560 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtmpn.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5429 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtmpn_bo.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    14456 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_dec.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4469 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_enc.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3731 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_enc_bo.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10483 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_vae.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13671 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_vae_bo.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    15087 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtprop_vae.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4603 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/mol_tree.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6355 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/mpn.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2053 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/nnutils.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5880 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/sascorer.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1607 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/vocab.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11730 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/jtvae.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      254 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1733 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/method/generator.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph/utils/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      589 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/utils/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     8862 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/utils/environment.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)  3848394 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/utils/fpscores.pkl.gz
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5330 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/utils/gen_mol_from_one_shot_tensor.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5661 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph/utils/sascorer.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph3D/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph3D/dataset/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       50 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/dataset/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11207 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/dataset/ggraph3D_dataset.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph3D/evaluation/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      116 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/evaluation/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3606 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/evaluation/metric.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       68 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4120 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/gspherenet.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       26 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1819 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/att.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9661 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/features.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4769 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/geometric_computing.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2762 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/net_utils.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11251 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/spherenet.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    14023 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/sphgen.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       70 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/method/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/ggraph3D/utils/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      147 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/utils/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2732 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/utils/eval_bond_mmd_utils.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1334 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/utils/eval_prop_utils.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10053 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/ggraph3D/utils/eval_validity_utils.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/sslgraph/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/sslgraph/dataset/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9090 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/dataset/TUDataset.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      166 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/dataset/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4025 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/dataset/datasets.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5309 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/dataset/feat_expansion.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/sslgraph/evaluation/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      193 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/evaluation/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    22838 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/evaluation/eval_graph.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    12591 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/evaluation/eval_node.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      215 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      160 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    17839 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/contrastive.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2133 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/grace.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3631 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/graphcl.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2744 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/infograph.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6997 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/mvgrl.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/objectives/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      102 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/objectives/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4311 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/objectives/infonce.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5820 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/objectives/jse.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/views_fn/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      373 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/views_fn/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1995 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/views_fn/combination.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3682 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/views_fn/feature.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4117 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/views_fn/sample.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     8891 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/views_fn/structure.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/sslgraph/utils/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      106 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/utils/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    15183 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/utils/encoders.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      358 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/sslgraph/utils/seed.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/threedgraph/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/threedgraph/dataset/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5546 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/dataset/PygMD17.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6567 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/dataset/PygQM93D.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       92 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/dataset/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/threedgraph/evaluation/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       70 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/evaluation/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1199 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/evaluation/eval.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      232 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/comenet/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       57 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/comenet/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13076 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/comenet/comenet.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    12640 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/comenet/features.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/dimenetpp/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      105 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/dimenetpp/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11896 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/dimenetpp/dimenetpp.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7645 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/dimenetpp/features.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9171 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/run.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/schnet/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       60 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/schnet/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6177 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/schnet/schnet.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/spherenet/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      118 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/spherenet/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9618 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/spherenet/features.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13272 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/method/spherenet/spherenet.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/threedgraph/utils/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       85 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/utils/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3360 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/threedgraph/utils/geometric_computing.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      101 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/version.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/xgraph/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/xgraph/dataset/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      348 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/dataset/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11963 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/dataset/mol_dataset.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6727 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/dataset/nlp_dataset.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13000 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/dataset/syn_dataset.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1237 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/dataset/utils_dataset.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/xgraph/evaluation/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      163 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/evaluation/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      176 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/evaluation/defi.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13435 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/evaluation/metrics.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/xgraph/method/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      392 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    20147 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/base_explainer.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4990 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/deeplift.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5643 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/gnn_gi.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10463 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/gnn_lrp.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6949 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/gnnexplainer.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13849 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/gradcam.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    35662 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/pgexplainer.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    12446 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/shapley.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    38224 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/method/subgraphx.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/xgraph/models/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      275 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/models/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/xgraph/models/ext/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      107 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/models/ext/__init__.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/xgraph/models/ext/deeplift/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/models/ext/deeplift/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    43350 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/models/ext/deeplift/deep_lift.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    30809 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/models/ext/deeplift/layer_deep_lift.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    24371 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/models/gradient_utils.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1371 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/models/model_manager.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    31784 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/models/models.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4215 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/models/utils.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dig/xgraph/utils/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/utils/__init__.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      591 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/utils/compatibility.py
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      523 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/dig/xgraph/utils/init.py
-drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dive_into_graphs.egg-info/
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10701 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dive_into_graphs.egg-info/PKG-INFO
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6453 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dive_into_graphs.egg-info/SOURCES.txt
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        1 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dive_into_graphs.egg-info/dependency_links.txt
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      158 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dive_into_graphs.egg-info/requires.txt
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        4 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/dive_into_graphs.egg-info/top_level.txt
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      107 2022-07-14 06:57:58.000000 dive_into_graphs-1.0.0/setup.cfg
--rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1617 2022-07-14 06:52:10.000000 dive_into_graphs-1.0.0/setup.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.587713 dive_into_graphs-1.1.0/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    35149 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/LICENSE
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      194 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/MANIFEST.in
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11709 2023-04-07 20:06:28.587713 dive_into_graphs-1.1.0/PKG-INFO
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11152 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/README.md
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.559713 dive_into_graphs-1.1.0/dig/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.559713 dive_into_graphs-1.1.0/dig/ggraph/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.559713 dive_into_graphs-1.1.0/dig/ggraph/dataset/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    16176 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/dataset/PygDataset.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      180 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/dataset/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1085 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/dataset/config.csv
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11965 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/dataset/ggraph_dataset.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.559713 dive_into_graphs-1.1.0/dig/ggraph/evaluation/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      168 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/evaluation/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     8836 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/evaluation/metric.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.559713 dive_into_graphs-1.1.0/dig/ggraph/method/
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.559713 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       63 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    20504 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/graphaf.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.559713 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       85 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13280 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/graphaf.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    15460 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/graphflow.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    89964 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/graphflow_con_rl.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    45868 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/graphflow_rl.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7169 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/model_utils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4689 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/rgcn.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6848 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/st_net.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      966 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/train_utils.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.559713 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       57 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    20434 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/graphdf.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.563713 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      133 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7509 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/df_utils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9258 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/disgraphaf.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    16549 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/graphflow.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    73720 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/graphflow_con_rl.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    41177 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/graphflow_rl.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4670 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/rgcn.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7854 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/st_net.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      937 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/train_utils.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.563713 dive_into_graphs-1.1.0/dig/ggraph/method/GraphEBM/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphEBM/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4247 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphEBM/energy_func.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    28490 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphEBM/graphebm.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1251 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/GraphEBM/util.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.563713 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       53 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.563713 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      273 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    17307 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/chemutils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5514 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/datautils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5560 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtmpn.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5429 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtmpn_bo.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    14456 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_dec.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4469 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_enc.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3731 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_enc_bo.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10483 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_vae.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13671 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_vae_bo.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    15087 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtprop_vae.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4603 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/mol_tree.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6355 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/mpn.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2053 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/nnutils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5880 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/sascorer.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1607 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/vocab.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11733 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/jtvae.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      254 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1733 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/method/generator.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/ggraph/utils/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      589 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/utils/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     8862 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/utils/environment.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)  3848394 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/utils/fpscores.pkl.gz
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5330 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/utils/gen_mol_from_one_shot_tensor.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5661 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph/utils/sascorer.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/ggraph3D/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/ggraph3D/dataset/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       98 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/dataset/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    15280 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/dataset/ggraph3D_dataset.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/ggraph3D/evaluation/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      116 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/evaluation/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6848 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/evaluation/metric.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/ggraph3D/method/
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       68 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7007 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/gspherenet.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       26 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1819 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/att.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9661 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/features.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4769 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/geometric_computing.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2762 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/net_utils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11256 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/spherenet.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    14023 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/sphgen.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       70 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/method/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/ggraph3D/utils/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      241 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/utils/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4137 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/utils/eval_bond_mmd_utils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1870 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/utils/eval_prop_utils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10238 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/ggraph3D/utils/eval_validity_utils.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/lsgraph/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/lsgraph/dataset/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      190 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/dataset/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3225 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/dataset/get_data.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4166 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/dataset/loader.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.571713 dive_into_graphs-1.1.0/dig/lsgraph/method/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2536 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/FM.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.575713 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      505 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2161 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/history.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4167 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/loader.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1847 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/metis.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.575713 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/models/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      317 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/models/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10674 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/models/base.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6109 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/models/gcn.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6359 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/models/gcn2.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     8241 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/models/pna.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5385 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/models/pna_jk.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5165 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/pool.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2088 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/GraphFMOB/utils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/lsgraph/method/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.575713 dive_into_graphs-1.1.0/dig/oodgraph/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      605 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/oodgraph/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4085 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/oodgraph/good_arxiv.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4061 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/oodgraph/good_cbas.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5562 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/oodgraph/good_cmnist.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3975 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/oodgraph/good_cora.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6034 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/oodgraph/good_hiv.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6295 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/oodgraph/good_motif.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6060 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/oodgraph/good_pcba.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6391 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/oodgraph/good_zinc.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.575713 dive_into_graphs-1.1.0/dig/sslgraph/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.575713 dive_into_graphs-1.1.0/dig/sslgraph/dataset/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9090 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/dataset/TUDataset.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      166 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/dataset/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4025 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/dataset/datasets.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5309 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/dataset/feat_expansion.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.575713 dive_into_graphs-1.1.0/dig/sslgraph/evaluation/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      193 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/evaluation/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    22838 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/evaluation/eval_graph.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    12564 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/evaluation/eval_node.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.575713 dive_into_graphs-1.1.0/dig/sslgraph/method/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      237 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.575713 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      186 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    17839 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/contrastive.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2133 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/grace.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3631 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/graphcl.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     2744 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/infograph.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6997 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/mvgrl.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4534 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/pgrace.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/objectives/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      103 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/objectives/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5179 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/objectives/infonce.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5820 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/objectives/jse.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/views_fn/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      461 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/views_fn/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1995 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/views_fn/combination.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7537 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/views_fn/feature.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4117 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/views_fn/sample.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11786 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/views_fn/structure.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/sslgraph/utils/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      106 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/utils/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7352 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/utils/adaptive.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    15183 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/utils/encoders.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      358 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/sslgraph/utils/seed.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/threedgraph/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/threedgraph/dataset/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10093 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/dataset/ECdataset.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9705 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/dataset/FOLDdataset.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5544 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/dataset/PygMD17.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6567 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/dataset/PygQM93D.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      198 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/dataset/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/threedgraph/evaluation/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       70 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/evaluation/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1199 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/evaluation/eval.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/threedgraph/method/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      273 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/threedgraph/method/comenet/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       57 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/comenet/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13216 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/comenet/comenet.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    12640 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/comenet/features.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.579713 dive_into_graphs-1.1.0/dig/threedgraph/method/dimenetpp/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      105 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/dimenetpp/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11902 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/dimenetpp/dimenetpp.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7655 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/dimenetpp/features.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.583713 dive_into_graphs-1.1.0/dig/threedgraph/method/pronet/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       54 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/pronet/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    12545 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/pronet/features.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    16850 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/pronet/pronet.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9171 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/run.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.583713 dive_into_graphs-1.1.0/dig/threedgraph/method/schnet/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       60 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/schnet/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6358 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/schnet/schnet.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.583713 dive_into_graphs-1.1.0/dig/threedgraph/method/spherenet/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      118 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/spherenet/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     9618 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/spherenet/features.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13277 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/method/spherenet/spherenet.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.583713 dive_into_graphs-1.1.0/dig/threedgraph/utils/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       85 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/utils/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     3408 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/threedgraph/utils/geometric_computing.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      101 2023-04-07 20:05:10.000000 dive_into_graphs-1.1.0/dig/version.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.583713 dive_into_graphs-1.1.0/dig/xgraph/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.583713 dive_into_graphs-1.1.0/dig/xgraph/dataset/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      348 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/dataset/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11963 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/dataset/mol_dataset.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     6727 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/dataset/nlp_dataset.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13000 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/dataset/syn_dataset.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1237 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/dataset/utils_dataset.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.583713 dive_into_graphs-1.1.0/dig/xgraph/evaluation/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      163 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/evaluation/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      176 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/evaluation/defi.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13435 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/evaluation/metrics.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.583713 dive_into_graphs-1.1.0/dig/xgraph/method/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      432 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    21209 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/base_explainer.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4990 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/deeplift.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    17269 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/flowx.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     5643 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/gnn_gi.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    10463 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/gnn_lrp.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     8519 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/gnnexplainer.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    13990 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/gradcam.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    35667 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/pgexplainer.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    12480 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/shapley.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    38313 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/subgraphx.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.587713 dive_into_graphs-1.1.0/dig/xgraph/method/utils/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)       67 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/utils/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1209 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/method/utils/symmetric_edge_mask.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.587713 dive_into_graphs-1.1.0/dig/xgraph/models/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      286 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/models/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.587713 dive_into_graphs-1.1.0/dig/xgraph/models/ext/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      107 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/models/ext/__init__.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.587713 dive_into_graphs-1.1.0/dig/xgraph/models/ext/deeplift/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/models/ext/deeplift/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    43350 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/models/ext/deeplift/deep_lift.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    30809 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/models/ext/deeplift/layer_deep_lift.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    24371 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/models/gradient_utils.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1371 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/models/model_manager.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    34870 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/models/models.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     4952 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/models/utils.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.587713 dive_into_graphs-1.1.0/dig/xgraph/utils/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/utils/__init__.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      591 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/utils/compatibility.py
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      523 2023-04-07 20:00:52.000000 dive_into_graphs-1.1.0/dig/xgraph/utils/init.py
+drwxrwxr-x   0 mengliu  (629008822) mengliu  (629008822)        0 2023-04-07 20:06:28.587713 dive_into_graphs-1.1.0/dive_into_graphs.egg-info/
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)    11709 2023-04-07 20:06:28.000000 dive_into_graphs-1.1.0/dive_into_graphs.egg-info/PKG-INFO
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     7753 2023-04-07 20:06:28.000000 dive_into_graphs-1.1.0/dive_into_graphs.egg-info/SOURCES.txt
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        1 2023-04-07 20:06:28.000000 dive_into_graphs-1.1.0/dive_into_graphs.egg-info/dependency_links.txt
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      164 2023-04-07 20:06:28.000000 dive_into_graphs-1.1.0/dive_into_graphs.egg-info/requires.txt
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)        4 2023-04-07 20:06:28.000000 dive_into_graphs-1.1.0/dive_into_graphs.egg-info/top_level.txt
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)      107 2023-04-07 20:06:28.587713 dive_into_graphs-1.1.0/setup.cfg
+-rw-rw-r--   0 mengliu  (629008822) mengliu  (629008822)     1673 2023-04-07 20:00:53.000000 dive_into_graphs-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dive_into_graphs-1.0.0/LICENSE` & `dive_into_graphs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/PKG-INFO` & `dive_into_graphs-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dive_into_graphs
-Version: 1.0.0
+Version: 1.1.0
 Summary: DIG: Dive into Graphs is a turnkey library for graph deep learning research.
 Home-page: https://github.com/divelab/DIG
 Author: DIVE Lab@TAMU
 Author-email: sji@tamu.edu
 Maintainer: DIVE Lab@TAMU
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
@@ -34,49 +34,49 @@
 [contributor-url]:https://github.com/divelab/DIG/graphs/contributors 
 [contributing-image]:https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
 [contributing-url]:https://diveintographs.readthedocs.io/en/latest/contribution/instruction.html
 
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Docs Status][docs-image]][docs-url]
-[![Build Status](https://travis-ci.com/divelab/DIG.svg?branch=dig)](https://travis-ci.com/divelab/DIG)
-[![codecov](https://codecov.io/gh/divelab/DIG/branch/dig/graph/badge.svg?token=KBJ1P31VCH)](https://codecov.io/gh/divelab/DIG)
+[![Build Status](https://travis-ci.com/divelab/DIG.svg?branch=dig-stable)](https://travis-ci.com/divelab/DIG)
+[![codecov](https://codecov.io/gh/divelab/DIG/branch/dig-stable/graph/badge.svg?token=KBJ1P31VCH)](https://codecov.io/gh/divelab/DIG)
 ![Last Commit](https://img.shields.io/github/last-commit/divelab/DIG)
 [![Contributing][contributing-image]][contributing-url]
 [![License][license-image]][license-url]
 ![visitors](https://visitor-badge.glitch.me/badge?page_id=jwenjian.visitor-badge)
 [![Downloads](https://pepy.tech/badge/dive-into-graphs)](https://pepy.tech/project/dive-into-graphs)
 <!--- [![Contributors][contributor-image]][contributor-url] -->
 
 
-**[Documentation](https://diveintographs.readthedocs.io)** | **[Paper [JMLR]](https://www.jmlr.org/papers/v22/21-0343.html)** | **[Tutorials](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html#)** | **[Benchmarks](https://github.com/divelab/DIG/tree/dig/benchmarks)** |  **[Examples](https://github.com/divelab/DIG/tree/dig/examples)**
+**[Documentation](https://diveintographs.readthedocs.io)** | **[Paper [JMLR]](https://www.jmlr.org/papers/v22/21-0343.html)** | **[Tutorials](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html#)** | **[Benchmarks](https://github.com/divelab/DIG/tree/dig-stable/benchmarks)** |  **[Examples](https://github.com/divelab/DIG/tree/dig-stable/examples)** | **[Join the DIG slack community now!:fire:](https://join.slack.com/t/dive-into-graphs/shared_invite/zt-1i9kn731c-RhLA1zcEGHXbIToxdVqo0g)**
 
 *DIG: Dive into Graphs* is a turnkey library for graph deep learning research.
 
 :fire:**Update (2022/07): We have upgraded our DIG library based on PyG 2.0.0. We recommend installing our latest version.**
 
 ## Why DIG?
 
-The key difference with current graph deep learning libraries, such as PyTorch Geometric (PyG) and Deep Graph Library (DGL), is that, while PyG and DGL support basic graph deep learning operations, DIG provides a unified testbed for higher level, research-oriented graph deep learning tasks, such as graph generation, self-supervised learning, explainability, and 3D graphs.
+The key difference with current graph deep learning libraries, such as PyTorch Geometric (PyG) and Deep Graph Library (DGL), is that, while PyG and DGL support basic graph deep learning operations, DIG provides a unified testbed for higher level, research-oriented graph deep learning tasks, such as graph generation, self-supervised learning, explainability, 3D graphs, and graph out-of-distribution.
 
 If you are working or plan to work on research in graph deep learning, DIG enables you to develop your own methods within our extensible framework, and compare with current baseline methods using common datasets and evaluation metrics without extra efforts.
 
 ## Overview
 
 It includes unified implementations of **data interfaces**, **common algorithms**, and **evaluation metrics** for several advanced tasks. Our goal is to enable researchers to easily implement and benchmark algorithms. Currently, we consider the following research directions.
 
 * **Graph Generation**: `dig.ggraph`
 * **Self-supervised Learning on Graphs**: `dig.sslgraph`
 * **Explainability of Graph Neural Networks**: `dig.xgraph`
 * **Deep Learning on 3D Graphs**: `dig.threedgraph`
-
+* **Graph OOD**: `dig.oodgraph`
 
 
 <p align="center">
-<img src="https://github.com/divelab/DIG/blob/dig/imgs/DIG-overview.png" width="700" class="center" alt="logo"/>
+<img src="https://github.com/divelab/DIG/blob/dig-stable/docs/imgs/DIG-overview.png" width="700" class="center" alt="logo"/>
     <br/>
 </p>
 
 
 ## Usage
 
 Example: a few lines of code to run [SphereNet](https://openreview.net/forum?id=givsRXsOt9r) on [QM9](https://www.nature.com/articles/sdata201422) to incorporate 3D information of molecules.
@@ -109,22 +109,22 @@
 run3d.run(device, train_dataset, valid_dataset, test_dataset, model, loss_func, evaluation,
           epochs=20, batch_size=32, vt_batch_size=32, lr=0.0005, lr_decay_factor=0.5, lr_decay_step_size=15)
 
 ```
 
 
 1. For details of all included APIs, please refer to the [documentation](https://diveintographs.readthedocs.io/). 
-2. We provide a hands-on tutorial for each direction to help you to get started with *DIG*: [Graph Generation](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html), [Self-supervised Learning on Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/sslgraph.html), [Explainability of Graph Neural Networks](https://diveintographs.readthedocs.io/en/latest/tutorials/subgraphx.html), and [Deep Learning on 3D Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/threedgraph.html).
-3. We also provide [examples](https://github.com/divelab/DIG/tree/dig/examples) to use APIs provided in *DIG*. You can get started with your interested directions by clicking the following links.
-
-* [Graph Generation](https://github.com/divelab/DIG/tree/dig/examples/ggraph): [`JT-VAE`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/JTVAE), [`GraphAF`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/GraphAF), [`GraphDF`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/GraphDF), [`GraphEBM`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/GraphEBM).
-* [Self-supervised Learning on Graphs](https://github.com/divelab/DIG/tree/dig/examples/sslgraph): [`InfoGraph`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_infograph.ipynb), [`GRACE`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_grace.ipynb), [`MVGRL`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_mvgrl.ipynb), [`GraphCL`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_graphcl.ipynb).
-* [Explainability of Graph Neural Networks](https://github.com/divelab/DIG/tree/dig/examples/xgraph): [`DeepLIFT`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/deeplift.ipynb), [`GNN-LRP`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/gnn_lrp.ipynb), [`GNNExplainer`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/gnnexplainer.ipynb), [`GradCAM`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/gradcam.ipynb), [`PGExplainer`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/pgexplainer.ipynb), [`SubgraphX`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/subgraphx.ipynb).
-* [Deep Learning on 3D Graphs](https://github.com/divelab/DIG/tree/dig/examples/threedgraph): [`SchNet`](https://github.com/divelab/DIG/blob/dig/examples/threedgraph/threedgraph.ipynb), [`DimeNet++`](https://github.com/divelab/DIG/blob/dig/examples/threedgraph/threedgraph.ipynb), [`SphereNet`](https://github.com/divelab/DIG/blob/dig/examples/threedgraph/threedgraph.ipynb).
+2. We provide a hands-on tutorial for each direction to help you to get started with *DIG*: [Graph Generation](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html), [Self-supervised Learning on Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/sslgraph.html), [Explainability of Graph Neural Networks](https://diveintographs.readthedocs.io/en/latest/tutorials/subgraphx.html), [Deep Learning on 3D Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/threedgraph.html), [Graph OOD (GOOD) datasets](https://diveintographs.readthedocs.io/en/latest/tutorials/oodgraph.html).
+3. We also provide [examples](https://github.com/divelab/DIG/tree/dig-stable/examples) to use APIs provided in *DIG*. You can get started with your interested directions by clicking the following links.
 
+* [Graph Generation](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph): [`JT-VAE`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/JTVAE), [`GraphAF`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphAF), [`GraphDF`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphDF), [`GraphEBM`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphEBM).
+* [Self-supervised Learning on Graphs](https://github.com/divelab/DIG/tree/dig-stable/examples/sslgraph): [`InfoGraph`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_infograph.ipynb), [`GRACE`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_grace.ipynb), [`MVGRL`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_mvgrl.ipynb), [`GraphCL`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_graphcl.ipynb), [`LaGraph (v1 supported)`](https://github.com/divelab/DIG/tree/dig/examples/sslgraph/LaGraph).
+* [Explainability of Graph Neural Networks](https://github.com/divelab/DIG/tree/dig-stable/examples/xgraph): [`DeepLIFT`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/deeplift.ipynb), [`GNN-LRP`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/gnn_lrp.ipynb), [`FlowX`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/flowx.ipynb), [`GNNExplainer`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/gnnexplainer.ipynb), [`GradCAM`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/gradcam.ipynb), [`PGExplainer`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/pgexplainer.ipynb), [`SubgraphX`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/subgraphx.ipynb).
+* [Deep Learning on 3D Graphs](https://github.com/divelab/DIG/tree/dig-stable/examples/threedgraph): [`SchNet`](https://github.com/divelab/DIG/blob/dig-stable/examples/threedgraph/threedgraph.ipynb), [`DimeNet++`](https://github.com/divelab/DIG/blob/dig-stable/examples/threedgraph/threedgraph.ipynb), [`SphereNet`](https://github.com/divelab/DIG/blob/dig-stable/examples/threedgraph/threedgraph.ipynb).
+* [Graph OOD (GOOD) datasets](https://github.com/divelab/DIG/tree/dig-stable/examples/oodgraph): `GOODHIV`, `GOODPCBA`, `GOODZINC`, `GOODCMNIST`, `GOODMotif`, `GOODCora`, `GOODArxiv`, `GOODCBAS`.
 
 
 ## Installation
 
 ### Install from pip
 The key dependencies of DIG: Dive into Graphs are PyTorch (>=1.10.0), PyTorch Geometric (>=2.0.0), and RDKit.
 
@@ -193,12 +193,12 @@
 
 ## The Team
 
 *DIG: Dive into Graphs* is developed by [DIVE](https://github.com/divelab/)@TAMU. Contributors are Meng Liu*, Youzhi Luo*, Limei Wang*, Yaochen Xie*, Hao Yuan*, Shurui Gui*, Haiyang Yu*, Zhao Xu, Jingtun Zhang, Yi Liu, Keqiang Yan, Haoran Liu, Cong Fu, Bora Oztekin, Xuan Zhang, and Shuiwang Ji.
 
 ## Contact
 
-If you have any technical questions, please submit new issues.
+If you have any technical questions, please submit new issues or raise it in our [DIG slack community:fire:](https://join.slack.com/t/dive-into-graphs/shared_invite/zt-1i9kn731c-RhLA1zcEGHXbIToxdVqo0g).
 
 If you have any other questions, please contact us: Meng Liu [mengliu@tamu.edu] and Shuiwang Ji [sji@tamu.edu].
```

### Comparing `dive_into_graphs-1.0.0/README.md` & `dive_into_graphs-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,49 +17,49 @@
 [contributor-url]:https://github.com/divelab/DIG/graphs/contributors 
 [contributing-image]:https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
 [contributing-url]:https://diveintographs.readthedocs.io/en/latest/contribution/instruction.html
 
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Docs Status][docs-image]][docs-url]
-[![Build Status](https://travis-ci.com/divelab/DIG.svg?branch=dig)](https://travis-ci.com/divelab/DIG)
-[![codecov](https://codecov.io/gh/divelab/DIG/branch/dig/graph/badge.svg?token=KBJ1P31VCH)](https://codecov.io/gh/divelab/DIG)
+[![Build Status](https://travis-ci.com/divelab/DIG.svg?branch=dig-stable)](https://travis-ci.com/divelab/DIG)
+[![codecov](https://codecov.io/gh/divelab/DIG/branch/dig-stable/graph/badge.svg?token=KBJ1P31VCH)](https://codecov.io/gh/divelab/DIG)
 ![Last Commit](https://img.shields.io/github/last-commit/divelab/DIG)
 [![Contributing][contributing-image]][contributing-url]
 [![License][license-image]][license-url]
 ![visitors](https://visitor-badge.glitch.me/badge?page_id=jwenjian.visitor-badge)
 [![Downloads](https://pepy.tech/badge/dive-into-graphs)](https://pepy.tech/project/dive-into-graphs)
 <!--- [![Contributors][contributor-image]][contributor-url] -->
 
 
-**[Documentation](https://diveintographs.readthedocs.io)** | **[Paper [JMLR]](https://www.jmlr.org/papers/v22/21-0343.html)** | **[Tutorials](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html#)** | **[Benchmarks](https://github.com/divelab/DIG/tree/dig/benchmarks)** |  **[Examples](https://github.com/divelab/DIG/tree/dig/examples)**
+**[Documentation](https://diveintographs.readthedocs.io)** | **[Paper [JMLR]](https://www.jmlr.org/papers/v22/21-0343.html)** | **[Tutorials](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html#)** | **[Benchmarks](https://github.com/divelab/DIG/tree/dig-stable/benchmarks)** |  **[Examples](https://github.com/divelab/DIG/tree/dig-stable/examples)** | **[Join the DIG slack community now!:fire:](https://join.slack.com/t/dive-into-graphs/shared_invite/zt-1i9kn731c-RhLA1zcEGHXbIToxdVqo0g)**
 
 *DIG: Dive into Graphs* is a turnkey library for graph deep learning research.
 
 :fire:**Update (2022/07): We have upgraded our DIG library based on PyG 2.0.0. We recommend installing our latest version.**
 
 ## Why DIG?
 
-The key difference with current graph deep learning libraries, such as PyTorch Geometric (PyG) and Deep Graph Library (DGL), is that, while PyG and DGL support basic graph deep learning operations, DIG provides a unified testbed for higher level, research-oriented graph deep learning tasks, such as graph generation, self-supervised learning, explainability, and 3D graphs.
+The key difference with current graph deep learning libraries, such as PyTorch Geometric (PyG) and Deep Graph Library (DGL), is that, while PyG and DGL support basic graph deep learning operations, DIG provides a unified testbed for higher level, research-oriented graph deep learning tasks, such as graph generation, self-supervised learning, explainability, 3D graphs, and graph out-of-distribution.
 
 If you are working or plan to work on research in graph deep learning, DIG enables you to develop your own methods within our extensible framework, and compare with current baseline methods using common datasets and evaluation metrics without extra efforts.
 
 ## Overview
 
 It includes unified implementations of **data interfaces**, **common algorithms**, and **evaluation metrics** for several advanced tasks. Our goal is to enable researchers to easily implement and benchmark algorithms. Currently, we consider the following research directions.
 
 * **Graph Generation**: `dig.ggraph`
 * **Self-supervised Learning on Graphs**: `dig.sslgraph`
 * **Explainability of Graph Neural Networks**: `dig.xgraph`
 * **Deep Learning on 3D Graphs**: `dig.threedgraph`
-
+* **Graph OOD**: `dig.oodgraph`
 
 
 <p align="center">
-<img src="https://github.com/divelab/DIG/blob/dig/imgs/DIG-overview.png" width="700" class="center" alt="logo"/>
+<img src="https://github.com/divelab/DIG/blob/dig-stable/docs/imgs/DIG-overview.png" width="700" class="center" alt="logo"/>
     <br/>
 </p>
 
 
 ## Usage
 
 Example: a few lines of code to run [SphereNet](https://openreview.net/forum?id=givsRXsOt9r) on [QM9](https://www.nature.com/articles/sdata201422) to incorporate 3D information of molecules.
@@ -92,22 +92,22 @@
 run3d.run(device, train_dataset, valid_dataset, test_dataset, model, loss_func, evaluation,
           epochs=20, batch_size=32, vt_batch_size=32, lr=0.0005, lr_decay_factor=0.5, lr_decay_step_size=15)
 
 ```
 
 
 1. For details of all included APIs, please refer to the [documentation](https://diveintographs.readthedocs.io/). 
-2. We provide a hands-on tutorial for each direction to help you to get started with *DIG*: [Graph Generation](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html), [Self-supervised Learning on Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/sslgraph.html), [Explainability of Graph Neural Networks](https://diveintographs.readthedocs.io/en/latest/tutorials/subgraphx.html), and [Deep Learning on 3D Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/threedgraph.html).
-3. We also provide [examples](https://github.com/divelab/DIG/tree/dig/examples) to use APIs provided in *DIG*. You can get started with your interested directions by clicking the following links.
-
-* [Graph Generation](https://github.com/divelab/DIG/tree/dig/examples/ggraph): [`JT-VAE`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/JTVAE), [`GraphAF`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/GraphAF), [`GraphDF`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/GraphDF), [`GraphEBM`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/GraphEBM).
-* [Self-supervised Learning on Graphs](https://github.com/divelab/DIG/tree/dig/examples/sslgraph): [`InfoGraph`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_infograph.ipynb), [`GRACE`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_grace.ipynb), [`MVGRL`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_mvgrl.ipynb), [`GraphCL`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_graphcl.ipynb).
-* [Explainability of Graph Neural Networks](https://github.com/divelab/DIG/tree/dig/examples/xgraph): [`DeepLIFT`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/deeplift.ipynb), [`GNN-LRP`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/gnn_lrp.ipynb), [`GNNExplainer`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/gnnexplainer.ipynb), [`GradCAM`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/gradcam.ipynb), [`PGExplainer`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/pgexplainer.ipynb), [`SubgraphX`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/subgraphx.ipynb).
-* [Deep Learning on 3D Graphs](https://github.com/divelab/DIG/tree/dig/examples/threedgraph): [`SchNet`](https://github.com/divelab/DIG/blob/dig/examples/threedgraph/threedgraph.ipynb), [`DimeNet++`](https://github.com/divelab/DIG/blob/dig/examples/threedgraph/threedgraph.ipynb), [`SphereNet`](https://github.com/divelab/DIG/blob/dig/examples/threedgraph/threedgraph.ipynb).
+2. We provide a hands-on tutorial for each direction to help you to get started with *DIG*: [Graph Generation](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html), [Self-supervised Learning on Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/sslgraph.html), [Explainability of Graph Neural Networks](https://diveintographs.readthedocs.io/en/latest/tutorials/subgraphx.html), [Deep Learning on 3D Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/threedgraph.html), [Graph OOD (GOOD) datasets](https://diveintographs.readthedocs.io/en/latest/tutorials/oodgraph.html).
+3. We also provide [examples](https://github.com/divelab/DIG/tree/dig-stable/examples) to use APIs provided in *DIG*. You can get started with your interested directions by clicking the following links.
 
+* [Graph Generation](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph): [`JT-VAE`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/JTVAE), [`GraphAF`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphAF), [`GraphDF`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphDF), [`GraphEBM`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphEBM).
+* [Self-supervised Learning on Graphs](https://github.com/divelab/DIG/tree/dig-stable/examples/sslgraph): [`InfoGraph`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_infograph.ipynb), [`GRACE`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_grace.ipynb), [`MVGRL`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_mvgrl.ipynb), [`GraphCL`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_graphcl.ipynb), [`LaGraph (v1 supported)`](https://github.com/divelab/DIG/tree/dig/examples/sslgraph/LaGraph).
+* [Explainability of Graph Neural Networks](https://github.com/divelab/DIG/tree/dig-stable/examples/xgraph): [`DeepLIFT`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/deeplift.ipynb), [`GNN-LRP`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/gnn_lrp.ipynb), [`FlowX`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/flowx.ipynb), [`GNNExplainer`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/gnnexplainer.ipynb), [`GradCAM`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/gradcam.ipynb), [`PGExplainer`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/pgexplainer.ipynb), [`SubgraphX`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/subgraphx.ipynb).
+* [Deep Learning on 3D Graphs](https://github.com/divelab/DIG/tree/dig-stable/examples/threedgraph): [`SchNet`](https://github.com/divelab/DIG/blob/dig-stable/examples/threedgraph/threedgraph.ipynb), [`DimeNet++`](https://github.com/divelab/DIG/blob/dig-stable/examples/threedgraph/threedgraph.ipynb), [`SphereNet`](https://github.com/divelab/DIG/blob/dig-stable/examples/threedgraph/threedgraph.ipynb).
+* [Graph OOD (GOOD) datasets](https://github.com/divelab/DIG/tree/dig-stable/examples/oodgraph): `GOODHIV`, `GOODPCBA`, `GOODZINC`, `GOODCMNIST`, `GOODMotif`, `GOODCora`, `GOODArxiv`, `GOODCBAS`.
 
 
 ## Installation
 
 ### Install from pip
 The key dependencies of DIG: Dive into Graphs are PyTorch (>=1.10.0), PyTorch Geometric (>=2.0.0), and RDKit.
 
@@ -176,12 +176,12 @@
 
 ## The Team
 
 *DIG: Dive into Graphs* is developed by [DIVE](https://github.com/divelab/)@TAMU. Contributors are Meng Liu*, Youzhi Luo*, Limei Wang*, Yaochen Xie*, Hao Yuan*, Shurui Gui*, Haiyang Yu*, Zhao Xu, Jingtun Zhang, Yi Liu, Keqiang Yan, Haoran Liu, Cong Fu, Bora Oztekin, Xuan Zhang, and Shuiwang Ji.
 
 ## Contact
 
-If you have any technical questions, please submit new issues.
+If you have any technical questions, please submit new issues or raise it in our [DIG slack community:fire:](https://join.slack.com/t/dive-into-graphs/shared_invite/zt-1i9kn731c-RhLA1zcEGHXbIToxdVqo0g).
 
 If you have any other questions, please contact us: Meng Liu [mengliu@tamu.edu] and Shuiwang Ji [sji@tamu.edu].
```

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/dataset/PygDataset.py` & `dive_into_graphs-1.1.0/dig/ggraph/dataset/PygDataset.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/dataset/config.csv` & `dive_into_graphs-1.1.0/dig/ggraph/dataset/config.csv`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/dataset/ggraph_dataset.py` & `dive_into_graphs-1.1.0/dig/ggraph/dataset/ggraph_dataset.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/evaluation/metric.py` & `dive_into_graphs-1.1.0/dig/ggraph/evaluation/metric.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/graphaf.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/graphaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .model import GraphFlowModel, GraphFlowModel_rl, GraphFlowModel_con_rl
 from .train_utils import adjust_learning_rate, DataIterator
 
 
 class GraphAF(Generator):
     r"""
         The method class for GraphAF algorithm proposed in the paper `GraphAF: a Flow-based Autoregressive Model for Molecular Graph Generation <https://arxiv.org/abs/2001.09382>`_. This class provides interfaces for running random generation, property
-        optimization, and constrained optimization with GraphAF. Please refer to the `benchmark codes <https://github.com/divelab/DIG/tree/dig/benchmarks/ggraph/GraphAF>`_ for usage examples.
+        optimization, and constrained optimization with GraphAF. Please refer to the `example codes <https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphAF>`_ for usage examples.
     """
     def __init__(self):
         super(GraphAF, self).__init__()
         self.model = None
     
 
     def get_model(self, task, model_conf_dict, checkpoint_path=None):
```

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/graphaf.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/graphaf.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/graphflow.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/graphflow.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/graphflow_con_rl.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/graphflow_con_rl.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/graphflow_rl.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/graphflow_rl.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/model_utils.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/model_utils.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/rgcn.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/rgcn.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/model/st_net.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/model/st_net.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphAF/train_utils.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphAF/train_utils.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/graphdf.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/graphdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .model import GraphFlowModel, GraphFlowModel_rl, GraphFlowModel_con_rl
 from .train_utils import adjust_learning_rate, DataIterator
 
 
 class GraphDF(Generator):
     r"""
         The method class for GraphDF algorithm proposed in the paper `GraphDF: A Discrete Flow Model for Molecular Graph Generation <https://arxiv.org/abs/2102.01189>`_. This class provides interfaces for running random generation, property
-        optimization, and constrained optimization with GraphDF algorithm. Please refer to the `benchmark codes <https://github.com/divelab/DIG/tree/dig/benchmarks/ggraph/GraphDF>`_ for usage examples.
+        optimization, and constrained optimization with GraphDF algorithm. Please refer to the `example codes <https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphDF>`_ for usage examples.
     """
 
     def __init__(self):
         super(GraphDF, self).__init__()
         self.model = None
```

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/df_utils.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/df_utils.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/disgraphaf.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/disgraphaf.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/graphflow.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/graphflow.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/graphflow_con_rl.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/graphflow_con_rl.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/graphflow_rl.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/graphflow_rl.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/rgcn.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/rgcn.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/model/st_net.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/model/st_net.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphDF/train_utils.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphDF/train_utils.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphEBM/energy_func.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphEBM/energy_func.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphEBM/graphebm.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphEBM/graphebm.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .energy_func import EnergyFunc
 from .util import rescale_adj, requires_grad, clip_grad
 
 
 class GraphEBM(Generator):
     r"""
         The method class for GraphEBM algorithm proposed in the paper `GraphEBM: Molecular Graph Generation with Energy-Based Models <https://arxiv.org/abs/2102.00546>`_. This class provides interfaces for running random generation, goal-directed generation (including property
-        optimization and constrained optimization), and compositional generation with GraphEBM algorithm. Please refer to the `benchmark codes <https://github.com/divelab/DIG/tree/dig/benchmarks/ggraph/GraphEBM>`_ for usage examples.
+        optimization and constrained optimization), and compositional generation with GraphEBM algorithm. Please refer to the `example codes <https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphEBM>`_ for usage examples.
         
         Args:
             n_atom (int): Maximum number of atoms.
             n_atom_type (int): Number of possible atom types.
             n_edge_type (int): Number of possible bond types.
             hidden (int): Hidden dimensions.
             device (torch.device, optional): The device where the model is deployed.
```

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/GraphEBM/util.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/GraphEBM/util.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/chemutils.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/chemutils.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/datautils.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/datautils.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtmpn.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtmpn.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtmpn_bo.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtmpn_bo.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_dec.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_dec.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_enc.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_enc.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_enc_bo.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_enc_bo.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_vae.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_vae.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_vae_bo.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtnn_vae_bo.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/jtprop_vae.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/jtprop_vae.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/mol_tree.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/mol_tree.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/mpn.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/mpn.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/nnutils.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/nnutils.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/sascorer.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/sascorer.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/fast_jtnn/vocab.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/fast_jtnn/vocab.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/JTVAE/jtvae.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/JTVAE/jtvae.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from dig.ggraph.method import Generator
 
 from . import fast_jtnn
 
 
 class JTVAE(Generator):
     r"""
-    The method class for the JTVAE algorithm proposed in the paper `Junction Tree Variational Autoencoder for Molecular Graph Generation <https://arxiv.org/abs/1802.04364>`_. This class provides interfaces for running random generation with the JTVAE algorithm. Please refer to the `benchmark codes <https://github.com/divelab/DIG/tree/dig/benchmarks/ggraph/JTVAE>`_ for usage examples.
+    The method class for the JTVAE algorithm proposed in the paper `Junction Tree Variational Autoencoder for Molecular Graph Generation <https://arxiv.org/abs/1802.04364>`_. This class provides interfaces for running random generation with the JTVAE algorithm. Please refer to the `example codes <https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/JTVAE>`_ for usage examples.
 
     Args:
         list_smiles (list): List of smiles in training data.
         training (boolean): If we are training (as opposed to testing).
         build_vocab (boolean): If we need to build the vocabulary (first time training with this dataset).
         device (torch.device, optional): The device where the model is deployed.
     """
```

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/method/generator.py` & `dive_into_graphs-1.1.0/dig/ggraph/method/generator.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/utils/__init__.py` & `dive_into_graphs-1.1.0/dig/ggraph/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/utils/environment.py` & `dive_into_graphs-1.1.0/dig/ggraph/utils/environment.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/utils/fpscores.pkl.gz` & `dive_into_graphs-1.1.0/dig/ggraph/utils/fpscores.pkl.gz`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/utils/gen_mol_from_one_shot_tensor.py` & `dive_into_graphs-1.1.0/dig/ggraph/utils/gen_mol_from_one_shot_tensor.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph/utils/sascorer.py` & `dive_into_graphs-1.1.0/dig/ggraph/utils/sascorer.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph3D/dataset/ggraph3D_dataset.py` & `dive_into_graphs-1.1.0/dig/ggraph3D/dataset/ggraph3D_dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 
 
 atomic_num_to_type={1:0, 6:1, 7:2, 8:3, 9:4}
 bond_to_type = {BondType.SINGLE: 1, BondType.DOUBLE: 2, BondType.TRIPLE: 3}
 
 
 def collate_fn(data_batch_list):
+    r"""
+        The collate function used to form a mini-batch of data when creating data loaders with the dataset class dig.ggraph3D.dataset.QM93DGEN.
+
+        Args:
+            data_batch_list: a list of python dict returned from the get function of dig.ggraph3D.dataset.QM93DGEN.
+        :rtype: :class:`dict` a python dict with the same keys as every python dict in data_batch_list.
+    """
     data_batch = {}
 
     for key in ['atom_type', 'position', 'new_atom_type', 'new_dist', 'new_angle', 'new_torsion', 'cannot_focus']:
         data_batch[key] = torch.cat([mol_dict[key] for mol_dict in data_batch_list], dim=0)
     
     num_steps_list = torch.tensor([0]+[len(data_batch_list[i]['new_atom_type']) for i in range(len(data_batch_list)-1)])
     batch_idx_offsets = torch.cumsum(num_steps_list, dim=0)
@@ -36,14 +43,38 @@
         atom_offseted = torch.cat([mol_dict[key] for mol_dict in data_batch_list], dim=0) + atom_idx_repeated_offsets[:,None]
         data_batch[key] = atom_offseted
 
     return data_batch
 
 
 class QM93DGEN(InMemoryDataset):
+    r"""
+        A `Pytorch Geometric <https://pytorch-geometric.readthedocs.io/en/latest/index.html>`_ data interface for datasets used in molecule generation.
+        
+        .. note::
+            When creating data loaders of this dataset class, only dig.ggraph3D.dataset.collate_fn can be used as the collate function.
+        
+        Args:
+            root (string, optional): Root directory where the dataset should be saved. (default: :obj:`./`)
+            subset_idxs (list, optional): if it is not None, only the data located 
+                at the indexs in subset_idxs of the dataset will be sampled.
+                (default: :obj:`None`)
+            transform (callable, optional): A function/transform that takes in an
+                :obj:`torch_geometric.data.Data` object and returns a transformed
+                version. The data object will be transformed before every access.
+                (default: :obj:`None`)
+            pre_transform (callable, optional): A function/transform that takes in
+                an :obj:`torch_geometric.data.Data` object and returns a
+                transformed version. The data object will be transformed before
+                being saved to disk. (default: :obj:`None`)
+            pre_filter (callable, optional): A function that takes in an
+                :obj:`torch_geometric.data.Data` object and returns a boolean
+                value, indicating whether the data object should be included in the
+                final dataset. (default: :obj:`None`)
+    """
     raw_url = "https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/gdb9.tar.gz"
     split_urls = [
         "https://github.com/divelab/DIG_storage/raw/main/ggraph3D/data/split.npz",
         "https://github.com/divelab/DIG_storage/raw/main/ggraph3D/data/alpha.npz",
         "https://github.com/divelab/DIG_storage/raw/main/ggraph3D/data/gap.npz"
     ]
     
@@ -84,14 +115,17 @@
         os.unlink(path)
         
         for split_url in self.split_urls:
             download_url(split_url, self.raw_dir)
     
 
     def process(self):
+        r"""
+            Processes the dataset from raw data file to the :obj:`self.processed_dir` folder.
+        """
         mols = Chem.SDMolSupplier(self.raw_paths[0], removeHs=False, sanitize=False)
         self.atom_type_list, self.position_list, self.con_mat_list = [], [], []
 
         for idx in range(len(mols)):
             mol = mols[idx]
             num_atoms = mol.GetNumAtoms()
             position = mols.GetItemText(idx).split('\n')[4:4+num_atoms]
@@ -119,18 +153,29 @@
             self.position_list.append(torch.tensor(position))
             self.con_mat_list.append(torch.tensor(con_mat))
         
         torch.save((self.atom_type_list, self.position_list, self.con_mat_list), self.processed_paths[0])
     
     
     def len(self):
+        r"""
+            Gets the number of molecular geometries that can be sampled in total.
+        """
         return len(self._indices)
     
 
     def get_idx_split(self, task):
+        r"""Gets the train-valid set split indices of the dataset for different tasks.
+        
+        Args:
+            task: The name of the task that the dataset will be used in, including 'rand_gen' for random molecular geometry generation, 
+                'gap_opt' for discovering molecular geometries with low HOMO-LUMO gaps, and 'alpha_opt' for discovering molecular geometries 
+                with high isotropic polarizabilities.
+        :rtype: A dictionary for training-validation split with key :obj:`train` and :obj:`valid`.
+        """
         assert task in ['rand_gen', 'gap_opt', 'alpha_opt']
         if task == 'rand_gen':
             split_idxs = np.load(osp.join(self.raw_dir, 'split.npz'))
         elif task == 'gap_opt':
             split_idxs = np.load(osp.join(self.raw_dir, 'gap.npz'))
         elif task == 'alpha_opt':
             split_idxs = np.load(osp.join(self.raw_dir, 'alpha.npz'))
@@ -141,14 +186,31 @@
             'train': split_idxs['train_idx'].tolist(), 
             'valid': split_idxs['val_idx'].tolist()
         }
         return split_dict
 
 
     def get(self, idx):
+        r"""Gets the data object at index :idx:.
+        
+        Args:
+            idx: The index of the data that you want to reach.
+        :rtype: :class:`dict` a python dict with the following items:
+                    "atom_type" --- the atom types of previously generated geometries at each generation step;
+                    "position" --- the atom coordinates of previously generated geometries at each generation step;
+                    "batch" --- the identity indexes used to discriminate different generation step;
+                    "focus" --- the index of focus atom at each generation step;
+                    "c1_focus" --- the index of c1 and focus atom at each generation step;
+                    "c2_c1_focus" --- the index of c2, c1, and focus atom at each generation step;
+                    "new_atom_type" --- the atom types to be generated at each generation step;
+                    "new_dist" --- the distances to be generated at each generation step;
+                    "new_angle" --- the angles to be generated at each generation step;
+                    "new_torsion" --- the torsion angles to be generated at each generation step;
+                    "cannot_focus" --- the labels denoting whether each atom can serve as the focus atom or not in the previously generated geometries at each generation step.
+        """
         atom_type, position, con_mat = self.atom_type_list[idx], self.position_list[idx], self.con_mat_list[idx]
         atom_valency = torch.sum(con_mat, dim=1)
 
         squared_dist = torch.sum(torch.square(position[:,None,:] - position[None,:,:]), dim=-1)      
         nx_graph = nx.from_numpy_matrix(squared_dist.numpy())
         edges = list(tree.minimum_spanning_edges(nx_graph, algorithm='prim', data=False))
```

### Comparing `dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/att.py` & `dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/att.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/features.py` & `dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/features.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/geometric_computing.py` & `dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/geometric_computing.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/net_utils.py` & `dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/net_utils.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/spherenet.py` & `dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/spherenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import torch
 from torch import nn
 from torch.nn import Linear, Embedding
-from torch_geometric.nn.acts import swish
 from torch_geometric.nn.inits import glorot_orthogonal
 from torch_geometric.nn import radius_graph
 from torch_scatter import scatter
 import torch.nn.functional as F
 from math import sqrt
 
 from .geometric_computing import xyztodat
@@ -14,14 +13,17 @@
 try:
     import sympy as sym
 except ImportError:
     sym = None
 
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
+def swish(x):
+    return x * torch.sigmoid(x)
+
 class emb(torch.nn.Module):
     def __init__(self, num_spherical, num_radial, cutoff, envelope_exponent):
         super(emb, self).__init__()
         self.dist_emb = dist_emb(num_radial, cutoff, envelope_exponent)
         self.angle_emb = angle_emb(num_spherical, num_radial, cutoff, envelope_exponent)
         self.torsion_emb = torsion_emb(num_spherical, num_radial, cutoff, envelope_exponent)
         self.reset_parameters()
```

### Comparing `dive_into_graphs-1.0.0/dig/ggraph3D/method/G_SphereNet/model/sphgen.py` & `dive_into_graphs-1.1.0/dig/ggraph3D/method/G_SphereNet/model/sphgen.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/ggraph3D/utils/eval_prop_utils.py` & `dive_into_graphs-1.1.0/dig/ggraph3D/utils/eval_prop_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -36,14 +36,25 @@
 
     polar = mf.Polarizability().polarizability()
     xx, yy, zz = polar.diagonal()
     return (xx + yy + zz) / 3
 
 
 def compute_prop(atomic_number, position, prop_name):
+    """
+    Calculate the quantum property score of the given molecular geometry with `PySCF <https://pyscf.org/index.html>`_.
+
+    Args:
+        atomic_number (numpy array): the numpy array indicating the atomic number of atoms in the molecular geometry.
+        position (numpy array): the numpy array indicating the coordinates of atoms in the molecular geometry.
+        prop_name (string): the name of quantum property, 'gap' for HOMO-LUMO gap, 'alpha' for isotropic polarizability.
+    
+    :rtype:
+        :class:`float`
+    """
     ptb = Chem.GetPeriodicTable()
     geom = [[ptb.GetElementSymbol(int(z)), position[i]] for i, z in enumerate(atomic_number)]
 
     if prop_name == 'gap':
         prop = geom2gap(geom)
     elif prop_name == 'alpha':
         prop = geom2alpha(geom)
```

### Comparing `dive_into_graphs-1.0.0/dig/ggraph3D/utils/eval_validity_utils.py` & `dive_into_graphs-1.1.0/dig/ggraph3D/utils/eval_validity_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -377,29 +377,25 @@
         return True
     except:
         return False
 
 
 def xyz2mol(atoms, coordinates, use_graph=True):
     """
-    Generate a rdkit molobj from atoms, coordinates and a total_charge.
+    Convert the given molecular geometry to a 2D molecular graph and check if it is chemically valid through valency check with the algorithm 
+    in `this paper <https://onlinelibrary.wiley.com/doi/abs/10.1002/bkcs.10334>`_.
 
-    args:
-        atoms - list of atom types (int)
-        coordinates - 3xN Cartesian coordinates
-        charge - total charge of the system (default: 0)
-
-    optional:
-        allow_charged_fragments - alternatively radicals are made
-        use_graph - use graph (networkx)
-        use_huckel - Use Huckel method for atom connectivity prediction
-        embed_chiral - embed chiral information to the molecule
-
-    returns:
-        mols - list of rdkit molobjects
+    Args:
+        atoms (numpy array): the numpy array indicating the atomic number of atoms in the molecular geometry.
+        coordinates (numpy array): the numpy array indicating the coordinates of atoms in the molecular geometry.
+        use_graph (bool): whether use networkx to compute the maximum-weighted matching of the graph or not. (default: :obj:`True`)
+    
+    :rtype:
+        BO: bond order matrix.
+        valid: a bool value denoting whether the molecular geometry is valid or not.
 
     """
 
     # Get atom connectivity (AC) matrix, list of atomic numbers, molecular charge,
     # and mol object with no connectivity information
     AC = xyz2AC_vdW(atoms, coordinates)
```

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/dataset/TUDataset.py` & `dive_into_graphs-1.1.0/dig/sslgraph/dataset/TUDataset.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/dataset/datasets.py` & `dive_into_graphs-1.1.0/dig/sslgraph/dataset/datasets.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/dataset/feat_expansion.py` & `dive_into_graphs-1.1.0/dig/sslgraph/dataset/feat_expansion.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/evaluation/eval_graph.py` & `dive_into_graphs-1.1.0/dig/sslgraph/evaluation/eval_graph.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/evaluation/eval_node.py` & `dive_into_graphs-1.1.0/dig/sslgraph/evaluation/eval_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def weights_init(self, m):
         if isinstance(m, nn.Linear):
             torch.nn.init.xavier_uniform_(m.weight.data)
             if m.bias is not None:
                 m.bias.data.fill_(0.0)
 
     def forward(self, seq):
-        ret = torch.log_softmax(self.fc(seq), dim=-1)
+        ret = self.fc(seq)
         return ret
 
 
 class NodeUnsupervised(object):
     r"""
     The evaluation interface for unsupervised graph representation learning evaluated with 
     linear classification. You can refer to `the benchmark code
```

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/contrastive.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/contrastive.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/grace.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/grace.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/graphcl.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/graphcl.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/infograph.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/infograph.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/model/mvgrl.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/model/mvgrl.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/objectives/infonce.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/objectives/infonce.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,21 +25,23 @@
     else:
         tau = 0.5
     
     if 'norm' in kwargs:
         norm = kwargs['norm']
     else:
         norm = True
+    
+    mean = kwargs['mean'] if 'mean' in kwargs else True
         
     if zs_n is not None:
         if zs is None:
             # InfoNCE in GRACE
             assert len(zs_n)==2
-            return (infoNCE_local_intra_node(zs_n[0], zs_n[1], tau, norm)+
-                    infoNCE_local_intra_node(zs_n[1], zs_n[0], tau, norm))*0.5
+            return (infoNCE_local_intra_node(zs_n[0], zs_n[1], tau, norm, batch)+
+                    infoNCE_local_intra_node(zs_n[1], zs_n[0], tau, norm, batch))*0.5
         else:
             assert len(zs_n)==len(zs)
             assert batch is not None
             
             if len(zs)==1:
                 return infoNCE_local_global(zs[0], zs_n[0], batch, tau, norm)
             elif len(zs)==2:
@@ -61,28 +63,47 @@
         loss = 0
         for (i, j) in itertools.combinations(range(len(zs)), 2):
             if sigma[i][j]:
                 loss += NT_Xent(zs[i], zs[j], tau, norm)
         return loss
 
     
-def infoNCE_local_intra_node(z1_n, z2_n, tau=0.5, norm=True):
+def infoNCE_local_intra_node(z1_n, z2_n, tau=0.5, norm=True, batch=None):
     '''
     Args:
         z1_n: Tensor of shape [n_nodes, z_dim].
         z2_n: Tensor of shape [n_nodes, z_dim].
         tau: Float. Usually in (0,1].
         norm: Boolean. Whether to apply normlization.
+        batch: Tensor of shape [batch_size]
     '''
-    if norm:
-        z1_n = F.normalize(z1_n)
-        z2_n = F.normalize(z2_n)
+    def sim(z1:torch.Tensor, z2:torch.Tensor):
+            if norm:
+                z1 = F.normalize(z1)
+                z2 = F.normalize(z2)
+            return torch.mm(z1, z2.t())
+    
     exp = lambda x: torch.exp(x / tau)
-    refl_sim = exp(torch.mm(z1_n, z1_n.t()))
-    between_sim = exp(torch.mm(z1_n, z2_n.t()))
+    if batch is not None:
+        batch_size = batch.size(0)
+        num_nodes = z1_n.size(0)
+        indices = torch.arange(0, num_nodes).to(z1_n.device)
+        losses = []
+        for i in range(0, num_nodes, batch_size):
+            mask = indices[i:i+batch_size]
+            refl_sim = exp(sim(z1_n[mask], z1_n))
+            between_sim = exp(sim(z1_n[mask], z2_n))
+            losses.append(-torch.log(between_sim[:, i:i+batch_size].diag()
+                            / (refl_sim.sum(1) + between_sim.sum(1)
+                            - refl_sim[:, i:i+batch_size].diag())))
+        losses = torch.cat(losses)
+        return losses.mean()
+
+    refl_sim = exp(sim(z1_n, z1_n))
+    between_sim = exp(sim(z1_n, z2_n))
     
     pos_sim = between_sim.diag()
     intra_sim = refl_sim.sum(1) - refl_sim.diag()
     inter_pos_sim = between_sim.sum(1)
     
     loss = pos_sim / (intra_sim + inter_pos_sim)
     loss = -torch.log(loss).mean()
```

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/objectives/jse.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/objectives/jse.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/views_fn/combination.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/views_fn/combination.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/views_fn/sample.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/views_fn/sample.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/method/contrastive/views_fn/structure.py` & `dive_into_graphs-1.1.0/dig/sslgraph/method/contrastive/views_fn/structure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
-from torch_geometric.utils import to_dense_adj, dense_to_sparse, dropout_adj
+from torch_geometric.utils import to_dense_adj, dense_to_sparse, dropout_adj, degree, add_remaining_self_loops
 from sklearn.preprocessing import MinMaxScaler
 from torch_geometric.data import Batch, Data
-
+from dig.sslgraph.utils.adaptive import degree_drop_weights, pr_drop_weights, evc_drop_weights, drop_edge_weighted
 
 class EdgePerturbation():
     '''Edge perturbation on the given graph or batched graphs. Class objects callable via 
     method :meth:`views_fn`.
     
     Args:
         add (bool, optional): Set :obj:`True` if randomly add edges in a given graph.
@@ -51,15 +51,65 @@
         """
         if isinstance(data, Batch):
             dlist = [self.do_trans(d) for d in data.to_data_list()]
             return Batch.from_data_list(dlist)
         elif isinstance(data, Data):
             return self.do_trans(data)
 
-
+class AdaEdgePerturbation():
+    '''Proabilistic edge perturbation on the given graph or batched graphs. Perturbations are adaptive i.e. critical edges have lower probability of being removed.
+    Adaptations based on the paper `Graph Contrastive Learning with Adaptive Augmentation <https://arxiv.org/abs/2010.14945>`
+    Refer to `source implementation <https://github.com/CRIPAC-DIG/GCA>` for more details.
+    Class objects callable via method :meth:`views_fn`.
+    
+    Args:
+        centrality_measure (str): Method for computing edge centrality. Set `degree` for degree centrality,
+        `pr` for PageRank centrality and `evc` for eigen-vector centrality
+        prob (float): Probability factor used for calculating edge-drop probability
+        threshold (float): Upper-bound probability for dropping any edge, defaults to 0.7
+    '''
+    def __init__(self, centrality_measure : str, prob : float, threshold : float):
+        self.centrality_measure = centrality_measure
+        self.prob = prob
+        self.threshold = threshold
+    def __call__(self, data):
+        return self.views_fn(data)
+    def do_trans(self, data):
+        if self.centrality_measure not in ['degree', 'pr', 'evc']:
+            raise ValueError("Invalid drop scheme {}".format(self.centrality_measure))
+        drop_weights = self._get_edge_weights(data)
+        new_edge_index = drop_edge_weighted(data.edge_index, drop_weights, p=self.prob, threshold=self.threshold)
+        return Data(x=data.x, edge_index=new_edge_index)
+        
+    def _get_edge_weights(self, data):
+        # Add self loops if the degree returns for only a subset of nodes
+        if degree(data.edge_index[1]).size(0) != data.x.size(0):
+            edge_index_ = add_remaining_self_loops(data.edge_index, num_nodes=data.x.size(0))[0]
+        else:
+            edge_index_ = data.edge_index
+        if self.centrality_measure == 'degree':
+            drop_weights = degree_drop_weights(edge_index_)
+        elif self.centrality_measure == 'pr':
+            drop_weights = pr_drop_weights(edge_index_, aggr='sink', k=200)
+        elif self.centrality_measure == 'evc':
+            drop_weights = evc_drop_weights(data)
+        return drop_weights
+    def views_fn(self, data):
+        r"""Method to be called when :class:`AdaEdgePerturbation` object is called.
+        
+        Args:
+            data (:class:`torch_geometric.data.Data`): The input graph or batched graphs.
+            
+        :rtype: :class:`torch_geometric.data.Data`.  
+        """
+        if isinstance(data, Batch):
+            dlist = [self.do_trans(d) for d in data.to_data_list()]
+            return Batch.from_data_list(dlist)
+        elif isinstance(data, Data):
+            return self.do_trans(data)
 
 class Diffusion():
     '''Diffusion on the given graph or batched graphs, used in 
     `MVGRL <https://arxiv.org/pdf/2006.05582v1.pdf>`_. Class objects callable via 
     method :meth:`views_fn`.
     
     Args:
@@ -194,15 +244,15 @@
             scaler.fit(diff_adj)
             diff_adj = torch.tensor(scaler.transform(diff_adj), device=data.x.device)
 
         dlist_orig_x = []
         dlist_diff_x = []
         drop_num = node_num - self.sample_size
         for b in range(self.batch_size):
-            idx_drop = torch.randperm(node_num, device=x.device)[:drop_num]
+            idx_drop = torch.randperm(node_num, device=data.x.device)[:drop_num]
             idx_nondrop = [n for n in range(node_num) if not n in idx_drop]
 
             sample_orig_adj = orig_adj.clone()
             sample_orig_adj = sample_orig_adj[idx_nondrop, :][:, idx_nondrop]
 
             sample_diff_adj = diff_adj.clone()
             sample_diff_adj = sample_diff_adj[idx_nondrop, :][:, idx_nondrop]
@@ -213,8 +263,8 @@
 
             dlist_orig_x.append(Data(x=sample_orig_x, 
                                      edge_index=dense_to_sparse(sample_orig_adj)[0]))
             dlist_diff_x.append(Data(x=sample_orig_x, 
                                      edge_index=edge_ind, 
                                      edge_attr=edge_attr))
 
-        return Batch.from_data_list(dlist_orig_x), Batch.from_data_list(dlist_diff_x)
+        return Batch.from_data_list(dlist_orig_x), Batch.from_data_list(dlist_diff_x)
```

### Comparing `dive_into_graphs-1.0.0/dig/sslgraph/utils/encoders.py` & `dive_into_graphs-1.1.0/dig/sslgraph/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/dataset/PygMD17.py` & `dive_into_graphs-1.1.0/dig/threedgraph/dataset/PygMD17.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 value, indicating whether the data object should be included in the
                 final dataset. (default: :obj:`None`)
 
         Example:
         --------
 
         >>> dataset = MD17(name='aspirin')
-        >>> split_idx = dataset.get_idx_split(len(dataset.data.y), train_size=1000, valid_size=10000, seed=42)
+        >>> split_idx = dataset.get_idx_split(len(dataset.data.y), train_size=1000, valid_size=1000, seed=42)
         >>> train_dataset, valid_dataset, test_dataset = dataset[split_idx['train']], dataset[split_idx['valid']], dataset[split_idx['test']]
         >>> train_loader = DataLoader(train_dataset, batch_size=32, shuffle=True)
         >>> data = next(iter(train_loader))
         >>> data
         Batch(batch=[672], force=[672, 3], pos=[672, 3], ptr=[33], y=[32], z=[672])
 
         Where the attributes of the output data indicates:
@@ -111,14 +111,14 @@
 if __name__ == '__main__':
     dataset = MD17(name='aspirin')
     print(dataset)
     print(dataset.data.z.shape)
     print(dataset.data.pos.shape)
     print(dataset.data.y.shape)
     print(dataset.data.force.shape)
-    split_idx = dataset.get_idx_split(len(dataset.data.y), train_size=1000, valid_size=10000, seed=42)
+    split_idx = dataset.get_idx_split(len(dataset.data.y), train_size=1000, valid_size=1000, seed=42)
     print(split_idx)
     print(dataset[split_idx['train']])
     train_dataset, valid_dataset, test_dataset = dataset[split_idx['train']], dataset[split_idx['valid']], dataset[split_idx['test']]
     train_loader = DataLoader(train_dataset, batch_size=32, shuffle=True)
     data = next(iter(train_loader))
     print(data)
```

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/dataset/PygQM93D.py` & `dive_into_graphs-1.1.0/dig/threedgraph/dataset/PygQM93D.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/evaluation/eval.py` & `dive_into_graphs-1.1.0/dig/threedgraph/evaluation/eval.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/method/comenet/comenet.py` & `dive_into_graphs-1.1.0/dig/threedgraph/method/comenet/comenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from torch_cluster import radius_graph
 from torch_geometric.nn import GraphConv, GraphNorm
-from torch_geometric.nn.acts import swish
 from torch_geometric.nn import inits
 
 from .features import angle_emb, torsion_emb
 
 from torch_scatter import scatter, scatter_min
 
 from torch.nn import Embedding
@@ -20,14 +19,16 @@
 try:
     import sympy as sym
 except ImportError:
     sym = None
 
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
+def swish(x):
+    return x * torch.sigmoid(x)
 
 class Linear(torch.nn.Module):
 
     def __init__(self, in_channels, out_channels, bias=True,
                  weight_initializer='glorot',
                  bias_initializer='zeros'):
         super().__init__()
@@ -132,20 +133,20 @@
         return x_j if edge_weight is None else edge_weight * x_j
 
 
 class SimpleInteractionBlock(torch.nn.Module):
     def __init__(
             self,
             hidden_channels,
+            middle_channels,
             num_radial,
             num_spherical,
             num_layers,
             output_channels,
-            act=swish,
-            inits='glorot',
+            act=swish
     ):
         super(SimpleInteractionBlock, self).__init__()
         self.act = act
 
         self.conv1 = EdgeGraphConv(hidden_channels, hidden_channels)
 
         self.conv2 = EdgeGraphConv(hidden_channels, hidden_channels)
@@ -155,23 +156,23 @@
         self.lin2 = Linear(hidden_channels, hidden_channels)
 
         self.lin_cat = Linear(2 * hidden_channels, hidden_channels)
 
         self.norm = GraphNorm(hidden_channels)
 
         # Transformations of Bessel and spherical basis representations.
-        self.lin_feature1 = TwoLayerLinear(num_radial * num_spherical ** 2, hidden_channels, hidden_channels)
-        self.lin_feature2 = TwoLayerLinear(num_radial * num_spherical, hidden_channels, hidden_channels)
+        self.lin_feature1 = TwoLayerLinear(num_radial * num_spherical ** 2, middle_channels, hidden_channels)
+        self.lin_feature2 = TwoLayerLinear(num_radial * num_spherical, middle_channels, hidden_channels)
 
         # Dense transformations of input messages.
         self.lin = Linear(hidden_channels, hidden_channels)
         self.lins = torch.nn.ModuleList()
         for _ in range(num_layers):
             self.lins.append(Linear(hidden_channels, hidden_channels))
-        self.final = Linear(hidden_channels, output_channels, weight_initializer=inits)
+        self.final = Linear(hidden_channels, output_channels)
 
         self.reset_parameters()
 
     def reset_parameters(self):
         self.conv1.reset_parameters()
         self.conv2.reset_parameters()
 
@@ -218,24 +219,26 @@
     r"""
          The ComENet from the `"ComENet: Towards Complete and Efficient Message Passing for 3D Molecular Graphs" <https://arxiv.org/abs/2206.08515>`_ paper.
         
         Args:
             cutoff (float, optional): Cutoff distance for interatomic interactions. (default: :obj:`8.0`)
             num_layers (int, optional): Number of building blocks. (default: :obj:`4`)
             hidden_channels (int, optional): Hidden embedding size. (default: :obj:`256`)
+            middle_channels (int, optional): Middle embedding size for the two layer linear block. (default: :obj:`256`)
             out_channels (int, optional): Size of each output sample. (default: :obj:`1`)
             num_radial (int, optional): Number of radial basis functions. (default: :obj:`3`)
             num_spherical (int, optional): Number of spherical harmonics. (default: :obj:`2`)
             num_output_layers (int, optional): Number of linear layers for the output blocks. (default: :obj:`3`)
     """
     def __init__(
             self,
             cutoff=8.0,
             num_layers=4,
             hidden_channels=256,
+            middle_channels=64,
             out_channels=1,
             num_radial=3,
             num_spherical=2,
             num_output_layers=3,
     ):
         super(ComENet, self).__init__()
         self.out_channels = out_channels
@@ -253,28 +256,29 @@
 
         self.emb = EmbeddingBlock(hidden_channels, act)
 
         self.interaction_blocks = torch.nn.ModuleList(
             [
                 SimpleInteractionBlock(
                     hidden_channels,
+                    middle_channels,
                     num_radial,
                     num_spherical,
                     num_output_layers,
                     hidden_channels,
                     act,
                 )
                 for _ in range(num_layers)
             ]
         )
 
         self.lins = torch.nn.ModuleList()
         for _ in range(num_output_layers):
             self.lins.append(Linear(hidden_channels, hidden_channels))
-        self.lin_out = Linear(hidden_channels, out_channels, weight_initializer='zeros')
+        self.lin_out = Linear(hidden_channels, out_channels)
         self.reset_parameters()
 
     def reset_parameters(self):
         self.emb.reset_parameters()
         for interaction in self.interaction_blocks:
             interaction.reset_parameters()
         for lin in self.lins:
```

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/method/comenet/features.py` & `dive_into_graphs-1.1.0/dig/threedgraph/method/comenet/features.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/method/dimenetpp/dimenetpp.py` & `dive_into_graphs-1.1.0/dig/threedgraph/method/dimenetpp/dimenetpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import torch
 from torch import nn
-from torch.nn import Linear, Embedding
-from torch_geometric.nn.acts import swish
+from torch.nn import Linear, Embedding 
 from torch_geometric.nn.inits import glorot_orthogonal
 from torch_geometric.nn import radius_graph
 from torch_scatter import scatter
 from math import sqrt
 
 from ...utils import xyz_to_dat
 from .features import dist_emb, angle_emb
 
 try:
     import sympy as sym
 except ImportError:
     sym = None
 
+def swish(x):
+    return x * torch.sigmoid(x)
+
 class emb(torch.nn.Module):
     def __init__(self, num_spherical, num_radial, cutoff, envelope_exponent):
         super(emb, self).__init__()
         self.dist_emb = dist_emb(num_radial, cutoff, envelope_exponent)
         self.angle_emb = angle_emb(num_spherical, num_radial, cutoff, envelope_exponent)
         self.reset_parameters()
```

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/method/dimenetpp/features.py` & `dive_into_graphs-1.1.0/dig/threedgraph/method/dimenetpp/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         self.envelope = Envelope(envelope_exponent)
 
         self.freq = torch.nn.Parameter(torch.Tensor(num_radial))
 
         self.reset_parameters()
 
     def reset_parameters(self):
-        torch.arange(1, self.freq.numel() + 1, out=self.freq).mul_(PI)
+        self.freq.data = torch.arange(1, self.freq.numel() + 1).float().mul_(PI)
 
     def forward(self, dist):
         dist = dist.unsqueeze(-1) / self.cutoff
         return self.envelope(dist) * (self.freq * dist).sin()
 
 
 class angle_emb(torch.nn.Module):
```

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/method/run.py` & `dive_into_graphs-1.1.0/dig/threedgraph/method/run.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/method/schnet/schnet.py` & `dive_into_graphs-1.1.0/dig/threedgraph/method/schnet/schnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,19 +56,19 @@
         out = self.lin1(out)
         out = self.act(out)
         out = self.lin2(out)
         return v + out
 
 
 class update_u(torch.nn.Module):
-    def __init__(self, hidden_channels):
+    def __init__(self, hidden_channels, out_channels):
         super(update_u, self).__init__()
         self.lin1 = Linear(hidden_channels, hidden_channels // 2)
         self.act = ShiftedSoftplus()
-        self.lin2 = Linear(hidden_channels // 2, 1)
+        self.lin2 = Linear(hidden_channels // 2, out_channels)
 
         self.reset_parameters()
 
     def reset_parameters(self):
         torch.nn.init.xavier_uniform_(self.lin1.weight)
         self.lin1.bias.data.fill_(0)
         torch.nn.init.xavier_uniform_(self.lin2.weight)
@@ -108,37 +108,39 @@
         The re-implementation for SchNet from the `"SchNet: A Continuous-filter Convolutional Neural Network for Modeling Quantum Interactions" <https://arxiv.org/abs/1706.08566>`_ paper
         under the 3DGN gramework from `"Spherical Message Passing for 3D Molecular Graphs" <https://openreview.net/forum?id=givsRXsOt9r>`_ paper.
         
         Args:
             energy_and_force (bool, optional): If set to :obj:`True`, will predict energy and take the negative of the derivative of the energy with respect to the atomic positions as predicted forces. (default: :obj:`False`)
             num_layers (int, optional): The number of layers. (default: :obj:`6`)
             hidden_channels (int, optional): Hidden embedding size. (default: :obj:`128`)
+            out_channels (int, optional): Output embedding size. (default: :obj:`1`)
             num_filters (int, optional): The number of filters to use. (default: :obj:`128`)
             num_gaussians (int, optional): The number of gaussians :math:`\mu`. (default: :obj:`50`)
             cutoff (float, optional): Cutoff distance for interatomic interactions. (default: :obj:`10.0`).
     """
-    def __init__(self, energy_and_force=False, cutoff=10.0, num_layers=6, hidden_channels=128, num_filters=128, num_gaussians=50):
+    def __init__(self, energy_and_force=False, cutoff=10.0, num_layers=6, hidden_channels=128, out_channels=1, num_filters=128, num_gaussians=50):
         super(SchNet, self).__init__()
 
         self.energy_and_force = energy_and_force
         self.cutoff = cutoff
         self.num_layers = num_layers
         self.hidden_channels = hidden_channels
+        self.out_channels = out_channels
         self.num_filters = num_filters
         self.num_gaussians = num_gaussians
 
         self.init_v = Embedding(100, hidden_channels)
         self.dist_emb = emb(0.0, cutoff, num_gaussians)
 
         self.update_vs = torch.nn.ModuleList([update_v(hidden_channels, num_filters) for _ in range(num_layers)])
 
         self.update_es = torch.nn.ModuleList([
             update_e(hidden_channels, num_filters, num_gaussians, cutoff) for _ in range(num_layers)])
         
-        self.update_u = update_u(hidden_channels)
+        self.update_u = update_u(hidden_channels, out_channels)
 
         self.reset_parameters()
 
     def reset_parameters(self):
         self.init_v.reset_parameters()
         for update_e in self.update_es:
             update_e.reset_parameters()
```

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/method/spherenet/features.py` & `dive_into_graphs-1.1.0/dig/threedgraph/method/spherenet/features.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/method/spherenet/spherenet.py` & `dive_into_graphs-1.1.0/dig/threedgraph/method/spherenet/spherenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import torch
 from torch import nn
 from torch.nn import Linear, Embedding
-from torch_geometric.nn.acts import swish
 from torch_geometric.nn.inits import glorot_orthogonal
 from torch_geometric.nn import radius_graph
 from torch_scatter import scatter
 from math import sqrt
 
 from ...utils import xyz_to_dat
 from .features import dist_emb, angle_emb, torsion_emb
 
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
+def swish(x):
+    return x * torch.sigmoid(x)
+
 class emb(torch.nn.Module):
     def __init__(self, num_spherical, num_radial, cutoff, envelope_exponent):
         super(emb, self).__init__()
         self.dist_emb = dist_emb(num_radial, cutoff, envelope_exponent)
         self.angle_emb = angle_emb(num_spherical, num_radial, cutoff, envelope_exponent)
         self.torsion_emb = torsion_emb(num_spherical, num_radial, cutoff, envelope_exponent)
         self.reset_parameters()
```

### Comparing `dive_into_graphs-1.0.0/dig/threedgraph/utils/geometric_computing.py` & `dive_into_graphs-1.1.0/dig/threedgraph/utils/geometric_computing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def xyz_to_dat(pos, edge_index, num_nodes, use_torsion = False):
     """
     Compute the diatance, angle, and torsion from geometric information.
 
     Args:
         pos: Geometric information for every node in the graph.
-        edgee_index: Edge index of the graph.
+        edge_index: Edge index of the graph.
         number_nodes: Number of nodes in the graph.
         use_torsion: If set to :obj:`True`, will return distance, angle and torsion, otherwise only return distance and angle (also retrun some useful index). (default: :obj:`False`)
     """
     j, i = edge_index  # j->i
 
     # Calculate distances. # number of edges
     dist = (pos[i] - pos[j]).pow(2).sum(dim=-1).sqrt()
@@ -42,36 +42,38 @@
 
     # Calculate angles. 0 to pi
     pos_ji = pos[idx_i] - pos[idx_j]
     pos_jk = pos[idx_k] - pos[idx_j]
     a = (pos_ji * pos_jk).sum(dim=-1) # cos_angle * |pos_ji| * |pos_jk|
     b = torch.cross(pos_ji, pos_jk).norm(dim=-1) # sin_angle * |pos_ji| * |pos_jk|
     angle = torch.atan2(b, a)
-            
-    idx_batch = torch.arange(len(idx_i),device=device)
-    idx_k_n = adj_t[idx_j].storage.col()
-    repeat = num_triplets
-    num_triplets_t = num_triplets.repeat_interleave(repeat)[mask]
-    idx_i_t = idx_i.repeat_interleave(num_triplets_t)
-    idx_j_t = idx_j.repeat_interleave(num_triplets_t)
-    idx_k_t = idx_k.repeat_interleave(num_triplets_t)
-    idx_batch_t = idx_batch.repeat_interleave(num_triplets_t)
-    mask = idx_i_t != idx_k_n       
-    idx_i_t, idx_j_t, idx_k_t, idx_k_n, idx_batch_t = idx_i_t[mask], idx_j_t[mask], idx_k_t[mask], idx_k_n[mask], idx_batch_t[mask]
 
-    # Calculate torsions.
+
     if use_torsion:
+        # Prepare torsion idxes.
+        idx_batch = torch.arange(len(idx_i),device=device)
+        idx_k_n = adj_t[idx_j].storage.col()
+        repeat = num_triplets
+        num_triplets_t = num_triplets.repeat_interleave(repeat)[mask]
+        idx_i_t = idx_i.repeat_interleave(num_triplets_t)
+        idx_j_t = idx_j.repeat_interleave(num_triplets_t)
+        idx_k_t = idx_k.repeat_interleave(num_triplets_t)
+        idx_batch_t = idx_batch.repeat_interleave(num_triplets_t)
+        mask = idx_i_t != idx_k_n   
+        idx_i_t, idx_j_t, idx_k_t, idx_k_n, idx_batch_t = idx_i_t[mask], idx_j_t[mask], idx_k_t[mask], idx_k_n[mask], idx_batch_t[mask]
+
+        # Calculate torsions.
         pos_j0 = pos[idx_k_t] - pos[idx_j_t]
         pos_ji = pos[idx_i_t] - pos[idx_j_t]
         pos_jk = pos[idx_k_n] - pos[idx_j_t]
-        # dist_ji = pos_ji.pow(2).sum(dim=-1).sqrt()
+        dist_ji = pos_ji.pow(2).sum(dim=-1).sqrt()
         plane1 = torch.cross(pos_ji, pos_j0)
         plane2 = torch.cross(pos_ji, pos_jk)
         a = (plane1 * plane2).sum(dim=-1) # cos_angle * |plane1| * |plane2|
-        b = torch.cross(plane1, plane2).norm(dim=-1) # sin_angle * |plane1| * |plane2|
+        b = (torch.cross(plane1, plane2) * pos_ji).sum(dim=-1) / dist_ji 
         torsion1 = torch.atan2(b, a) # -pi to pi
         torsion1[torsion1<=0]+=2*PI # 0 to 2pi
         torsion = scatter(torsion1,idx_batch_t,reduce='min')
 
         return dist, angle, torsion, i, j, idx_kj, idx_ji
     
     else:
```

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/dataset/mol_dataset.py` & `dive_into_graphs-1.1.0/dig/xgraph/dataset/mol_dataset.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/dataset/nlp_dataset.py` & `dive_into_graphs-1.1.0/dig/xgraph/dataset/nlp_dataset.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/dataset/syn_dataset.py` & `dive_into_graphs-1.1.0/dig/xgraph/dataset/syn_dataset.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/dataset/utils_dataset.py` & `dive_into_graphs-1.1.0/dig/xgraph/dataset/utils_dataset.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/evaluation/metrics.py` & `dive_into_graphs-1.1.0/dig/xgraph/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/method/base_explainer.py` & `dive_into_graphs-1.1.0/dig/xgraph/method/base_explainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,22 @@
             unimportant_indices = indices[split_point:]
             trans_mask = mask.clone()
             trans_mask[important_indices] = float('inf')
             trans_mask[unimportant_indices] = - float('inf')
 
         return trans_mask
 
+    def batch_input(self, x, edge_index, batch_size):
+        batch_x = x.repeat(batch_size, 1)
+        batch_batch = torch.arange(batch_size, device=self.device).unsqueeze(1).repeat(1, self.num_nodes).view(-1)
+        batch_edge_batch = torch.arange(batch_size, device=self.device).unsqueeze(1).repeat(1, self.num_edges).view(-1)
+        batch_edge_index = edge_index.repeat(1, batch_size) + batch_edge_batch * self.num_nodes
+        batch = Batch(x=batch_x, edge_index=batch_edge_index, batch=batch_batch)
+        return batch
+
     def visualize_graph(self, node_idx: int, edge_index: Tensor, edge_mask: Tensor, y: Tensor = None,
                         threshold: float = None, nolabel: bool = True, **kwargs) -> Tuple[Axes, nx.DiGraph]:
         r"""Visualizes the subgraph around :attr:`node_idx` given an edge mask
         :attr:`edge_mask`.
 
         Args:
             node_idx (int): The node id to explain.
@@ -468,7 +476,23 @@
             for idx, module in enumerate(self.cls.mp_layers):
                 module._explain = True
                 module.__edge_mask__ = self.cls.edge_mask[idx]
 
         def __exit__(self, *args):
             for idx, module in enumerate(self.cls.mp_layers):
                 module._explain = False
+
+    class temp_mask(object):
+
+        def __init__(self, cls, temp_edge_mask):
+            self.cls = cls
+            self.temp_edge_mask = temp_edge_mask
+
+        def __enter__(self):
+
+            for idx, module in enumerate(self.cls.mp_layers):
+                module.__explain_flow__ = True
+                module.layer_edge_mask = self.temp_edge_mask[idx]
+
+        def __exit__(self, *args):
+            for idx, module in enumerate(self.cls.mp_layers):
+                module.__explain_flow__ = False
```

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/method/deeplift.py` & `dive_into_graphs-1.1.0/dig/xgraph/method/deeplift.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/method/gnn_gi.py` & `dive_into_graphs-1.1.0/dig/xgraph/method/gnn_gi.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/method/gnn_lrp.py` & `dive_into_graphs-1.1.0/dig/xgraph/method/gnn_lrp.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/method/gnnexplainer.py` & `dive_into_graphs-1.1.0/dig/xgraph/method/gnnexplainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import torch
 from torch import Tensor
 from torch_geometric.utils.loop import add_remaining_self_loops
 from dig.version import debug
 from ..models.utils import subgraph
+from .utils import symmetric_edge_mask_indirect_graph
 from torch.nn.functional import cross_entropy
 from .base_explainer import ExplainerBase
 from typing import Union
 EPS = 1e-15
 
 
 def cross_entropy_with_logit(y_pred: torch.Tensor, y_true: torch.Tensor, **kwargs):
@@ -25,42 +26,51 @@
         model (torch.nn.Module): The GNN module to explain.
         epochs (int, optional): The number of epochs to train.
             (default: :obj:`100`)
         lr (float, optional): The learning rate to apply.
             (default: :obj:`0.01`)
         explain_graph (bool, optional): Whether to explain graph classification model
             (default: :obj:`False`)
+        indirect_graph_symmetric_weights (bool, optional): If `True`, then the explainer
+            will first realize whether this graph input has indirect edges, 
+            then makes its edge weights symmetric. (default: :obj:`False`)
     """
     def __init__(self,
                  model: torch.nn.Module,
                  epochs: int = 100,
                  lr: float = 0.01,
-                 coff_size: float = 0.001,
-                 coff_ent: float = 0.001,
-                 explain_graph: bool = False):
+                 coff_edge_size: float = 0.001,
+                 coff_edge_ent: float = 0.001,
+                 coff_node_feat_size: float = 1.0,
+                 coff_node_feat_ent: float = 0.1,
+                 explain_graph: bool = False,
+                 indirect_graph_symmetric_weights: bool = False):
         super(GNNExplainer, self).__init__(model, epochs, lr, explain_graph)
-        self.coff_ent = coff_ent
-        self.coff_size = coff_size
+        self.coff_node_feat_size = coff_node_feat_size
+        self.coff_node_feat_ent = coff_node_feat_ent
+        self.coff_edge_size = coff_edge_size
+        self.coff_edge_ent = coff_edge_ent
+        self._symmetric_edge_mask_indirect_graph: bool = indirect_graph_symmetric_weights
 
     def __loss__(self, raw_preds: Tensor, x_label: Union[Tensor, int]):
         if self.explain_graph:
             loss = cross_entropy_with_logit(raw_preds, x_label)
         else:
             loss = cross_entropy_with_logit(raw_preds[self.node_idx].reshape(1, -1), x_label)
 
         m = self.edge_mask.sigmoid()
-        loss = loss + self.coff_size * m.sum()
+        loss = loss + self.coff_edge_size * m.sum()
         ent = -m * torch.log(m + EPS) - (1 - m) * torch.log(1 - m + EPS)
-        loss = loss + self.coff_ent * ent.mean()
+        loss = loss + self.coff_edge_ent * ent.mean()
 
         if self.mask_features:
             m = self.node_feat_mask.sigmoid()
-            loss = loss + self.coeffs['node_feat_size'] * m.sum()
+            loss = loss + self.coff_node_feat_size * m.sum()
             ent = -m * torch.log(m + EPS) - (1 - m) * torch.log(1 - m + EPS)
-            loss = loss + self.coeffs['node_feat_ent'] * ent.mean()
+            loss = loss + self.coff_node_feat_ent * ent.mean()
 
         return loss
 
     def gnn_explainer_alg(self,
                           x: Tensor,
                           edge_index: Tensor,
                           ex_label: Tensor,
@@ -90,24 +100,25 @@
             optimizer.zero_grad()
             loss.backward()
             torch.nn.utils.clip_grad_value_(self.model.parameters(), clip_value=2.0)
             optimizer.step()
 
         return self.edge_mask.data
 
-    def forward(self, x, edge_index, mask_features=False, **kwargs):
+    def forward(self, x, edge_index, mask_features=False, target_label=None, **kwargs):
         r"""
         Run the explainer for a specific graph instance.
         Args:
             x (torch.Tensor): The graph instance's input node features.
             edge_index (torch.Tensor): The graph instance's edge index.
             mask_features (bool, optional): Whether to use feature mask. Not recommended.
                 (Default: :obj:`False`)
+            target_label (torch.Tensor, optional): if given then apply optimization only on this label
             **kwargs (dict):
-                :obj:`node_idx` （int): The index of node that is pending to be explained.
+                :obj:`node_idx` （int, list, tuple, torch.Tensor): The index of node that is pending to be explained.
                 (for node classification)
                 :obj:`sparsity` (float): The Sparsity we need to control to transform a
                 soft mask to a hard mask. (Default: :obj:`0.7`)
                 :obj:`num_classes` (int): The number of task's classes.
         :rtype: (None, list, list)
         .. note::
             (None, edge_masks, related_predictions):
@@ -119,42 +130,51 @@
         self.model.eval()
 
         self_loop_edge_index, _ = add_remaining_self_loops(edge_index, num_nodes=self.num_nodes)
 
         # Only operate on a k-hop subgraph around `node_idx`.
         # Get subgraph and relabel the node, mapping is the relabeled given node_idx.
         if not self.explain_graph:
-            node_idx = kwargs.get('node_idx')
-            if not node_idx.dim():
-                node_idx = node_idx.reshape(-1)
-            node_idx = node_idx.to(self.device)
-            assert node_idx is not None
+            self.node_idx = node_idx = kwargs.get('node_idx')
+            assert node_idx is not None, 'An node explanation needs kwarg node_idx, but got None.'
+            if isinstance(node_idx, torch.Tensor) and not node_idx.dim():
+                node_idx = node_idx.to(self.device).flatten()
+            elif isinstance(node_idx, (int, list, tuple)):
+                node_idx = torch.tensor([node_idx], device=self.device, dtype=torch.int64).flatten()
+            else:
+                raise TypeError(f'node_idx should be in types of int, list, tuple, '
+                                f'or torch.Tensor, but got {type(node_idx)}')
             self.subset, _, _, self.hard_edge_mask = subgraph(
                 node_idx, self.__num_hops__, self_loop_edge_index, relabel_nodes=True,
                 num_nodes=None, flow=self.__flow__())
-            self.node_idx = node_idx
             self.new_node_idx = torch.where(self.subset == node_idx)[0]
 
         if kwargs.get('edge_masks'):
             edge_masks = kwargs.pop('edge_masks')
             self.__set_masks__(x, self_loop_edge_index)
 
         else:
             # Assume the mask we will predict
             labels = tuple(i for i in range(kwargs.get('num_classes')))
             ex_labels = tuple(torch.tensor([label]).to(self.device) for label in labels)
 
             # Calculate mask
             edge_masks = []
             for ex_label in ex_labels:
-                self.__clear_masks__()
-                self.__set_masks__(x, self_loop_edge_index)
-                edge_masks.append(self.gnn_explainer_alg(x, edge_index, ex_label))
+                if target_label is None or ex_label.item() == target_label.item():
+                    self.__clear_masks__()
+                    self.__set_masks__(x, self_loop_edge_index)
+                    edge_mask = self.gnn_explainer_alg(x, edge_index, ex_label).sigmoid()
+                    
+                    if self._symmetric_edge_mask_indirect_graph:
+                        edge_mask = symmetric_edge_mask_indirect_graph(self_loop_edge_index, edge_mask)
+
+                    edge_masks.append(edge_mask)
 
-        hard_edge_masks = [self.control_sparsity(mask, sparsity=kwargs.get('sparsity')).sigmoid()
+        hard_edge_masks = [self.control_sparsity(mask, sparsity=kwargs.get('sparsity'))
                            for mask in edge_masks]
 
         with torch.no_grad():
             related_preds = self.eval_related_pred(x, edge_index, hard_edge_masks, **kwargs)
 
         self.__clear_masks__()
```

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/method/gradcam.py` & `dive_into_graphs-1.1.0/dig/xgraph/method/gradcam.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         labels = tuple(i for i in range(kwargs.get('num_classes')))
         ex_labels = tuple(torch.tensor([label]).to(self.device) for label in labels)
 
         self_loop_edge_index, _ = add_remaining_self_loops(edge_index, num_nodes=self.num_nodes)
 
         if not self.explain_graph:
             node_idx = kwargs.get('node_idx')
+            if isinstance(node_idx, int):
+                node_idx = torch.tensor([node_idx], device=self.device, dtype=torch.long)
             if not node_idx.dim():
                 node_idx = node_idx.reshape(-1)
             node_idx = node_idx.to(self.device)
             assert node_idx is not None
             self.subset, _, _, self.hard_edge_mask = subgraph(
                 node_idx, self.__num_hops__, self_loop_edge_index, relabel_nodes=True,
                 num_nodes=None, flow=self.__flow__())
@@ -110,15 +112,15 @@
                 model = model_node(self)
             self.explain_method = GraphLayerGradCam(model, model.convs[-1])
             # --- setting end ---
 
             edge_masks = []
             hard_edge_masks = []
             for ex_label in ex_labels:
-                attr_wo_relu = self.explain_method.attribute(x, ex_label, additional_forward_args=edge_index)
+                attr_wo_relu = self.explain_method.attribute(x, ex_label, additional_forward_args=edge_index).detach()
                 mask = normalize(attr_wo_relu.relu())
                 mask = mask.squeeze()
                 mask = (mask[self_loop_edge_index[0]] + mask[self_loop_edge_index[1]]) / 2
                 edge_masks.append(mask.detach())
                 mask = self.control_sparsity(mask, kwargs.get('sparsity'))
                 mask = mask.sigmoid()
                 hard_edge_masks.append(mask.detach())
```

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/method/pgexplainer.py` & `dive_into_graphs-1.1.0/dig/xgraph/method/pgexplainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -789,15 +789,15 @@
                                                words=words,
                                                figname=vis_name)
             else:
                 plot_utils.plot_soft_edge_mask(graph,
                                                edge_mask,
                                                top_k=top_k,
                                                un_directed=True,
-                                               x=x,
+                                               x=data.x,
                                                figname=vis_name)
         else:
             assert node_idx is not None, "visualization method doesn't get the target node index"
             x, edge_index, y, subset, kwargs = \
                 self.get_subgraph(node_idx=node_idx, x=data.x, edge_index=data.edge_index, y=data.y)
             new_node_idx = torch.where(subset == node_idx)[0]
             new_data = Data(x=x, edge_index=edge_index)
```

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/method/shapley.py` & `dive_into_graphs-1.1.0/dig/xgraph/method/shapley.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import copy
 import torch
 import numpy as np
 from scipy.special import comb
 from itertools import combinations
 import torch.nn.functional as F
 from torch_geometric.utils import to_networkx
-from torch_geometric.data import Data, Batch, Dataset, DataLoader
+from torch_geometric.data import Data, Batch, Dataset
+from torch_geometric.loader import DataLoader
 
 
 def GnnNetsGC2valueFunc(gnnNets, target_class):
     def value_func(batch):
         with torch.no_grad():
             logits = gnnNets(data=batch)
             probs = F.softmax(logits, dim=-1)
```

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/method/subgraphx.py` & `dive_into_graphs-1.1.0/dig/xgraph/method/subgraphx.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,14 +467,17 @@
         self.c_puct = c_puct
         self.expand_atoms = expand_atoms
         self.high2low = high2low
         self.new_node_idx = None
 
         # extract the sub-graph and change the node indices.
         if node_idx is not None:
+            if isinstance(node_idx, Tensor):
+                node_idx = node_idx.item()
+
             self.ori_node_idx = node_idx
             self.ori_graph = copy.copy(self.graph)
             x, edge_index, subset, edge_mask, kwargs = \
                 self.__subgraph__(node_idx, self.X, self.edge_index, self.num_hops)
             self.data = Batch.from_data_list([Data(x=x, edge_index=edge_index)])
             self.graph = self.ori_graph.subgraph(subset.tolist())
             mapping = {int(v): k for k, v in enumerate(subset)}
```

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/models/ext/deeplift/deep_lift.py` & `dive_into_graphs-1.1.0/dig/xgraph/models/ext/deeplift/deep_lift.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/models/ext/deeplift/layer_deep_lift.py` & `dive_into_graphs-1.1.0/dig/xgraph/models/ext/deeplift/layer_deep_lift.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/models/gradient_utils.py` & `dive_into_graphs-1.1.0/dig/xgraph/models/gradient_utils.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/models/model_manager.py` & `dive_into_graphs-1.1.0/dig/xgraph/models/model_manager.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/models/models.py` & `dive_into_graphs-1.1.0/dig/xgraph/models/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,33 @@
     def get_emb(self, *args, **kwargs) -> torch.Tensor:
         x, edge_index, batch = self.arguments_read(*args, **kwargs)
         post_conv = self.relu1(self.conv1(x, edge_index))
         for conv, relu in zip(self.convs, self.relus):
             post_conv = relu(conv(post_conv, edge_index))
         return post_conv
 
+class GCN_3l_BN(GCN_3l):
+    def __init__(self, model_level, dim_node, dim_hidden, num_classes):
+        super().__init__(model_level, dim_node, dim_hidden, num_classes)
+        num_layer = 3
+
+        self.relu1 = nn.Sequential(
+            nn.BatchNorm1d(dim_hidden),
+            nn.ReLU()
+        )
+
+        self.relus = nn.ModuleList(
+            [
+                nn.Sequential(
+                    nn.BatchNorm1d(dim_hidden),
+                    nn.ReLU(),
+                )
+                for _ in range(num_layer - 1)
+            ]
+        )
 
 class GCN_2l(GNNBasic):
 
     def __init__(self, model_level, dim_node, dim_hidden, num_classes):
         super().__init__()
         num_layer = 2
 
@@ -286,15 +305,17 @@
         return post_conv
 
 
 class GCNConv(gnn.GCNConv):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.__explain_flow__ = False
         self.edge_weight = None
+        self.layer_edge_mask = None
         self.weight = nn.Parameter(self.lin.weight.data.T.clone().detach())
 
     def forward(self, x: Tensor, edge_index: Adj,
                 edge_weight: OptTensor = None) -> Tensor:
         """"""
 
         if self.normalize and edge_weight is None:
@@ -369,28 +390,39 @@
                 # Some ops add self-loops to `edge_index`. We need to do the
                 # same for `edge_mask` (but do not train those).
                 if out.size(self.node_dim) != edge_mask.size(0):
                     loop = edge_mask.new_ones(size[0])
                     edge_mask = torch.cat([edge_mask, loop], dim=0)
                 assert out.size(self.node_dim) == edge_mask.size(0)
                 out = out * edge_mask.view([-1] + [1] * (out.dim() - 1))
+            elif self.__explain_flow__:
+                edge_mask = self.layer_edge_mask
+                # Some ops add self-loops to `edge_index`. We need to do the
+                # same for `edge_mask` (but do not train those).
+                if out.size(self.node_dim) != edge_mask.size(0):
+                    loop = edge_mask.new_ones(size[0])
+                    edge_mask = torch.cat([edge_mask, loop], dim=0)
+                assert out.size(self.node_dim) == edge_mask.size(0)
+                out = out * edge_mask.view([-1] + [1] * (out.dim() - 1))
 
             aggr_kwargs = self.inspector.distribute('aggregate', coll_dict)
             out = self.aggregate(out, **aggr_kwargs)
 
             update_kwargs = self.inspector.distribute('update', coll_dict)
             return self.update(out, **update_kwargs)
 
 
 class GINConv(gnn.GINConv):
 
     def __init__(self, nn: Callable, eps: float = 0., train_eps: bool = False,
                  **kwargs):
         super().__init__(nn, eps, train_eps, **kwargs)
+        self.__explain_flow__ = False
         self.edge_weight = None
+        self.layer_edge_mask = None
         self.fc_steps = None
         self.reweight = None
 
 
     def forward(self, x: Union[Tensor, OptPairTensor], edge_index: Adj,
                 edge_weight: OptTensor = None, task='explain', **kwargs) -> Tensor:
         """"""
@@ -495,14 +527,23 @@
                 # Some ops add self-loops to `edge_index`. We need to do the
                 # same for `edge_mask` (but do not train those).
                 if out.size(self.node_dim) != edge_mask.size(0):
                     loop = edge_mask.new_ones(size[0])
                     edge_mask = torch.cat([edge_mask, loop], dim=0)
                 assert out.size(self.node_dim) == edge_mask.size(0)
                 out = out * edge_mask.view([-1] + [1] * (out.dim() - 1))
+            elif self.__explain_flow__:
+                edge_mask = self.layer_edge_mask
+                # Some ops add self-loops to `edge_index`. We need to do the
+                # same for `edge_mask` (but do not train those).
+                if out.size(self.node_dim) != edge_mask.size(0):
+                    loop = edge_mask.new_ones(size[0])
+                    edge_mask = torch.cat([edge_mask, loop], dim=0)
+                assert out.size(self.node_dim) == edge_mask.size(0)
+                out = out * edge_mask.view([-1] + [1] * (out.dim() - 1))
 
             aggr_kwargs = self.inspector.distribute('aggregate', coll_dict)
             out = self.aggregate(out, **aggr_kwargs)
 
             update_kwargs = self.inspector.distribute('update', coll_dict)
             return self.update(out, **update_kwargs)
 
@@ -663,15 +704,17 @@
         return post_conv
 
 
 class GCNConv_mask(gnn.GCNConv):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.__explain_flow__ = False
         self.edge_weight = None
+        self.layer_edge_mask = None
         self.weight = nn.Parameter(self.lin.weight.data.T.clone().detach())
 
     def forward(self, x: Tensor, edge_index: Adj,
                 edge_weight: OptTensor = None) -> Tensor:
         """"""
 
         if self.normalize and edge_weight is None:
@@ -746,28 +789,39 @@
                 # Some ops add self-loops to `edge_index`. We need to do the
                 # same for `edge_mask` (but do not train those).
                 if out.size(self.node_dim) != edge_mask.size(0):
                     loop = edge_mask.new_ones(size[0])
                     edge_mask = torch.cat([edge_mask, loop], dim=0)
                 assert out.size(self.node_dim) == edge_mask.size(0)
                 out = out * edge_mask.view([-1] + [1] * (out.dim() - 1))
+            elif self.__explain_flow__:
+                edge_mask = self.layer_edge_mask
+                # Some ops add self-loops to `edge_index`. We need to do the
+                # same for `edge_mask` (but do not train those).
+                if out.size(self.node_dim) != edge_mask.size(0):
+                    loop = edge_mask.new_ones(size[0])
+                    edge_mask = torch.cat([edge_mask, loop], dim=0)
+                assert out.size(self.node_dim) == edge_mask.size(0)
+                out = out * edge_mask.view([-1] + [1] * (out.dim() - 1))
 
             aggr_kwargs = self.inspector.distribute('aggregate', coll_dict)
             out = self.aggregate(out, **aggr_kwargs)
 
             update_kwargs = self.inspector.distribute('update', coll_dict)
             return self.update(out, **update_kwargs)
 
 
 class GINConv_mask(gnn.GINConv):
 
     def __init__(self, nn: Callable, eps: float = 0., train_eps: bool = False,
                  **kwargs):
         super().__init__(nn, eps, train_eps, **kwargs)
+        self.__explain_flow__ = False
         self.edge_weight = None
+        self.layer_edge_mask = None
         self.fc_steps = None
         self.reweight = None
 
 
     def forward(self, x: Union[Tensor, OptPairTensor], edge_index: Adj,
                 edge_weight: OptTensor = None, task='explain', **kwargs) -> Tensor:
         """"""
@@ -872,13 +926,22 @@
                 # Some ops add self-loops to `edge_index`. We need to do the
                 # same for `edge_mask` (but do not train those).
                 if out.size(self.node_dim) != edge_mask.size(0):
                     loop = edge_mask.new_ones(size[0])
                     edge_mask = torch.cat([edge_mask, loop], dim=0)
                 assert out.size(self.node_dim) == edge_mask.size(0)
                 out = out * edge_mask.view([-1] + [1] * (out.dim() - 1))
+            elif self.__explain_flow__:
+                edge_mask = self.layer_edge_mask
+                # Some ops add self-loops to `edge_index`. We need to do the
+                # same for `edge_mask` (but do not train those).
+                if out.size(self.node_dim) != edge_mask.size(0):
+                    loop = edge_mask.new_ones(size[0])
+                    edge_mask = torch.cat([edge_mask, loop], dim=0)
+                assert out.size(self.node_dim) == edge_mask.size(0)
+                out = out * edge_mask.view([-1] + [1] * (out.dim() - 1))
 
             aggr_kwargs = self.inspector.distribute('aggregate', coll_dict)
             out = self.aggregate(out, **aggr_kwargs)
 
             update_kwargs = self.inspector.distribute('update', coll_dict)
             return self.update(out, **update_kwargs)
```

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/models/utils.py` & `dive_into_graphs-1.1.0/dig/xgraph/models/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         out_readoout = torch.cat(graph, dim=0)
 
         return out_readoout
 
 
 def normalize(x: torch.Tensor):
-    x -= x.min()
+    x -= x.min()  # This operation -= may lead to mem leak without detach() before this assignment. (x = x - x.min() won't lead to such a problem.)
     if x.max() == 0:
         return torch.zeros(x.size(), device=x.device)
     x /= x.max()
     return x
 
 
 def subgraph(node_idx, num_hops, edge_index, relabel_nodes=False,
@@ -121,7 +121,24 @@
 
     if relabel_nodes:
         node_idx = row.new_full((num_nodes, ), -1)
         node_idx[subset] = torch.arange(subset.size(0), device=row.device)
         edge_index = node_idx[edge_index]
 
     return subset, edge_index, inv, edge_mask
+
+
+def gumbel_softmax(log_alpha: torch.Tensor, beta: float = 1.0, training: bool = True):
+    r""" Sample from the instantiation of concrete distribution when training
+    Args:
+        log_alpha: input probabilities
+        beta: temperature for softmax
+    """
+    if training:
+        random_noise = torch.rand(log_alpha.shape)
+        random_noise = torch.log(random_noise) - torch.log(1.0 - random_noise)
+        gate_inputs = (random_noise.to(log_alpha.device) + log_alpha) / beta
+        gate_inputs = gate_inputs.sigmoid()
+    else:
+        gate_inputs = log_alpha.sigmoid()
+
+    return gate_inputs
```

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/utils/compatibility.py` & `dive_into_graphs-1.1.0/dig/xgraph/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dig/xgraph/utils/init.py` & `dive_into_graphs-1.1.0/dig/xgraph/utils/init.py`

 * *Files identical despite different names*

### Comparing `dive_into_graphs-1.0.0/dive_into_graphs.egg-info/PKG-INFO` & `dive_into_graphs-1.1.0/dive_into_graphs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dive-into-graphs
-Version: 1.0.0
+Version: 1.1.0
 Summary: DIG: Dive into Graphs is a turnkey library for graph deep learning research.
 Home-page: https://github.com/divelab/DIG
 Author: DIVE Lab@TAMU
 Author-email: sji@tamu.edu
 Maintainer: DIVE Lab@TAMU
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
@@ -34,49 +34,49 @@
 [contributor-url]:https://github.com/divelab/DIG/graphs/contributors 
 [contributing-image]:https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
 [contributing-url]:https://diveintographs.readthedocs.io/en/latest/contribution/instruction.html
 
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Docs Status][docs-image]][docs-url]
-[![Build Status](https://travis-ci.com/divelab/DIG.svg?branch=dig)](https://travis-ci.com/divelab/DIG)
-[![codecov](https://codecov.io/gh/divelab/DIG/branch/dig/graph/badge.svg?token=KBJ1P31VCH)](https://codecov.io/gh/divelab/DIG)
+[![Build Status](https://travis-ci.com/divelab/DIG.svg?branch=dig-stable)](https://travis-ci.com/divelab/DIG)
+[![codecov](https://codecov.io/gh/divelab/DIG/branch/dig-stable/graph/badge.svg?token=KBJ1P31VCH)](https://codecov.io/gh/divelab/DIG)
 ![Last Commit](https://img.shields.io/github/last-commit/divelab/DIG)
 [![Contributing][contributing-image]][contributing-url]
 [![License][license-image]][license-url]
 ![visitors](https://visitor-badge.glitch.me/badge?page_id=jwenjian.visitor-badge)
 [![Downloads](https://pepy.tech/badge/dive-into-graphs)](https://pepy.tech/project/dive-into-graphs)
 <!--- [![Contributors][contributor-image]][contributor-url] -->
 
 
-**[Documentation](https://diveintographs.readthedocs.io)** | **[Paper [JMLR]](https://www.jmlr.org/papers/v22/21-0343.html)** | **[Tutorials](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html#)** | **[Benchmarks](https://github.com/divelab/DIG/tree/dig/benchmarks)** |  **[Examples](https://github.com/divelab/DIG/tree/dig/examples)**
+**[Documentation](https://diveintographs.readthedocs.io)** | **[Paper [JMLR]](https://www.jmlr.org/papers/v22/21-0343.html)** | **[Tutorials](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html#)** | **[Benchmarks](https://github.com/divelab/DIG/tree/dig-stable/benchmarks)** |  **[Examples](https://github.com/divelab/DIG/tree/dig-stable/examples)** | **[Join the DIG slack community now!:fire:](https://join.slack.com/t/dive-into-graphs/shared_invite/zt-1i9kn731c-RhLA1zcEGHXbIToxdVqo0g)**
 
 *DIG: Dive into Graphs* is a turnkey library for graph deep learning research.
 
 :fire:**Update (2022/07): We have upgraded our DIG library based on PyG 2.0.0. We recommend installing our latest version.**
 
 ## Why DIG?
 
-The key difference with current graph deep learning libraries, such as PyTorch Geometric (PyG) and Deep Graph Library (DGL), is that, while PyG and DGL support basic graph deep learning operations, DIG provides a unified testbed for higher level, research-oriented graph deep learning tasks, such as graph generation, self-supervised learning, explainability, and 3D graphs.
+The key difference with current graph deep learning libraries, such as PyTorch Geometric (PyG) and Deep Graph Library (DGL), is that, while PyG and DGL support basic graph deep learning operations, DIG provides a unified testbed for higher level, research-oriented graph deep learning tasks, such as graph generation, self-supervised learning, explainability, 3D graphs, and graph out-of-distribution.
 
 If you are working or plan to work on research in graph deep learning, DIG enables you to develop your own methods within our extensible framework, and compare with current baseline methods using common datasets and evaluation metrics without extra efforts.
 
 ## Overview
 
 It includes unified implementations of **data interfaces**, **common algorithms**, and **evaluation metrics** for several advanced tasks. Our goal is to enable researchers to easily implement and benchmark algorithms. Currently, we consider the following research directions.
 
 * **Graph Generation**: `dig.ggraph`
 * **Self-supervised Learning on Graphs**: `dig.sslgraph`
 * **Explainability of Graph Neural Networks**: `dig.xgraph`
 * **Deep Learning on 3D Graphs**: `dig.threedgraph`
-
+* **Graph OOD**: `dig.oodgraph`
 
 
 <p align="center">
-<img src="https://github.com/divelab/DIG/blob/dig/imgs/DIG-overview.png" width="700" class="center" alt="logo"/>
+<img src="https://github.com/divelab/DIG/blob/dig-stable/docs/imgs/DIG-overview.png" width="700" class="center" alt="logo"/>
     <br/>
 </p>
 
 
 ## Usage
 
 Example: a few lines of code to run [SphereNet](https://openreview.net/forum?id=givsRXsOt9r) on [QM9](https://www.nature.com/articles/sdata201422) to incorporate 3D information of molecules.
@@ -109,22 +109,22 @@
 run3d.run(device, train_dataset, valid_dataset, test_dataset, model, loss_func, evaluation,
           epochs=20, batch_size=32, vt_batch_size=32, lr=0.0005, lr_decay_factor=0.5, lr_decay_step_size=15)
 
 ```
 
 
 1. For details of all included APIs, please refer to the [documentation](https://diveintographs.readthedocs.io/). 
-2. We provide a hands-on tutorial for each direction to help you to get started with *DIG*: [Graph Generation](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html), [Self-supervised Learning on Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/sslgraph.html), [Explainability of Graph Neural Networks](https://diveintographs.readthedocs.io/en/latest/tutorials/subgraphx.html), and [Deep Learning on 3D Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/threedgraph.html).
-3. We also provide [examples](https://github.com/divelab/DIG/tree/dig/examples) to use APIs provided in *DIG*. You can get started with your interested directions by clicking the following links.
-
-* [Graph Generation](https://github.com/divelab/DIG/tree/dig/examples/ggraph): [`JT-VAE`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/JTVAE), [`GraphAF`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/GraphAF), [`GraphDF`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/GraphDF), [`GraphEBM`](https://github.com/divelab/DIG/tree/dig/examples/ggraph/GraphEBM).
-* [Self-supervised Learning on Graphs](https://github.com/divelab/DIG/tree/dig/examples/sslgraph): [`InfoGraph`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_infograph.ipynb), [`GRACE`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_grace.ipynb), [`MVGRL`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_mvgrl.ipynb), [`GraphCL`](https://github.com/divelab/DIG/blob/dig/examples/sslgraph/example_graphcl.ipynb).
-* [Explainability of Graph Neural Networks](https://github.com/divelab/DIG/tree/dig/examples/xgraph): [`DeepLIFT`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/deeplift.ipynb), [`GNN-LRP`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/gnn_lrp.ipynb), [`GNNExplainer`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/gnnexplainer.ipynb), [`GradCAM`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/gradcam.ipynb), [`PGExplainer`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/pgexplainer.ipynb), [`SubgraphX`](https://github.com/divelab/DIG/blob/dig/examples/xgraph/subgraphx.ipynb).
-* [Deep Learning on 3D Graphs](https://github.com/divelab/DIG/tree/dig/examples/threedgraph): [`SchNet`](https://github.com/divelab/DIG/blob/dig/examples/threedgraph/threedgraph.ipynb), [`DimeNet++`](https://github.com/divelab/DIG/blob/dig/examples/threedgraph/threedgraph.ipynb), [`SphereNet`](https://github.com/divelab/DIG/blob/dig/examples/threedgraph/threedgraph.ipynb).
+2. We provide a hands-on tutorial for each direction to help you to get started with *DIG*: [Graph Generation](https://diveintographs.readthedocs.io/en/latest/tutorials/graphdf.html), [Self-supervised Learning on Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/sslgraph.html), [Explainability of Graph Neural Networks](https://diveintographs.readthedocs.io/en/latest/tutorials/subgraphx.html), [Deep Learning on 3D Graphs](https://diveintographs.readthedocs.io/en/latest/tutorials/threedgraph.html), [Graph OOD (GOOD) datasets](https://diveintographs.readthedocs.io/en/latest/tutorials/oodgraph.html).
+3. We also provide [examples](https://github.com/divelab/DIG/tree/dig-stable/examples) to use APIs provided in *DIG*. You can get started with your interested directions by clicking the following links.
 
+* [Graph Generation](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph): [`JT-VAE`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/JTVAE), [`GraphAF`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphAF), [`GraphDF`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphDF), [`GraphEBM`](https://github.com/divelab/DIG/tree/dig-stable/examples/ggraph/GraphEBM).
+* [Self-supervised Learning on Graphs](https://github.com/divelab/DIG/tree/dig-stable/examples/sslgraph): [`InfoGraph`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_infograph.ipynb), [`GRACE`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_grace.ipynb), [`MVGRL`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_mvgrl.ipynb), [`GraphCL`](https://github.com/divelab/DIG/blob/dig-stable/examples/sslgraph/example_graphcl.ipynb), [`LaGraph (v1 supported)`](https://github.com/divelab/DIG/tree/dig/examples/sslgraph/LaGraph).
+* [Explainability of Graph Neural Networks](https://github.com/divelab/DIG/tree/dig-stable/examples/xgraph): [`DeepLIFT`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/deeplift.ipynb), [`GNN-LRP`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/gnn_lrp.ipynb), [`FlowX`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/flowx.ipynb), [`GNNExplainer`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/gnnexplainer.ipynb), [`GradCAM`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/gradcam.ipynb), [`PGExplainer`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/pgexplainer.ipynb), [`SubgraphX`](https://github.com/divelab/DIG/blob/dig-stable/examples/xgraph/subgraphx.ipynb).
+* [Deep Learning on 3D Graphs](https://github.com/divelab/DIG/tree/dig-stable/examples/threedgraph): [`SchNet`](https://github.com/divelab/DIG/blob/dig-stable/examples/threedgraph/threedgraph.ipynb), [`DimeNet++`](https://github.com/divelab/DIG/blob/dig-stable/examples/threedgraph/threedgraph.ipynb), [`SphereNet`](https://github.com/divelab/DIG/blob/dig-stable/examples/threedgraph/threedgraph.ipynb).
+* [Graph OOD (GOOD) datasets](https://github.com/divelab/DIG/tree/dig-stable/examples/oodgraph): `GOODHIV`, `GOODPCBA`, `GOODZINC`, `GOODCMNIST`, `GOODMotif`, `GOODCora`, `GOODArxiv`, `GOODCBAS`.
 
 
 ## Installation
 
 ### Install from pip
 The key dependencies of DIG: Dive into Graphs are PyTorch (>=1.10.0), PyTorch Geometric (>=2.0.0), and RDKit.
 
@@ -193,12 +193,12 @@
 
 ## The Team
 
 *DIG: Dive into Graphs* is developed by [DIVE](https://github.com/divelab/)@TAMU. Contributors are Meng Liu*, Youzhi Luo*, Limei Wang*, Yaochen Xie*, Hao Yuan*, Shurui Gui*, Haiyang Yu*, Zhao Xu, Jingtun Zhang, Yi Liu, Keqiang Yan, Haoran Liu, Cong Fu, Bora Oztekin, Xuan Zhang, and Shuiwang Ji.
 
 ## Contact
 
-If you have any technical questions, please submit new issues.
+If you have any technical questions, please submit new issues or raise it in our [DIG slack community:fire:](https://join.slack.com/t/dive-into-graphs/shared_invite/zt-1i9kn731c-RhLA1zcEGHXbIToxdVqo0g).
 
 If you have any other questions, please contact us: Meng Liu [mengliu@tamu.edu] and Shuiwang Ji [sji@tamu.edu].
```

### Comparing `dive_into_graphs-1.0.0/dive_into_graphs.egg-info/SOURCES.txt` & `dive_into_graphs-1.1.0/dive_into_graphs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -78,14 +78,41 @@
 dig/ggraph3D/method/G_SphereNet/model/net_utils.py
 dig/ggraph3D/method/G_SphereNet/model/spherenet.py
 dig/ggraph3D/method/G_SphereNet/model/sphgen.py
 dig/ggraph3D/utils/__init__.py
 dig/ggraph3D/utils/eval_bond_mmd_utils.py
 dig/ggraph3D/utils/eval_prop_utils.py
 dig/ggraph3D/utils/eval_validity_utils.py
+dig/lsgraph/__init__.py
+dig/lsgraph/dataset/__init__.py
+dig/lsgraph/dataset/get_data.py
+dig/lsgraph/dataset/loader.py
+dig/lsgraph/method/FM.py
+dig/lsgraph/method/__init__.py
+dig/lsgraph/method/GraphFMOB/__init__.py
+dig/lsgraph/method/GraphFMOB/history.py
+dig/lsgraph/method/GraphFMOB/loader.py
+dig/lsgraph/method/GraphFMOB/metis.py
+dig/lsgraph/method/GraphFMOB/pool.py
+dig/lsgraph/method/GraphFMOB/utils.py
+dig/lsgraph/method/GraphFMOB/models/__init__.py
+dig/lsgraph/method/GraphFMOB/models/base.py
+dig/lsgraph/method/GraphFMOB/models/gcn.py
+dig/lsgraph/method/GraphFMOB/models/gcn2.py
+dig/lsgraph/method/GraphFMOB/models/pna.py
+dig/lsgraph/method/GraphFMOB/models/pna_jk.py
+dig/oodgraph/__init__.py
+dig/oodgraph/good_arxiv.py
+dig/oodgraph/good_cbas.py
+dig/oodgraph/good_cmnist.py
+dig/oodgraph/good_cora.py
+dig/oodgraph/good_hiv.py
+dig/oodgraph/good_motif.py
+dig/oodgraph/good_pcba.py
+dig/oodgraph/good_zinc.py
 dig/sslgraph/__init__.py
 dig/sslgraph/dataset/TUDataset.py
 dig/sslgraph/dataset/__init__.py
 dig/sslgraph/dataset/datasets.py
 dig/sslgraph/dataset/feat_expansion.py
 dig/sslgraph/evaluation/__init__.py
 dig/sslgraph/evaluation/eval_graph.py
@@ -94,39 +121,46 @@
 dig/sslgraph/method/contrastive/__init__.py
 dig/sslgraph/method/contrastive/model/__init__.py
 dig/sslgraph/method/contrastive/model/contrastive.py
 dig/sslgraph/method/contrastive/model/grace.py
 dig/sslgraph/method/contrastive/model/graphcl.py
 dig/sslgraph/method/contrastive/model/infograph.py
 dig/sslgraph/method/contrastive/model/mvgrl.py
+dig/sslgraph/method/contrastive/model/pgrace.py
 dig/sslgraph/method/contrastive/objectives/__init__.py
 dig/sslgraph/method/contrastive/objectives/infonce.py
 dig/sslgraph/method/contrastive/objectives/jse.py
 dig/sslgraph/method/contrastive/views_fn/__init__.py
 dig/sslgraph/method/contrastive/views_fn/combination.py
 dig/sslgraph/method/contrastive/views_fn/feature.py
 dig/sslgraph/method/contrastive/views_fn/sample.py
 dig/sslgraph/method/contrastive/views_fn/structure.py
 dig/sslgraph/utils/__init__.py
+dig/sslgraph/utils/adaptive.py
 dig/sslgraph/utils/encoders.py
 dig/sslgraph/utils/seed.py
 dig/threedgraph/__init__.py
+dig/threedgraph/dataset/ECdataset.py
+dig/threedgraph/dataset/FOLDdataset.py
 dig/threedgraph/dataset/PygMD17.py
 dig/threedgraph/dataset/PygQM93D.py
 dig/threedgraph/dataset/__init__.py
 dig/threedgraph/evaluation/__init__.py
 dig/threedgraph/evaluation/eval.py
 dig/threedgraph/method/__init__.py
 dig/threedgraph/method/run.py
 dig/threedgraph/method/comenet/__init__.py
 dig/threedgraph/method/comenet/comenet.py
 dig/threedgraph/method/comenet/features.py
 dig/threedgraph/method/dimenetpp/__init__.py
 dig/threedgraph/method/dimenetpp/dimenetpp.py
 dig/threedgraph/method/dimenetpp/features.py
+dig/threedgraph/method/pronet/__init__.py
+dig/threedgraph/method/pronet/features.py
+dig/threedgraph/method/pronet/pronet.py
 dig/threedgraph/method/schnet/__init__.py
 dig/threedgraph/method/schnet/schnet.py
 dig/threedgraph/method/spherenet/__init__.py
 dig/threedgraph/method/spherenet/features.py
 dig/threedgraph/method/spherenet/spherenet.py
 dig/threedgraph/utils/__init__.py
 dig/threedgraph/utils/geometric_computing.py
@@ -138,21 +172,24 @@
 dig/xgraph/dataset/utils_dataset.py
 dig/xgraph/evaluation/__init__.py
 dig/xgraph/evaluation/defi.py
 dig/xgraph/evaluation/metrics.py
 dig/xgraph/method/__init__.py
 dig/xgraph/method/base_explainer.py
 dig/xgraph/method/deeplift.py
+dig/xgraph/method/flowx.py
 dig/xgraph/method/gnn_gi.py
 dig/xgraph/method/gnn_lrp.py
 dig/xgraph/method/gnnexplainer.py
 dig/xgraph/method/gradcam.py
 dig/xgraph/method/pgexplainer.py
 dig/xgraph/method/shapley.py
 dig/xgraph/method/subgraphx.py
+dig/xgraph/method/utils/__init__.py
+dig/xgraph/method/utils/symmetric_edge_mask.py
 dig/xgraph/models/__init__.py
 dig/xgraph/models/gradient_utils.py
 dig/xgraph/models/model_manager.py
 dig/xgraph/models/models.py
 dig/xgraph/models/utils.py
 dig/xgraph/models/ext/__init__.py
 dig/xgraph/models/ext/deeplift/__init__.py
```

### Comparing `dive_into_graphs-1.0.0/setup.py` & `dive_into_graphs-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,21 +32,23 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     install_requires=['scipy',
                       'cilog',
                       'typed-argument-parser==1.7.2',
                       'captum==0.2.0',
+                      'munch',
+                      'gdown',
                       'shap',
                       'IPython',
                       'tqdm',
                       'rdkit-pypi',
                       'pandas',
                       'sympy',
-                      'pyscf==1.7.6.post1',
+                      'pyscf>=1.7.6',
                       'hydra-core'],
     python_requires='>=3.6',
     setup_requires=setup_requires,
     tests_require=tests_require,
     extras_require={'test': tests_require},
     include_package_data=True
 )
```

