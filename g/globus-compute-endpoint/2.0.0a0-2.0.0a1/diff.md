# Comparing `tmp/globus-compute-endpoint-2.0.0a0.tar.gz` & `tmp/globus-compute-endpoint-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.0.0a0.tar", last modified: Wed Mar 29 22:31:50 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.0.0a1.tar", last modified: Mon Apr  3 22:15:27 2023, max compression
```

## Comparing `globus-compute-endpoint-2.0.0a0.tar` & `globus-compute-endpoint-2.0.0a1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.792512 globus-compute-endpoint-2.0.0a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)      734 2023-03-29 22:31:50.792571 globus-compute-endpoint-2.0.0a0/PKG-INFO
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.786499 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    13715 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.788465 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2895 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/config.py
--rw-r--r--   0 lei        (501) staff       (20)      707 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)    24813 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    19658 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    21117 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.789083 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.789342 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     4374 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/utils/config.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.789469 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.790959 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2104 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    34995 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    48886 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8427 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    18606 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8219 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.791091 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.791436 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12874 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.792056 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6989 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5106 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      393 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.787302 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)      734 2023-03-29 22:31:50.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     2637 2023-03-29 22:31:50.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-03-29 22:31:50.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-03-29 22:31:50.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-03-29 22:31:50.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-03-29 22:31:50.000000 globus-compute-endpoint-2.0.0a0/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-03-29 22:31:50.792848 globus-compute-endpoint-2.0.0a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3181 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-29 22:31:50.792408 globus-compute-endpoint-2.0.0a0/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1937 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2276 2023-03-29 20:22:52.000000 globus-compute-endpoint-2.0.0a0/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.226771 globus-compute-endpoint-2.0.0a1/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)      734 2023-04-03 22:15:27.226829 globus-compute-endpoint-2.0.0a1/PKG-INFO
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.221092 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    19121 2023-04-03 22:11:17.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.222938 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      707 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)    24947 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    21117 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.223536 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.223773 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     4374 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/config.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.223900 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.225294 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    34995 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8427 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.225410 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.225759 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.226333 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6989 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-03 22:13:08.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.221797 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)      734 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     2637 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-03 22:15:27.227104 globus-compute-endpoint-2.0.0a1/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3181 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.226656 globus-compute-endpoint-2.0.0a1/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1937 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.0.0a0/LICENSE` & `globus-compute-endpoint-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/PKG-INFO` & `globus-compute-endpoint-2.0.0a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.0a0
+Version: 2.0.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 from __future__ import annotations
 
 import importlib.util
 import json
 import logging
+import os.path
 import pathlib
+import shutil
 import sys
+import uuid
 
 import click
 from click import ClickException
 from globus_compute_sdk.sdk.login_manager import LoginManager
 from globus_compute_sdk.sdk.login_manager.whoami import print_whoami_info
 
 from .endpoint.endpoint import Endpoint
 from .endpoint.endpoint_manager import EndpointManager
 from .endpoint.utils.config import Config
 from .logging_config import setup_logging
+from .version import DEPRECATION_FUNCX_ENDPOINT
 
 log = logging.getLogger(__name__)
 
 
 class CommandState:
     def __init__(self):
         self.endpoint_config_dir: str = str(pathlib.Path.home() / ".funcx")
         self.debug = False
         self.no_color = False
         self.log_to_console = False
+        self.endpoint_uuid = None
+        self.die_with_parent = False
 
     @classmethod
     def ensure(cls) -> CommandState:
         return click.get_current_context().ensure_object(CommandState)
 
 
 def init_endpoint_configuration_dir(conf_dir: pathlib.Path):
@@ -66,20 +72,25 @@
 
     state = CommandState.ensure()
     endpoint = Endpoint(debug=state.debug)
 
     return endpoint
 
 
+def set_param_to_config(ctx, param, value):
+    state = CommandState.ensure()
+    setattr(state, param.name, value)
+    return state
+
+
 def log_flag_callback(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
 
-    state = CommandState.ensure()
-    setattr(state, param.name, value)
+    state = set_param_to_config(ctx, param, value)
     setup_logging(debug=state.debug, no_color=state.no_color)
 
 
 def common_options(f):
     f = click.option(
         "--debug",
         is_flag=True,
@@ -98,31 +109,33 @@
     )(f)
     f = click.option(
         "--no-color",
         is_flag=True,
         expose_value=False,
         is_eager=True,
         callback=log_flag_callback,
-        help="Colorize the (console) log lines",
+        help="Do not colorize the (console) log lines",
     )(f)
 
     f = click.help_option("-h", "--help")(f)
     return f
 
 
 def start_options(f):
     f = click.option(
         "--endpoint-uuid",
         default=None,
+        callback=set_param_to_config,
         help="The UUID to register with the Globus Compute services",
     )(f)
     f = click.option(
         "--die-with-parent",
         is_flag=True,
         hidden=True,
+        callback=set_param_to_config,
         help="Shutdown if parent process goes away",
     )(f)
     return f
 
 
 def name_arg(f):
     return click.argument("name", required=False, default="default")(f)
@@ -177,24 +190,24 @@
     multi_tenant: bool,
 ):
     """Configure an endpoint
 
     Drops a config.py template into the funcx configs directory.
     The template usually goes to ~/.funcx/<ENDPOINT_NAME>/config.py
     """
-    funcx_dir = get_config_dir()
-    ep_dir = funcx_dir / name
+    compute_dir = get_config_dir()
+    ep_dir = compute_dir / name
     Endpoint.configure_endpoint(ep_dir, endpoint_config, multi_tenant)
 
 
 @app.command(name="start", help="Start an endpoint by name")
 @name_arg
 @start_options
 @common_options
-def start_endpoint(*, name: str, endpoint_uuid: str | None, die_with_parent=False):
+def start_endpoint(*, name: str, **_kwargs):
     """Start an endpoint
 
     This function will do:
     1. Connect to the broker service, and register itself
     2. Get connection info from broker service
     3. Start the interchange as a daemon
 
@@ -206,18 +219,19 @@
           1     4                 6
           |     v                 |
     +-----+-----+-----+           v
     |      Start      |---5---> EndpointInterchange
     |     Endpoint    |         daemon
     +-----------------+
     """
+    state = CommandState.ensure()
     _do_start_endpoint(
         name=name,
-        endpoint_uuid=endpoint_uuid,
-        die_with_parent=die_with_parent,
+        endpoint_uuid=state.endpoint_uuid,
+        die_with_parent=state.die_with_parent,
     )
 
 
 @app.command(name="logout", help="Logout from all endpoints")
 @click.option(
     "--force",
     is_flag=True,
@@ -255,16 +269,16 @@
     """
     Logout from all endpoints and remove cached authentication credentials
 
     Returns True, None if logout was successful and tokens were found and revoked
     Returns False, error_msg if token revocation was not done
     """
     if running_endpoints is None:
-        funcx_dir = get_config_dir()
-        running_endpoints = Endpoint.get_running_endpoints(funcx_dir)
+        compute_dir = get_config_dir()
+        running_endpoints = Endpoint.get_running_endpoints(compute_dir)
     tokens_revoked = False
     error_msg = None
     if running_endpoints and not force:
         running_list = ", ".join(running_endpoints.keys())
         log.info(
             "The following endpoints are currently running: "
             + running_list
@@ -277,15 +291,99 @@
             log.info("Logout succeeded and all cached credentials were revoked")
         else:
             error_msg = "No cached tokens were found, already logged out?"
             log.info(error_msg)
     return tokens_revoked, error_msg
 
 
-def read_config(endpoint_dir: pathlib.Path) -> Config:
+FUNCX_COMPUTE_IMPORT_UPDATES = {
+    "from funcx_endpoint.endpoint.utils.config": "from globus_compute_endpoint.endpoint.utils.config",  # noqa E501
+    "from funcx_endpoint.executors": "from globus_compute_endpoint.executors",  # noqa E501
+}
+
+
+def _upgrade_funcx_imports_in_config(name: str, force=False) -> str:
+    """
+    This only modifies unindented import lines, as are in the original
+    config.py.  Indented matching lines are user created and would have to be
+    updated manually by the user.
+
+    The force flag will overwrite an existing (non-directory) config.py.bak
+
+    This method uses a randomly generated intermediate output file in case
+    there are any permission or unforeseen file system issues
+    """
+    ep_dir = get_config_dir() / name
+    old_config = ep_dir / "config.py"
+    config_backup = ep_dir / "config.py.bak"
+
+    try:
+        # Scan config.py first in case it's a no-op
+        with open(old_config) as f:
+            lines = f.readlines()
+        reformatted_count = 0
+        output_lines = []
+        if lines:
+            for line in lines:
+                modified_line = False
+                for k, v in FUNCX_COMPUTE_IMPORT_UPDATES.items():
+                    if line.startswith(k):
+                        modified_line = True
+                        output_lines.append(line.replace(k, v, 1))
+                        break
+                if not modified_line:
+                    output_lines.append(line)
+                else:
+                    reformatted_count += 1
+        format_msg = f"No funcX import statements found in config.py for {name}"
+        if reformatted_count == 0:
+            return format_msg
+
+        remove_backup = False
+        if os.path.exists(config_backup):
+            if not force:
+                msg = (
+                    f"{config_backup} already exists.\n"
+                    "Rename it or use the --force flag to update config."
+                )
+                raise ClickException(msg)
+            if os.path.isdir(config_backup):
+                msg = (
+                    f"{config_backup} is a directory.\n"
+                    "Rename it before proceeding with config update."
+                )
+                raise ClickException(msg)
+            remove_backup = True
+
+        # Write to temporary file in case of unexpected file errors
+        tmp_output_path = ep_dir / ("config.py." + uuid.uuid4().hex)
+        with open(tmp_output_path.name, "w") as f:
+            for line in output_lines:
+                f.write(line)
+        if remove_backup:
+            os.remove(config_backup)
+        shutil.move(old_config, config_backup)  # Preserve file timestamp
+        os.rename(tmp_output_path.name, old_config)
+        format_msg = (
+            f"{reformatted_count} lines were modified for endpoint {name}\n"
+            f"  The previous config has been renamed to {config_backup}"
+        )
+        return format_msg
+
+    except FileNotFoundError as err:
+        msg = f"No config.py was found for endpoint ({name}) in {ep_dir}"
+        raise ClickException(msg) from err
+    except ClickException:
+        raise
+    except Exception as err:
+        msg = f"Unknown Exception {err} attempting to reformat config.py in {ep_dir}"
+        raise ClickException(msg) from err
+
+
+def read_config(endpoint_dir: pathlib.Path, warn_funcx_imports: bool = True) -> Config:
     endpoint_name = endpoint_dir.name
 
     try:
         conf_path = endpoint_dir / "config.py"
         spec = importlib.util.spec_from_file_location("config", conf_path)
         if not (spec and spec.loader):
             raise Exception(f"Unable to import configuration (no spec): {conf_path}")
@@ -320,14 +418,36 @@
         msg = (
             f"{err}"
             "\n\nFailed to find expected data structure in configuration file."
             "\nHas the configuration file been corrupted or modified incorrectly?\n"
         )
         raise ClickException(msg) from err
 
+    except ModuleNotFoundError as err:
+        # Catch specific error when old config.py references funcx_endpoint
+        if warn_funcx_imports and "No module named 'funcx_endpoint." in err.msg:
+            msg = (
+                f"{conf_path} contains import statements from a previously "
+                "configured endpoint that uses the (deprecated) "
+                "funcx-endpoint library. Please update the imports to reference "
+                "globus_compute_endpoint.\n\ni.e.\n"
+                "    from funcx_endpoint.endpoint.utils.config -> "
+                "from globus_compute_endpoint.endpoint.utils.config\n"
+                "    from funcx_endpoint.executors -> "
+                "from globus_compute_endpoint.executors\n"
+                "\n"
+                "You can also use the command "
+                "`globus-compute-endpoint update_funcx_config [endpoint_name]` "
+                "to update them\n"
+            )
+            raise ClickException(msg) from err
+        else:
+            log.exception(err.msg)
+            raise
+
     except Exception:
         log.exception(
             "Globus Compute v0.2.0 made several non-backwards compatible changes to "
             "the config. Your config might be out of date. "
             "Refer to "
             "https://funcx.readthedocs.io/en/latest/endpoints.html#configuring-funcx"
         )
@@ -390,39 +510,57 @@
 )
 @common_options
 def stop_endpoint(*, name: str, remote: bool):
     """Stops an endpoint using the pidfile"""
     _do_stop_endpoint(name=name, remote=remote)
 
 
+@app.command("update_funcx_config")
+@name_arg
+@click.option(
+    "--force",
+    is_flag=True,
+    default=False,
+    help="update config and backup to config.py.bak even if it already exists",
+)
+def update_funcx_endpoint_config(*, name: str, force: bool):
+    """
+    Update imports file from funcx_endpoint.* to globus_compute_endpoint.*
+
+    Either should raise ClickException or returns modification result message
+    """
+    print(_upgrade_funcx_imports_in_config(name=name, force=force))
+
+
 def _do_stop_endpoint(*, name: str, remote: bool = False) -> None:
     ep_dir = get_config_dir() / name
     Endpoint.stop_endpoint(ep_dir, read_config(ep_dir), remote=remote)
 
 
 @app.command("restart")
 @name_arg
 @common_options
 @start_options
-def restart_endpoint(*, name: str, endpoint_uuid: str | None, die_with_parent=False):
+def restart_endpoint(*, name: str, **_kwargs):
     """Restarts an endpoint"""
+    state = CommandState.ensure()
     _do_stop_endpoint(name=name)
     _do_start_endpoint(
         name=name,
-        endpoint_uuid=endpoint_uuid,
-        die_with_parent=die_with_parent,
+        endpoint_uuid=state.endpoint_uuid,
+        die_with_parent=state.die_with_parent,
     )
 
 
 @app.command("list")
 @common_options
 def list_endpoints():
     """List all available endpoints"""
-    funcx_dir = get_config_dir()
-    Endpoint.print_endpoint_table(funcx_dir)
+    compute_dir = get_config_dir()
+    Endpoint.print_endpoint_table(compute_dir)
 
 
 @app.command("delete")
 @name_arg
 @click.option(
     "--force",
     default=False,
@@ -445,9 +583,15 @@
 
 
 def cli_run():
     """Entry point for setuptools to point to"""
     app()
 
 
+def cli_run_funcx():
+    """Entry point that prints a custom message. i.e. deprecation warnings"""
+    print(DEPRECATION_FUNCX_ENDPOINT)
+    app()
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/config.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,16 @@
             print(f"Created multi-tenant profile for <{ep_name}>")
         else:
             print(f"Created profile for <{ep_name}>")
         print(
             f"\n    Configuration file: {config_path}\n"
             "\nUse the `start` subcommand to run it:\n"
             f"\n    $ globus-compute-endpoint start {ep_name}"
+            # If we want to show 'funcx-endpoint start' when using the wrapper
+            # f"\n    $ {sys.argv[0]} start {ep_name}"
         )
 
     @staticmethod
     def get_endpoint_id(endpoint_dir: pathlib.Path) -> str | None:
         info_file_path = endpoint_dir / "endpoint.json"
         try:
             return json.loads(info_file_path.read_bytes())["endpoint_id"]
```

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.0a0
+Version: 2.0.0a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `globus-compute-endpoint-2.0.0a0/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/setup.py` & `globus-compute-endpoint-2.0.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/tests/conftest.py` & `globus-compute-endpoint-2.0.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a0/tests/utils.py` & `globus-compute-endpoint-2.0.0a1/tests/utils.py`

 * *Files identical despite different names*

