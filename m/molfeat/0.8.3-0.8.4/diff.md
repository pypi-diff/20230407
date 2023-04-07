# Comparing `tmp/molfeat-0.8.3.tar.gz` & `tmp/molfeat-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molfeat-0.8.3.tar", last modified: Tue Apr  4 14:07:51 2023, max compression
+gzip compressed data, was "molfeat-0.8.4.tar", last modified: Fri Apr  7 16:17:34 2023, max compression
```

## Comparing `molfeat-0.8.3.tar` & `molfeat-0.8.4.tar`

### file list

```diff
@@ -1,163 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.855444 molfeat-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-04 14:06:34.000000 molfeat-0.8.3/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.835444 molfeat-0.8.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.835444 molfeat-0.8.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/ISSUE_TEMPLATE/1_bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/ISSUE_TEMPLATE/2_refactor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/ISSUE_TEMPLATE/3_documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.835444 molfeat-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-04 14:06:34.000000 molfeat-0.8.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-04 14:06:34.000000 molfeat-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-04 14:06:34.000000 molfeat-0.8.3/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-04 14:06:34.000000 molfeat-0.8.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-04 14:06:34.000000 molfeat-0.8.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-04 14:06:34.000000 molfeat-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-04 14:07:51.855444 molfeat-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-04 14:06:34.000000 molfeat-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.835444 molfeat-0.8.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.839444 molfeat-0.8.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.calc.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.store.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.trans.base.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.trans.concat.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.trans.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.trans.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.trans.pretrained.fcd.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.trans.pretrained.graphormer.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.trans.pretrained.hf_transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.trans.struct.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/api/molfeat.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.827444 molfeat-0.8.3/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.839444 molfeat-0.8.3/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/assets/css/custom-molfeat.css
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/assets/css/tweak-width.css
--rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/benchmark.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.839444 molfeat-0.8.3/docs/developers/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/developers/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/developers/create-plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/developers/register-plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.839444 molfeat-0.8.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.843444 molfeat-0.8.3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/tutorials/add_your_own.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/tutorials/datacache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/tutorials/graphs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/tutorials/integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/tutorials/pyg_integration.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/tutorials/save_and_load.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/tutorials/transformer_finetuning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/tutorials/types_of_featurizers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-04 14:06:34.000000 molfeat-0.8.3/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-04 14:06:34.000000 molfeat-0.8.3/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-04 14:06:34.000000 molfeat-0.8.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.843444 molfeat-0.8.3/molfeat/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.847444 molfeat-0.8.3/molfeat/calc/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/_atom_bond_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/_map4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/_mhfp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/cats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    22488 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/skeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/calc/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.847444 molfeat-0.8.3/molfeat/data/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/data/cats_features.fdef
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/data/elements.xz
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/data/elements_completed.xz
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/data/origin.xz
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/data/skey_parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.847444 molfeat-0.8.3/molfeat/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/plugins/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/plugins/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/plugins/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.847444 molfeat-0.8.3/molfeat/store/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/store/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/store/modelcard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/store/modelstore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.851444 molfeat-0.8.3/molfeat/trans/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33566 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.851444 molfeat-0.8.3/molfeat/trans/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27395 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/graph/adj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.851444 molfeat-0.8.3/molfeat/trans/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/pretrained/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/pretrained/dgl_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/pretrained/fcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/pretrained/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/pretrained/hf_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.851444 molfeat-0.8.3/molfeat/trans/struct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/struct/esm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/trans/struct/prot1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.855444 molfeat-0.8.3/molfeat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25556 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/utils/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-04 14:06:34.000000 molfeat-0.8.3/molfeat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.843444 molfeat-0.8.3/molfeat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-04 14:07:51.000000 molfeat-0.8.3/molfeat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-04 14:07:51.000000 molfeat-0.8.3/molfeat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:07:51.000000 molfeat-0.8.3/molfeat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:07:39.000000 molfeat-0.8.3/molfeat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-04 14:07:51.000000 molfeat-0.8.3/molfeat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 14:07:51.000000 molfeat-0.8.3/molfeat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.855444 molfeat-0.8.3/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-04 14:06:34.000000 molfeat-0.8.3/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-04 14:06:34.000000 molfeat-0.8.3/plugin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-04 14:06:34.000000 molfeat-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-04 14:06:34.000000 molfeat-0.8.3/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 14:07:51.855444 molfeat-0.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:07:51.855444 molfeat-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_atom_bond_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_pharmacophore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_prot_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-04 14:06:34.000000 molfeat-0.8.3/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.851633 molfeat-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-07 16:16:13.000000 molfeat-0.8.4/.authors.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.835633 molfeat-0.8.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.835633 molfeat-0.8.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/ISSUE_TEMPLATE/1_bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/ISSUE_TEMPLATE/2_refactor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/ISSUE_TEMPLATE/3_documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.835633 molfeat-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-07 16:16:13.000000 molfeat-0.8.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-07 16:16:13.000000 molfeat-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-07 16:16:13.000000 molfeat-0.8.4/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-07 16:16:13.000000 molfeat-0.8.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-07 16:16:13.000000 molfeat-0.8.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-07 16:16:13.000000 molfeat-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-07 16:17:34.851633 molfeat-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-07 16:16:13.000000 molfeat-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.835633 molfeat-0.8.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.839633 molfeat-0.8.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.calc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.store.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.trans.base.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.trans.concat.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.trans.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.trans.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.trans.pretrained.dgl_pretrained.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.trans.pretrained.fcd.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.trans.pretrained.graphormer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.trans.pretrained.hf_transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.trans.struct.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/api/molfeat.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.831633 molfeat-0.8.4/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.839633 molfeat-0.8.4/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/assets/css/custom-molfeat.css
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.839633 molfeat-0.8.4/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)   107857 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/benchmark.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.839633 molfeat-0.8.4/docs/developers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/developers/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/developers/create-plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/developers/register-plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.839633 molfeat-0.8.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18421 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.839633 molfeat-0.8.4/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/tutorials/add_your_own.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/tutorials/datacache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37937 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/tutorials/graphs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/tutorials/integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59383 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/tutorials/pyg_integration.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/tutorials/save_and_load.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/tutorials/transformer_finetuning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/tutorials/types_of_featurizers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-07 16:16:13.000000 molfeat-0.8.4/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-07 16:16:13.000000 molfeat-0.8.4/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-07 16:16:13.000000 molfeat-0.8.4/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.839633 molfeat-0.8.4/molfeat/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.843633 molfeat-0.8.4/molfeat/calc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/_atom_bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/_map4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/_mhfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/cats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27461 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22488 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/skeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/calc/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.843633 molfeat-0.8.4/molfeat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/data/cats_features.fdef
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/data/elements.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/data/elements_completed.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/data/origin.xz
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/data/skey_parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.843633 molfeat-0.8.4/molfeat/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/plugins/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/plugins/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/plugins/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.843633 molfeat-0.8.4/molfeat/store/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/store/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/store/modelcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/store/modelstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.847633 molfeat-0.8.4/molfeat/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33035 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.847633 molfeat-0.8.4/molfeat/trans/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27395 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/graph/adj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.847633 molfeat-0.8.4/molfeat/trans/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/pretrained/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/pretrained/dgl_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/pretrained/fcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/pretrained/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/pretrained/hf_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.847633 molfeat-0.8.4/molfeat/trans/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/struct/esm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/trans/struct/prot1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.847633 molfeat-0.8.4/molfeat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25556 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/utils/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-07 16:16:13.000000 molfeat-0.8.4/molfeat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.843633 molfeat-0.8.4/molfeat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-07 16:17:34.000000 molfeat-0.8.4/molfeat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-07 16:17:34.000000 molfeat-0.8.4/molfeat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:17:34.000000 molfeat-0.8.4/molfeat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:17:22.000000 molfeat-0.8.4/molfeat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-07 16:17:34.000000 molfeat-0.8.4/molfeat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 16:17:34.000000 molfeat-0.8.4/molfeat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.847633 molfeat-0.8.4/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-07 16:16:13.000000 molfeat-0.8.4/news/TEMPLATE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-07 16:16:13.000000 molfeat-0.8.4/plugin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-07 16:16:13.000000 molfeat-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-07 16:16:13.000000 molfeat-0.8.4/rever.xsh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:17:34.851633 molfeat-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:17:34.851633 molfeat-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_atom_bond_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_pharmacophore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_prot_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-07 16:16:13.000000 molfeat-0.8.4/tests/test_viz.py
```

### Comparing `molfeat-0.8.3/.authors.yml` & `molfeat-0.8.4/.authors.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 - name: maclandrol
   email: emmanuel.noutahi@hotmail.ca
-  num_commits: 28
+  num_commits: 29
   first_commit: 2021-04-06 11:53:10
 - name: Cas Wognum
   email: caswognum@outlook.com
   aliases:
   - cwognum
-  num_commits: 23
+  num_commits: 28
   first_commit: 2023-03-20 13:05:13
 - name: Hadrien Mary
   email: hadrien.mary@gmail.com
   alternate_emails:
   - hadim@users.noreply.github.com
   num_commits: 23
   first_commit: 2023-03-21 12:50:42
 - name: Therence
   email: 38595485+Therence1@users.noreply.github.com
   num_commits: 2
   first_commit: 2023-03-26 23:33:17
 - name: Honore Hounwanou
   email: mercuryseries@gmail.com
-  num_commits: 1
+  num_commits: 3
   first_commit: 2023-04-03 19:51:15
 - name: Saurav Maheshkar
   github: SauravMaheshkar
   email: sauravvmaheshkar@gmail.com
   num_commits: 1
   first_commit: 2023-04-04 07:44:44
```

### Comparing `molfeat-0.8.3/.github/CODE_OF_CONDUCT.md` & `molfeat-0.8.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.github/ISSUE_TEMPLATE/1_bug_report.yaml` & `molfeat-0.8.4/.github/ISSUE_TEMPLATE/1_bug_report.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.github/ISSUE_TEMPLATE/2_refactor.yaml` & `molfeat-0.8.4/.github/ISSUE_TEMPLATE/2_refactor.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.github/ISSUE_TEMPLATE/3_documentation.yaml` & `molfeat-0.8.4/.github/ISSUE_TEMPLATE/3_documentation.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml` & `molfeat-0.8.4/.github/ISSUE_TEMPLATE/4_featurizer_request.yaml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.github/ISSUE_TEMPLATE/config.yml` & `molfeat-0.8.4/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.github/workflows/doc.yml` & `molfeat-0.8.4/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.github/workflows/release.yml` & `molfeat-0.8.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.github/workflows/test.yml` & `molfeat-0.8.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.gitignore` & `molfeat-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/.mailmap` & `molfeat-0.8.4/.mailmap`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/CHANGELOG.rst` & `molfeat-0.8.4/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,36 @@
 ==================
 molfeat Change Log
 ==================
 
 .. current developments
 
+v0.8.4
+====================
+
+**Added:**
+
+* Add Google Analytics support.
+
+**Removed:**
+
+* Remove support for the `np.float128` dtype (issue #26)
+
+**Fixed:**
+
+* Color bug of the search input bar
+
+**Authors:**
+
+* Cas Wognum
+* Honore Hounwanou
+* maclandrol
+
+
+
 v0.8.3
 ====================
 
 **Added:**
 
 * More documentation and tutorials
 * pip dependencies and optional dependencies in pyproject.toml
```

### Comparing `molfeat-0.8.3/LICENSE` & `molfeat-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/PKG-INFO` & `molfeat-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.3
+Version: 0.8.4
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.3 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.4 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
```

### Comparing `molfeat-0.8.3/README.md` & `molfeat-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/assets/css/custom-molfeat.css` & `molfeat-0.8.4/docs/assets/css/custom-molfeat.css`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,18 @@
   color: rgb(255, 255, 255) !important;
 }
 
 .md-search__form {
   background-color: rgba(255, 255, 255, 0.2);
 }
 
+.md-search__input {
+  color: #222222 !important;
+}
+
 .md-header__topic {
   color: rgb(255, 255, 255);
   font-size: 1.4em;
 }
 
 /* Increase the size of the logo */
 .md-header__button.md-logo img,
```

### Comparing `molfeat-0.8.3/docs/assets/css/custom.css` & `molfeat-0.8.4/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/benchmark.ipynb` & `molfeat-0.8.4/docs/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/developers/contribute.md` & `molfeat-0.8.4/docs/developers/contribute.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/developers/create-plugin.md` & `molfeat-0.8.4/docs/developers/create-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/developers/register-plugin.md` & `molfeat-0.8.4/docs/developers/register-plugin.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/images/logo-black.png` & `molfeat-0.8.4/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/images/logo-black.svg` & `molfeat-0.8.4/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/images/logo-title.svg` & `molfeat-0.8.4/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/images/logo.png` & `molfeat-0.8.4/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/images/logo.svg` & `molfeat-0.8.4/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/index.md` & `molfeat-0.8.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/tutorials/add_your_own.ipynb` & `molfeat-0.8.4/docs/tutorials/add_your_own.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/tutorials/datacache.ipynb` & `molfeat-0.8.4/docs/tutorials/datacache.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/tutorials/graphs.ipynb` & `molfeat-0.8.4/docs/tutorials/graphs.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/tutorials/integrations.ipynb` & `molfeat-0.8.4/docs/tutorials/integrations.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/tutorials/pyg_integration.ipynb` & `molfeat-0.8.4/docs/tutorials/pyg_integration.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/tutorials/save_and_load.ipynb` & `molfeat-0.8.4/docs/tutorials/save_and_load.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/tutorials/transformer_finetuning.ipynb` & `molfeat-0.8.4/docs/tutorials/transformer_finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/tutorials/types_of_featurizers.ipynb` & `molfeat-0.8.4/docs/tutorials/types_of_featurizers.ipynb`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/docs/usage.md` & `molfeat-0.8.4/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/env.yml` & `molfeat-0.8.4/env.yml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/mkdocs.yml` & `molfeat-0.8.4/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,17 @@
   logo: images/logo.svg
 
 extra_css:
   - assets/css/custom.css
   - assets/css/custom-molfeat.css
   - assets/css/tweak-width.css
 
+extra_javascript:
+  - assets/js/google-analytics.js
+
 markdown_extensions:
   - admonition
   - markdown_include.include
   - pymdownx.emoji
   - pymdownx.highlight
   - pymdownx.magiclink
   - pymdownx.superfences
```

### Comparing `molfeat-0.8.3/molfeat/calc/__init__.py` & `molfeat-0.8.4/molfeat/calc/__init__.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/_atom_bond_features.py` & `molfeat-0.8.4/molfeat/calc/_atom_bond_features.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/_map4.py` & `molfeat-0.8.4/molfeat/calc/_map4.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/_mhfp.py` & `molfeat-0.8.4/molfeat/calc/_mhfp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/atom.py` & `molfeat-0.8.4/molfeat/calc/atom.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/base.py` & `molfeat-0.8.4/molfeat/calc/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/bond.py` & `molfeat-0.8.4/molfeat/calc/bond.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/cats.py` & `molfeat-0.8.4/molfeat/calc/cats.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/descriptors.py` & `molfeat-0.8.4/molfeat/calc/descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/fingerprints.py` & `molfeat-0.8.4/molfeat/calc/fingerprints.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/pharmacophore.py` & `molfeat-0.8.4/molfeat/calc/pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/shape.py` & `molfeat-0.8.4/molfeat/calc/shape.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/skeys.py` & `molfeat-0.8.4/molfeat/calc/skeys.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/calc/tree.py` & `molfeat-0.8.4/molfeat/calc/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/data/cats_features.fdef` & `molfeat-0.8.4/molfeat/data/cats_features.fdef`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/data/elements.xz` & `molfeat-0.8.4/molfeat/data/elements.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/data/elements_completed.xz` & `molfeat-0.8.4/molfeat/data/elements_completed.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/data/origin.xz` & `molfeat-0.8.4/molfeat/data/origin.xz`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/data/skey_parameters.csv` & `molfeat-0.8.4/molfeat/data/skey_parameters.csv`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/plugins/entry_point.py` & `molfeat-0.8.4/molfeat/plugins/entry_point.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/plugins/factories.py` & `molfeat-0.8.4/molfeat/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/store/loader.py` & `molfeat-0.8.4/molfeat/store/loader.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/store/modelcard.py` & `molfeat-0.8.4/molfeat/store/modelcard.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/store/modelstore.py` & `molfeat-0.8.4/molfeat/store/modelstore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/base.py` & `molfeat-0.8.4/molfeat/trans/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Dict
 from collections.abc import Iterable
 
 import abc
 import copy
 import joblib
 import json
+
 import yaml
 import fsspec
 import pandas as pd
 import datamol as dm
 import numpy as np
 
 from rdkit.Chem import rdchem
@@ -29,21 +30,19 @@
 from molfeat.utils import datatype
 from molfeat.utils.cache import _Cache, FileCache, MPDataCache
 from molfeat.utils.cache import CacheList
 from molfeat.utils.commons import fn_to_hex
 from molfeat.utils.commons import hex_to_fn
 from molfeat.utils.parsing import get_input_args
 from molfeat.utils.parsing import import_from_string
-from molfeat.utils.state import DTYPES_MAPPING
-from molfeat.utils.state import DTYPES_MAPPING_REVERSE
+from molfeat.utils.state import map_dtype
 from molfeat.utils.state import ATOM_FEATURIZER_MAPPING
 from molfeat.utils.state import BOND_FEATURIZER_MAPPING
 from molfeat.utils.state import ATOM_FEATURIZER_MAPPING_REVERSE
 from molfeat.utils.state import BOND_FEATURIZER_MAPPING_REVERSE
-from molfeat.utils.state import get_type_mapping
 
 _TRANSFORMERS = {}
 
 
 class _TransformerMeta(abc.ABCMeta):
     """Metaclass to register all transformers automatically"""
 
@@ -510,21 +509,17 @@
 
         if getattr(self, "_input_args") is None:
             raise ValueError(f"Cannot save state for this transformer '{self.__class__.__name__}'")
 
         # Process the input arguments before building the state
         args = copy.deepcopy(self._input_args)
 
-        ## Deal with dtype
+        # Deal with dtype
         if "dtype" in args and not isinstance(args["dtype"], str):
-            if args["dtype"] not in DTYPES_MAPPING:
-                raise ValueError(
-                    f"Invalid dtype {args['dtype']}. Valid dtypes are {DTYPES_MAPPING.keys()}"
-                )
-            args["dtype"] = DTYPES_MAPPING[args["dtype"]]
+            args["dtype"] = map_dtype(args["dtype"])
 
         ## Deal with graph atom/bond featurizers
         # NOTE(hadim): it's important to highlight that atom/bond featurizers can't be
         # customized with this logic.
         if args.get("atom_featurizer") is not None:
             if hasattr(args.get("atom_featurizer"), "to_state_dict"):
                 args["atom_featurizer"] = args["atom_featurizer"].to_state_dict()
@@ -605,22 +600,17 @@
         if isinstance(transformer_class, str):
             # Get the transformer class from its path
             transformer_class = import_from_string(transformer_class)
 
         # Process the state as needed
         args = state.get("args", {})
 
-        ## Deal with dtype
-        if "dtype" in args:
-            if args["dtype"] not in DTYPES_MAPPING_REVERSE:
-                raise ValueError(
-                    f"Invalid dtype {args['dtype']}. Valid dtypes are"
-                    f" {DTYPES_MAPPING_REVERSE.keys()}"
-                )
-            args["dtype"] = DTYPES_MAPPING_REVERSE[args["dtype"]]
+        # Deal with dtype
+        if "dtype" in args and isinstance(args["dtype"], str):
+            args["dtype"] = map_dtype(args["dtype"])
 
         ## Deal with graph atom/bond featurizers
         if args.get("atom_featurizer") is not None:
             if not args.get("_atom_featurizer_is_pickled"):
                 klass_name = args["atom_featurizer"].get("name")
                 args["atom_featurizer"] = ATOM_FEATURIZER_MAPPING_REVERSE[
                     klass_name
```

### Comparing `molfeat-0.8.3/molfeat/trans/concat.py` & `molfeat-0.8.4/molfeat/trans/concat.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/fp.py` & `molfeat-0.8.4/molfeat/trans/fp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/graph/adj.py` & `molfeat-0.8.4/molfeat/trans/graph/adj.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/graph/tree.py` & `molfeat-0.8.4/molfeat/trans/graph/tree.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/pretrained/base.py` & `molfeat-0.8.4/molfeat/trans/pretrained/base.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/pretrained/dgl_pretrained.py` & `molfeat-0.8.4/molfeat/trans/pretrained/dgl_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/pretrained/fcd.py` & `molfeat-0.8.4/molfeat/trans/pretrained/fcd.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/pretrained/graphormer.py` & `molfeat-0.8.4/molfeat/trans/pretrained/graphormer.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/pretrained/hf_transformers.py` & `molfeat-0.8.4/molfeat/trans/pretrained/hf_transformers.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/struct/esm.py` & `molfeat-0.8.4/molfeat/trans/struct/esm.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/trans/struct/prot1D.py` & `molfeat-0.8.4/molfeat/trans/struct/prot1D.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/cache.py` & `molfeat-0.8.4/molfeat/utils/cache.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/commons.py` & `molfeat-0.8.4/molfeat/utils/commons.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/const.py` & `molfeat-0.8.4/molfeat/utils/const.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/converters.py` & `molfeat-0.8.4/molfeat/utils/converters.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/datatype.py` & `molfeat-0.8.4/molfeat/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/log.py` & `molfeat-0.8.4/molfeat/utils/log.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/parsing.py` & `molfeat-0.8.4/molfeat/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/pooler.py` & `molfeat-0.8.4/molfeat/utils/pooler.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/requires.py` & `molfeat-0.8.4/molfeat/utils/requires.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat/utils/state.py` & `molfeat-0.8.4/molfeat/utils/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     torch.int32: "torch.int32",
     torch.int64: "torch.int64",
     torch.uint8: "torch.uint8",
     torch.bool: "torch.bool",
     np.float16: "np.float16",
     np.float32: "np.float32",
     np.float64: "np.float64",
-    np.float128: "np.float128",
     np.int8: "np.int8",
     np.int16: "np.int16",
     np.int32: "np.int32",
     np.int64: "np.int64",
     np.uint8: "np.uint8",
     np.uint16: "np.uint16",
     np.uint32: "np.uint32",
@@ -58,20 +57,27 @@
     DGLCanonicalBondCalculator: "DGLCanonicalBondCalculator",
     DGLWeaveEdgeCalculator: "DGLWeaveEdgeCalculator",
 }
 
 BOND_FEATURIZER_MAPPING_REVERSE = {v: k for k, v in BOND_FEATURIZER_MAPPING.items()}
 
 
-def get_type_mapping(obj, mapping):
-    for k, v in mapping.items():
-        if type(obj) is k:
-            return v
+def map_dtype(dtype: Optional[Union[str, torch.dtype, np.dtype]]):
+    """Map a dtype to a string representation or the other way around"""
 
-    raise ValueError(f"No mapping found for obj {obj}. Valid types are {mapping.keys()}")
+    if isinstance(dtype, str):
+        mapping = DTYPES_MAPPING_REVERSE
+    else:
+        mapping = DTYPES_MAPPING
+
+    if dtype not in mapping:
+        msg = f"{dtype} is not a valid dtype. The valid dtypes are {list(mapping.keys())}."
+        raise ValueError(msg)
+
+    return mapping[dtype]
 
 
 def compare_state(
     state_dict_1, state_dict_2, allow_version_level: Optional[Union[str, int]] = None
 ):
     """Compare two state dict and allow version matching
     Args:
```

### Comparing `molfeat-0.8.3/molfeat/viz.py` & `molfeat-0.8.4/molfeat/viz.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/molfeat.egg-info/PKG-INFO` & `molfeat-0.8.4/molfeat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molfeat
-Version: 0.8.3
+Version: 0.8.4
 Summary: molfeat - the hub for all your molecular featurizers
 Author-email: Emmanuel Noutahi <emmanuel.noutahi@hotmail.ca>
 License: Apache
 Project-URL: Website, https://molfeat.datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/molfeat
 Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: molfeat Version: 0.8.3 Summary: molfeat - the hub
+Metadata-Version: 2.1 Name: molfeat Version: 0.8.4 Summary: molfeat - the hub
 for all your molecular featurizers Author-email: Emmanuel Noutahi
 noutahi@hotmail.ca> License: Apache Project-URL: Website, https://
 molfeat.datamol.io Project-URL: Source Code, https://github.com/datamol-io/
 molfeat Project-URL: Bug Tracker, https://github.com/datamol-io/molfeat/issues
 Project-URL: Documentation, https://molfeat-docs.datamol.io/ Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Healthcare Industry Classifier:
```

### Comparing `molfeat-0.8.3/molfeat.egg-info/SOURCES.txt` & `molfeat-0.8.4/molfeat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 docs/api/molfeat.trans.pretrained.hf_transformers.md
 docs/api/molfeat.trans.struct.md
 docs/api/molfeat.utils.md
 docs/api/molfeat.viz.md
 docs/assets/css/custom-molfeat.css
 docs/assets/css/custom.css
 docs/assets/css/tweak-width.css
+docs/assets/js/google-analytics.js
 docs/developers/contribute.md
 docs/developers/create-plugin.md
 docs/developers/register-plugin.md
 docs/images/logo-black.png
 docs/images/logo-black.svg
 docs/images/logo-title.svg
 docs/images/logo.png
```

### Comparing `molfeat-0.8.3/pyproject.toml` & `molfeat-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/tests/test_atom_bond_calculator.py` & `molfeat-0.8.4/tests/test_atom_bond_calculator.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/tests/test_descriptors.py` & `molfeat-0.8.4/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/tests/test_fp.py` & `molfeat-0.8.4/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/tests/test_graphs.py` & `molfeat-0.8.4/tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/tests/test_pharmacophore.py` & `molfeat-0.8.4/tests/test_pharmacophore.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/tests/test_pretrained.py` & `molfeat-0.8.4/tests/test_pretrained.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/tests/test_prot_embed.py` & `molfeat-0.8.4/tests/test_prot_embed.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/tests/test_state.py` & `molfeat-0.8.4/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `molfeat-0.8.3/tests/test_utils.py` & `molfeat-0.8.4/tests/test_utils.py`

 * *Files identical despite different names*

