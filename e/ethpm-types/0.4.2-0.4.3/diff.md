# Comparing `tmp/ethpm-types-0.4.2.tar.gz` & `tmp/ethpm-types-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpm-types-0.4.2.tar", last modified: Tue Apr  4 16:08:15 2023, max compression
+gzip compressed data, was "ethpm-types-0.4.3.tar", last modified: Fri Apr  7 18:12:22 2023, max compression
```

## Comparing `ethpm-types-0.4.2.tar` & `ethpm-types-0.4.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.993711 ethpm-types-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.981711 ethpm-types-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.981711 ethpm-types-0.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.981711 ethpm-types-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-04 16:08:15.993711 ethpm-types-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.981711 ethpm-types-0.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.985711 ethpm-types-0.4.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.985711 ethpm-types-0.4.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.985711 ethpm-types-0.4.2/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/methoddocs/abi.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/methoddocs/contract_type.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/methoddocs/manifest.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/methoddocs/source.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.985711 ethpm-types-0.4.2/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.985711 ethpm-types-0.4.2/ethpm_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15290 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/ethpm_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 16:08:15.000000 ethpm-types-0.4.2/ethpm_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.985711 ethpm-types-0.4.2/ethpm_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-04 16:08:15.000000 ethpm-types-0.4.2/ethpm_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-04 16:08:15.000000 ethpm-types-0.4.2/ethpm_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:08:15.000000 ethpm-types-0.4.2/ethpm_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:08:15.000000 ethpm-types-0.4.2/ethpm_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-04 16:08:15.000000 ethpm-types-0.4.2/ethpm_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 16:08:15.000000 ethpm-types-0.4.2/ethpm_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-04 16:08:15.993711 ethpm-types-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.985711 ethpm-types-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:08:15.993711 ethpm-types-0.4.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/data/OpenZeppelinContracts.json
--rw-r--r--   0 runner    (1001) docker     (123)    20063 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/data/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/data/TestStrategy.srcmap
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/data/VyperContract.json
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_cairo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_hexbytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_package_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_pc_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-04 16:07:56.000000 ethpm-types-0.4.2/tests/test_sourcemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.951879 ethpm-types-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-07 18:12:22.951879 ethpm-types-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/abi.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/contract_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.939879 ethpm-types-0.4.3/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.943879 ethpm-types-0.4.3/ethpm_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/ethpm_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.943879 ethpm-types-0.4.3/ethpm_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 18:12:22.000000 ethpm-types-0.4.3/ethpm_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 18:12:22.951879 ethpm-types-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.943879 ethpm-types-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:12:22.951879 ethpm-types-0.4.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/data/OpenZeppelinContracts.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/data/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/data/TestStrategy.srcmap
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/data/VyperContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_hexbytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_package_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_pc_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-07 18:12:05.000000 ethpm-types-0.4.3/tests/test_sourcemap.py
```

### Comparing `ethpm-types-0.4.2/.github/ISSUE_TEMPLATE/bug.md` & `ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.github/ISSUE_TEMPLATE/feature.md` & `ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.github/ISSUE_TEMPLATE/work-item.md` & `ethpm-types-0.4.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.github/release-drafter.yml` & `ethpm-types-0.4.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.github/workflows/commitlint.yaml` & `ethpm-types-0.4.3/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.github/workflows/docs.yaml` & `ethpm-types-0.4.3/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.github/workflows/prtitle.yaml` & `ethpm-types-0.4.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.github/workflows/publish.yaml` & `ethpm-types-0.4.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.github/workflows/test.yaml` & `ethpm-types-0.4.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.gitignore` & `ethpm-types-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/.pre-commit-config.yaml` & `ethpm-types-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/CONTRIBUTING.md` & `ethpm-types-0.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/LICENSE` & `ethpm-types-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/PKG-INFO` & `ethpm-types-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.4.2
+Version: 0.4.3
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ethpm-types-0.4.2/README.md` & `ethpm-types-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/build_docs.py` & `ethpm-types-0.4.3/build_docs.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/docs/_static/custom.css` & `ethpm-types-0.4.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/docs/_static/custom.js` & `ethpm-types-0.4.3/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/docs/_templates/layout.html` & `ethpm-types-0.4.3/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/docs/conf.py` & `ethpm-types-0.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/docs/favicon.ico` & `ethpm-types-0.4.3/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/docs/logo.gif` & `ethpm-types-0.4.3/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/ethpm_types/__init__.py` & `ethpm-types-0.4.3/ethpm_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/ethpm_types/abi.py` & `ethpm-types-0.4.3/ethpm_types/abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/ethpm_types/ast.py` & `ethpm-types-0.4.3/ethpm_types/ast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import List, Optional, Tuple, Union
+from typing import Iterator, List, Optional, Tuple, Union
 
 from pydantic import root_validator
 
 from ethpm_types.base import BaseModel
 from ethpm_types.sourcemap import SourceMapItem
 
 SourceLocation = Tuple[int, int, int, int]
@@ -110,14 +110,31 @@
         All function nodes defined at this level.
 
         **NOTE**: This is only populated on a ``Module`` AST node.
         """
 
         return [n for n in self.children if n.ast_type == "FunctionDef"]
 
+    def __repr__(self) -> str:
+        return str(self)
+
+    def __str__(self):
+        num_children = len(self.children)
+        stats = "leaf" if num_children == 0 else f"children={num_children}"
+        return f"<{self.ast_type}Node {stats}>"
+
+    def iter_nodes(self) -> Iterator["ASTNode"]:
+        """
+        Yield through all nodes in the tree, including this one.
+        """
+
+        yield self
+        for node in self.children:
+            yield from node.iter_nodes()
+
     def get_node(self, src: SourceMapItem) -> Optional["ASTNode"]:
         """
         Get a node by source.
 
         Args:
             src (:class:`~ethpm_types.sourcemap.SourceMapItem`): The source map
               item to seek in the AST.
```

### Comparing `ethpm-types-0.4.2/ethpm_types/base.py` & `ethpm-types-0.4.3/ethpm_types/base.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/ethpm_types/contract_type.py` & `ethpm-types-0.4.3/ethpm_types/contract_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     Adds selection by name, selector and keccak(selector).
     """
 
     def __init__(
         self,
         iterable: Optional[Iterable[T]] = None,
         *,
-        selector_id_size=32,
+        selector_id_size: int = 32,
         selector_hash_fn: Optional[Callable[[str], bytes]] = None,
     ):
         self._selector_id_size = selector_id_size
         self._selector_hash_fn = selector_hash_fn
         super().__init__(iterable or ())
 
     @singledispatchmethod
@@ -358,82 +358,85 @@
     def view_methods(self) -> ABIList[MethodABI]:
         """
         The call-methods (read-only method, non-payable methods) defined in a smart contract.
 
         Returns:
             List[:class:`~ethpm_types.abi.ABI`]
         """
-
-        method_abis = [
-            abi for abi in self.abi if isinstance(abi, MethodABI) and not abi.is_stateful
-        ]
-        for abi in method_abis:
-            abi.contract_type = self
-
-        return ABIList(
-            method_abis,
-            selector_id_size=4,
-            selector_hash_fn=self._selector_hash_fn,
+        return self._get_abis(
+            selector_id_size=4, filter_fn=lambda x: isinstance(x, MethodABI) and not x.is_stateful
         )
 
     @property
     def mutable_methods(self) -> ABIList[MethodABI]:
         """
         The transaction-methods (stateful or payable methods) defined in a smart contract.
 
         Returns:
             List[:class:`~ethpm_types.abi.ABI`]
         """
-
-        method_abis = [abi for abi in self.abi if isinstance(abi, MethodABI) and abi.is_stateful]
-        for abi in method_abis:
-            abi.contract_type = self
-
-        return ABIList(
-            method_abis,
-            selector_id_size=4,
-            selector_hash_fn=self._selector_hash_fn,
+        return self._get_abis(
+            selector_id_size=4, filter_fn=lambda x: isinstance(x, MethodABI) and x.is_stateful
         )
 
     @property
     def events(self) -> ABIList[EventABI]:
         """
         The events defined in a smart contract.
 
         Returns:
-            List[:class:`~ethpm_types.abi.ABI`]
+            :class:`~ethpm_types.contract_type.ABIList`
         """
+        return self._get_abis(filter_fn=lambda a: isinstance(a, EventABI))
 
-        event_abis = [abi for abi in self.abi if isinstance(abi, EventABI)]
-        for abi in event_abis:
-            abi.contract_type = self
+    @property
+    def errors(self) -> ABIList[ErrorABI]:
+        """
+        The errors defined in a smart contract.
 
-        return ABIList(
-            event_abis,
-            selector_hash_fn=self._selector_hash_fn,
-        )
+        Returns:
+            :class:`~ethpm_types.contract_type.ABIList`
+        """
+        return self._get_abis(selector_id_size=4, filter_fn=lambda a: isinstance(a, ErrorABI))
 
     @property
     def methods(self) -> ABIList:
-        method_abis = [abi for abi in self.abi if isinstance(abi, MethodABI)]
-        for abi in method_abis:
-            abi.contract_type = self
+        """
+        All methods defined in a smart contract.
 
-        return ABIList(
-            method_abis,
-            selector_id_size=4,
-            selector_hash_fn=self._selector_hash_fn,
-        )
+        Returns:
+            :class:`~ethpm_types.contract_type.ABIList`
+        """
+        return self._get_abis(selector_id_size=4, filter_fn=lambda a: isinstance(a, MethodABI))
 
     def _selector_hash_fn(self, selector: str) -> bytes:
         # keccak is the default on most ecosystems, other ecosystems can subclass to override it
         from eth_utils import keccak
 
         return keccak(text=selector)
 
+    def _get_abis(
+        self,
+        selector_id_size: int = 32,
+        filter_fn: Optional[Callable[[ABI], bool]] = None,
+    ):
+        def noop(a: ABI) -> bool:
+            return True
+
+        filter_fn = filter_fn or noop
+        method_abis = [abi for abi in self.abi if filter_fn(abi)]
+        for abi in method_abis:
+            abi.contract_type = self
+
+        return ABIList(
+            method_abis,
+            selector_id_size=selector_id_size,
+            selector_hash_fn=self._selector_hash_fn,
+        )
+
 
 class BIP122_URI(str):
     """
     A URI scheme for looking up blocks.
     `BIP-122 <https://github.com/bitcoin/bips/blob/master/bip-0122.mediawiki>`__.
 
     URI Format::
```

### Comparing `ethpm-types-0.4.2/ethpm_types/manifest.py` & `ethpm-types-0.4.3/ethpm_types/manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/ethpm_types/source.py` & `ethpm-types-0.4.3/ethpm_types/source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/ethpm_types/sourcemap.py` & `ethpm-types-0.4.3/ethpm_types/sourcemap.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/ethpm_types/utils.py` & `ethpm-types-0.4.3/ethpm_types/utils.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/ethpm_types.egg-info/PKG-INFO` & `ethpm-types-0.4.3/ethpm_types.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.4.2
+Version: 0.4.3
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ethpm-types-0.4.2/ethpm_types.egg-info/SOURCES.txt` & `ethpm-types-0.4.3/ethpm_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/ethpm_types.egg-info/requires.txt` & `ethpm-types-0.4.3/ethpm_types.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/pyproject.toml` & `ethpm-types-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/setup.py` & `ethpm-types-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/conftest.py` & `ethpm-types-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/data/OpenZeppelinContracts.json` & `ethpm-types-0.4.3/tests/data/OpenZeppelinContracts.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/data/SolidityContract.json` & `ethpm-types-0.4.3/tests/data/SolidityContract.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965986394557823%*

 * *Differences: {"'abi'": "{insert: [(2, OrderedDict([('inputs', [OrderedDict([('internalType', 'address'), "*

 * *          "('name', 'addr'), ('type', 'address')]), OrderedDict([('internalType', 'uint256'), "*

 * *          "('name', 'counter'), ('type', 'uint256')])]), ('name', 'FooError'), ('type', "*

 * *          "'error')]))]}"}*

```diff
@@ -21,14 +21,30 @@
                     "type": "uint256"
                 }
             ],
             "name": "NumberChange",
             "type": "event"
         },
         {
+            "inputs": [
+                {
+                    "internalType": "address",
+                    "name": "addr",
+                    "type": "address"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "counter",
+                    "type": "uint256"
+                }
+            ],
+            "name": "FooError",
+            "type": "error"
+        },
+        {
             "inputs": [],
             "name": "getAddressList",
             "outputs": [
                 {
                     "internalType": "address[2]",
                     "name": "",
                     "type": "address[2]"
```

### Comparing `ethpm-types-0.4.2/tests/data/TestStrategy.srcmap` & `ethpm-types-0.4.3/tests/data/TestStrategy.srcmap`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/data/VyperContract.json` & `ethpm-types-0.4.3/tests/data/VyperContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/test_ast.py` & `ethpm-types-0.4.3/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/test_cairo.py` & `ethpm-types-0.4.3/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/test_contract_type.py` & `ethpm-types-0.4.3/tests/test_contract_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 from pathlib import Path
 from typing import Dict
 
 import pytest
 from eth_utils import keccak
 
 from ethpm_types import ContractType
-from ethpm_types.abi import ABI, EventABI, MethodABI
+from ethpm_types.abi import ABI, ErrorABI, EventABI, MethodABI
 
 CONTRACT_NAMES = ("SolidityContract.json", "VyperContract.json")
 DATA_FILES = {
     p.name: p for p in (Path(__file__).parent / "data").iterdir() if p.name in CONTRACT_NAMES
 }
 MUTABLE_METHOD_SELECTOR_BYTES = keccak(text="setNumber(uint256)")
 VIEW_METHOD_SELECTOR_BYTES = keccak(text="getStruct()")
 EVENT_SELECTOR_BYTES = keccak(text="NumberChange(uint256,uint256)")
+ERROR_SELECTOR_BYTES = keccak(text="FooError(address,uint256)")
 
 
 view_selector_parametrization = pytest.mark.parametrize(
     "selector",
     (
         "getStruct",
         "getStruct()",
@@ -46,14 +47,25 @@
         "NumberChange(uint256,uint256)",
         EVENT_SELECTOR_BYTES,
         EVENT_SELECTOR_BYTES[:32],
         f"0x{EVENT_SELECTOR_BYTES.hex()}",
         f"0x{EVENT_SELECTOR_BYTES[:32].hex()}",
     ),
 )
+error_selector_parametrization = pytest.mark.parametrize(
+    "selector",
+    (
+        "FooError",
+        "FooError(address,uint256)",
+        ERROR_SELECTOR_BYTES,
+        ERROR_SELECTOR_BYTES[:32],
+        f"0x{ERROR_SELECTOR_BYTES.hex()}",
+        f"0x{ERROR_SELECTOR_BYTES[:32].hex()}",
+    ),
+)
 
 
 @pytest.fixture
 def solidity_contract():
     return _get_contract(CONTRACT_NAMES[0])
 
 
@@ -171,14 +183,23 @@
     contract_type = ContractType.parse_obj(vyper_contract)
     assert selector in contract_type.events
     event = contract_type.events[selector]
     assert isinstance(event, EventABI)
     assert event.name == "NumberChange"
 
 
+@error_selector_parametrization
+def test_elect_and_contains_error_by_name_and_selectors(selector, solidity_contract):
+    contract_type = ContractType.parse_obj(solidity_contract)
+    assert selector in contract_type.errors
+    event = contract_type.errors[selector]
+    assert isinstance(event, ErrorABI)
+    assert event.name == "FooError"
+
+
 def test_select_and_contains_by_abi(vyper_contract):
     contract_type = ContractType.parse_obj(vyper_contract)
     event = contract_type.events[0]
     view = contract_type.view_methods[0]
     mutable = contract_type.mutable_methods[0]
     assert contract_type.events[event] == event
     assert contract_type.view_methods[view] == view
```

### Comparing `ethpm-types-0.4.2/tests/test_hexbytes.py` & `ethpm-types-0.4.3/tests/test_hexbytes.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/test_package_manifest.py` & `ethpm-types-0.4.3/tests/test_package_manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/test_pc_map.py` & `ethpm-types-0.4.3/tests/test_pc_map.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/test_schema_fuzzing.py` & `ethpm-types-0.4.3/tests/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/test_source.py` & `ethpm-types-0.4.3/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.2/tests/test_sourcemap.py` & `ethpm-types-0.4.3/tests/test_sourcemap.py`

 * *Files identical despite different names*

