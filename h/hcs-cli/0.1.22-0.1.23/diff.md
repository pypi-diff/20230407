# Comparing `tmp/hcs-cli-0.1.22.tar.gz` & `tmp/hcs-cli-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.22.tar", last modified: Fri Apr  7 00:43:58 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.23.tar", last modified: Fri Apr  7 18:57:05 2023, max compression
```

## Comparing `hcs-cli-0.1.22.tar` & `hcs-cli-0.1.23.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.191244 hcs-cli-0.1.22/
--rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.22/.gitignore
--rw-r--r--   0 nanw       (501) staff       (20)      709 2023-04-07 00:38:46.000000 hcs-cli-0.1.22/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      151 2023-04-07 00:43:58.190177 hcs-cli-0.1.22/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1194 2023-04-06 16:09:03.000000 hcs-cli-0.1.22/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.113412 hcs-cli-0.1.22/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)      151 2023-04-07 00:43:57.000000 hcs-cli-0.1.22/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2075 2023-04-07 00:43:58.000000 hcs-cli-0.1.22/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-07 00:43:57.000000 hcs-cli-0.1.22/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-07 00:43:57.000000 hcs-cli-0.1.22/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 00:43:57.000000 hcs-cli-0.1.22/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)        5 2023-04-07 00:43:57.000000 hcs-cli-0.1.22/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)      297 2023-01-11 22:10:27.000000 hcs-cli-0.1.22/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-07 00:43:58.191478 hcs-cli-0.1.22/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      754 2023-04-07 00:43:52.000000 hcs-cli-0.1.22/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.114333 hcs-cli-0.1.22/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.22/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.116264 hcs-cli-0.1.22/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.118828 hcs-cli-0.1.22/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/cli/cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      486 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/cli/cmds/auth.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.120935 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.126172 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      294 2023-04-06 22:10:53.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      285 2023-04-06 22:13:28.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      225 2023-04-06 22:11:04.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.131363 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      760 2023-04-06 22:11:12.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      450 2023-04-06 22:11:17.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      285 2023-04-06 22:11:23.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      225 2023-04-06 22:11:29.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)      169 2023-04-07 00:30:38.000000 hcs-cli-0.1.22/vhcs/cli/cmds/lcm/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.137118 hcs-cli-0.1.22/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.22/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      623 2023-04-06 22:11:46.000000 hcs-cli-0.1.22/vhcs/cli/cmds/pki/delete-org-cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      262 2023-04-06 22:11:57.000000 hcs-cli-0.1.22/vhcs/cli/cmds/pki/get-root-ca.py
--rw-r--r--   0 nanw       (501) staff       (20)      398 2023-04-06 22:11:51.000000 hcs-cli-0.1.22/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.22/vhcs/cli/cmds/pki/sign-resource-cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      154 2023-04-06 22:12:12.000000 hcs-cli-0.1.22/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.138762 hcs-cli-0.1.22/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3727 2023-04-07 00:28:32.000000 hcs-cli-0.1.22/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.142548 hcs-cli-0.1.22/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.22/vhcs/cli/cmds/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      748 2023-04-06 22:12:30.000000 hcs-cli-0.1.22/vhcs/cli/cmds/vmhub/redeem-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      616 2023-04-06 22:12:37.000000 hcs-cli-0.1.22/vhcs/cli/cmds/vmhub/request-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      158 2023-04-06 22:12:43.000000 hcs-cli-0.1.22/vhcs/cli/cmds/vmhub/test.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     1815 2023-04-07 00:37:01.000000 hcs-cli-0.1.22/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.144827 hcs-cli-0.1.22/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.165451 hcs-cli-0.1.22/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      143 2023-04-07 00:17:27.000000 hcs-cli-0.1.22/vhcs/common/ctxp/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.168823 hcs-cli-0.1.22/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1222 2023-04-07 00:29:32.000000 hcs-cli-0.1.22/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     1266 2023-04-07 00:29:43.000000 hcs-cli-0.1.22/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     3049 2023-04-07 00:27:51.000000 hcs-cli-0.1.22/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/common/ctxp/cli_state.py
--rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.22/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.22/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.22/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)      541 2023-04-06 23:32:48.000000 hcs-cli-0.1.22/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     3689 2023-04-07 00:29:12.000000 hcs-cli-0.1.22/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.22/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.22/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.175812 hcs-cli-0.1.22/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.22/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.22/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     3790 2023-04-07 00:18:58.000000 hcs-cli-0.1.22/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      500 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-07 00:40:33.000000 hcs-cli-0.1.22/vhcs/common/sglib/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.178144 hcs-cli-0.1.22/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.22/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.183488 hcs-cli-0.1.22/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2138 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/service/lcm.py
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-04-06 22:13:28.000000 hcs-cli-0.1.22/vhcs/service/pki.py
--rw-r--r--   0 nanw       (501) staff       (20)     1545 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/service/vmhub.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 00:43:58.187198 hcs-cli-0.1.22/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/util/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      221 2023-04-06 02:05:21.000000 hcs-cli-0.1.22/vhcs/util/shell.py
--rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 00:34:40.000000 hcs-cli-0.1.22/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.401372 hcs-cli-0.1.23/
+-rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.23/.gitignore
+-rw-r--r--   0 nanw       (501) staff       (20)      710 2023-04-07 00:48:10.000000 hcs-cli-0.1.23/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)     1963 2023-04-07 18:57:05.400799 hcs-cli-0.1.23/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1194 2023-04-06 16:09:03.000000 hcs-cli-0.1.23/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.263767 hcs-cli-0.1.23/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     1963 2023-04-07 18:57:04.000000 hcs-cli-0.1.23/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2113 2023-04-07 18:57:05.000000 hcs-cli-0.1.23/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-07 18:57:04.000000 hcs-cli-0.1.23/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-07 18:57:04.000000 hcs-cli-0.1.23/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      126 2023-04-07 18:57:04.000000 hcs-cli-0.1.23/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        5 2023-04-07 18:57:04.000000 hcs-cli-0.1.23/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.23/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      126 2023-04-07 18:35:26.000000 hcs-cli-0.1.23/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-07 18:57:05.401535 hcs-cli-0.1.23/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      526 2023-04-07 18:56:55.000000 hcs-cli-0.1.23/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.264467 hcs-cli-0.1.23/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.23/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.265531 hcs-cli-0.1.23/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.268063 hcs-cli-0.1.23/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/cli/cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.23/vhcs/cli/cmds/auth.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.276001 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.287143 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      129 2023-04-07 18:26:44.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.303518 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      503 2023-04-07 18:57:03.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      352 2023-04-07 18:24:18.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:57:03.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      129 2023-04-07 18:26:50.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1260 2023-04-07 18:57:03.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.23/vhcs/cli/cmds/lcm/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.315468 hcs-cli-0.1.23/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.23/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.23/vhcs/cli/cmds/pki/delete-org-cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.23/vhcs/cli/cmds/pki/get-root-ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.23/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.23/vhcs/cli/cmds/pki/sign-resource-cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.23/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.316694 hcs-cli-0.1.23/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3656 2023-04-07 18:21:47.000000 hcs-cli-0.1.23/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      251 2023-04-07 18:30:52.000000 hcs-cli-0.1.23/vhcs/cli/cmds/test.py
+-rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.23/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.326881 hcs-cli-0.1.23/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.23/vhcs/cli/cmds/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.23/vhcs/cli/cmds/vmhub/redeem-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.23/vhcs/cli/cmds/vmhub/request-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.23/vhcs/cli/cmds/vmhub/test.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2072 2023-04-07 18:57:03.000000 hcs-cli-0.1.23/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.341198 hcs-cli-0.1.23/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.371806 hcs-cli-0.1.23/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      146 2023-04-07 18:02:08.000000 hcs-cli-0.1.23/vhcs/common/ctxp/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.378287 hcs-cli-0.1.23/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1222 2023-04-07 00:29:32.000000 hcs-cli-0.1.23/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1266 2023-04-07 00:29:43.000000 hcs-cli-0.1.23/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3925 2023-04-07 18:57:03.000000 hcs-cli-0.1.23/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/common/ctxp/cli_state.py
+-rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.23/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.23/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.23/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.23/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3611 2023-04-07 17:17:57.000000 hcs-cli-0.1.23/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1252 2023-04-07 18:57:03.000000 hcs-cli-0.1.23/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.23/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.23/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.388360 hcs-cli-0.1.23/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.23/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.23/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3790 2023-04-07 00:18:58.000000 hcs-cli-0.1.23/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      500 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-07 00:40:33.000000 hcs-cli-0.1.23/vhcs/common/sglib/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.390915 hcs-cli-0.1.23/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.23/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.394830 hcs-cli-0.1.23/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2115 2023-04-07 18:18:52.000000 hcs-cli-0.1.23/vhcs/service/lcm.py
+-rw-r--r--   0 nanw       (501) staff       (20)      767 2023-04-07 18:21:10.000000 hcs-cli-0.1.23/vhcs/service/pki.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1522 2023-04-07 18:22:23.000000 hcs-cli-0.1.23/vhcs/service/vmhub.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-07 18:57:05.399675 hcs-cli-0.1.23/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/util/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.23/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 00:34:40.000000 hcs-cli-0.1.23/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.22/.gitignore` & `hcs-cli-0.1.23/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/Makefile` & `hcs-cli-0.1.23/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 	export SCM_REV=$(shell git rev-parse --short HEAD); \
 	pip3 install -e .
 
 dev: clean uninstall lint build devinstall
 
 SHELL := /bin/bash
 test:
-	python -m unittest discover ./test
+	python -m unittest discover ./tests
 
 publish:
 	twine upload dist/*
 
 install:
 	pip3 install hcs-cli
```

### Comparing `hcs-cli-0.1.22/README.md` & `hcs-cli-0.1.23/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.23/hcs_cli.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 hcs_cli.egg-info/requires.txt
 hcs_cli.egg-info/top_level.txt
 vhcs/__init__.py
 vhcs/cli/__init__.py
 vhcs/cli/main.py
 vhcs/cli/cmds/__init__.py
 vhcs/cli/cmds/auth.py
+vhcs/cli/cmds/test.py
 vhcs/cli/cmds/upgrade.py
 vhcs/cli/cmds/lcm/__init__.py
 vhcs/cli/cmds/lcm/test.py
 vhcs/cli/cmds/lcm/provider/__init__.py
 vhcs/cli/cmds/lcm/provider/delete.py
 vhcs/cli/cmds/lcm/provider/get.py
 vhcs/cli/cmds/lcm/provider/list.py
 vhcs/cli/cmds/lcm/template/__init__.py
 vhcs/cli/cmds/lcm/template/create.py
 vhcs/cli/cmds/lcm/template/delete.py
 vhcs/cli/cmds/lcm/template/get.py
 vhcs/cli/cmds/lcm/template/list.py
+vhcs/cli/cmds/lcm/template/wait.py
 vhcs/cli/cmds/pki/__init__.py
 vhcs/cli/cmds/pki/delete-org-cert.py
 vhcs/cli/cmds/pki/get-root-ca.py
 vhcs/cli/cmds/pki/get_org_cert.py
 vhcs/cli/cmds/pki/sign-resource-cert.py
 vhcs/cli/cmds/pki/test.py
 vhcs/cli/cmds/profile/__init__.py
@@ -66,9 +68,8 @@
 vhcs/config/hcs-deployments.yaml
 vhcs/service/__init__.py
 vhcs/service/lcm.py
 vhcs/service/pki.py
 vhcs/service/vmhub.py
 vhcs/util/__init__.py
 vhcs/util/pki_util.py
-vhcs/util/shell.py
 vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.22/vhcs/cli/cmds/pki/delete-org-cert.py` & `hcs-cli-0.1.23/vhcs/cli/cmds/pki/delete-org-cert.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import click
-from vhcs.common.ctxp import option_output, show, panic
+from vhcs.common.ctxp import panic
 from vhcs.service import pki
 from vhcs.common.sglib.util import option_org_id, get_org_id
 
 
 @click.command()
 @option_org_id
 @click.option("--confirm/--no-confirm", default=False)
-@option_output
-def delete_org_cert(org: str, confirm: bool, output: str):
+def delete_org_cert(org: str, confirm: bool):
     """Delete the signing certificate of a specific org"""
 
     if not confirm:
         panic('Delete an org certificate will impact some service. Specify "--confirm" to perform the deletion.')
     org_id = get_org_id(org)
-    ret = pki.delete_org_cert(org_id)
-    show(ret, output)
+    return pki.delete_org_cert(org_id)
```

### Comparing `hcs-cli-0.1.22/vhcs/cli/cmds/pki/sign-resource-cert.py` & `hcs-cli-0.1.23/vhcs/cli/cmds/pki/sign-resource-cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.23/vhcs/cli/cmds/profile/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,9 +106,8 @@
             if csp_client_key:
                 doc.csp.clientId = csp_client_id
                 doc.csp.clientKey = csp_client_key
                 break
         break
 
     profile.create(name, doc)
-    click.echo(json.dumps(profile.current(), indent=4))
-    click.echo("Profile created: " + name)
+    return profile.current()
```

### Comparing `hcs-cli-0.1.22/vhcs/cli/cmds/vmhub/redeem-otp.py` & `hcs-cli-0.1.23/vhcs/cli/cmds/vmhub/redeem-otp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import click
-from vhcs.common.ctxp import option_output, show
 from vhcs.service import vmhub
 from vhcs.util import pki_util
 
 
 @click.command()
 @click.option(
     "--region",
     type=str,
     default=None,
     required=False,
     help="Specify region name",
 )
 @click.argument("resource-name", type=str, required=True)
 @click.argument("otp", type=str, required=True)
-@option_output
-def redeem_otp(region: str, resource_name: str, otp: str, output: str):
+def redeem_otp(region: str, resource_name: str, otp: str):
     """Redeem OTP with CSR, receive resource cert."""
 
     vmhub.use_region(region)
     csr_pem, private_key_pem = pki_util.generate_CSR(resource_name)
 
     ret = vmhub.redeem_otp(resource_name, otp, csr_pem)
     ret.private_key = private_key_pem
-    show(ret, output)
+    return ret
```

### Comparing `hcs-cli-0.1.22/vhcs/cli/cmds/vmhub/request-otp.py` & `hcs-cli-0.1.23/vhcs/cli/cmds/vmhub/request-otp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import click
-from vhcs.common.ctxp import show
 from vhcs.common.sglib.util import option_org_id, get_org_id
 from vhcs.service import vmhub
 
 
 @click.command()
 @option_org_id
 @click.option(
@@ -14,9 +13,8 @@
     help="Specify region name",
 )
 @click.argument("resource-name", type=str, required=True)
 def request_otp(org: str, region: str, resource_name: str):
     """Request an one-time password for a specific resource"""
     org_id = get_org_id(org)
     vmhub.use_region(region)
-    ret = vmhub.request_otp(org_id, resource_name)
-    show(ret)
+    return vmhub.request_otp(org_id, resource_name)
```

### Comparing `hcs-cli-0.1.22/vhcs/cli/main.py` & `hcs-cli-0.1.23/vhcs/cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,30 +23,38 @@
 logging.getLogger("context").setLevel(logging.WARN)
 logging.getLogger("init").setLevel(logging.WARN)
 logging.getLogger("profile").setLevel(logging.WARN)
 # -----------------------------------------------------------
 
 
 @click.group()
-@click.option("--verbose/--no-verbose", "-v", default=False)
+@click.option("--verbose", "-v", count=True, default=False, help="Print details")
+@click.option(
+    "--output",
+    "-o",
+    type=click.Choice(["json", "json-compact", "yaml", "text"]),
+    default="json",
+    help="Specify output format",
+)
 @click.option("--profile", "-p", type=str, required=False, help="Specify the profile to use. Optional.")
 @click.option("--upgrade-check/--no-upgrade-check", default=True, help="Check new version of HCS CLI.")
 @click.option("--telemetry/--no-telemetry", default=True, help="Send telemetry")
-def cli(verbose: bool, profile: str, upgrade_check: bool, telemetry: bool):
+def cli(verbose: bool, output: str, profile: str, upgrade_check: bool, telemetry: bool):
     if upgrade_check:
         from vhcs.util.versions import check_upgrade
 
         check_upgrade()
     if profile:
-        os.environ["HCS_PROFILE"] = profile
+        ctxp.profile._active_profile_name = profile
 
 
-@cli.result_callback()
-def _process_result(result, **kwargs):
-    pass
+# @cli.result_callback()
+# def _process_result(result, **kwargs):
+#     print("_process_result", result, kwargs)
+#     pass
 
 
 def main():
     try:
         commands_dir = path.join(_module_dir, "cli/cmds")
         config_path = path.join(_module_dir, "config")
         ctxp.init(cli_name="hcs", main_cli=cli, commands_dir=commands_dir, config_path=config_path)
```

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.23/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.23/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.23/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.23/vhcs/common/ctxp/cli_processor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 import click
+import sys
 import yaml
 from click.core import Group
 import os.path as path
+import os
 import importlib
 import importlib.util
 from pathlib import Path
+from . import util
+
+_eager_loading = os.environ.get("_CTXP_EAGER_LOAD")
+if _eager_loading:
+    print("_CTXP_EAGER_LOAD:", _eager_loading, file=sys.stderr)
 
 
 class LazyGroup(click.Group):
     def __init__(self, mod_path: Path, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.mod_path = mod_path
+        if _eager_loading:
+            self._lazy_ensure_subcommands()
 
     def list_commands(self, ctx):
         self._lazy_ensure_subcommands()
         return super().list_commands(ctx)
 
     def get_command(self, ctx, cmd_name):
         self._lazy_ensure_subcommands()
@@ -92,11 +101,27 @@
 
     for foo in cli_methods:
         t = type(foo)
         if t is click.core.Command:
             parent.add_command(foo)
 
 
+def _process_result(result, **kwargs):
+    if result is not None:
+        if isinstance(result, tuple):
+            data, return_code = result
+            if data is not None:
+                util.print_output(data, kwargs.get("output"))
+            if isinstance(return_code, int):
+                ctx = click.get_current_context()
+                ctx.exit(return_code)
+            else:
+                raise Exception("Invalid command return code. Expect int, actual=" + str(type(return_code)))
+        else:
+            util.print_output(result, kwargs.get("output"))
+
+
 def init(main_cli: click.Group, commands_dir: str):
     _add_built_in_commands(main_cli)
     _add_subcommands(commands_dir, main_cli)
-    main_cli(obj={})
+    main_cli.result_callback()(_process_result)
+    return main_cli(obj={})
```

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.23/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.23/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.23/vhcs/common/ctxp/init.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     config_path="./config",
 ):
     real_store_path = path.join(store_path, "." + cli_name)
     profile_path = path.join(real_store_path, "profile")
     profile.init(profile_path)
     config._init(config_path)
 
-    cli_processor.init(main_cli, commands_dir)
+    return cli_processor.init(main_cli, commands_dir)
```

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.23/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.23/vhcs/common/ctxp/profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 _active_profile_store_item = ".active"
 
 
 def init(repo_path: str, active_profile_name: str = None) -> None:
     global _store, _active_profile_name
     _store = fstore(repo_path)
-    _active_profile_name = active_profile_name
+    if active_profile_name:
+        _active_profile_name = active_profile_name
 
 
 def path() -> str:
     """Get directory name of the current active profile"""
     active_profile = name()
     if not active_profile:
         return None
@@ -39,17 +40,14 @@
     global _plain
     _plain = None
     return data
 
 
 def name() -> str:
     """Get the current active profile name"""
-    profile_override = os.environ.get("HCS_PROFILE")
-    if profile_override:
-        return profile_override
 
     global _active_profile_name
     if not _active_profile_name:
         # Try load from "default"
         _active_profile_name = _store.get(key=_active_profile_store_item, format="text")
         if not _active_profile_name:
             # If only one profile, use it
```

### Comparing `hcs-cli-0.1.22/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.23/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/logger.py` & `hcs-cli-0.1.23/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.23/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.23/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.23/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.23/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/service/lcm.py` & `hcs-cli-0.1.23/vhcs/service/lcm.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,9 +76,9 @@
         return _client().get("/providers")
 
     @staticmethod
     def delete():
         return _client().delete(f"/providers/{id}")
 
 
-def test(fn_output: callable):
-    fn_output("test")
+def test():
+    print("test")
```

### Comparing `hcs-cli-0.1.22/vhcs/service/vmhub.py` & `hcs-cli-0.1.23/vhcs/service/vmhub.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,9 +48,9 @@
 def redeem_otp(resource_name: str, otp: str, csr: str):
     base64_encoded_csr = base64.b64encode(csr.encode("ascii")).decode("ascii")
 
     credentials_request = {"vmId": resource_name, "otp": otp, "clientCsr": base64_encoded_csr}
     return _vmhub_client().post("/credentials", credentials_request)
 
 
-def test(fn_output: callable):
-    fn_output("TODO")
+def test():
+    print("TODO")
```

### Comparing `hcs-cli-0.1.22/vhcs/util/pki_util.py` & `hcs-cli-0.1.23/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.22/vhcs/util/versions.py` & `hcs-cli-0.1.23/vhcs/util/versions.py`

 * *Files identical despite different names*

