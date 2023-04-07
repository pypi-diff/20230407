# Comparing `tmp/mythic_container-0.2.0rc8.tar.gz` & `tmp/mythic_container-0.2.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic_container-0.2.0rc8.tar", last modified: Thu Mar 23 14:07:24 2023, max compression
+gzip compressed data, was "mythic_container-0.2.0rc9.tar", last modified: Sat Mar 25 00:42:19 2023, max compression
```

## Comparing `mythic_container-0.2.0rc8.tar` & `mythic_container-0.2.0rc9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-23 14:07:24.283469 mythic_container-0.2.0rc8/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.0rc8/LICENSE.md
--rw-r--r--   0 itsafeature   (501) staff       (20)     1517 2023-03-23 14:07:24.283239 mythic_container-0.2.0rc8/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1069 2023-02-27 20:26:00.000000 mythic_container-0.2.0rc8/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-23 14:07:24.237460 mythic_container-0.2.0rc8/mythic_container/
--rw-r--r--   0 itsafeature   (501) staff       (20)    16293 2023-02-21 17:50:11.000000 mythic_container-0.2.0rc8/mythic_container/C2ProfileBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3070 2023-02-23 00:16:47.000000 mythic_container-0.2.0rc8/mythic_container/LoggingBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    49127 2023-03-21 20:11:05.000000 mythic_container-0.2.0rc8/mythic_container/MythicCommandBase.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-23 14:07:24.280333 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2481 2023-02-17 22:40:44.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7424 2023-03-23 13:36:37.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2272 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3182 2023-03-13 17:15:03.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_command_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4442 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     5343 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1327 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1394 2023-03-19 15:05:35.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.0rc8/mythic_container/MythicRPC.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    13243 2023-03-06 23:50:17.000000 mythic_container-0.2.0rc8/mythic_container/PayloadBuilder.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     6104 2023-02-28 00:19:56.000000 mythic_container-0.2.0rc8/mythic_container/TranslationBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7240 2023-02-22 22:10:41.000000 mythic_container-0.2.0rc8/mythic_container/WebhookBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2507 2023-03-23 14:06:53.000000 mythic_container-0.2.0rc8/mythic_container/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    35588 2023-03-21 20:03:40.000000 mythic_container-0.2.0rc8/mythic_container/agent_utils.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    27628 2023-02-28 22:44:25.000000 mythic_container-0.2.0rc8/mythic_container/c2_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.0rc8/mythic_container/config.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-23 14:07:24.282449 mythic_container-0.2.0rc8/mythic_container/grpc/
--rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.0rc8/mythic_container/grpc/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.0rc8/mythic_container/grpc/translationContainerGRPC_pb2.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.0rc8/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.0rc8/mythic_container/logging.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)    24443 2023-03-13 14:01:12.000000 mythic_container-0.2.0rc8/mythic_container/mythic_service.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    14031 2023-03-03 14:56:12.000000 mythic_container-0.2.0rc8/mythic_container/rabbitmq.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.0rc8/mythic_container/utils_mythic_file_transfer.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1732 2023-02-22 03:09:36.000000 mythic_container-0.2.0rc8/mythic_container/webhook_utils.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-23 14:07:24.239382 mythic_container-0.2.0rc8/mythic_container.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1517 2023-03-23 14:07:24.000000 mythic_container-0.2.0rc8/mythic_container.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)     4340 2023-03-23 14:07:24.000000 mythic_container-0.2.0rc8/mythic_container.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-03-23 14:07:24.000000 mythic_container-0.2.0rc8/mythic_container.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-03-23 14:07:24.000000 mythic_container-0.2.0rc8/mythic_container.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-03-23 14:07:24.000000 mythic_container-0.2.0rc8/mythic_container.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-03-23 14:07:24.283689 mythic_container-0.2.0rc8/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1092 2023-03-23 14:06:46.000000 mythic_container-0.2.0rc8/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.749052 mythic_container-0.2.0rc9/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.0rc9/LICENSE.md
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1517 2023-03-25 00:42:19.748774 mythic_container-0.2.0rc9/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1069 2023-02-27 20:26:00.000000 mythic_container-0.2.0rc9/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.702612 mythic_container-0.2.0rc9/mythic_container/
+-rw-r--r--   0 itsafeature   (501) staff       (20)    16293 2023-02-21 17:50:11.000000 mythic_container-0.2.0rc9/mythic_container/C2ProfileBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3070 2023-02-23 00:16:47.000000 mythic_container-0.2.0rc9/mythic_container/LoggingBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    49127 2023-03-21 20:11:05.000000 mythic_container-0.2.0rc9/mythic_container/MythicCommandBase.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.746133 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2481 2023-02-17 22:40:44.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7424 2023-03-23 13:36:37.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2272 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3182 2023-03-13 17:15:03.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_command_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4442 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     5343 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1327 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.0rc9/mythic_container/MythicRPC.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    13243 2023-03-06 23:50:17.000000 mythic_container-0.2.0rc9/mythic_container/PayloadBuilder.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     6104 2023-02-28 00:19:56.000000 mythic_container-0.2.0rc9/mythic_container/TranslationBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7240 2023-02-22 22:10:41.000000 mythic_container-0.2.0rc9/mythic_container/WebhookBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2507 2023-03-25 00:42:02.000000 mythic_container-0.2.0rc9/mythic_container/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    35588 2023-03-21 20:03:40.000000 mythic_container-0.2.0rc9/mythic_container/agent_utils.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    27628 2023-02-28 22:44:25.000000 mythic_container-0.2.0rc9/mythic_container/c2_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.0rc9/mythic_container/config.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.748018 mythic_container-0.2.0rc9/mythic_container/grpc/
+-rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.0rc9/mythic_container/grpc/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.0rc9/mythic_container/grpc/translationContainerGRPC_pb2.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.0rc9/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.0rc9/mythic_container/logging.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)    24443 2023-03-13 14:01:12.000000 mythic_container-0.2.0rc9/mythic_container/mythic_service.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    14031 2023-03-03 14:56:12.000000 mythic_container-0.2.0rc9/mythic_container/rabbitmq.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.0rc9/mythic_container/utils_mythic_file_transfer.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1732 2023-02-22 03:09:36.000000 mythic_container-0.2.0rc9/mythic_container/webhook_utils.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.705034 mythic_container-0.2.0rc9/mythic_container.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1517 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4340 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-03-25 00:42:19.749315 mythic_container-0.2.0rc9/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1092 2023-03-25 00:41:58.000000 mythic_container-0.2.0rc9/setup.py
```

### Comparing `mythic_container-0.2.0rc8/LICENSE.md` & `mythic_container-0.2.0rc9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/PKG-INFO` & `mythic_container-0.2.0rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic_container
-Version: 0.2.0rc8
+Version: 0.2.0rc9
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.0rc8/README.md` & `mythic_container-0.2.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/C2ProfileBase.py` & `mythic_container-0.2.0rc9/mythic_container/C2ProfileBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/LoggingBase.py` & `mythic_container-0.2.0rc9/mythic_container/LoggingBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicCommandBase.py` & `mythic_container-0.2.0rc9/mythic_container/MythicCommandBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/__init__.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/__init__.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_command_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_command_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.Response = Response
         for k, v in kwargs.items():
             logger.info(f"Unknown kwarg {k} - {v}")
 
     def to_json(self):
         return {
             "task_id": self.TaskID,
-            "response": base64.b64encode(self.Response.encode()) if isinstance(self.Response, str) else base64.b64encode(self.Response).decode()
+            "response": base64.b64encode(self.Response.encode()).decode() if isinstance(self.Response, str) else base64.b64encode(self.Response).decode()
         }
 
 
 class MythicRPCResponseCreateMessageResponse:
     def __init__(self,
                  success: bool = False,
                  error: str = "",
```

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py` & `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/MythicRPC.py` & `mythic_container-0.2.0rc9/mythic_container/MythicRPC.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/PayloadBuilder.py` & `mythic_container-0.2.0rc9/mythic_container/PayloadBuilder.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/TranslationBase.py` & `mythic_container-0.2.0rc9/mythic_container/TranslationBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/WebhookBase.py` & `mythic_container-0.2.0rc9/mythic_container/WebhookBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/__init__.py` & `mythic_container-0.2.0rc9/mythic_container/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .rabbitmq import rabbitmqConnectionClass
 from .mythic_service import start_and_run_forever, test_command
 
 containerVersion = "v1.0.0-0.0.7"
 
-PyPi_version = "0.2.0-rc8"
+PyPi_version = "0.2.0-rc9"
 
 RabbitmqConnection = rabbitmqConnectionClass()
 
 MYTHIC_RPC_OTHER_SERVICES_RPC = "mythic_rpc_other_service_rpc"
 PAYLOAD_BUILD_C2_ROUTING_KEY = "payload_c2_build"
 # payload routes
 PT_SYNC_ROUTING_KEY = "pt_sync"
```

### Comparing `mythic_container-0.2.0rc8/mythic_container/agent_utils.py` & `mythic_container-0.2.0rc9/mythic_container/agent_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/c2_utils.py` & `mythic_container-0.2.0rc9/mythic_container/c2_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/grpc/translationContainerGRPC_pb2.py` & `mythic_container-0.2.0rc9/mythic_container/grpc/translationContainerGRPC_pb2.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py` & `mythic_container-0.2.0rc9/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/logging.py` & `mythic_container-0.2.0rc9/mythic_container/logging.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/mythic_service.py` & `mythic_container-0.2.0rc9/mythic_container/mythic_service.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/rabbitmq.py` & `mythic_container-0.2.0rc9/mythic_container/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/utils_mythic_file_transfer.py` & `mythic_container-0.2.0rc9/mythic_container/utils_mythic_file_transfer.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container/webhook_utils.py` & `mythic_container-0.2.0rc9/mythic_container/webhook_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/mythic_container.egg-info/PKG-INFO` & `mythic_container-0.2.0rc9/mythic_container.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic-container
-Version: 0.2.0rc8
+Version: 0.2.0rc9
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.0rc8/mythic_container.egg-info/SOURCES.txt` & `mythic_container-0.2.0rc9/mythic_container.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc8/setup.py` & `mythic_container-0.2.0rc9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic_container",
-    version="0.2.0-rc8",
+    version="0.2.0-rc9",
     description="Functionality for Mythic Services",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/customizing/payload-type-development",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

