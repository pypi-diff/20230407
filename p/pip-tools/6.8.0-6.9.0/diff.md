# Comparing `tmp/pip-tools-6.8.0.tar.gz` & `tmp/pip-tools-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-tools-6.8.0.tar", last modified: Thu Jun 30 09:24:47 2022, max compression
+gzip compressed data, was "pip-tools-6.9.0.tar", last modified: Wed Oct  5 19:50:10 2022, max compression
```

## Comparing `pip-tools-6.8.0.tar` & `pip-tools-6.9.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.430174 pip-tools-6.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.bandit
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.422174 pip-tools-6.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.422174 pip-tools-6.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.422174 pip-tools-6.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.github/workflows/qa.yml
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-06-30 09:24:26.000000 pip-tools-6.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    36190 2022-06-30 09:24:26.000000 pip-tools-6.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-06-30 09:24:26.000000 pip-tools-6.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-06-30 09:24:26.000000 pip-tools-6.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-06-30 09:24:26.000000 pip-tools-6.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    19928 2022-06-30 09:24:47.430174 pip-tools-6.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18804 2022-06-30 09:24:26.000000 pip-tools-6.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-30 09:24:26.000000 pip-tools-6.8.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.422174 pip-tools-6.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-30 09:24:26.000000 pip-tools-6.8.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-30 09:24:26.000000 pip-tools-6.8.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-06-30 09:24:26.000000 pip-tools-6.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-06-30 09:24:26.000000 pip-tools-6.8.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-06-30 09:24:26.000000 pip-tools-6.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-06-30 09:24:26.000000 pip-tools-6.8.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.422174 pip-tools-6.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-06-30 09:24:26.000000 pip-tools-6.8.0/examples/django.in
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-30 09:24:26.000000 pip-tools-6.8.0/examples/flask.in
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-30 09:24:26.000000 pip-tools-6.8.0/examples/hypothesis.in
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-30 09:24:26.000000 pip-tools-6.8.0/examples/protection.in
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-30 09:24:26.000000 pip-tools-6.8.0/examples/sentry.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.422174 pip-tools-6.8.0/img/
--rw-r--r--   0 runner    (1001) docker     (121)    10481 2022-06-30 09:24:26.000000 pip-tools-6.8.0/img/pip-tools-overview.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.422174 pip-tools-6.8.0/pip_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    19928 2022-06-30 09:24:46.000000 pip-tools-6.8.0/pip_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-06-30 09:24:47.000000 pip-tools-6.8.0/pip_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-30 09:24:46.000000 pip-tools-6.8.0/pip_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-06-30 09:24:47.000000 pip-tools-6.8.0/pip_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-30 09:24:46.000000 pip-tools-6.8.0/pip_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-06-30 09:24:47.000000 pip-tools-6.8.0/pip_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-30 09:24:47.000000 pip-tools-6.8.0/pip_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.426174 pip-tools-6.8.0/piptools/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.426174 pip-tools-6.8.0/piptools/_compat/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/_compat/click.py
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/_compat/pip_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     5981 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/locations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.426174 pip-tools-6.8.0/piptools/repositories/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/repositories/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3670 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/repositories/local.py
--rw-r--r--   0 runner    (1001) docker     (121)    20253 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/repositories/pypi.py
--rw-r--r--   0 runner    (1001) docker     (121)    30231 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.426174 pip-tools-6.8.0/piptools/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17128 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/scripts/compile.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9158 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/scripts/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8208 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)    16164 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10670 2022-06-30 09:24:26.000000 pip-tools-6.8.0/piptools/writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2505 2022-06-30 09:24:47.430174 pip-tools-6.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-30 09:24:26.000000 pip-tools-6.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.426174 pip-tools-6.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11576 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    72944 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_cli_compile.py
--rw-r--r--   0 runner    (1001) docker     (121)    10435 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_cli_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.426174 pip-tools-6.8.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/fake-editables.json
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/fake-index.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.426174 pip-tools-6.8.0/tests/test_data/minimal_wheels/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.418174 pip-tools-6.8.0/tests/test_data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.426174 pip-tools-6.8.0/tests/test_data/packages/fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/packages/fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.426174 pip-tools-6.8.0/tests/test_data/packages/small_fake_a/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/packages/small_fake_a/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.430174 pip-tools-6.8.0/tests/test_data/packages/small_fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/packages/small_fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.430174 pip-tools-6.8.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.418174 pip-tools-6.8.0/tests/test_data/packages/small_fake_with_subdir/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.430174 pip-tools-6.8.0/tests/test_data/packages/small_fake_with_subdir/subdir/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:47.430174 pip-tools-6.8.0/tests/test_data/packages/small_fake_with_unpinned_deps/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_fake_index.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_minimal_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_repository_local.py
--rw-r--r--   0 runner    (1001) docker     (121)    13116 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_repository_pypi.py
--rw-r--r--   0 runner    (1001) docker     (121)    22201 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14541 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_top_level_editable.py
--rw-r--r--   0 runner    (1001) docker     (121)    19334 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12133 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-06-30 09:24:26.000000 pip-tools-6.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.651691 pip-tools-6.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.635689 pip-tools-6.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.635689 pip-tools-6.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     4548 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/qa.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    36887 2022-10-05 19:49:52.000000 pip-tools-6.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-10-05 19:49:52.000000 pip-tools-6.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-10-05 19:49:52.000000 pip-tools-6.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-10-05 19:49:52.000000 pip-tools-6.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    22014 2022-10-05 19:50:10.651691 pip-tools-6.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    20862 2022-10-05 19:49:52.000000 pip-tools-6.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-05 19:49:52.000000 pip-tools-6.9.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/django.in
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/flask.in
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/hypothesis.in
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/protection.in
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/sentry.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/img/
+-rw-r--r--   0 runner    (1001) docker     (121)    10481 2022-10-05 19:49:52.000000 pip-tools-6.9.0/img/pip-tools-overview.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/pip_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    22014 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.643690 pip-tools-6.9.0/piptools/
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.643690 pip-tools-6.9.0/piptools/_compat/
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/_compat/click.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/_compat/pip_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5981 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/locations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.643690 pip-tools-6.9.0/piptools/repositories/
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/repositories/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3685 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/repositories/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20253 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/repositories/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29822 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.643690 pip-tools-6.9.0/piptools/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    17876 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/scripts/compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9158 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/scripts/sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8208 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16164 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10670 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-10-05 19:50:10.651691 pip-tools-6.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-05 19:49:52.000000 pip-tools-6.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11576 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74698 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_cli_compile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10435 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_cli_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/fake-editables.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/fake-index.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/minimal_wheels/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.631688 pip-tools-6.9.0/tests/test_data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/packages/fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/packages/small_fake_a/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_a/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.631688 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_subdir/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.651691 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_subdir/subdir/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.651691 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_unpinned_deps/
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_fake_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_minimal_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_repository_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13116 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_repository_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23734 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14541 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_top_level_editable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19334 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12133 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tox.ini
```

### Comparing `pip-tools-6.8.0/.github/ISSUE_TEMPLATE/feature-request.md` & `pip-tools-6.9.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/.github/PULL_REQUEST_TEMPLATE.md` & `pip-tools-6.9.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/.github/release-drafter.yml` & `pip-tools-6.9.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/.github/workflows/ci.yml` & `pip-tools-6.9.0/.github/workflows/ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,30 @@
     # Run everyday at 03:53 UTC
     - cron: 53 3 * * *
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
+env:
+  FORCE_COLOR: 1 # Request colored output from CLI tools supporting it
+  MYPY_FORCE_COLOR: 1 # MyPy's color enforcement
+  PIP_DISABLE_PIP_VERSION_CHECK: 1
+  PIP_NO_PYTHON_VERSION_WARNING: 1
+  PIP_NO_WARN_SCRIPT_LOCATION: 1
+  PY_COLORS: 1 # Recognized by the `py` package, dependency of `pytest`
+  TOX_PARALLEL_NO_SPINNER: 1
+  TOX_TESTENV_PASSENV: >-
+    FORCE_COLOR
+    MYPY_FORCE_COLOR
+    NO_COLOR
+    PY_COLORS
+    PYTEST_THEME
+    PYTEST_THEME_MODE
+
 jobs:
   test:
     name: ${{ matrix.os }} / ${{ matrix.python-version }} / ${{ matrix.pip-version }}
     runs-on: ${{ matrix.os }}-latest
     strategy:
       fail-fast: false
       matrix:
@@ -37,37 +53,36 @@
           - os: Ubuntu
             python-version: 3.11-dev
             pip-version: latest
           - os: Ubuntu
             python-version: 3.7
             pip-version: main
     env:
-      PY_COLORS: 1
       TOXENV: pip${{ matrix.pip-version }}-coverage
-      TOX_PARALLEL_NO_SPINNER: 1
     steps:
-      - uses: actions/checkout@master
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }} from GitHub
+        id: python-install
         if: "!endsWith(matrix.python-version, '-dev')"
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Set up Python ${{ matrix.python-version }} from deadsnakes
         if: endsWith(matrix.python-version, '-dev')
-        uses: deadsnakes/action@v2.0.1
+        uses: deadsnakes/action@v2.1.1
         with:
           python-version: ${{ matrix.python-version }}
       - name: Log python version info (${{ matrix.python-version }})
         run: python --version --version
       - name: Get pip cache dir
         id: pip-cache
         run: |
           echo "::set-output name=dir::$(pip cache dir)"
       - name: Pip cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key: >-
             ${{ runner.os }}-pip-${{ hashFiles('setup.cfg') }}-${{
             hashFiles('setup.py') }}-${{ hashFiles('tox.ini') }}-${{
             hashFiles('.pre-commit-config.yaml') }}
           restore-keys: |
@@ -76,18 +91,28 @@
       - name: Install test dependencies
         run: python -m pip install -U tox virtualenv
       - name: Prepare test environment
         run: tox --notest -p auto --parallel-live
       - name: Test pip ${{ matrix.pip-version }}
         run: tox
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v1.0.15
+        uses: codecov/codecov-action@v3
         with:
-          file: ./coverage.xml
-          name: ${{ runner.os }}-${{ matrix.python-version }}-${{ matrix.pip-version }}
+          files: ./coverage.xml
+          flags: >-
+            CI-GHA,
+            OS-${{ runner.os }},
+            VM-${{ matrix.os }},
+            Py-${{ steps.python-install.outputs.python-version }},
+            Pip-${{ matrix.pip-version }}
+          name: >-
+            OS-${{ runner.os }},
+            VM-${{ matrix.os }},
+            Py-${{ steps.python-install.outputs.python-version }},
+            Pip-${{ matrix.pip-version }}
 
   pypy:
     name: ${{ matrix.os }} / ${{ matrix.python-version }} / ${{ matrix.pip-version }}
     runs-on: ${{ matrix.os }}-latest
     strategy:
       fail-fast: false
       matrix:
@@ -96,22 +121,35 @@
           - MacOS
           - Windows
         python-version:
           - pypy-3.7
         pip-version:
           - latest
     env:
-      PY_COLORS: 1
       TOXENV: pip${{ matrix.pip-version }}
-      TOX_PARALLEL_NO_SPINNER: 1
     steps:
-      - uses: actions/checkout@master
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install tox
         run: pip install tox
       - name: Prepare test environment
         run: tox --notest -p auto --parallel-live
       - name: Test pip ${{ matrix.pip-version }}
         run: tox
+
+  check: # This job does nothing and is only used for the branch protection
+    if: always()
+
+    needs:
+      - pypy
+      - test
+
+    runs-on: ubuntu-latest
+
+    steps:
+      - name: Decide whether the needed jobs succeeded or failed
+        uses: re-actors/alls-green@13b4244b312e8a314951e03958a2f91519a6a3c9
+        with:
+          jobs: ${{ toJSON(needs) }}
```

### Comparing `pip-tools-6.8.0/.github/workflows/cron.yml` & `pip-tools-6.9.0/.github/workflows/cron.yml`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     env:
       PY_COLORS: 1
       TOXENV: pip${{ matrix.pip-version }}
       TOX_PARALLEL_NO_SPINNER: 1
     steps:
       - uses: actions/checkout@master
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Get pip cache dir
         id: pip-cache
         run: |
           echo "::set-output name=dir::$(pip cache dir)"
       - name: Pip cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key: >-
             ${{ runner.os }}-pip-${{ hashFiles('setup.cfg') }}-${{
             hashFiles('setup.py') }}-${{ hashFiles('tox.ini') }}-${{
             hashFiles('.pre-commit-config.yaml') }}
           restore-keys: |
@@ -72,23 +72,23 @@
     env:
       PY_COLORS: 1
       TOXENV: pip${{ matrix.pip-version }}
       TOX_PARALLEL_NO_SPINNER: 1
     steps:
       - uses: actions/checkout@master
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Get pip cache dir
         id: pip-cache
         run: |
           echo "::set-output name=dir::$(pip cache dir)"
       - name: Pip cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key: >-
             ${{ runner.os }}-pip-${{ hashFiles('setup.cfg') }}-${{
             hashFiles('setup.py') }}-${{ hashFiles('tox.ini') }}-${{
             hashFiles('.pre-commit-config.yaml') }}
           restore-keys: |
```

### Comparing `pip-tools-6.8.0/.github/workflows/qa.yml` & `pip-tools-6.9.0/.github/workflows/qa.yml`

 * *Files 5% similar despite different names*

```diff
@@ -27,36 +27,36 @@
     env:
       PY_COLORS: 1
       TOXENV: ${{ matrix.toxenv }}
       TOX_PARALLEL_NO_SPINNER: 1
     steps:
       - uses: actions/checkout@master
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Get pip cache dir
         id: pip-cache
         run: |
           echo "::set-output name=dir::$(pip cache dir)"
       - name: Pip cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key: >-
             ${{ runner.os }}-pip-${{ hashFiles('setup.cfg') }}-${{
             hashFiles('setup.py') }}-${{ hashFiles('tox.ini') }}-${{
             hashFiles('.pre-commit-config.yaml') }}
           restore-keys: |
             ${{ runner.os }}-pip-
             ${{ runner.os }}-
       - name: Prepare cache key
         id: cache-key
         run: echo "::set-output name=sha-256::$(python -VV | sha256sum | cut -d' ' -f1)"
-      - uses: actions/cache@v1
+      - uses: actions/cache@v3
         with:
           path: ~/.cache/pre-commit
           key: pre-commit|${{ steps.cache-key.outputs.sha-256 }}|${{ hashFiles('.pre-commit-config.yaml') }}
       - name: Install tox
         run: pip install tox
       - name: Prepare test environment
         run: tox --notest -p auto --parallel-live
```

### Comparing `pip-tools-6.8.0/.github/workflows/release-drafter.yml` & `pip-tools-6.9.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/.github/workflows/release.yml` & `pip-tools-6.9.0/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: 3.9
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U setuptools twine wheel
```

### Comparing `pip-tools-6.8.0/.pre-commit-config.yaml` & `pip-tools-6.9.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 22.8.0
     hooks:
       - id: black
         args: [--target-version=py36]
   - repo: https://github.com/PyCQA/isort
     rev: 5.10.1
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.1
+    rev: v2.38.2
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 5.0.4
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-pytest-style
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.942
+    rev: v0.981
     hooks:
       - id: mypy
         # Avoid error: Duplicate module named 'setup'
         # https://github.com/python/mypy/issues/4008
         # Keep exclude in sync with mypy own excludes
         exclude: ^tests/test_data/
         additional_dependencies:
@@ -35,10 +35,10 @@
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.4
     hooks:
       - id: bandit
         args: [--ini, .bandit]
         exclude: ^tests/
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.6.2
+    rev: v3.0.0-alpha.0
     hooks:
       - id: prettier
```

### Comparing `pip-tools-6.8.0/CHANGELOG.md` & `pip-tools-6.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+## 6.9.0 (2022-10-05)
+
+Features:
+
+- Add `--all-extras` flag to `pip-compile`
+  ([#1630](https://github.com/jazzband/pip-tools/pull/1630)). Thanks @apljungquist
+- Support Exclude Package with custom unsafe packages
+  ([#1509](https://github.com/jazzband/pip-tools/pull/1509)). Thanks @hmc-cs-mdrissi
+
+Bug Fixes:
+
+- Fix compile cached vcs packages
+  ([#1649](https://github.com/jazzband/pip-tools/pull/1649)). Thanks @atugushev
+- Include `py.typed` in wheel file
+  ([#1648](https://github.com/jazzband/pip-tools/pull/1648)). Thanks @FlorentJeannot
+
+Other Changes:
+
+- Add pyproject.toml & modern packaging to introduction.
+  ([#1668](https://github.com/jazzband/pip-tools/pull/1668)). Thanks @hynek
+
 ## 6.8.0 (2022-06-30)
 
 Features:
 
 - Add support for pip's 2020 dependency resolver. Use
   `pip-compile --resolver backtracking` to enable new resolver
   ([#1539](https://github.com/jazzband/pip-tools/pull/1539)). Thanks @atugushev
```

### Comparing `pip-tools-6.8.0/CODE_OF_CONDUCT.md` & `pip-tools-6.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/CONTRIBUTING.md` & `pip-tools-6.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/LICENSE` & `pip-tools-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/PKG-INFO` & `pip-tools-6.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-tools
-Version: 6.8.0
+Version: 6.9.0
 Summary: pip-tools keeps your pinned dependencies fresh.
 Home-page: https://github.com/jazzband/pip-tools/
 Author: Vincent Driessen
 Author-email: me@nvie.com
 License: BSD 3 Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Systems Administration
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: coverage
 License-File: LICENSE
 
 |jazzband| |pypi| |pyversions| |pre-commit| |buildstatus-gha| |codecov|
 
@@ -74,15 +75,16 @@
 
 .. _virtual environments: https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments
 
 Example usage for ``pip-compile``
 =================================
 
 The ``pip-compile`` command lets you compile a ``requirements.txt`` file from
-your dependencies, specified in either ``setup.py`` or ``requirements.in``.
+your dependencies, specified in either ``pyproject.toml``, ``setup.cfg``,
+``setup.py``, or ``requirements.in``.
 
 Run it with ``pip-compile`` or ``python -m piptools compile``. If you use
 multiple Python versions, you can also run ``py -X.Y -m piptools compile`` on
 Windows and ``pythonX.Y -m piptools compile`` on other systems.
 
 ``pip-compile`` should be run from the same virtual environment as your
 project so conditional dependencies that require a specific Python version,
@@ -91,47 +93,113 @@
 
 **Note**: If ``pip-compile`` finds an existing ``requirements.txt`` file that
 fulfils the dependencies then no changes will be made, even if updates are
 available. To compile from scratch, first delete the existing
 ``requirements.txt`` file, or see `Updating requirements`_ for alternative
 approaches.
 
-Requirements from ``setup.py``
-------------------------------
+Requirements from ``pyproject.toml``
+------------------------------------
 
-Suppose you have a Django project, and want to pin it for production.
-If you have a ``setup.py`` with ``install_requires=['django']``, then run
-``pip-compile`` without any arguments:
+The ``pyproject.toml`` file is the
+`latest standard <https://peps.python.org/pep-0621/>`_ for configuring
+packages and applications, and is recommended for new projects. ``pip-compile``
+supports both installing your ``project.dependencies`` as well as your
+``project.optional-dependencies``. Thanks to the fact that this is an
+official standard, you can use ``pip-compile`` to pin the dependencies
+in projects that use modern standards-adhering packaging tools like
+`Hatch <https://hatch.pypa.io/>`_ or `flit <https://flit.pypa.io/>`_.
+
+Suppose you have a Django application that is packaged using ``Hatch``, and you
+want to pin it for production. You also want to pin your development tools
+in a separate pin file. You declare ``django`` as a dependency and create an
+optional dependency ``dev`` that includes ``pytest``:
+
+.. code-block:: toml
+
+    [build-system]
+    requires = ["hatchling"]
+    build-backend = "hatchling.build"
+
+    [project]
+    name = "my-cool-django-app"
+    version = "42"
+    dependencies = ["django"]
+    
+    [project.optional-dependencies]
+    dev = ["pytest"]
 
-.. code-block:: bash
+You can produce your pin files as easily as:
+
+.. code-block:: console
 
-    $ pip-compile
+    $ pip-compile -o requirements.txt pyproject.toml
     #
-    # This file is autogenerated by pip-compile
+    # This file is autogenerated by pip-compile with python 3.10
     # To update, run:
     #
-    #    pip-compile
+    #    pip-compile --output-file=requirements.txt pyproject.toml
     #
-    asgiref==3.2.3
-        # via django
-    django==3.0.3
-        # via my_django_project (setup.py)
-    pytz==2019.3
-        # via django
-    sqlparse==0.3.0
-        # via django
 
-``pip-compile`` will produce your ``requirements.txt``, with all the Django
-dependencies (and all underlying dependencies) pinned.
+    asgiref==3.5.2
+       # via django
+    django==4.1
+        # via my-cool-django-app (pyproject.toml)
+    sqlparse==0.4.2
+        # via django
 
-Without ``setup.py``
---------------------
+    $ pip-compile --extra dev -o dev-requirements.txt pyproject.toml
+    #  
+    # This file is autogenerated by pip-compile with python 3.10
+    # To update, run:
+    #
+    #    pip-compile --extra=dev --output-file=dev-requirements.txt pyproject.toml
+    #
 
-If you don't use ``setup.py`` (`it's easy to write one`_), you can create a
-``requirements.in`` file to declare the Django dependency:
+    asgiref==3.5.2
+        # via django
+    attrs==22.1.0
+        # via pytest
+    django==4.1
+        # via my-cool-django-app (pyproject.toml)
+    iniconfig==1.1.1
+        # via pytest
+    packaging==21.3
+        # via pytest
+    pluggy==1.0.0
+        # via pytest
+    py==1.11.0
+        # via pytest
+    pyparsing==3.0.9
+        # via packaging
+    pytest==7.1.2
+        # via my-cool-django-app (pyproject.toml)
+    sqlparse==0.4.2
+        # via django
+    tomli==2.0.1
+        # via pytest
+
+This is great for both pinning your applications, but also to keep the CI
+of your open-source Python package stable.
+
+Requirements from ``setup.py`` and ``setup.cfg``
+------------------------------------------------
+
+``pip-compile`` has also full support for ``setup.py``- and
+``setup.cfg``-based projects that use ``setuptools``.
+
+Just define your dependencies and extras as usual and run
+``pip-compile`` as above.
+
+Requirements from ``requirements.in``
+-------------------------------------
+
+You can also use plain text files for your requirements (e.g. if you don't
+want your application to be a package). To use a ``requirements.in`` file to
+declare the Django dependency:
 
 .. code-block:: ini
 
     # requirements.in
     django
 
 Now, run ``pip-compile requirements.in``:
@@ -153,23 +221,21 @@
         # via django
     sqlparse==0.3.0
         # via django
 
 And it will produce your ``requirements.txt``, with all the Django dependencies
 (and all underlying dependencies) pinned.
 
-.. _it's easy to write one: https://packaging.python.org/guides/distributing-packages-using-setuptools/#configuring-your-project
-
 .. _Updating requirements:
 
 Updating requirements
 ---------------------
 
 ``pip-compile`` generates a ``requirements.txt`` file using the latest versions
-that fulfil the dependencies of ``setup.py`` or ``requirements.in``.
+that fulfil the dependencies you specify in the supported files.
 
 If ``pip-compile`` finds an existing ``requirements.txt`` file that fulfils the
 dependencies then no changes will be made, even if updates are available.
 
 To force ``pip-compile`` to update all packages in an existing
 ``requirements.txt``, run ``pip-compile --upgrade``.
```

### Comparing `pip-tools-6.8.0/README.rst` & `pip-tools-6.9.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 
 .. _virtual environments: https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments
 
 Example usage for ``pip-compile``
 =================================
 
 The ``pip-compile`` command lets you compile a ``requirements.txt`` file from
-your dependencies, specified in either ``setup.py`` or ``requirements.in``.
+your dependencies, specified in either ``pyproject.toml``, ``setup.cfg``,
+``setup.py``, or ``requirements.in``.
 
 Run it with ``pip-compile`` or ``python -m piptools compile``. If you use
 multiple Python versions, you can also run ``py -X.Y -m piptools compile`` on
 Windows and ``pythonX.Y -m piptools compile`` on other systems.
 
 ``pip-compile`` should be run from the same virtual environment as your
 project so conditional dependencies that require a specific Python version,
@@ -63,47 +64,113 @@
 
 **Note**: If ``pip-compile`` finds an existing ``requirements.txt`` file that
 fulfils the dependencies then no changes will be made, even if updates are
 available. To compile from scratch, first delete the existing
 ``requirements.txt`` file, or see `Updating requirements`_ for alternative
 approaches.
 
-Requirements from ``setup.py``
-------------------------------
+Requirements from ``pyproject.toml``
+------------------------------------
 
-Suppose you have a Django project, and want to pin it for production.
-If you have a ``setup.py`` with ``install_requires=['django']``, then run
-``pip-compile`` without any arguments:
+The ``pyproject.toml`` file is the
+`latest standard <https://peps.python.org/pep-0621/>`_ for configuring
+packages and applications, and is recommended for new projects. ``pip-compile``
+supports both installing your ``project.dependencies`` as well as your
+``project.optional-dependencies``. Thanks to the fact that this is an
+official standard, you can use ``pip-compile`` to pin the dependencies
+in projects that use modern standards-adhering packaging tools like
+`Hatch <https://hatch.pypa.io/>`_ or `flit <https://flit.pypa.io/>`_.
+
+Suppose you have a Django application that is packaged using ``Hatch``, and you
+want to pin it for production. You also want to pin your development tools
+in a separate pin file. You declare ``django`` as a dependency and create an
+optional dependency ``dev`` that includes ``pytest``:
+
+.. code-block:: toml
+
+    [build-system]
+    requires = ["hatchling"]
+    build-backend = "hatchling.build"
+
+    [project]
+    name = "my-cool-django-app"
+    version = "42"
+    dependencies = ["django"]
+    
+    [project.optional-dependencies]
+    dev = ["pytest"]
 
-.. code-block:: bash
+You can produce your pin files as easily as:
+
+.. code-block:: console
 
-    $ pip-compile
+    $ pip-compile -o requirements.txt pyproject.toml
     #
-    # This file is autogenerated by pip-compile
+    # This file is autogenerated by pip-compile with python 3.10
     # To update, run:
     #
-    #    pip-compile
+    #    pip-compile --output-file=requirements.txt pyproject.toml
     #
-    asgiref==3.2.3
-        # via django
-    django==3.0.3
-        # via my_django_project (setup.py)
-    pytz==2019.3
-        # via django
-    sqlparse==0.3.0
-        # via django
 
-``pip-compile`` will produce your ``requirements.txt``, with all the Django
-dependencies (and all underlying dependencies) pinned.
+    asgiref==3.5.2
+       # via django
+    django==4.1
+        # via my-cool-django-app (pyproject.toml)
+    sqlparse==0.4.2
+        # via django
 
-Without ``setup.py``
---------------------
+    $ pip-compile --extra dev -o dev-requirements.txt pyproject.toml
+    #  
+    # This file is autogenerated by pip-compile with python 3.10
+    # To update, run:
+    #
+    #    pip-compile --extra=dev --output-file=dev-requirements.txt pyproject.toml
+    #
 
-If you don't use ``setup.py`` (`it's easy to write one`_), you can create a
-``requirements.in`` file to declare the Django dependency:
+    asgiref==3.5.2
+        # via django
+    attrs==22.1.0
+        # via pytest
+    django==4.1
+        # via my-cool-django-app (pyproject.toml)
+    iniconfig==1.1.1
+        # via pytest
+    packaging==21.3
+        # via pytest
+    pluggy==1.0.0
+        # via pytest
+    py==1.11.0
+        # via pytest
+    pyparsing==3.0.9
+        # via packaging
+    pytest==7.1.2
+        # via my-cool-django-app (pyproject.toml)
+    sqlparse==0.4.2
+        # via django
+    tomli==2.0.1
+        # via pytest
+
+This is great for both pinning your applications, but also to keep the CI
+of your open-source Python package stable.
+
+Requirements from ``setup.py`` and ``setup.cfg``
+------------------------------------------------
+
+``pip-compile`` has also full support for ``setup.py``- and
+``setup.cfg``-based projects that use ``setuptools``.
+
+Just define your dependencies and extras as usual and run
+``pip-compile`` as above.
+
+Requirements from ``requirements.in``
+-------------------------------------
+
+You can also use plain text files for your requirements (e.g. if you don't
+want your application to be a package). To use a ``requirements.in`` file to
+declare the Django dependency:
 
 .. code-block:: ini
 
     # requirements.in
     django
 
 Now, run ``pip-compile requirements.in``:
@@ -125,23 +192,21 @@
         # via django
     sqlparse==0.3.0
         # via django
 
 And it will produce your ``requirements.txt``, with all the Django dependencies
 (and all underlying dependencies) pinned.
 
-.. _it's easy to write one: https://packaging.python.org/guides/distributing-packages-using-setuptools/#configuring-your-project
-
 .. _Updating requirements:
 
 Updating requirements
 ---------------------
 
 ``pip-compile`` generates a ``requirements.txt`` file using the latest versions
-that fulfil the dependencies of ``setup.py`` or ``requirements.in``.
+that fulfil the dependencies you specify in the supported files.
 
 If ``pip-compile`` finds an existing ``requirements.txt`` file that fulfils the
 dependencies then no changes will be made, even if updates are available.
 
 To force ``pip-compile`` to update all packages in an existing
 ``requirements.txt``, run ``pip-compile --upgrade``.
```

### Comparing `pip-tools-6.8.0/docs/conf.py` & `pip-tools-6.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/docs/index.rst` & `pip-tools-6.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/img/pip-tools-overview.svg` & `pip-tools-6.9.0/img/pip-tools-overview.svg`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/pip_tools.egg-info/PKG-INFO` & `pip-tools-6.9.0/pip_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-tools
-Version: 6.8.0
+Version: 6.9.0
 Summary: pip-tools keeps your pinned dependencies fresh.
 Home-page: https://github.com/jazzband/pip-tools/
 Author: Vincent Driessen
 Author-email: me@nvie.com
 License: BSD 3 Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Systems Administration
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: coverage
 License-File: LICENSE
 
 |jazzband| |pypi| |pyversions| |pre-commit| |buildstatus-gha| |codecov|
 
@@ -74,15 +75,16 @@
 
 .. _virtual environments: https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments
 
 Example usage for ``pip-compile``
 =================================
 
 The ``pip-compile`` command lets you compile a ``requirements.txt`` file from
-your dependencies, specified in either ``setup.py`` or ``requirements.in``.
+your dependencies, specified in either ``pyproject.toml``, ``setup.cfg``,
+``setup.py``, or ``requirements.in``.
 
 Run it with ``pip-compile`` or ``python -m piptools compile``. If you use
 multiple Python versions, you can also run ``py -X.Y -m piptools compile`` on
 Windows and ``pythonX.Y -m piptools compile`` on other systems.
 
 ``pip-compile`` should be run from the same virtual environment as your
 project so conditional dependencies that require a specific Python version,
@@ -91,47 +93,113 @@
 
 **Note**: If ``pip-compile`` finds an existing ``requirements.txt`` file that
 fulfils the dependencies then no changes will be made, even if updates are
 available. To compile from scratch, first delete the existing
 ``requirements.txt`` file, or see `Updating requirements`_ for alternative
 approaches.
 
-Requirements from ``setup.py``
-------------------------------
+Requirements from ``pyproject.toml``
+------------------------------------
 
-Suppose you have a Django project, and want to pin it for production.
-If you have a ``setup.py`` with ``install_requires=['django']``, then run
-``pip-compile`` without any arguments:
+The ``pyproject.toml`` file is the
+`latest standard <https://peps.python.org/pep-0621/>`_ for configuring
+packages and applications, and is recommended for new projects. ``pip-compile``
+supports both installing your ``project.dependencies`` as well as your
+``project.optional-dependencies``. Thanks to the fact that this is an
+official standard, you can use ``pip-compile`` to pin the dependencies
+in projects that use modern standards-adhering packaging tools like
+`Hatch <https://hatch.pypa.io/>`_ or `flit <https://flit.pypa.io/>`_.
+
+Suppose you have a Django application that is packaged using ``Hatch``, and you
+want to pin it for production. You also want to pin your development tools
+in a separate pin file. You declare ``django`` as a dependency and create an
+optional dependency ``dev`` that includes ``pytest``:
+
+.. code-block:: toml
+
+    [build-system]
+    requires = ["hatchling"]
+    build-backend = "hatchling.build"
+
+    [project]
+    name = "my-cool-django-app"
+    version = "42"
+    dependencies = ["django"]
+    
+    [project.optional-dependencies]
+    dev = ["pytest"]
 
-.. code-block:: bash
+You can produce your pin files as easily as:
+
+.. code-block:: console
 
-    $ pip-compile
+    $ pip-compile -o requirements.txt pyproject.toml
     #
-    # This file is autogenerated by pip-compile
+    # This file is autogenerated by pip-compile with python 3.10
     # To update, run:
     #
-    #    pip-compile
+    #    pip-compile --output-file=requirements.txt pyproject.toml
     #
-    asgiref==3.2.3
-        # via django
-    django==3.0.3
-        # via my_django_project (setup.py)
-    pytz==2019.3
-        # via django
-    sqlparse==0.3.0
-        # via django
 
-``pip-compile`` will produce your ``requirements.txt``, with all the Django
-dependencies (and all underlying dependencies) pinned.
+    asgiref==3.5.2
+       # via django
+    django==4.1
+        # via my-cool-django-app (pyproject.toml)
+    sqlparse==0.4.2
+        # via django
 
-Without ``setup.py``
---------------------
+    $ pip-compile --extra dev -o dev-requirements.txt pyproject.toml
+    #  
+    # This file is autogenerated by pip-compile with python 3.10
+    # To update, run:
+    #
+    #    pip-compile --extra=dev --output-file=dev-requirements.txt pyproject.toml
+    #
 
-If you don't use ``setup.py`` (`it's easy to write one`_), you can create a
-``requirements.in`` file to declare the Django dependency:
+    asgiref==3.5.2
+        # via django
+    attrs==22.1.0
+        # via pytest
+    django==4.1
+        # via my-cool-django-app (pyproject.toml)
+    iniconfig==1.1.1
+        # via pytest
+    packaging==21.3
+        # via pytest
+    pluggy==1.0.0
+        # via pytest
+    py==1.11.0
+        # via pytest
+    pyparsing==3.0.9
+        # via packaging
+    pytest==7.1.2
+        # via my-cool-django-app (pyproject.toml)
+    sqlparse==0.4.2
+        # via django
+    tomli==2.0.1
+        # via pytest
+
+This is great for both pinning your applications, but also to keep the CI
+of your open-source Python package stable.
+
+Requirements from ``setup.py`` and ``setup.cfg``
+------------------------------------------------
+
+``pip-compile`` has also full support for ``setup.py``- and
+``setup.cfg``-based projects that use ``setuptools``.
+
+Just define your dependencies and extras as usual and run
+``pip-compile`` as above.
+
+Requirements from ``requirements.in``
+-------------------------------------
+
+You can also use plain text files for your requirements (e.g. if you don't
+want your application to be a package). To use a ``requirements.in`` file to
+declare the Django dependency:
 
 .. code-block:: ini
 
     # requirements.in
     django
 
 Now, run ``pip-compile requirements.in``:
@@ -153,23 +221,21 @@
         # via django
     sqlparse==0.3.0
         # via django
 
 And it will produce your ``requirements.txt``, with all the Django dependencies
 (and all underlying dependencies) pinned.
 
-.. _it's easy to write one: https://packaging.python.org/guides/distributing-packages-using-setuptools/#configuring-your-project
-
 .. _Updating requirements:
 
 Updating requirements
 ---------------------
 
 ``pip-compile`` generates a ``requirements.txt`` file using the latest versions
-that fulfil the dependencies of ``setup.py`` or ``requirements.in``.
+that fulfil the dependencies you specify in the supported files.
 
 If ``pip-compile`` finds an existing ``requirements.txt`` file that fulfils the
 dependencies then no changes will be made, even if updates are available.
 
 To force ``pip-compile`` to update all packages in an existing
 ``requirements.txt``, run ``pip-compile --upgrade``.
```

### Comparing `pip-tools-6.8.0/pip_tools.egg-info/SOURCES.txt` & `pip-tools-6.9.0/pip_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/piptools/_compat/pip_compat.py` & `pip-tools-6.9.0/piptools/_compat/pip_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         get_build_tracker,
         update_env_context_manager,
     )
 
 
 # The Distribution interface has changed between pkg_resources and
 # importlib.metadata, so this compat layer allows for a consistent access
-# pattern. In pip 22.1, importlib.metdata became the default on Python 3.11
-# (and later), but is overrideable. `select_backend` returns what's being used.
+# pattern. In pip 22.1, importlib.metadata became the default on Python 3.11
+# (and later), but is overridable. `select_backend` returns what's being used.
 
 
 def _uses_pkg_resources() -> bool:
 
     if PIP_VERSION[:2] < (22, 1):
         return True
     else:
```

### Comparing `pip-tools-6.8.0/piptools/cache.py` & `pip-tools-6.9.0/piptools/cache.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/piptools/exceptions.py` & `pip-tools-6.9.0/piptools/exceptions.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/piptools/logging.py` & `pip-tools-6.9.0/piptools/logging.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/piptools/repositories/base.py` & `pip-tools-6.9.0/piptools/repositories/base.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/piptools/repositories/local.py` & `pip-tools-6.9.0/piptools/repositories/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import optparse
 from contextlib import contextmanager
 from typing import Iterator, Mapping, Optional, Set, cast
 
 from pip._internal.commands.install import InstallCommand
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.models.candidate import InstallationCandidate
+from pip._internal.network.session import PipSession
 from pip._internal.req import InstallRequirement
 from pip._internal.utils.hashes import FAVORITE_HASH
-from pip._vendor.requests import Session
 
 from piptools.utils import as_tuple, key_from_ireq, make_install_requirement
 
 from .base import BaseRepository
 from .pypi import PyPIRepository
 
 
@@ -55,15 +55,15 @@
         return self.repository.options
 
     @property
     def finder(self) -> PackageFinder:
         return self.repository.finder
 
     @property
-    def session(self) -> Session:
+    def session(self) -> PipSession:
         return self.repository.session
 
     @property
     def command(self) -> InstallCommand:
         """Return an install command instance."""
         return self.repository.command
```

### Comparing `pip-tools-6.8.0/piptools/repositories/pypi.py` & `pip-tools-6.9.0/piptools/repositories/pypi.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/piptools/resolver.py` & `pip-tools-6.9.0/piptools/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import collections
 import copy
 from abc import ABCMeta, abstractmethod
 from functools import partial
 from itertools import chain, count, groupby
 from typing import (
     Any,
+    Container,
     DefaultDict,
     Dict,
     Iterable,
     Iterator,
     List,
     Optional,
     Set,
@@ -172,58 +173,51 @@
         log.debug("Generating hashes:")
         with self.repository.allow_all_wheels(), log.indentation():
             return {ireq: self.repository.get_hashes(ireq) for ireq in ireqs}
 
     def _filter_out_unsafe_constraints(
         self,
         ireqs: Set[InstallRequirement],
-        reverse_dependencies: Dict[str, Set[str]],
+        unsafe_packages: Container[str],
     ) -> None:
         """
         Remove from a given set of ``InstallRequirement``'s unsafe constraints.
-
-        Reverse_dependencies is used to filter out packages that are only
-        required by unsafe packages. This logic is incomplete, as it would
-        fail to filter sub-sub-dependencies of unsafe packages. None of the
-        UNSAFE_PACKAGES currently have any dependencies at all (which makes
-        sense for installation tools) so this seems sufficient.
         """
         for req in ireqs.copy():
-            required_by = reverse_dependencies.get(req.name.lower(), set())
-            if req.name in UNSAFE_PACKAGES or (
-                required_by and all(name in UNSAFE_PACKAGES for name in required_by)
-            ):
+            if req.name in unsafe_packages:
                 self.unsafe_constraints.add(req)
                 ireqs.remove(req)
 
 
 class LegacyResolver(BaseResolver):
     def __init__(
         self,
         constraints: Iterable[InstallRequirement],
         existing_constraints: Dict[str, InstallRequirement],
         repository: BaseRepository,
         cache: DependencyCache,
         prereleases: Optional[bool] = False,
         clear_caches: bool = False,
         allow_unsafe: bool = False,
+        unsafe_packages: Optional[Set[str]] = None,
     ) -> None:
         """
         This class resolves a given set of constraints (a collection of
         InstallRequirement objects) by consulting the given Repository and the
         DependencyCache.
         """
         self.our_constraints = set(constraints)
         self.their_constraints: Set[InstallRequirement] = set()
         self.repository = repository
         self.dependency_cache = cache
         self.prereleases = prereleases
         self.clear_caches = clear_caches
         self.allow_unsafe = allow_unsafe
         self.unsafe_constraints: Set[InstallRequirement] = set()
+        self.unsafe_packages = unsafe_packages or UNSAFE_PACKAGES
 
         options = self.repository.options
         if "legacy-resolver" not in options.deprecated_features_enabled:
             raise PipToolsError("Legacy resolver deprecated feature must be enabled.")
 
         # Make sure there is no enabled 2020-resolver
         options.features_enabled = omit_list_value(
@@ -277,15 +271,15 @@
         # Only include hard requirements and not pip constraints
         results = {req for req in best_matches if not req.constraint}
 
         # Filter out unsafe requirements.
         if not self.allow_unsafe:
             self._filter_out_unsafe_constraints(
                 ireqs=results,
-                reverse_dependencies=self.reverse_dependencies(results),
+                unsafe_packages=self.unsafe_packages,
             )
 
         return results
 
     def _group_constraints(
         self, constraints: Iterable[InstallRequirement]
     ) -> Iterator[InstallRequirement]:
@@ -486,37 +480,31 @@
         # produced the dependency_strings, but they lack `markers` on their
         # underlying Requirements:
         for dependency_string in dependency_strings:
             yield install_req_from_line(
                 dependency_string, constraint=ireq.constraint, comes_from=ireq
             )
 
-    def reverse_dependencies(
-        self, ireqs: Iterable[InstallRequirement]
-    ) -> Dict[str, Set[str]]:
-        non_editable = [
-            ireq for ireq in ireqs if not (ireq.editable or is_url_requirement(ireq))
-        ]
-        return self.dependency_cache.reverse_dependencies(non_editable)
-
 
 class BacktrackingResolver(BaseResolver):
     """A wrapper for backtracking resolver."""
 
     def __init__(
         self,
         constraints: Iterable[InstallRequirement],
         existing_constraints: Dict[str, InstallRequirement],
         repository: BaseRepository,
         allow_unsafe: bool = False,
+        unsafe_packages: Optional[Set[str]] = None,
         **kwargs: Any,
     ) -> None:
         self.constraints = list(constraints)
         self.repository = repository
         self.allow_unsafe = allow_unsafe
+        self.unsafe_packages = unsafe_packages or UNSAFE_PACKAGES
 
         options = self.options = self.repository.options
         self.session = self.repository.session
         self.finder = self.repository.finder
         self.command = self.repository.command
         self.unsafe_constraints: Set[InstallRequirement] = set()
 
@@ -617,28 +605,22 @@
                 )
                 if is_resolved:
                     break
 
         resolver_result = resolver._result
         assert isinstance(resolver_result, Result)
 
-        # Get reverse requirements from the resolver result graph.
-        reverse_dependencies = self._get_reverse_dependencies(resolver_result)
-
         # Prepare set of install requirements from resolver result.
-        result_ireqs = self._get_install_requirements(
-            resolver_result=resolver_result,
-            reverse_dependencies=reverse_dependencies,
-        )
+        result_ireqs = self._get_install_requirements(resolver_result=resolver_result)
 
         # Filter out unsafe requirements.
         if not self.allow_unsafe:
             self._filter_out_unsafe_constraints(
                 ireqs=result_ireqs,
-                reverse_dependencies=reverse_dependencies,
+                unsafe_packages=self.unsafe_packages,
             )
 
         return result_ireqs
 
     def _do_resolve(
         self,
         resolver: Resolver,
@@ -684,21 +666,22 @@
                 del compatible_existing_constraints[cause_ireq_name]
 
             return False
 
         return True
 
     def _get_install_requirements(
-        self,
-        resolver_result: Result,
-        reverse_dependencies: Dict[str, Set[str]],
+        self, resolver_result: Result
     ) -> Set[InstallRequirement]:
         """Return a set of install requirements from resolver results."""
         result_ireqs: Dict[str, InstallRequirement] = {}
 
+        # Get reverse requirements from the resolver result graph.
+        reverse_dependencies = self._get_reverse_dependencies(resolver_result)
+
         # Transform candidates to install requirements
         resolved_candidates = tuple(resolver_result.mapping.values())
         for candidate in resolved_candidates:
             ireq = self._get_install_requirement_from_candidate(
                 candidate=candidate,
                 reverse_dependencies=reverse_dependencies,
             )
@@ -759,15 +742,22 @@
         for specifier in ireq.specifier:
             if specifier.operator == "===" and specifier.version == version_as_str:
                 version_pin_operator = "==="
                 break
 
         # Prepare pinned install requirement. Copy it from candidate's install
         # requirement so that it could be mutated later.
-        pinned_ireq = copy_install_requirement(ireq)
+        pinned_ireq = copy_install_requirement(
+            template=ireq,
+            # The link this candidate "originates" from. This is different
+            # from ``ireq.link`` when the link is found in the wheel cache.
+            # ``ireq.link`` would point to the wheel cache, while this points
+            # to the found remote link (e.g. from pypi.org).
+            link=candidate.source_link,
+        )
 
         # Canonicalize name
         assert ireq.name is not None
         pinned_ireq.req.name = canonicalize_name(ireq.name)
 
         # Pin requirement to a resolved version
         pinned_ireq.req.specifier = SpecifierSet(
```

### Comparing `pip-tools-6.8.0/piptools/scripts/compile.py` & `pip-tools-6.9.0/piptools/scripts/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,20 @@
 @click.option(
     "--extra",
     "extras",
     multiple=True,
     help="Name of an extras_require group to install; may be used more than once",
 )
 @click.option(
+    "--all-extras",
+    is_flag=True,
+    default=False,
+    help="Install all extras_require groups",
+)
+@click.option(
     "-f",
     "--find-links",
     multiple=True,
     help="Look for archives in this directory or on this HTML page; may be used more than once",
 )
 @click.option(
     "-i",
@@ -241,22 +247,29 @@
 )
 @click.option(
     "--emit-options/--no-emit-options",
     is_flag=True,
     default=True,
     help="Add options to generated file",
 )
+@click.option(
+    "--unsafe-package",
+    multiple=True,
+    help="Specify a package to consider unsafe; may be used more than once. "
+    f"Replaces default unsafe packages: {', '.join(sorted(UNSAFE_PACKAGES))}",
+)
 def cli(
     ctx: click.Context,
     verbose: int,
     quiet: int,
     dry_run: bool,
     pre: bool,
     rebuild: bool,
     extras: Tuple[str, ...],
+    all_extras: bool,
     find_links: Tuple[str, ...],
     index_url: str,
     extra_index_url: Tuple[str, ...],
     cert: Optional[str],
     client_cert: Optional[str],
     trusted_host: Tuple[str, ...],
     header: bool,
@@ -275,16 +288,20 @@
     build_isolation: bool,
     emit_find_links: bool,
     cache_dir: str,
     pip_args_str: Optional[str],
     resolver_name: str,
     emit_index_url: bool,
     emit_options: bool,
+    unsafe_package: Tuple[str, ...],
 ) -> None:
-    """Compiles requirements.txt from requirements.in specs."""
+    """
+    Compiles requirements.txt from requirements.in, pyproject.toml, setup.cfg,
+    or setup.py specs.
+    """
     log.verbosity = verbose - quiet
 
     if len(src_files) == 0:
         if os.path.exists(DEFAULT_REQUIREMENTS_FILE):
             src_files = (DEFAULT_REQUIREMENTS_FILE,)
         elif os.path.exists("setup.py"):
             src_files = ("setup.py",)
@@ -428,14 +445,19 @@
             comes_from = f"{metadata.get_all('Name')[0]} ({src_file})"
             constraints.extend(
                 [
                     install_req_from_line(req, comes_from=comes_from)
                     for req in metadata.get_all("Requires-Dist") or []
                 ]
             )
+            if all_extras:
+                if extras:
+                    msg = "--extra has no effect when used with --all-extras"
+                    raise click.BadParameter(msg)
+                extras = tuple(metadata.get_all("Provides-Extra"))
         else:
             constraints.extend(
                 parse_requirements(
                     src_file,
                     finder=repository.finder,
                     session=repository.session,
                     options=repository.options,
@@ -479,14 +501,15 @@
             constraints=constraints,
             existing_constraints=existing_pins,
             repository=repository,
             prereleases=repository.finder.allow_all_prereleases or pre,
             cache=DependencyCache(cache_dir),
             clear_caches=rebuild,
             allow_unsafe=allow_unsafe,
+            unsafe_packages=set(unsafe_package),
         )
         results = resolver.resolve(max_rounds=max_rounds)
         hashes = resolver.resolve_hashes(results) if generate_hashes else None
     except PipToolsError as e:
         log.error(str(e))
         sys.exit(2)
```

### Comparing `pip-tools-6.8.0/piptools/scripts/sync.py` & `pip-tools-6.9.0/piptools/scripts/sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/piptools/subprocess_utils.py` & `pip-tools-6.9.0/piptools/subprocess_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     """
     py_exec_cmd = python_executable, "-c", code_to_run
 
     # subprocess module should never be used with untrusted input
     return subprocess.check_output(  # nosec
         py_exec_cmd,
         shell=False,
-        universal_newlines=True,
+        text=True,
     )
```

### Comparing `pip-tools-6.8.0/piptools/sync.py` & `pip-tools-6.9.0/piptools/sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/piptools/utils.py` & `pip-tools-6.9.0/piptools/utils.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/piptools/writer.py` & `pip-tools-6.9.0/piptools/writer.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/setup.cfg` & `pip-tools-6.9.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: System :: Systems Administration
+	Typing :: Typed
 
 [options]
 python_requires = >=3.7
 setup_requires = setuptools_scm
 packages = find:
 zip_safe = false
 install_requires = 
@@ -34,14 +35,17 @@
 	pip >= 21.2
 	setuptools  # typically needed when pip-tools invokes setup.py
 	wheel  # pip plugin needed by pip-tools
 
 [options.packages.find]
 exclude = tests
 
+[options.package_data]
+piptools = py.typed
+
 [options.extras_require]
 testing = 
 	pytest
 	pytest-rerunfailures
 	pytest-xdist
 coverage = pytest-cov
```

### Comparing `pip-tools-6.8.0/tests/conftest.py` & `pip-tools-6.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_cache.py` & `pip-tools-6.9.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_cli_compile.py` & `pip-tools-6.9.0/tests/test_cli_compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1270,31 +1270,31 @@
             ),
             id="allow all packages",
         ),
         pytest.param(
             "--no-allow-unsafe",
             dedent(
                 """\
+                small-fake-a==0.1
                 small-fake-b==0.3
 
                 # The following packages are considered to be unsafe in a requirements file:
-                # small-fake-a
                 # small-fake-with-deps
                 """
             ),
             id="comment out small-fake-with-deps and its dependencies",
         ),
         pytest.param(
             None,
             dedent(
                 """\
+                small-fake-a==0.1
                 small-fake-b==0.3
 
                 # The following packages are considered to be unsafe in a requirements file:
-                # small-fake-a
                 # small-fake-with-deps
                 """
             ),
             id="allow unsafe is default option",
         ),
     ),
 )
@@ -1599,15 +1599,15 @@
         pytest.param("small-fake-b==0.2", "small-fake-b==0.1", id="downgrade"),
     ),
 )
 def test_upgrade_packages_option_subdependency(
     pip_conf, runner, current_package, upgraded_package
 ):
     """
-    Test that pip-compile --upgrade-package/-P upgrades/dpwngrades subdependencies.
+    Test that pip-compile --upgrade-package/-P upgrades/downgrades subdependencies.
     """
 
     with open("requirements.in", "w") as reqs:
         reqs.write("small-fake-with-unpinned-deps\n")
 
     with open("requirements.txt", "w") as reqs:
         reqs.write("small-fake-a==0.1\n")
@@ -2186,14 +2186,78 @@
     assert "small-fake-c==0.3" in out.stderr
     assert "small-fake-d==0.4" in out.stderr
     assert "small-fake-e==0.5" in out.stderr
     assert "small-fake-f==0.6" in out.stderr
     assert "extra ==" not in out.stderr
 
 
+@pytest.mark.network
+@pytest.mark.parametrize(("fname", "content"), METADATA_TEST_CASES)
+def test_all_extras(fake_dists, runner, make_module, fname, content):
+    """
+    Test passing `--all-extras` includes all applicable extras.
+    """
+    meta_path = make_module(fname=fname, content=content)
+    out = runner.invoke(
+        cli,
+        [
+            "-n",
+            "--all-extras",
+            "--find-links",
+            fake_dists,
+            "--no-annotate",
+            "--no-emit-options",
+            "--no-header",
+            meta_path,
+        ],
+    )
+    assert out.exit_code == 0, out.stderr
+    assert (
+        dedent(
+            """\
+            small-fake-a==0.1
+            small-fake-b==0.2
+            small-fake-c==0.3
+            small-fake-d==0.4
+            small-fake-e==0.5
+            small-fake-f==0.6
+            Dry-run, so nothing updated.
+            """
+        )
+        == out.stderr
+    )
+
+
+# This should not depend on the metadata format so testing all cases is wasteful
+@pytest.mark.parametrize(("fname", "content"), METADATA_TEST_CASES[:1])
+def test_all_extras_fail_with_extra(fake_dists, runner, make_module, fname, content):
+    """
+    Test that passing `--all-extras` and `--extra` fails.
+    """
+    meta_path = make_module(fname=fname, content=content)
+    out = runner.invoke(
+        cli,
+        [
+            "-n",
+            "--all-extras",
+            "--extra",
+            "dev",
+            "--find-links",
+            fake_dists,
+            "--no-annotate",
+            "--no-emit-options",
+            "--no-header",
+            meta_path,
+        ],
+    )
+    assert out.exit_code == 2
+    exp = "--extra has no effect when used with --all-extras"
+    assert exp in out.stderr
+
+
 def test_extras_fail_with_requirements_in(runner, tmpdir):
     """
     Test that passing `--extra` with `requirements.in` input file fails.
     """
     path = os.path.join(tmpdir, "requirements.in")
     with open(path, "w") as stream:
         stream.write("\n")
```

### Comparing `pip-tools-6.8.0/tests/test_cli_sync.py` & `pip-tools-6.9.0/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/fake-index.json` & `pip-tools-6.9.0/tests/test_data/fake-index.json`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl` & `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_data/packages/fake_with_deps/setup.py` & `pip-tools-6.9.0/tests/test_data/packages/fake_with_deps/setup.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_fake_index.py` & `pip-tools-6.9.0/tests/test_fake_index.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_logging.py` & `pip-tools-6.9.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_minimal_upgrade.py` & `pip-tools-6.9.0/tests/test_minimal_upgrade.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_repository_local.py` & `pip-tools-6.9.0/tests/test_repository_local.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_repository_pypi.py` & `pip-tools-6.9.0/tests/test_repository_pypi.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_resolver.py` & `pip-tools-6.9.0/tests/test_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,29 +148,27 @@
                 ["setuptools==35.0.0", "anyjson==0.3.3"],
                 ["anyjson==0.3.3"],
                 False,
                 {"setuptools==35.0.0"},
             ),
             (
                 ["fake-piptools-test-with-unsafe-deps==0.1"],
-                ["fake-piptools-test-with-unsafe-deps==0.1"],
+                [
+                    "appdirs==1.4.9 (from "
+                    "setuptools==34.0.0->fake-piptools-test-with-unsafe-deps==0.1)",
+                    "fake-piptools-test-with-unsafe-deps==0.1",
+                    "packaging==16.8 (from "
+                    "setuptools==34.0.0->fake-piptools-test-with-unsafe-deps==0.1)",
+                ],
                 False,
                 {
                     (
                         "setuptools==34.0.0 (from "
                         "fake-piptools-test-with-unsafe-deps==0.1)"
                     ),
-                    (
-                        "appdirs==1.4.9 (from "
-                        "setuptools==34.0.0->fake-piptools-test-with-unsafe-deps==0.1)"
-                    ),
-                    (
-                        "packaging==16.8 (from "
-                        "setuptools==34.0.0->fake-piptools-test-with-unsafe-deps==0.1)"
-                    ),
                 },
             ),
             # Git URL requirement
             # See: GH-851
             (
                 [
                     "git+https://github.com/celery/billiard#egg=billiard==3.5.9999",
@@ -246,14 +244,63 @@
     input = [line if isinstance(line, tuple) else (line, False) for line in input]
     input = [from_line(req[0], constraint=req[1]) for req in input]
     output = resolver(input, prereleases=prereleases, allow_unsafe=True).resolve()
     output = {str(line) for line in output}
     assert output == {str(line) for line in expected}
 
 
+@pytest.mark.parametrize(
+    (
+        "input",
+        "expected",
+        "unsafe_packages",
+        "unsafe_constraints",
+    ),
+    (
+        (
+            ["fake-piptools-test-with-pinned-deps==0.1"],
+            {
+                "fake-piptools-test-with-pinned-deps==0.1",
+                "pytz==2016.4 (from celery==3.1.18->fake-piptools-test-with-pinned-deps==0.1)",
+                "billiard==3.3.0.23 (from "
+                "celery==3.1.18->fake-piptools-test-with-pinned-deps==0.1)",
+                "celery==3.1.18 (from fake-piptools-test-with-pinned-deps==0.1)",
+                "anyjson==0.3.3 (from "
+                "kombu==3.0.35->celery==3.1.18->fake-piptools-test-with-pinned-deps==0.1)",
+                "amqp==1.4.9 (from "
+                "kombu==3.0.35->celery==3.1.18->fake-piptools-test-with-pinned-deps==0.1)",
+            },
+            {"kombu"},
+            {
+                "kombu==3.0.35 (from celery==3.1.18->fake-piptools-test-with-pinned-deps==0.1)",
+            },
+        ),
+    ),
+)
+def test_resolver__custom_unsafe_deps(
+    resolver,
+    from_line,
+    input,
+    expected,
+    unsafe_packages,
+    unsafe_constraints,
+):
+    input = [line if isinstance(line, tuple) else (line, False) for line in input]
+    input = [from_line(req[0], constraint=req[1]) for req in input]
+    resolver = resolver(
+        input,
+        unsafe_packages=unsafe_packages,
+    )
+    output = resolver.resolve()
+    output = {str(line) for line in output}
+
+    assert output == expected
+    assert {str(line) for line in resolver.unsafe_constraints} == unsafe_constraints
+
+
 def test_resolver__max_number_rounds_reached(resolver, from_line):
     """
     Resolver should raise an exception if max round has been reached.
     """
     input = [from_line("django")]
     with pytest.raises(RuntimeError, match="after 0 rounds of resolving"):
         resolver(input).resolve(max_rounds=0)
```

### Comparing `pip-tools-6.8.0/tests/test_sync.py` & `pip-tools-6.9.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_utils.py` & `pip-tools-6.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tests/test_writer.py` & `pip-tools-6.9.0/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `pip-tools-6.8.0/tox.ini` & `pip-tools-6.9.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     testing
     coverage: coverage
 deps =
     pipprevious: pip==21.3.*
     piplatest: pip
     pipmain: -e git+https://github.com/pypa/pip.git@main#egg=pip
 setenv =
-    coverage: PYTEST_ADDOPTS=--strict --doctest-modules --cov --cov-report=term-missing --cov-report=xml {env:PYTEST_ADDOPTS:}
+    coverage: PYTEST_ADDOPTS=--strict-markers --doctest-modules --cov --cov-report=term-missing --cov-report=xml {env:PYTEST_ADDOPTS:}
 commands_pre =
     piplatest: python -m pip install -U pip
     pip --version
 commands = pytest {posargs}
 passenv = CI GITHUB_ACTIONS
 pip_pre=True
```

