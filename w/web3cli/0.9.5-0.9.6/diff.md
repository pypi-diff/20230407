# Comparing `tmp/web3cli-0.9.5.tar.gz` & `tmp/web3cli-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3cli-0.9.5.tar", last modified: Sat Dec  3 21:05:59 2022, max compression
+gzip compressed data, was "web3cli-0.9.6.tar", last modified: Sun Dec 11 20:04:43 2022, max compression
```

## Comparing `web3cli-0.9.5.tar` & `web3cli-0.9.6.tar`

### file list

```diff
@@ -1,81 +1,80 @@
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1069 2022-10-24 15:49:55.999119 web3cli-0.9.5/LICENSE
--rw-r--r--   0 coccoinomane   (502) staff       (20)     8641 2022-12-03 18:18:45.591730 web3cli-0.9.5/README.md
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2257 2022-12-03 21:05:36.937620 web3cli-0.9.5/pyproject.toml
--rw-r--r--   0 coccoinomane   (502) staff       (20)     6148 2022-11-13 07:56:22.807127 web3cli-0.9.5/src/web3cli/.DS_Store
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-18 22:32:14.016225 web3cli-0.9.5/src/web3cli/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-10-24 15:34:40.198985 web3cli-0.9.5/src/web3cli/controllers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2052 2022-12-03 12:55:29.496647 web3cli-0.9.5/src/web3cli/controllers/base_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2359 2022-12-03 10:51:12.400264 web3cli-0.9.5/src/web3cli/controllers/config_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1108 2022-12-03 10:52:07.292763 web3cli-0.9.5/src/web3cli/controllers/controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2538 2022-12-03 11:08:30.876281 web3cli-0.9.5/src/web3cli/controllers/db/address_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     4018 2022-12-03 11:08:39.937873 web3cli-0.9.5/src/web3cli/controllers/db/chain_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      700 2022-12-03 10:49:19.507131 web3cli-0.9.5/src/web3cli/controllers/db/db_base_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3548 2022-12-03 11:09:01.224477 web3cli-0.9.5/src/web3cli/controllers/db/rpc_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     4205 2022-12-03 11:09:14.366589 web3cli-0.9.5/src/web3cli/controllers/db/signer_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3058 2022-12-03 11:09:19.399304 web3cli-0.9.5/src/web3cli/controllers/db/tx_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2126 2022-12-03 10:51:06.945706 web3cli-0.9.5/src/web3cli/controllers/key_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1299 2022-12-03 12:55:44.118274 web3cli-0.9.5/src/web3cli/controllers/misc_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2279 2022-12-03 12:47:55.890188 web3cli-0.9.5/src/web3cli/controllers/send_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      120 2022-11-03 17:39:28.958124 web3cli-0.9.5/src/web3cli/core/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1194 2022-12-01 17:32:47.153512 web3cli-0.9.5/src/web3cli/core/exceptions.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-03 17:39:28.958845 web3cli-0.9.5/src/web3cli/core/helpers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1715 2022-12-01 17:32:41.983115 web3cli-0.9.5/src/web3cli/core/helpers/client_factory.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1059 2022-11-13 21:16:43.600419 web3cli-0.9.5/src/web3cli/core/helpers/crypto.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      879 2022-12-01 15:14:54.384063 web3cli-0.9.5/src/web3cli/core/helpers/database.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      434 2022-11-28 18:04:28.138080 web3cli-0.9.5/src/web3cli/core/helpers/format.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      547 2022-12-01 15:47:50.137183 web3cli-0.9.5/src/web3cli/core/helpers/input.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      327 2022-11-05 10:06:17.379240 web3cli-0.9.5/src/web3cli/core/helpers/os.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      516 2022-11-21 18:11:44.306582 web3cli-0.9.5/src/web3cli/core/helpers/rpc.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1209 2022-12-01 15:48:21.715482 web3cli-0.9.5/src/web3cli/core/helpers/yaml.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-05 09:21:32.723633 web3cli-0.9.5/src/web3cli/core/models/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3449 2022-12-03 21:05:04.266707 web3cli-0.9.5/src/web3cli/core/models/address.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      771 2022-12-01 16:54:00.585577 web3cli-0.9.5/src/web3cli/core/models/base_model.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     5219 2022-12-03 21:02:52.946105 web3cli-0.9.5/src/web3cli/core/models/chain.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1556 2022-12-01 17:28:54.846253 web3cli-0.9.5/src/web3cli/core/models/signer.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1056 2022-12-02 22:09:26.397612 web3cli-0.9.5/src/web3cli/core/models/timestamps_model.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2966 2022-12-03 21:05:11.976714 web3cli-0.9.5/src/web3cli/core/models/tx.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1036 2022-12-02 20:11:58.691980 web3cli-0.9.5/src/web3cli/core/models/types.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)       48 2022-11-18 22:43:37.360850 web3cli-0.9.5/src/web3cli/core/seeds/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1299 2022-12-03 17:12:38.552472 web3cli-0.9.5/src/web3cli/core/seeds/chain_seeds.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)       60 2022-11-20 21:14:50.670605 web3cli-0.9.5/src/web3cli/core/types.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      289 2022-12-03 18:13:48.115404 web3cli-0.9.5/src/web3cli/extensions/ext_prettydict.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-10-24 15:34:40.191413 web3cli-0.9.5/src/web3cli/helpers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3007 2022-12-03 11:09:23.233451 web3cli-0.9.5/src/web3cli/helpers/args.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      929 2022-12-03 11:09:26.353421 web3cli-0.9.5/src/web3cli/helpers/client_factory.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1258 2022-12-01 15:48:40.508984 web3cli-0.9.5/src/web3cli/helpers/config.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      936 2022-11-24 17:21:33.254156 web3cli-0.9.5/src/web3cli/helpers/crypto.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1019 2022-11-13 21:59:26.623692 web3cli-0.9.5/src/web3cli/helpers/database.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      347 2022-11-21 18:39:07.034800 web3cli-0.9.5/src/web3cli/helpers/misc.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      808 2022-12-03 18:29:40.979538 web3cli-0.9.5/src/web3cli/helpers/render.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2113 2022-11-21 18:06:06.928432 web3cli-0.9.5/src/web3cli/helpers/send.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      434 2022-12-03 21:05:42.147594 web3cli-0.9.5/src/web3cli/helpers/version.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2094 2022-11-28 18:19:24.889986 web3cli-0.9.5/src/web3cli/hooks.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3897 2022-12-03 21:03:50.306041 web3cli-0.9.5/src/web3cli/main.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-10-24 15:34:40.196707 web3cli-0.9.5/src/web3cli/templates/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)       82 2022-12-03 16:44:27.366677 web3cli-0.9.5/src/web3cli/templates/balance.jinja2
--rw-r--r--   0 coccoinomane   (502) staff       (20)     6148 2022-12-03 17:32:49.089202 web3cli-0.9.5/tests/.DS_Store
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.296564 web3cli-0.9.5/tests/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2463 2022-12-03 17:32:27.616031 web3cli-0.9.5/tests/brownie/build/tests.json
--rw-r--r--   0 coccoinomane   (502) staff       (20)       50 2022-12-03 17:35:04.016328 web3cli-0.9.5/tests/brownie/contracts/.gitignore
--rw-r--r--   0 coccoinomane   (502) staff       (20)     5737 2022-12-02 22:06:52.240730 web3cli-0.9.5/tests/conftest.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.297637 web3cli-0.9.5/tests/controllers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3800 2022-12-03 11:08:00.178773 web3cli-0.9.5/tests/controllers/db/test_address.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3205 2022-12-03 11:02:45.632355 web3cli-0.9.5/tests/controllers/db/test_chain.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3778 2022-12-03 10:58:08.499190 web3cli-0.9.5/tests/controllers/db/test_rpc.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     5040 2022-12-03 11:08:03.254225 web3cli-0.9.5/tests/controllers/db/test_signer.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2643 2022-12-03 10:58:53.760955 web3cli-0.9.5/tests/controllers/db/test_tx.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3030 2022-12-03 10:56:33.399744 web3cli-0.9.5/tests/controllers/test_base.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1816 2022-11-24 17:21:33.295121 web3cli-0.9.5/tests/controllers/test_key.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.301380 web3cli-0.9.5/tests/core/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.301610 web3cli-0.9.5/tests/core/helpers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      530 2022-11-10 21:50:51.303151 web3cli-0.9.5/tests/core/helpers/test_crypto.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1183 2022-11-13 21:19:59.445849 web3cli-0.9.5/tests/helper.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.303802 web3cli-0.9.5/tests/helpers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1676 2022-12-03 10:54:01.164673 web3cli-0.9.5/tests/helpers/test_client_factory.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      675 2022-11-21 18:49:29.825823 web3cli-0.9.5/tests/helpers/test_crypto.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1395 2022-11-23 09:21:24.664025 web3cli-0.9.5/tests/main.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.305787 web3cli-0.9.5/tests/resolvers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1514 2022-12-01 18:58:26.365291 web3cli-0.9.5/tests/resolvers/test_resolve_address.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3219 2022-12-03 17:14:55.639133 web3cli-0.9.5/tests/seeder.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      385 2022-12-03 11:01:40.965568 web3cli-0.9.5/tests/test_main.py
--rw-------   0 coccoinomane   (502) staff       (20)     9100 2022-12-03 21:05:59.813202 web3cli-0.9.5/PKG-INFO
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1069 2022-10-24 15:49:55.999119 web3cli-0.9.6/LICENSE
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     8703 2022-12-11 19:42:34.523799 web3cli-0.9.6/README.md
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2376 2022-12-11 20:04:17.698155 web3cli-0.9.6/pyproject.toml
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     6148 2022-11-13 07:56:22.807127 web3cli-0.9.6/src/web3cli/.DS_Store
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-18 22:32:14.016225 web3cli-0.9.6/src/web3cli/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-10-24 15:34:40.198985 web3cli-0.9.6/src/web3cli/controllers/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2052 2022-12-03 21:33:10.100716 web3cli-0.9.6/src/web3cli/controllers/base_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2359 2022-12-03 21:55:45.786745 web3cli-0.9.6/src/web3cli/controllers/config_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1108 2022-12-03 10:52:07.292763 web3cli-0.9.6/src/web3cli/controllers/controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2538 2022-12-03 11:08:30.876281 web3cli-0.9.6/src/web3cli/controllers/db/address_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     4018 2022-12-03 11:08:39.937873 web3cli-0.9.6/src/web3cli/controllers/db/chain_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1232 2022-12-11 20:02:34.012601 web3cli-0.9.6/src/web3cli/controllers/db/db_base_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3548 2022-12-03 11:09:01.224477 web3cli-0.9.6/src/web3cli/controllers/db/rpc_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     4205 2022-12-03 11:09:14.366589 web3cli-0.9.6/src/web3cli/controllers/db/signer_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3084 2022-12-03 21:56:25.229723 web3cli-0.9.6/src/web3cli/controllers/db/tx_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2126 2022-12-03 10:51:06.945706 web3cli-0.9.6/src/web3cli/controllers/key_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1299 2022-12-03 12:55:44.118274 web3cli-0.9.6/src/web3cli/controllers/misc_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2279 2022-12-03 12:47:55.890188 web3cli-0.9.6/src/web3cli/controllers/send_controller.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      120 2022-11-03 17:39:28.958124 web3cli-0.9.6/src/web3cli/core/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1194 2022-12-01 17:32:47.153512 web3cli-0.9.6/src/web3cli/core/exceptions.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-03 17:39:28.958845 web3cli-0.9.6/src/web3cli/core/helpers/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1715 2022-12-01 17:32:41.983115 web3cli-0.9.6/src/web3cli/core/helpers/client_factory.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1059 2022-11-13 21:16:43.600419 web3cli-0.9.6/src/web3cli/core/helpers/crypto.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      879 2022-12-01 15:14:54.384063 web3cli-0.9.6/src/web3cli/core/helpers/database.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      434 2022-11-28 18:04:28.138080 web3cli-0.9.6/src/web3cli/core/helpers/format.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      562 2022-12-11 19:57:58.584818 web3cli-0.9.6/src/web3cli/core/helpers/input.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      327 2022-11-05 10:06:17.379240 web3cli-0.9.6/src/web3cli/core/helpers/os.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      516 2022-11-21 18:11:44.306582 web3cli-0.9.6/src/web3cli/core/helpers/rpc.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1209 2022-12-01 15:48:21.715482 web3cli-0.9.6/src/web3cli/core/helpers/yaml.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-05 09:21:32.723633 web3cli-0.9.6/src/web3cli/core/models/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3449 2022-12-03 21:05:04.266707 web3cli-0.9.6/src/web3cli/core/models/address.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      771 2022-12-01 16:54:00.585577 web3cli-0.9.6/src/web3cli/core/models/base_model.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     5219 2022-12-03 21:02:52.946105 web3cli-0.9.6/src/web3cli/core/models/chain.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1556 2022-12-01 17:28:54.846253 web3cli-0.9.6/src/web3cli/core/models/signer.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1056 2022-12-02 22:09:26.397612 web3cli-0.9.6/src/web3cli/core/models/timestamps_model.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2966 2022-12-03 21:05:11.976714 web3cli-0.9.6/src/web3cli/core/models/tx.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1036 2022-12-02 20:11:58.691980 web3cli-0.9.6/src/web3cli/core/models/types.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)       48 2022-11-18 22:43:37.360850 web3cli-0.9.6/src/web3cli/core/seeds/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1299 2022-12-03 17:12:38.552472 web3cli-0.9.6/src/web3cli/core/seeds/chain_seeds.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)       60 2022-11-20 21:14:50.670605 web3cli-0.9.6/src/web3cli/core/types.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-10-24 15:34:40.191413 web3cli-0.9.6/src/web3cli/helpers/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3007 2022-12-03 11:09:23.233451 web3cli-0.9.6/src/web3cli/helpers/args.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      929 2022-12-03 11:09:26.353421 web3cli-0.9.6/src/web3cli/helpers/client_factory.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1258 2022-12-01 15:48:40.508984 web3cli-0.9.6/src/web3cli/helpers/config.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      936 2022-11-24 17:21:33.254156 web3cli-0.9.6/src/web3cli/helpers/crypto.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1124 2022-12-11 20:00:04.245201 web3cli-0.9.6/src/web3cli/helpers/database.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      347 2022-11-21 18:39:07.034800 web3cli-0.9.6/src/web3cli/helpers/misc.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      808 2022-12-03 18:29:40.979538 web3cli-0.9.6/src/web3cli/helpers/render.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2113 2022-11-21 18:06:06.928432 web3cli-0.9.6/src/web3cli/helpers/send.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      434 2022-12-11 20:04:05.874534 web3cli-0.9.6/src/web3cli/helpers/version.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2094 2022-11-28 18:19:24.889986 web3cli-0.9.6/src/web3cli/hooks.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3897 2022-12-11 19:56:44.416663 web3cli-0.9.6/src/web3cli/main.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-10-24 15:34:40.196707 web3cli-0.9.6/src/web3cli/templates/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)       82 2022-12-03 16:44:27.366677 web3cli-0.9.6/src/web3cli/templates/balance.jinja2
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     6148 2022-12-03 17:32:49.089202 web3cli-0.9.6/tests/.DS_Store
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.296564 web3cli-0.9.6/tests/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2463 2022-12-03 21:58:57.495576 web3cli-0.9.6/tests/brownie/build/tests.json
+-rw-r--r--   0 coccoinomane   (502) staff       (20)       50 2022-12-03 17:35:04.016328 web3cli-0.9.6/tests/brownie/contracts/.gitignore
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     5737 2022-12-02 22:06:52.240730 web3cli-0.9.6/tests/conftest.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.297637 web3cli-0.9.6/tests/controllers/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3800 2022-12-03 11:08:00.178773 web3cli-0.9.6/tests/controllers/db/test_address.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3205 2022-12-03 11:02:45.632355 web3cli-0.9.6/tests/controllers/db/test_chain.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3778 2022-12-03 10:58:08.499190 web3cli-0.9.6/tests/controllers/db/test_rpc.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     5040 2022-12-03 11:08:03.254225 web3cli-0.9.6/tests/controllers/db/test_signer.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     2643 2022-12-03 10:58:53.760955 web3cli-0.9.6/tests/controllers/db/test_tx.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3030 2022-12-03 10:56:33.399744 web3cli-0.9.6/tests/controllers/test_base.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1816 2022-11-24 17:21:33.295121 web3cli-0.9.6/tests/controllers/test_key.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.301380 web3cli-0.9.6/tests/core/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.301610 web3cli-0.9.6/tests/core/helpers/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      530 2022-11-10 21:50:51.303151 web3cli-0.9.6/tests/core/helpers/test_crypto.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1183 2022-11-13 21:19:59.445849 web3cli-0.9.6/tests/helper.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.303802 web3cli-0.9.6/tests/helpers/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1676 2022-12-03 10:54:01.164673 web3cli-0.9.6/tests/helpers/test_client_factory.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      675 2022-11-21 18:49:29.825823 web3cli-0.9.6/tests/helpers/test_crypto.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1395 2022-11-23 09:21:24.664025 web3cli-0.9.6/tests/main.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.305787 web3cli-0.9.6/tests/resolvers/__init__.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     1514 2022-12-01 18:58:26.365291 web3cli-0.9.6/tests/resolvers/test_resolve_address.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)     3219 2022-12-03 17:14:55.639133 web3cli-0.9.6/tests/seeder.py
+-rw-r--r--   0 coccoinomane   (502) staff       (20)      385 2022-12-03 11:01:40.965568 web3cli-0.9.6/tests/test_main.py
+-rw-------   0 coccoinomane   (502) staff       (20)     9162 2022-12-11 20:04:43.466283 web3cli-0.9.6/PKG-INFO
```

### Comparing `web3cli-0.9.5/LICENSE` & `web3cli-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/README.md` & `web3cli-0.9.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,15 @@
 
 Thank you very much to the [web3.py](https://github.com/ethereum/web3.py) and [`brownie`](https://github.com/eth-brownie/brownie) teams: `web3` would not exist without your efforts!
 
 
 # TODO
 - Define command shortcuts using argparse aliases, e.g. `w3 add-chain` instead of `w3 db chain add`
 - Use different db file for dev environment
+- README: Explain json output + trick `| python3 -mjson.tool`
 - Implement `w3 block`
 - Implement `w3 tx fetch`
 - Move tests/seeder to core (in models?)
 - Tests: use london hardfork instead of istanbul?
 - Send command: option to wait for receipt
 - Retry transactions until gas fee goes below x gwei
 - README badges: web3.py, brownie, PDM, cement
```

### Comparing `web3cli-0.9.5/pyproject.toml` & `web3cli-0.9.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3cli"
-version = "0.9.5"
+version = "0.9.6"
 description = "Interact with blockchains and smart contracts using the command line"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
@@ -50,14 +50,15 @@
 [tool.pdm.scripts]
 test = "brownie test tests"
 test_verbose = "brownie test tests -s"
 test_fast = "brownie test tests -m 'not slow'"
 db_open = "open -a TablePlus $HOME/.web3cli/database/web3cli.sqlite"
 db_clean = "rm -rf $HOME/.web3cli/database"
 docker = "pdm run clean && docker build -t web3cli:latest ."
+release = "gh release create v{args} dist/web3cli-{args}.tar.gz dist/web3cli-{args}-py3-none-any.whl --generate-notes"
 
 [tool.pdm.scripts.w3]
 help = "Run the CLI in development mode"
 cmd = "w3"
 
 [tool.pdm.build]
 includes = [
```

### Comparing `web3cli-0.9.5/src/web3cli/.DS_Store` & `web3cli-0.9.6/src/web3cli/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/base_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/config_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/config_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/controller.py` & `web3cli-0.9.6/src/web3cli/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/db/address_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/db/address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/db/chain_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/db/chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/db/rpc_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/db/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/db/signer_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/db/signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/db/tx_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/db/tx_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         help="show details of the given transaction",
         arguments=[
             (["hash"], {"help": "hash of the transaction"}),
         ],
     )
     def get(self) -> None:
         tx = Tx.get_by_hash_or_raise(self.app.pargs.hash)
-        self.app.render(model_to_dict(tx))
+        self.app.render(model_to_dict(tx), indent=4, handler="json")
 
     @ex(
         help="add a new transaction to the database",
         arguments=[
             (["hash"], {"help": "hash of the transaction"}),
             (
                 ["from"],
```

### Comparing `web3cli-0.9.5/src/web3cli/controllers/key_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/key_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/misc_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/controllers/send_controller.py` & `web3cli-0.9.6/src/web3cli/controllers/send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/exceptions.py` & `web3cli-0.9.6/src/web3cli/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/helpers/client_factory.py` & `web3cli-0.9.6/src/web3cli/core/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/helpers/crypto.py` & `web3cli-0.9.6/src/web3cli/core/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/helpers/database.py` & `web3cli-0.9.6/src/web3cli/core/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/helpers/rpc.py` & `web3cli-0.9.6/src/web3cli/core/helpers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/helpers/yaml.py` & `web3cli-0.9.6/src/web3cli/core/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/models/address.py` & `web3cli-0.9.6/src/web3cli/core/models/address.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/models/base_model.py` & `web3cli-0.9.6/src/web3cli/core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/models/chain.py` & `web3cli-0.9.6/src/web3cli/core/models/chain.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/models/signer.py` & `web3cli-0.9.6/src/web3cli/core/models/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/models/timestamps_model.py` & `web3cli-0.9.6/src/web3cli/core/models/timestamps_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/models/tx.py` & `web3cli-0.9.6/src/web3cli/core/models/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/models/types.py` & `web3cli-0.9.6/src/web3cli/core/models/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/core/seeds/chain_seeds.py` & `web3cli-0.9.6/src/web3cli/core/seeds/chain_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/helpers/args.py` & `web3cli-0.9.6/src/web3cli/helpers/args.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/helpers/client_factory.py` & `web3cli-0.9.6/src/web3cli/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/helpers/config.py` & `web3cli-0.9.6/src/web3cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/helpers/crypto.py` & `web3cli-0.9.6/src/web3cli/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/helpers/render.py` & `web3cli-0.9.6/src/web3cli/helpers/render.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/helpers/send.py` & `web3cli-0.9.6/src/web3cli/helpers/send.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/hooks.py` & `web3cli-0.9.6/src/web3cli/hooks.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/src/web3cli/main.py` & `web3cli-0.9.6/src/web3cli/main.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/.DS_Store` & `web3cli-0.9.6/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/brownie/build/tests.json` & `web3cli-0.9.6/tests/brownie/build/tests.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965277777777777%*

 * *Differences: {"'tests'": "{'tests/controllers/db/test_address.py': {'sha1': "*

 * *            "'8796dd41c3abfcd171156e30aea6b476e232e14e'}, 'tests/controllers/db/test_chain.py': "*

 * *            "{'sha1': '868a26c3e9acb4c0467d7d587e7e06a377a7b868'}, "*

 * *            "'tests/controllers/db/test_rpc.py': {'sha1': "*

 * *            "'4bd939d93d093a7222b6faf1fa95d2d74c7518e7'}, 'tests/controllers/db/test_tx.py': "*

 * *            "{'sha1': '47a34a69df38b60f21d2d40bd234e0d16717da73'}, "*

 * *            "'tests/resolvers/test_resolve_address.py':  […]*

```diff
@@ -1,43 +1,43 @@
 {
     "contracts": {},
     "tests": {
         "tests/controllers/db/test_address.py": {
             "coverage": false,
             "isolated": false,
             "results": "........",
-            "sha1": "9b5eb58b5d326e6c9c6e73874b1c94f3bc038c97",
+            "sha1": "8796dd41c3abfcd171156e30aea6b476e232e14e",
             "txhash": []
         },
         "tests/controllers/db/test_chain.py": {
             "coverage": false,
             "isolated": false,
             "results": ".....",
-            "sha1": "250a3db5df1b30b1182c5b14850976acd58782d5",
+            "sha1": "868a26c3e9acb4c0467d7d587e7e06a377a7b868",
             "txhash": []
         },
         "tests/controllers/db/test_rpc.py": {
             "coverage": false,
             "isolated": false,
             "results": "......",
-            "sha1": "64dfa50f26017281927e989f77ecb1769c0b0d21",
+            "sha1": "4bd939d93d093a7222b6faf1fa95d2d74c7518e7",
             "txhash": []
         },
         "tests/controllers/db/test_signer.py": {
             "coverage": false,
             "isolated": false,
             "results": ".....",
             "sha1": "f5b0b4e250dfe355e1726493bcf5168109e21ea3",
             "txhash": []
         },
         "tests/controllers/db/test_tx.py": {
             "coverage": false,
             "isolated": false,
             "results": ".....",
-            "sha1": "80ef54b7caa1ac1140f99f4a8a708186d00ea10c",
+            "sha1": "47a34a69df38b60f21d2d40bd234e0d16717da73",
             "txhash": []
         },
         "tests/controllers/test_base.py": {
             "coverage": false,
             "isolated": false,
             "results": "......",
             "sha1": "ec7102b06ec226e1bcdd7ca0226b3b811aa05b6b",
@@ -71,15 +71,15 @@
             "sha1": "f5acb62600b7a1bdc9f42293ae592496cb8b77eb",
             "txhash": []
         },
         "tests/resolvers/test_resolve_address.py": {
             "coverage": false,
             "isolated": false,
             "results": "...",
-            "sha1": "469408c12f1a5998f1dc659ee6d61e06d2e7425e",
+            "sha1": "92a4cc5877bc1b88bf4f99714133869b82ec947f",
             "txhash": []
         },
         "tests/test_main.py": {
             "coverage": false,
             "isolated": false,
             "results": "..",
             "sha1": "2d57a9895f637315577935f81fd92e667acc6741",
```

### Comparing `web3cli-0.9.5/tests/conftest.py` & `web3cli-0.9.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/controllers/db/test_address.py` & `web3cli-0.9.6/tests/controllers/db/test_address.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/controllers/db/test_chain.py` & `web3cli-0.9.6/tests/controllers/db/test_chain.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/controllers/db/test_rpc.py` & `web3cli-0.9.6/tests/controllers/db/test_rpc.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/controllers/db/test_signer.py` & `web3cli-0.9.6/tests/controllers/db/test_signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/controllers/db/test_tx.py` & `web3cli-0.9.6/tests/controllers/db/test_tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/controllers/test_base.py` & `web3cli-0.9.6/tests/controllers/test_base.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/controllers/test_key.py` & `web3cli-0.9.6/tests/controllers/test_key.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/core/helpers/test_crypto.py` & `web3cli-0.9.6/tests/core/helpers/test_crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/helper.py` & `web3cli-0.9.6/tests/helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/helpers/test_client_factory.py` & `web3cli-0.9.6/tests/helpers/test_client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/helpers/test_crypto.py` & `web3cli-0.9.6/tests/helpers/test_crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/main.py` & `web3cli-0.9.6/tests/main.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/resolvers/test_resolve_address.py` & `web3cli-0.9.6/tests/resolvers/test_resolve_address.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/tests/seeder.py` & `web3cli-0.9.6/tests/seeder.py`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.5/PKG-INFO` & `web3cli-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3cli
-Version: 0.9.5
+Version: 0.9.6
 Summary: Interact with blockchains and smart contracts using the command line
 License: MIT
 Keywords: web3,w3,cli,evm,blockchain,ethereum,binance,avalanche
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.7.2,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3cli
 Project-URL: repository, https://github.com/coccoinomane/web3cli
@@ -252,14 +252,15 @@
 
 Thank you very much to the [web3.py](https://github.com/ethereum/web3.py) and [`brownie`](https://github.com/eth-brownie/brownie) teams: `web3` would not exist without your efforts!
 
 
 # TODO
 - Define command shortcuts using argparse aliases, e.g. `w3 add-chain` instead of `w3 db chain add`
 - Use different db file for dev environment
+- README: Explain json output + trick `| python3 -mjson.tool`
 - Implement `w3 block`
 - Implement `w3 tx fetch`
 - Move tests/seeder to core (in models?)
 - Tests: use london hardfork instead of istanbul?
 - Send command: option to wait for receipt
 - Retry transactions until gas fee goes below x gwei
 - README badges: web3.py, brownie, PDM, cement
```

