# Comparing `tmp/whatrecord-0.4.2.tar.gz` & `tmp/whatrecord-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatrecord-0.4.2.tar", last modified: Tue Nov 22 17:08:54 2022, max compression
+gzip compressed data, was "whatrecord-0.4.4.tar", last modified: Fri Apr  7 19:50:01 2023, max compression
```

## Comparing `whatrecord-0.4.2.tar` & `whatrecord-0.4.4.tar`

### file list

```diff
@@ -1,184 +1,278 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.425271 whatrecord-0.4.2/
--rw-r--r--   0 klauer   (1318172782) 1704612529      152 2022-06-03 18:48:21.000000 whatrecord-0.4.2/AUTHORS.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529     7604 2022-06-03 18:48:21.000000 whatrecord-0.4.2/LICENSE.md
--rw-r--r--   0 klauer   (1318172782) 1704612529      491 2022-06-03 18:48:21.000000 whatrecord-0.4.2/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529     6078 2022-11-22 17:08:54.425492 whatrecord-0.4.2/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     5676 2022-11-22 17:08:44.000000 whatrecord-0.4.2/README.rst
--rw-r--r--   0 klauer   (1318172782) 1704612529      342 2022-11-22 17:08:44.000000 whatrecord-0.4.2/dev-requirements.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      156 2022-11-22 17:08:44.000000 whatrecord-0.4.2/pyproject.toml
--rw-r--r--   0 klauer   (1318172782) 1704612529       68 2022-11-22 17:08:44.000000 whatrecord-0.4.2/requirements.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      179 2022-11-22 17:08:54.426198 whatrecord-0.4.2/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529     1530 2022-11-22 17:08:44.000000 whatrecord-0.4.2/setup.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    78255 2022-06-03 18:48:21.000000 whatrecord-0.4.2/versioneer.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.426700 whatrecord-0.4.2/whatrecord/
--rw-r--r--   0 klauer   (1318172782) 1704612529      797 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529       52 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/__main__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2022-11-22 17:08:54.426838 whatrecord-0.4.2/whatrecord/_version.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    14971 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/access_security.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     6002 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/asyn.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    28661 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/autosave.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.360230 whatrecord-0.4.2/whatrecord/bin/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/bin/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2764 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/bin/deps.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     6205 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/bin/graph.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1237 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/bin/info.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      817 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/bin/iocmanager_loader.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3864 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/bin/lint.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3029 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/bin/main.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5111 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/bin/parse.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1630 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/bin/server.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5791 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/cache.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1453 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/client.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    48823 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/common.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    30702 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/db.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    14604 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/dbtemplate.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4743 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/format.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10330 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/gateway.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.367018 whatrecord-0.4.2/whatrecord/grammar/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2002 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/access_security.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529     2077 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/autosave_save.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529     3401 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/db.v3.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529     5278 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/db.v4.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529     2155 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/dbtemplate.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529      816 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/gateway.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529      728 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/lcls_epicsarch.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529     1660 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/msi-sub.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529    11254 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/snl.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529     4367 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/grammar/streamdevice.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529    36587 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/graph.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      758 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/graphql.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5195 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/gv_compat.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2725 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/ioc_finder.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4860 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/iocmanager.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2274 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/iocsh.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3866 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/macro.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    22133 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/makefile.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    29557 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/motor.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5245 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/parse.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.371274 whatrecord-0.4.2/whatrecord/plugins/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/plugins/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    13136 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/plugins/epicsarch.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5316 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/plugins/gdb_binary_info.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10626 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/plugins/happi.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4011 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/plugins/netconfig.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    14302 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/plugins/twincat_pytmc.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1012 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/plugins/util.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.373925 whatrecord-0.4.2/whatrecord/server/
--rw-r--r--   0 klauer   (1318172782) 1704612529       45 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/server/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5562 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/server/common.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    32740 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/server/server.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1067 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/server/util.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2070 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/settings.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    42728 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/shell.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    42851 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/snl.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10742 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/streamdevice.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.388868 whatrecord-0.4.2/whatrecord/tests/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5905 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/access.acf
--rw-r--r--   0 klauer   (1318172782) 1704612529      648 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/conftest.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.328407 whatrecord-0.4.2/whatrecord/tests/deps/
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.389175 whatrecord-0.4.2/whatrecord/tests/deps/base/
--rw-r--r--   0 klauer   (1318172782) 1704612529       22 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/deps/base/Makefile
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.389658 whatrecord-0.4.2/whatrecord/tests/deps/module_a/
--rw-r--r--   0 klauer   (1318172782) 1704612529       53 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/deps/module_a/Makefile
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.390050 whatrecord-0.4.2/whatrecord/tests/deps/module_b/
--rw-r--r--   0 klauer   (1318172782) 1704612529       53 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/deps/module_b/Makefile
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.390471 whatrecord-0.4.2/whatrecord/tests/deps/module_c/
--rw-r--r--   0 klauer   (1318172782) 1704612529      133 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/deps/module_c/Makefile
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.391108 whatrecord-0.4.2/whatrecord/tests/epicsarch/
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/epicsarch/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      326 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/epicsarch/test.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      984 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/example.acf
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.394937 whatrecord-0.4.2/whatrecord/tests/iocs/
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.402000 whatrecord-0.4.2/whatrecord/tests/iocs/db/
--rw-r--r--   0 klauer   (1318172782) 1704612529     1993 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/basic_asyn_motor.db
--rw-r--r--   0 klauer   (1318172782) 1704612529    18914 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/configMenu.db
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.406427 whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/
--rw-r--r--   0 klauer   (1318172782) 1704612529      283 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/basic.db
--rw-r--r--   0 klauer   (1318172782) 1704612529     1500 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/circle.db
--rw-r--r--   0 klauer   (1318172782) 1704612529      651 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/circle2.db
--rw-r--r--   0 klauer   (1318172782) 1704612529     1725 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/image.db
--rw-r--r--   0 klauer   (1318172782) 1704612529     1525 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/iq.db
--rw-r--r--   0 klauer   (1318172782) 1704612529     1354 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/pva.db
--rw-r--r--   0 klauer   (1318172782) 1704612529      955 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/table.db
--rw-r--r--   0 klauer   (1318172782) 1704612529     7592 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/save_restoreStatus.db
--rw-r--r--   0 klauer   (1318172782) 1704612529     1783 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/test.substitutions
--rw-r--r--   0 klauer   (1318172782) 1704612529    12397 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/db/test.substitutions.expanded
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.407042 whatrecord-0.4.2/whatrecord/tests/iocs/fake_ad/
--rw-r--r--   0 klauer   (1318172782) 1704612529      275 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/fake_ad/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.408297 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_a/
--rw-r--r--   0 klauer   (1318172782) 1704612529       49 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_a/ioc_a.db
--rw-r--r--   0 klauer   (1318172782) 1704612529      349 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_a/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.409538 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_access_security/
--rw-r--r--   0 klauer   (1318172782) 1704612529      116 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_access_security/as.db
--rw-r--r--   0 klauer   (1318172782) 1704612529      406 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_access_security/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.410174 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_autosave/
--rw-r--r--   0 klauer   (1318172782) 1704612529     3744 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_autosave/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.411479 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_b/
--rw-r--r--   0 klauer   (1318172782) 1704612529       66 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_b/ioc_b.db
--rw-r--r--   0 klauer   (1318172782) 1704612529      349 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_b/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.412742 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_c/
--rw-r--r--   0 klauer   (1318172782) 1704612529       49 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_c/ioc.db
--rw-r--r--   0 klauer   (1318172782) 1704612529      383 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_c/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.414193 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_d/
--rw-r--r--   0 klauer   (1318172782) 1704612529       49 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_d/ioc.db
--rw-r--r--   0 klauer   (1318172782) 1704612529      446 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_d/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.414995 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_dbloadtemplate/
--rw-r--r--   0 klauer   (1318172782) 1704612529      358 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_dbloadtemplate/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.415636 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_failure/
--rw-r--r--   0 klauer   (1318172782) 1704612529      474 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_failure/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.418024 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_sequencer/
--rw-r--r--   0 klauer   (1318172782) 1704612529     4149 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_sequencer/LICENSE
--rw-r--r--   0 klauer   (1318172782) 1704612529      811 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_sequencer/sncExEntry.st
--rw-r--r--   0 klauer   (1318172782) 1704612529     1060 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_sequencer/sncExOpt.st
--rw-r--r--   0 klauer   (1318172782) 1704612529      654 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/ioc_sequencer/sncExample.st
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.418641 whatrecord-0.4.2/whatrecord/tests/iocs/pva_misc/
--rw-r--r--   0 klauer   (1318172782) 1704612529      690 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/pva_misc/st.cmd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.420005 whatrecord-0.4.2/whatrecord/tests/iocs/pva_simple/
--rw-r--r--   0 klauer   (1318172782) 1704612529      277 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/pva_simple/ioc_pva_simple.db
--rw-r--r--   0 klauer   (1318172782) 1704612529      378 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/pva_simple/st.cmd
--rw-r--r--   0 klauer   (1318172782) 1704612529   429832 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/softIoc.dbd
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.423527 whatrecord-0.4.2/whatrecord/tests/iocs/streamdevice/
--rw-r--r--   0 klauer   (1318172782) 1704612529     1346 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/streamdevice/example.proto
--rw-r--r--   0 klauer   (1318172782) 1704612529      130 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/streamdevice/hex.proto
--rw-r--r--   0 klauer   (1318172782) 1704612529      302 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/streamdevice/st.cmd
--rw-r--r--   0 klauer   (1318172782) 1704612529     3834 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/streamdevice/test.db
--rw-r--r--   0 klauer   (1318172782) 1704612529     1308 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/streamdevice/test.proto
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.424823 whatrecord-0.4.2/whatrecord/tests/iocs/v3_ioc_a/
--rw-r--r--   0 klauer   (1318172782) 1704612529       49 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/v3_ioc_a/ioc_a.db
--rw-r--r--   0 klauer   (1318172782) 1704612529      359 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/v3_ioc_a/st.cmd
--rw-r--r--   0 klauer   (1318172782) 1704612529   387868 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/iocs/v3_softIoc.dbd
--rw-r--r--   0 klauer   (1318172782) 1704612529     3676 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/kfe.pvlist
--rw-r--r--   0 klauer   (1318172782) 1704612529      206 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/t1-include.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529     6433 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_access.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5605 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_autosave.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1596 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_bin_graph.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      657 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/test_bin_lint.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2790 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/test_bin_parse.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3276 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_cache.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    15415 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_dbtemplate.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1778 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_epicsarch.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     6471 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_gateway.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1409 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/test_gdb_integration.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10875 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/test_graph.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8872 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_iocmanager_loader.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1665 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/test_macro.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9240 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/test_makefile.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8569 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/test_pva_parsing.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     4672 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/test_serialization.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8885 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_server_handler.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1688 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_server_state.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3332 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_snl.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      894 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_streamdevice.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      695 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/tests/test_util.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10597 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/tests/test_v3_parsing.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     1515 2022-06-03 18:48:21.000000 whatrecord-0.4.2/whatrecord/transformer.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     8398 2022-11-22 17:08:44.000000 whatrecord-0.4.2/whatrecord/util.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-11-22 17:08:54.355620 whatrecord-0.4.2/whatrecord.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529     6078 2022-11-22 17:08:53.000000 whatrecord-0.4.2/whatrecord.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     4827 2022-11-22 17:08:54.000000 whatrecord-0.4.2/whatrecord.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2022-11-22 17:08:53.000000 whatrecord-0.4.2/whatrecord.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       56 2022-11-22 17:08:53.000000 whatrecord-0.4.2/whatrecord.egg-info/entry_points.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       67 2022-11-22 17:08:53.000000 whatrecord-0.4.2/whatrecord.egg-info/requires.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       11 2022-11-22 17:08:54.000000 whatrecord-0.4.2/whatrecord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.179140 whatrecord-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.151140 whatrecord-0.4.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.151140 whatrecord-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1103 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-04-07 19:49:23.000000 whatrecord-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-07 19:49:23.000000 whatrecord-0.4.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-04-07 19:49:23.000000 whatrecord-0.4.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7604 2023-04-07 19:49:23.000000 whatrecord-0.4.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-04-07 19:49:23.000000 whatrecord-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-04-07 19:49:23.000000 whatrecord-0.4.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    14825 2023-04-07 19:50:01.179140 whatrecord-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5676 2023-04-07 19:49:23.000000 whatrecord-0.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-07 19:49:23.000000 whatrecord-0.4.4/conda-recipe/conda_build_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      871 2023-04-07 19:49:23.000000 whatrecord-0.4.4/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-04-07 19:49:23.000000 whatrecord-0.4.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/docker/
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/.env
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/docker/cache/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/cache/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     1367 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/env.default
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/docker/support/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/docker/support/gateway/
+-rw-r--r--   0 runner    (1001) docker     (122)     2934 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/support/gateway/las.pvlist
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/support/happi.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1346 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/support/happi_db.json
+-rwxr-xr-x   0 runner    (1001) docker     (122)       61 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/support/run_frontend.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docker/support/start_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     4864 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/cli.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/docs/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4040 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/iocsh.md
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/lcls.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/server_client.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/tests.md
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/docs/utilities.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-07 19:49:23.000000 whatrecord-0.4.4/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/frontend/
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      330 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/babel.config.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/package.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.155140 whatrecord-0.4.4/frontend/public/
+-rw-r--r--   0 runner    (1001) docker     (122)     4414 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.159140 whatrecord-0.4.4/frontend/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/App.vue
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.159140 whatrecord-0.4.4/frontend/src/components/
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/asyn-port.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     3886 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/dictionary-table.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/epics-format-field.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     4387 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/epics-format-record.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/gateway-matches.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     3164 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/ioc-info.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/linter-results.vue
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/record-field-table.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     8346 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/recordinfo.vue
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/script-context-link.vue
+-rw-r--r--   0 runner    (1001) docker     (122)      847 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/script-context-one-link.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     6247 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/script-line.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/components/searchbar.vue
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/main.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2693 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/router.js
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/settings.js
+-rw-r--r--   0 runner    (1001) docker     (122)     8828 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/store.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.159140 whatrecord-0.4.4/frontend/src/views/
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/duplicates.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     7036 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/gateway.vue
+-rw-r--r--   0 runner    (1001) docker     (122)    10145 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/happi.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     9714 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/iocs.vue
+-rw-r--r--   0 runner    (1001) docker     (122)    10101 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/lcls_epicsarch.vue
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/logs.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/netconfig.vue
+-rw-r--r--   0 runner    (1001) docker     (122)    15702 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/pv_relations.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/script-view.vue
+-rw-r--r--   0 runner    (1001) docker     (122)    10081 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/twincat_pytmc.vue
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/src/views/whatrec.vue
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/vue.config.js
+-rw-r--r--   0 runner    (1001) docker     (122)   336369 2023-04-07 19:49:23.000000 whatrecord-0.4.4/frontend/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-07 19:49:23.000000 whatrecord-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-07 19:49:23.000000 whatrecord-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-07 19:50:01.179140 whatrecord-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.163140 whatrecord-0.4.4/whatrecord/
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-07 19:50:00.000000 whatrecord-0.4.4/whatrecord/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14971 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/access_security.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6002 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28661 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/autosave.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.167140 whatrecord-0.4.4/whatrecord/bin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/bin/deps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/bin/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/bin/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/bin/iocmanager_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3864 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/bin/lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3020 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/bin/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5111 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/bin/parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/bin/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48823 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30702 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/db.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14604 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/dbtemplate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/format.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10330 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.167140 whatrecord-0.4.4/whatrecord/grammar/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/access_security.lark
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/autosave_save.lark
+-rw-r--r--   0 runner    (1001) docker     (122)     3401 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/db.v3.lark
+-rw-r--r--   0 runner    (1001) docker     (122)     5278 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/db.v4.lark
+-rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/dbtemplate.lark
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/gateway.lark
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/lcls_epicsarch.lark
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/msi-sub.lark
+-rw-r--r--   0 runner    (1001) docker     (122)    11254 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/snl.lark
+-rw-r--r--   0 runner    (1001) docker     (122)     4367 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/grammar/streamdevice.lark
+-rw-r--r--   0 runner    (1001) docker     (122)    36587 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5195 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/gv_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/ioc_finder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4860 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/iocmanager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/iocsh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3866 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/macro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22133 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29557 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.167140 whatrecord-0.4.4/whatrecord/plugins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13136 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/plugins/epicsarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5316 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/plugins/gdb_binary_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/plugins/happi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/plugins/netconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14284 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/plugins/twincat_pytmc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/plugins/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.167140 whatrecord-0.4.4/whatrecord/server/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/server/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32740 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/server/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42728 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/shell.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42851 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/snl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/streamdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.171140 whatrecord-0.4.4/whatrecord/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5905 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/access.acf
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.147140 whatrecord-0.4.4/whatrecord/tests/deps/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.171140 whatrecord-0.4.4/whatrecord/tests/deps/base/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/deps/base/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.171140 whatrecord-0.4.4/whatrecord/tests/deps/module_a/
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/deps/module_a/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.171140 whatrecord-0.4.4/whatrecord/tests/deps/module_b/
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/deps/module_b/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.171140 whatrecord-0.4.4/whatrecord/tests/deps/module_c/
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/deps/module_c/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.171140 whatrecord-0.4.4/whatrecord/tests/epicsarch/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/epicsarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/epicsarch/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/example.acf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.171140 whatrecord-0.4.4/whatrecord/tests/iocs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/db/
+-rw-r--r--   0 runner    (1001) docker     (122)     1993 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/basic_asyn_motor.db
+-rw-r--r--   0 runner    (1001) docker     (122)    18914 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/configMenu.db
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/basic.db
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/circle.db
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/circle2.db
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/image.db
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/iq.db
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/pva.db
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/table.db
+-rw-r--r--   0 runner    (1001) docker     (122)     7592 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/save_restoreStatus.db
+-rw-r--r--   0 runner    (1001) docker     (122)     1783 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/test.substitutions
+-rw-r--r--   0 runner    (1001) docker     (122)    12397 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/db/test.substitutions.expanded
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/fake_ad/
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/fake_ad/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_a/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_a/ioc_a.db
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_a/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_access_security/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_access_security/as.db
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_access_security/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_autosave/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_autosave/autosave/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_autosave/autosave/auto_positions.req
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_autosave/autosave/auto_settings.req
+-rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_autosave/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_b/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_b/ioc_b.db
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_b/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_c/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_c/ioc.db
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_c/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_d/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_d/ioc.db
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_d/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_dbloadtemplate/
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_dbloadtemplate/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.175140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_failure/
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_failure/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.179140 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_sequencer/
+-rw-r--r--   0 runner    (1001) docker     (122)     4149 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_sequencer/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_sequencer/sncExEntry.st
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_sequencer/sncExOpt.st
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/ioc_sequencer/sncExample.st
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.179140 whatrecord-0.4.4/whatrecord/tests/iocs/pva_misc/
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/pva_misc/st.cmd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.179140 whatrecord-0.4.4/whatrecord/tests/iocs/pva_simple/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/pva_simple/ioc_pva_simple.db
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/pva_simple/st.cmd
+-rw-r--r--   0 runner    (1001) docker     (122)   429832 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/softIoc.dbd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.179140 whatrecord-0.4.4/whatrecord/tests/iocs/streamdevice/
+-rw-r--r--   0 runner    (1001) docker     (122)     1346 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/streamdevice/example.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/streamdevice/hex.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/streamdevice/st.cmd
+-rw-r--r--   0 runner    (1001) docker     (122)     3834 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/streamdevice/test.db
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/streamdevice/test.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.179140 whatrecord-0.4.4/whatrecord/tests/iocs/v3_ioc_a/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/v3_ioc_a/ioc_a.db
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/v3_ioc_a/st.cmd
+-rw-r--r--   0 runner    (1001) docker     (122)   387868 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/iocs/v3_softIoc.dbd
+-rw-r--r--   0 runner    (1001) docker     (122)     3676 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/kfe.pvlist
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/t1-include.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6433 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5605 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_autosave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_bin_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_bin_lint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2790 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_bin_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15415 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_dbtemplate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_epicsarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6471 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_gdb_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10875 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8872 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_iocmanager_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_macro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9240 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_makefile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8569 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_pva_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8885 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_server_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_server_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3332 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_snl.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_streamdevice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10597 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/tests/test_v3_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1515 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-07 19:49:23.000000 whatrecord-0.4.4/whatrecord/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 19:50:01.163140 whatrecord-0.4.4/whatrecord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14825 2023-04-07 19:50:01.000000 whatrecord-0.4.4/whatrecord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-04-07 19:50:01.000000 whatrecord-0.4.4/whatrecord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 19:50:01.000000 whatrecord-0.4.4/whatrecord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-07 19:50:01.000000 whatrecord-0.4.4/whatrecord.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-07 19:50:01.000000 whatrecord-0.4.4/whatrecord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-07 19:50:01.000000 whatrecord-0.4.4/whatrecord.egg-info/top_level.txt
```

### Comparing `whatrecord-0.4.2/LICENSE.md` & `whatrecord-0.4.4/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021, The Board of Trustees of the Leland Stanford Junior
+Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt
 of any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 (1) Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.
```

### Comparing `whatrecord-0.4.2/PKG-INFO` & `whatrecord-0.4.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: whatrecord
-Version: 0.4.2
-Summary: EPICS IOC record search and meta information tool
-Author: SLAC National Accelerator Laboratory
-License: BSD
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-License-File: LICENSE.md
-License-File: AUTHORS.rst
-
 ===============================
 whatrecord
 ===============================
 
 .. image:: https://img.shields.io/travis/pcdshub/whatrecord.svg
         :target: https://travis-ci.org/pcdshub/whatrecord
 
@@ -222,9 +208,7 @@
           "+type": "plain",
           "+channel": "VAL"
         }
       }
     }
   ]
   ...
-
-
```

### Comparing `whatrecord-0.4.2/whatrecord/__init__.py` & `whatrecord-0.4.4/whatrecord/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-from . import _version
-
-__version__ = _version.get_versions()['version']
-
 from .access_security import AccessSecurityConfig
 from .common import FileFormat
 from .db import Database
 from .dbtemplate import TemplateSubstitution
 from .gateway import GatewayConfig
 from .gateway import PVList as GatewayPVList
 from .iocsh import parse_iocsh_line
 from .macro import MacroContext
 from .parse import parse
 from .plugins.epicsarch import LclsEpicsArchFile
 from .snl import SequencerProgram
 from .streamdevice import StreamProtocol
+from .version import __version__  # noqa: F401
 
 __all__ = [
     "AccessSecurityConfig",
     "Database",
     "FileFormat",
     "GatewayConfig",
     "GatewayPVList",
```

### Comparing `whatrecord-0.4.2/whatrecord/access_security.py` & `whatrecord-0.4.4/whatrecord/access_security.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/asyn.py` & `whatrecord-0.4.4/whatrecord/asyn.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/autosave.py` & `whatrecord-0.4.4/whatrecord/autosave.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/bin/deps.py` & `whatrecord-0.4.4/whatrecord/bin/deps.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/bin/graph.py` & `whatrecord-0.4.4/whatrecord/bin/graph.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/bin/info.py` & `whatrecord-0.4.4/whatrecord/bin/info.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/bin/iocmanager_loader.py` & `whatrecord-0.4.4/whatrecord/bin/iocmanager_loader.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/bin/lint.py` & `whatrecord-0.4.4/whatrecord/bin/lint.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/bin/main.py` & `whatrecord-0.4.4/whatrecord/bin/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,8 +118,8 @@
                 func.__name__, RETURN_VALUE
             )
     else:
         top_parser.print_help()
 
 
 if __name__ == "__main__":
-    result = main()
+    main()
```

### Comparing `whatrecord-0.4.2/whatrecord/bin/parse.py` & `whatrecord-0.4.4/whatrecord/bin/parse.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/bin/server.py` & `whatrecord-0.4.4/whatrecord/bin/server.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/cache.py` & `whatrecord-0.4.4/whatrecord/cache.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/client.py` & `whatrecord-0.4.4/whatrecord/client.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/common.py` & `whatrecord-0.4.4/whatrecord/common.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/db.py` & `whatrecord-0.4.4/whatrecord/db.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/dbtemplate.py` & `whatrecord-0.4.4/whatrecord/dbtemplate.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/format.py` & `whatrecord-0.4.4/whatrecord/format.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/gateway.py` & `whatrecord-0.4.4/whatrecord/gateway.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/access_security.lark` & `whatrecord-0.4.4/whatrecord/grammar/access_security.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/autosave_save.lark` & `whatrecord-0.4.4/whatrecord/grammar/autosave_save.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/db.v3.lark` & `whatrecord-0.4.4/whatrecord/grammar/db.v3.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/db.v4.lark` & `whatrecord-0.4.4/whatrecord/grammar/db.v4.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/dbtemplate.lark` & `whatrecord-0.4.4/whatrecord/grammar/dbtemplate.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/gateway.lark` & `whatrecord-0.4.4/whatrecord/grammar/gateway.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/lcls_epicsarch.lark` & `whatrecord-0.4.4/whatrecord/grammar/lcls_epicsarch.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/msi-sub.lark` & `whatrecord-0.4.4/whatrecord/grammar/msi-sub.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/snl.lark` & `whatrecord-0.4.4/whatrecord/grammar/snl.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/grammar/streamdevice.lark` & `whatrecord-0.4.4/whatrecord/grammar/streamdevice.lark`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/graph.py` & `whatrecord-0.4.4/whatrecord/graph.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/graphql.py` & `whatrecord-0.4.4/whatrecord/graphql.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/gv_compat.py` & `whatrecord-0.4.4/whatrecord/gv_compat.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/ioc_finder.py` & `whatrecord-0.4.4/whatrecord/ioc_finder.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/iocmanager.py` & `whatrecord-0.4.4/whatrecord/iocmanager.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/iocsh.py` & `whatrecord-0.4.4/whatrecord/iocsh.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,18 +33,15 @@
 
     Returns
     -------
     IocshResult
        A partially filled IocshResult, ready for interpreting by a
        higher-level function.
     """
-    result = IocshResult(
-       context=context,
-       line=line,
-    )
+    result = IocshResult(context=context, line=line)
     # Skip leading whitespace
     line = line.lstrip()
 
     if not line.startswith("#-"):
         result.outputs.append(line)
 
     if line.startswith('#'):
```

### Comparing `whatrecord-0.4.2/whatrecord/macro.py` & `whatrecord-0.4.4/whatrecord/macro.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/makefile.py` & `whatrecord-0.4.4/whatrecord/makefile.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/motor.py` & `whatrecord-0.4.4/whatrecord/motor.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/parse.py` & `whatrecord-0.4.4/whatrecord/parse.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/plugins/epicsarch.py` & `whatrecord-0.4.4/whatrecord/plugins/epicsarch.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/plugins/gdb_binary_info.py` & `whatrecord-0.4.4/whatrecord/plugins/gdb_binary_info.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/plugins/happi.py` & `whatrecord-0.4.4/whatrecord/plugins/happi.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 from ..server.common import PluginResults
 from ..util import get_file_sha256
 from .util import suppress_output_decorator
 
 try:
     import happi
+    import happi.backends
+    import happi.backends.json_db
     import ophyd
     from ophyd.ophydobj import OphydObject
     from ophyd.signal import EpicsSignalBase
 except ImportError as ex:
     raise ImportError(f"Dependency required for happi plugin unavailable: {ex}")
 
 
@@ -329,14 +331,35 @@
     )
     parser.add_argument(
         "-p", "--pretty", action="store_true", help="Pretty JSON output"
     )
     return parser
 
 
+def get_all_happi_items(client: happi.Client) -> Generator[happi.SearchResult, None, None]:
+    """
+    Get all happi search results from the given client.
+
+    Parameters
+    ----------
+    client : happi.Client
+        The happi client instance.
+
+    Yields
+    ------
+    SearchResult
+        The happi item wrapped in a SearchResult.
+    """
+    for name in client:
+        try:
+            yield client[name]
+        except Exception:
+            logger.debug("Failed to get happi item: %s", name, exc_info=True)
+
+
 @suppress_output_decorator
 def main(search_criteria: str, pretty: bool = False):
     client = happi.Client.from_config()
 
     files_to_monitor = {}
 
     if isinstance(client.backend, happi.backends.json_db.JSONBackend):
@@ -344,16 +367,16 @@
             client.backend.path
         )
 
     results = HappiPluginResults(
         files_to_monitor=files_to_monitor,
         record_to_metadata_keys=collections.defaultdict(list),
         metadata_by_key={
-            item["name"]: dict(item)
-            for item in dict(client).values()
+            result.item["name"]: dict(result.item)
+            for result in get_all_happi_items(client)
         },
         execution_info={},
     )
 
     criteria = _parse_criteria(search_criteria)
     for root, record, sig in find_signal_metadata_pairs(criteria):
         if "." in record:
```

### Comparing `whatrecord-0.4.2/whatrecord/plugins/netconfig.py` & `whatrecord-0.4.4/whatrecord/plugins/netconfig.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/plugins/twincat_pytmc.py` & `whatrecord-0.4.4/whatrecord/plugins/twincat_pytmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from typing import Dict, Generator, Iterable, List, Optional, Tuple
 
 import apischema
 import blark
 import blark.summary
 import pytmc
 import pytmc.bin.db
-import pytmc.code
 from blark import dependency_store
 
 from .. import cache, client, util
 from ..common import AnyPath, FullLoadContext, IocMetadata, LoadContext
 from ..server.common import PluginResults
 from ..util import get_file_sha256, read_text_file_with_hash
```

### Comparing `whatrecord-0.4.2/whatrecord/plugins/util.py` & `whatrecord-0.4.4/whatrecord/plugins/util.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/server/common.py` & `whatrecord-0.4.4/whatrecord/server/common.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/server/server.py` & `whatrecord-0.4.4/whatrecord/server/server.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/server/util.py` & `whatrecord-0.4.4/whatrecord/server/util.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/settings.py` & `whatrecord-0.4.4/whatrecord/settings.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/shell.py` & `whatrecord-0.4.4/whatrecord/shell.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/snl.py` & `whatrecord-0.4.4/whatrecord/snl.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/streamdevice.py` & `whatrecord-0.4.4/whatrecord/streamdevice.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/access.acf` & `whatrecord-0.4.4/whatrecord/tests/access.acf`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/conftest.py` & `whatrecord-0.4.4/whatrecord/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/example.acf` & `whatrecord-0.4.4/whatrecord/tests/example.acf`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/basic_asyn_motor.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/basic_asyn_motor.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/configMenu.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/configMenu.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/circle.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/circle.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/circle2.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/circle2.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/image.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/image.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/iq.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/iq.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/pva.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/pva.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/pva/table.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/pva/table.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/save_restoreStatus.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/save_restoreStatus.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/test.substitutions` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/test.substitutions`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/db/test.substitutions.expanded` & `whatrecord-0.4.4/whatrecord/tests/iocs/db/test.substitutions.expanded`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/ioc_autosave/st.cmd` & `whatrecord-0.4.4/whatrecord/tests/iocs/ioc_autosave/st.cmd`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/ioc_sequencer/LICENSE` & `whatrecord-0.4.4/whatrecord/tests/iocs/ioc_sequencer/LICENSE`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/ioc_sequencer/sncExEntry.st` & `whatrecord-0.4.4/whatrecord/tests/iocs/ioc_sequencer/sncExEntry.st`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/ioc_sequencer/sncExOpt.st` & `whatrecord-0.4.4/whatrecord/tests/iocs/ioc_sequencer/sncExOpt.st`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/ioc_sequencer/sncExample.st` & `whatrecord-0.4.4/whatrecord/tests/iocs/ioc_sequencer/sncExample.st`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/pva_misc/st.cmd` & `whatrecord-0.4.4/whatrecord/tests/iocs/pva_misc/st.cmd`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/softIoc.dbd` & `whatrecord-0.4.4/whatrecord/tests/iocs/softIoc.dbd`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/streamdevice/example.proto` & `whatrecord-0.4.4/whatrecord/tests/iocs/streamdevice/example.proto`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/streamdevice/test.db` & `whatrecord-0.4.4/whatrecord/tests/iocs/streamdevice/test.db`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/streamdevice/test.proto` & `whatrecord-0.4.4/whatrecord/tests/iocs/streamdevice/test.proto`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/iocs/v3_softIoc.dbd` & `whatrecord-0.4.4/whatrecord/tests/iocs/v3_softIoc.dbd`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/kfe.pvlist` & `whatrecord-0.4.4/whatrecord/tests/kfe.pvlist`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_access.py` & `whatrecord-0.4.4/whatrecord/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_autosave.py` & `whatrecord-0.4.4/whatrecord/tests/test_autosave.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_bin_graph.py` & `whatrecord-0.4.4/whatrecord/tests/test_bin_graph.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_bin_lint.py` & `whatrecord-0.4.4/whatrecord/tests/test_bin_lint.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_bin_parse.py` & `whatrecord-0.4.4/whatrecord/tests/test_bin_parse.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_cache.py` & `whatrecord-0.4.4/whatrecord/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_dbtemplate.py` & `whatrecord-0.4.4/whatrecord/tests/test_dbtemplate.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_epicsarch.py` & `whatrecord-0.4.4/whatrecord/tests/test_epicsarch.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_gateway.py` & `whatrecord-0.4.4/whatrecord/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_gdb_integration.py` & `whatrecord-0.4.4/whatrecord/tests/test_gdb_integration.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_graph.py` & `whatrecord-0.4.4/whatrecord/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_iocmanager_loader.py` & `whatrecord-0.4.4/whatrecord/tests/test_iocmanager_loader.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_macro.py` & `whatrecord-0.4.4/whatrecord/tests/test_macro.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_makefile.py` & `whatrecord-0.4.4/whatrecord/tests/test_makefile.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_pva_parsing.py` & `whatrecord-0.4.4/whatrecord/tests/test_pva_parsing.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_serialization.py` & `whatrecord-0.4.4/whatrecord/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_server_handler.py` & `whatrecord-0.4.4/whatrecord/tests/test_server_handler.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_server_state.py` & `whatrecord-0.4.4/whatrecord/tests/test_server_state.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_snl.py` & `whatrecord-0.4.4/whatrecord/tests/test_snl.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_streamdevice.py` & `whatrecord-0.4.4/whatrecord/tests/test_streamdevice.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_util.py` & `whatrecord-0.4.4/whatrecord/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/tests/test_v3_parsing.py` & `whatrecord-0.4.4/whatrecord/tests/test_v3_parsing.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/transformer.py` & `whatrecord-0.4.4/whatrecord/transformer.py`

 * *Files identical despite different names*

### Comparing `whatrecord-0.4.2/whatrecord/util.py` & `whatrecord-0.4.4/whatrecord/util.py`

 * *Files identical despite different names*

