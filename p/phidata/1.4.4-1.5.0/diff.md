# Comparing `tmp/phidata-1.4.4.tar.gz` & `tmp/phidata-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-1.4.4.tar", last modified: Wed Mar 15 00:28:56 2023, max compression
+gzip compressed data, was "phidata-1.5.0.tar", last modified: Fri Apr  7 15:53:22 2023, max compression
```

## Comparing `phidata-1.4.4.tar` & `phidata-1.5.0.tar`

### file list

```diff
@@ -1,486 +1,493 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.698399 phidata-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-03-15 00:28:33.000000 phidata-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-15 00:28:56.698399 phidata-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-03-15 00:28:33.000000 phidata-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.642398 phidata-1.4.4/phidata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.642398 phidata-1.4.4/phidata/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.642398 phidata-1.4.4/phidata/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.642398 phidata-1.4.4/phidata/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/alertmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/amundsen/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/amundsen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/amundsen/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/amundsen/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/amundsen/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/assistant/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/cadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/databox/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/databox/databox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/db/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/db/base_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48622 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.646398 phidata-1.4.4/phidata/app/grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/grafana/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.650398 phidata-1.4.4/phidata/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.650398 phidata-1.4.4/phidata/app/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/k8s/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/k8s/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/k8s/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.650398 phidata-1.4.4/phidata/app/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.650398 phidata-1.4.4/phidata/app/nodeexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47922 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28389 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/phidata_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.650398 phidata-1.4.4/phidata/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53160 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.650398 phidata-1.4.4/phidata/app/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.650398 phidata-1.4.4/phidata/app/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.650398 phidata-1.4.4/phidata/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/server/api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/server/app_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    46936 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/server/server_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.654398 phidata-1.4.4/phidata/app/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49371 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/spark/spark_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.654398 phidata-1.4.4/phidata/app/superset/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/superset/superset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/superset/superset_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/superset/superset_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.654398 phidata-1.4.4/phidata/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.654398 phidata-1.4.4/phidata/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.654398 phidata-1.4.4/phidata/asset/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/asset/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/asset/data_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.654398 phidata-1.4.4/phidata/asset/local/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/asset/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/asset/local/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/create/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/create/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/resource/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.658398 phidata-1.4.4/phidata/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.662398 phidata-1.4.4/phidata/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.662398 phidata-1.4.4/phidata/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.662398 phidata-1.4.4/phidata/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.662398 phidata-1.4.4/phidata/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.662398 phidata-1.4.4/phidata/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.662398 phidata-1.4.4/phidata/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/iam/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.662398 phidata-1.4.4/phidata/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.662398 phidata-1.4.4/phidata/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.666398 phidata-1.4.4/phidata/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.666398 phidata-1.4.4/phidata/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/s3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/s3/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/aws/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.666398 phidata-1.4.4/phidata/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/checks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/checks/not_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.666398 phidata-1.4.4/phidata/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/decorators/validate_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.666398 phidata-1.4.4/phidata/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.670398 phidata-1.4.4/phidata/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/resource/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/resource/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.670398 phidata-1.4.4/phidata/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.670398 phidata-1.4.4/phidata/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/exceptions/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/exceptions/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/exceptions/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.670398 phidata-1.4.4/phidata/infra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/infra/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/infra/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/infra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/infra/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.670398 phidata-1.4.4/phidata/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.670398 phidata-1.4.4/phidata/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.670398 phidata-1.4.4/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.670398 phidata-1.4.4/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.674398 phidata-1.4.4/phidata/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.674398 phidata-1.4.4/phidata/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.674398 phidata-1.4.4/phidata/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.674398 phidata-1.4.4/phidata/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.674398 phidata-1.4.4/phidata/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.674398 phidata-1.4.4/phidata/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.674398 phidata-1.4.4/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.674398 phidata-1.4.4/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.674398 phidata-1.4.4/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.678398 phidata-1.4.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.678398 phidata-1.4.4/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.678398 phidata-1.4.4/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.678398 phidata-1.4.4/phidata/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.678398 phidata-1.4.4/phidata/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.678398 phidata-1.4.4/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.678398 phidata-1.4.4/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.682398 phidata-1.4.4/phidata/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.682398 phidata-1.4.4/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.682398 phidata-1.4.4/phidata/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.682398 phidata-1.4.4/phidata/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.682398 phidata-1.4.4/phidata/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/k8s/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/utils/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/k8s/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/product/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/product/data_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/table/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/local/local_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/local/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.686399 phidata-1.4.4/phidata/table/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/s3/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/s3/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/table/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/sql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/task/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/task/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/task/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/task/aws/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/task/aws/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/task/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/task/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/task/download/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/download/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.690399 phidata-1.4.4/phidata/task/download/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/download/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/download/url/to_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/download/url/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.694399 phidata-1.4.4/phidata/task/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.694399 phidata-1.4.4/phidata/task/plot/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/plot/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/python_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.694399 phidata-1.4.4/phidata/task/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.694399 phidata-1.4.4/phidata/task/run/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/run/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/run/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/task_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.694399 phidata-1.4.4/phidata/task/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.694399 phidata-1.4.4/phidata/task/upload/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/upload/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.694399 phidata-1.4.4/phidata/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/types/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/types/phidata_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.698399 phidata-1.4.4/phidata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/prep_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/utils/workspace_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.698399 phidata-1.4.4/phidata/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/workflow/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.698399 phidata-1.4.4/phidata/workflow/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/workflow/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.698399 phidata-1.4.4/phidata/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-03-15 00:28:33.000000 phidata-1.4.4/phidata/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.642398 phidata-1.4.4/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-15 00:28:56.000000 phidata-1.4.4/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-03-15 00:28:56.000000 phidata-1.4.4/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 00:28:56.000000 phidata-1.4.4/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-15 00:28:56.000000 phidata-1.4.4/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 00:28:56.000000 phidata-1.4.4/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-15 00:28:33.000000 phidata-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 00:28:56.698399 phidata-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-15 00:28:33.000000 phidata-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 00:28:56.698399 phidata-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-15 00:28:33.000000 phidata-1.4.4/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.753758 phidata-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-07 15:53:03.000000 phidata-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-07 15:53:22.753758 phidata-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-07 15:53:03.000000 phidata-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.677757 phidata-1.5.0/phidata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.681757 phidata-1.5.0/phidata/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.681757 phidata-1.5.0/phidata/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.681757 phidata-1.5.0/phidata/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.681757 phidata-1.5.0/phidata/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.681757 phidata-1.5.0/phidata/app/alertmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/amundsen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/amundsen/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/assistant/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/cadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/databox/databox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/db/base_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48622 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/grafana/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/k8s/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/k8s/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/k8s/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.685757 phidata-1.5.0/phidata/app/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.689757 phidata-1.5.0/phidata/app/nodeexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47922 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/phidata_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.689757 phidata-1.5.0/phidata/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53160 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.689757 phidata-1.5.0/phidata/app/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.689757 phidata-1.5.0/phidata/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.689757 phidata-1.5.0/phidata/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/server/api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/server/app_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18334 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/server/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58047 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/server/server_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/server/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.693757 phidata-1.5.0/phidata/app/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49371 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/spark/spark_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.693757 phidata-1.5.0/phidata/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/superset/superset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/superset/superset_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.693757 phidata-1.5.0/phidata/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.693757 phidata-1.5.0/phidata/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.693757 phidata-1.5.0/phidata/asset/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/asset/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/asset/data_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.697757 phidata-1.5.0/phidata/asset/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/asset/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/asset/local/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.697757 phidata-1.5.0/phidata/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.697757 phidata-1.5.0/phidata/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.697757 phidata-1.5.0/phidata/aws/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.697757 phidata-1.5.0/phidata/aws/create/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/create/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.697757 phidata-1.5.0/phidata/aws/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.701757 phidata-1.5.0/phidata/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.701757 phidata-1.5.0/phidata/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.701757 phidata-1.5.0/phidata/aws/resource/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.701757 phidata-1.5.0/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.701757 phidata-1.5.0/phidata/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.701757 phidata-1.5.0/phidata/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.705757 phidata-1.5.0/phidata/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.705757 phidata-1.5.0/phidata/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.705757 phidata-1.5.0/phidata/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.705757 phidata-1.5.0/phidata/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.705757 phidata-1.5.0/phidata/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.705757 phidata-1.5.0/phidata/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.709757 phidata-1.5.0/phidata/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.709757 phidata-1.5.0/phidata/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.709757 phidata-1.5.0/phidata/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.709757 phidata-1.5.0/phidata/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/s3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/s3/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/aws/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.709757 phidata-1.5.0/phidata/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/checks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/checks/not_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.713757 phidata-1.5.0/phidata/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/decorators/validate_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.713757 phidata-1.5.0/phidata/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.713757 phidata-1.5.0/phidata/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/resource/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/resource/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.713757 phidata-1.5.0/phidata/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.717758 phidata-1.5.0/phidata/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/exceptions/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/exceptions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/exceptions/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.717758 phidata-1.5.0/phidata/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/infra/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/infra/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/infra/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/infra/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.717758 phidata-1.5.0/phidata/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.721758 phidata-1.5.0/phidata/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.721758 phidata-1.5.0/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.721758 phidata-1.5.0/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.721758 phidata-1.5.0/phidata/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.721758 phidata-1.5.0/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.721758 phidata-1.5.0/phidata/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.721758 phidata-1.5.0/phidata/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.725758 phidata-1.5.0/phidata/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.725758 phidata-1.5.0/phidata/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.725758 phidata-1.5.0/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.725758 phidata-1.5.0/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.725758 phidata-1.5.0/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.725758 phidata-1.5.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.725758 phidata-1.5.0/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.725758 phidata-1.5.0/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.729758 phidata-1.5.0/phidata/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.729758 phidata-1.5.0/phidata/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.729758 phidata-1.5.0/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.729758 phidata-1.5.0/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.729758 phidata-1.5.0/phidata/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.733758 phidata-1.5.0/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.733758 phidata-1.5.0/phidata/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.737758 phidata-1.5.0/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.737758 phidata-1.5.0/phidata/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.737758 phidata-1.5.0/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.737758 phidata-1.5.0/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.737758 phidata-1.5.0/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.737758 phidata-1.5.0/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.737758 phidata-1.5.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.737758 phidata-1.5.0/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.737758 phidata-1.5.0/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.741758 phidata-1.5.0/phidata/k8s/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/utils/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/k8s/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.741758 phidata-1.5.0/phidata/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/product/data_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.741758 phidata-1.5.0/phidata/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.741758 phidata-1.5.0/phidata/table/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/local/local_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/local/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.741758 phidata-1.5.0/phidata/table/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/s3/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/s3/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.741758 phidata-1.5.0/phidata/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/sql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/aws/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/aws/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/download/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/download/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/download/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/download/url/to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.745758 phidata-1.5.0/phidata/task/plot/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/plot/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/python_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.749758 phidata-1.5.0/phidata/task/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.749758 phidata-1.5.0/phidata/task/run/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/run/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/task_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.749758 phidata-1.5.0/phidata/task/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.749758 phidata-1.5.0/phidata/task/upload/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.749758 phidata-1.5.0/phidata/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/types/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/types/phidata_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.749758 phidata-1.5.0/phidata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/prep_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/utils/workspace_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.749758 phidata-1.5.0/phidata/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/workflow/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.749758 phidata-1.5.0/phidata/workflow/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.753758 phidata-1.5.0/phidata/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-07 15:53:03.000000 phidata-1.5.0/phidata/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.681757 phidata-1.5.0/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-07 15:53:22.000000 phidata-1.5.0/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-04-07 15:53:22.000000 phidata-1.5.0/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:53:22.000000 phidata-1.5.0/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 15:53:22.000000 phidata-1.5.0/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 15:53:22.000000 phidata-1.5.0/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-07 15:53:03.000000 phidata-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 15:53:22.753758 phidata-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-07 15:53:03.000000 phidata-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:53:22.753758 phidata-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-07 15:53:03.000000 phidata-1.5.0/tests/test_placeholder.py
```

### Comparing `phidata-1.4.4/LICENSE` & `phidata-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/PKG-INFO` & `phidata-1.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: phidata
-Version: 1.4.4
-Summary: Building blocks for Data Engineering
-Author-email: Ashpreet Bedi <ashpreet@phidata.com>
-Project-URL: homepage, https://www.phidata.com
-Project-URL: documentation, https://www.docs.phidata.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: aws
-License-File: LICENSE
-
 <h1 align="center">
   phidata
 </h1>
 <p align="center">
     <em>Building Blocks for Data Engineering</em>
 </p>
 
@@ -34,25 +21,26 @@
 <a href="https://github.com/phidatahq/phidata/actions/workflows/test.yml" target="_blank">
     <img src="https://github.com/phidatahq/phidata/actions/workflows/test.yml/badge.svg" alt="test-status">
 </a>
 </p>
 
 ---
 
-### **Phidata is a set of building blocks for data engineering**
+### **A python library of data engineering building blocks**
+
+Python library of OSS data tools, use it deliver high-quality data products on the cheap.
 
-It makes data tools plug-n-play so teams can deliver high-quality, reliable data products
+Honestly our goal is just to save money and run OSS on the cheap. So we run stuff locally using docker and in production on AWS. Because we're running OSS, we're OSS too with a MPL-2.0 license.
 
 ### How it works
 
-- You start with a codebase that has data tools pre-configured
-- Enable the Apps you need - Airflow, Superset, Jupyter, MLFlow
-- Build data products (tables, metrics) in a dev environment running locally on docker
-- Write pipelines in python or SQL. Use GPT-3 to generate boilerplate code
-- Run production on AWS. Infrastructure is also pre-configured
+- Phidata converts infrastructure, tools and data assets into python classes.
+- These classes are then put together to build data platforms, ML Apis, AI Apps, etc.
+- Run your platform locally for development using docker with `phi ws up dev:docker`
+- Run it in production on AWS: `phi ws up prod:aws`
 
 ### Advantages
 
 - Automate the grunt work
 - Recipes for common data tasks
 - Everything is version controlled: Infra, Apps and Workflows
 - Equal `dev` and `production` environments for data development at scale
```

#### html2text {}

```diff
@@ -1,54 +1,49 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.4.4 Summary: Building blocks for
-Data Engineering Author-email: Ashpreet Bedi
-phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
-documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
-File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
       [version] [pythonversion] [downloads] [build-status] [test-status]
---- ### **Phidata is a set of building blocks for data engineering** It makes
-data tools plug-n-play so teams can deliver high-quality, reliable data
-products ### How it works - You start with a codebase that has data tools pre-
-configured - Enable the Apps you need - Airflow, Superset, Jupyter, MLFlow -
-Build data products (tables, metrics) in a dev environment running locally on
-docker - Write pipelines in python or SQL. Use GPT-3 to generate boilerplate
-code - Run production on AWS. Infrastructure is also pre-configured ###
-Advantages - Automate the grunt work - Recipes for common data tasks -
-Everything is version controlled: Infra, Apps and Workflows - Equal `dev` and
-`production` environments for data development at scale - Multiple teams
-working together share code and define dependencies in a pythonic way -
-Formatting (`black`), linting (`ruff`), type-checking (`mypy`) and testing
-(`pytest`) included ### More Information: - **Website**: phidata.com -
-**Documentation**: https://docs.phidata.com - **Chat**: Discord --- ##
-Quickstart Let's build a data product using crypto data. Open the `Terminal`
-and follow along to download sample data and analyze it in a jupyter notebook.
-## Setup Create a python virtual environment ```bash python3 -m venv ~/.venvs/
-dpenv source ~/.venvs/dpenv/bin/activate ``` Install and initialize phidata
-```bash pip install phidata phi init ``` > If you encounter errors, try
-updating pip using `python -m pip install --upgrade pip` ## Create workspace
-**Workspace** is a directory containing the source code for your data platform.
-Run `phi ws init` to create a new workspace. Press Enter to select the default
-name (`data-platform`) and template (`aws-data-platform`) ```bash phi ws init
-``` cd into the new workspace directory ```bash cd data-platform ``` ## Run
-your first workflow The first step of building a data product is collecting the
-data. The `workflows/crypto/prices.py` file contains an example task for
-downloading crypto data locally to a CSV file. Run it using ```bash phi wf run
-crypto/prices ``` Note how we define the output as a `CsvTableLocal` object
-with partitions and pre-write checks ```python # Step 1: Define CsvTableLocal
-for storing data # Path: `storage/tables/crypto_prices` crypto_prices_local =
-CsvTableLocal( name="crypto_prices", database="crypto", partitions=["ds"],
-write_checks=[NotEmpty()], ) ``` Checkout `data-platform/storage/tables/
-crypto_prices` for the CSVs ## Run your first App **Docker** is a great tool
-for testing locally. Your workspace comes pre-configured with a jupyter
-notebook for analyzing data. Install [docker desktop](https://docs.docker.com/
-desktop/install/mac-install/) and after the engine is running, start the
-workspace using ```bash phi ws up ``` Press Enter to confirm. Verify the
-container is running using the docker dashboard or `docker ps` ```bash docker
-ps --format 'table {{.Names}}\t{{.Image}}' NAMES IMAGE jupyter-container
+--- ### **A python library of data engineering building blocks** Python library
+of OSS data tools, use it deliver high-quality data products on the cheap.
+Honestly our goal is just to save money and run OSS on the cheap. So we run
+stuff locally using docker and in production on AWS. Because we're running OSS,
+we're OSS too with a MPL-2.0 license. ### How it works - Phidata converts
+infrastructure, tools and data assets into python classes. - These classes are
+then put together to build data platforms, ML Apis, AI Apps, etc. - Run your
+platform locally for development using docker with `phi ws up dev:docker` - Run
+it in production on AWS: `phi ws up prod:aws` ### Advantages - Automate the
+grunt work - Recipes for common data tasks - Everything is version controlled:
+Infra, Apps and Workflows - Equal `dev` and `production` environments for data
+development at scale - Multiple teams working together share code and define
+dependencies in a pythonic way - Formatting (`black`), linting (`ruff`), type-
+checking (`mypy`) and testing (`pytest`) included ### More Information: -
+**Website**: phidata.com - **Documentation**: https://docs.phidata.com -
+**Chat**: Discord --- ## Quickstart Let's build a data product using crypto
+data. Open the `Terminal` and follow along to download sample data and analyze
+it in a jupyter notebook. ## Setup Create a python virtual environment ```bash
+python3 -m venv ~/.venvs/dpenv source ~/.venvs/dpenv/bin/activate ``` Install
+and initialize phidata ```bash pip install phidata phi init ``` > If you
+encounter errors, try updating pip using `python -m pip install --upgrade pip`
+## Create workspace **Workspace** is a directory containing the source code for
+your data platform. Run `phi ws init` to create a new workspace. Press Enter to
+select the default name (`data-platform`) and template (`aws-data-platform`)
+```bash phi ws init ``` cd into the new workspace directory ```bash cd data-
+platform ``` ## Run your first workflow The first step of building a data
+product is collecting the data. The `workflows/crypto/prices.py` file contains
+an example task for downloading crypto data locally to a CSV file. Run it using
+```bash phi wf run crypto/prices ``` Note how we define the output as a
+`CsvTableLocal` object with partitions and pre-write checks ```python # Step 1:
+Define CsvTableLocal for storing data # Path: `storage/tables/crypto_prices`
+crypto_prices_local = CsvTableLocal( name="crypto_prices", database="crypto",
+partitions=["ds"], write_checks=[NotEmpty()], ) ``` Checkout `data-platform/
+storage/tables/crypto_prices` for the CSVs ## Run your first App **Docker** is
+a great tool for testing locally. Your workspace comes pre-configured with a
+jupyter notebook for analyzing data. Install [docker desktop](https://
+docs.docker.com/desktop/install/mac-install/) and after the engine is running,
+start the workspace using ```bash phi ws up ``` Press Enter to confirm. Verify
+the container is running using the docker dashboard or `docker ps` ```bash
+docker ps --format 'table {{.Names}}\t{{.Image}}' NAMES IMAGE jupyter-container
 phidata/jupyter-aws-dp:dev ``` ## Jupyter UI Open [localhost:8888](http://
 localhost:8888) in a new tab to view the jupyterlab UI. Password: **admin**
 Navigate to `notebooks/examples/crypto_prices.ipynb` and run all cells. ##
 Shutdown Play around and then stop the workspace using ```bash phi ws down ```
 ## Next Checkout the [documentation](https://docs.phidata.com) for more
 information or chat with us on [discord](https://discord.gg/4MtYHHrgA8) ---
```

### Comparing `phidata-1.4.4/README.md` & `phidata-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: phidata
+Version: 1.5.0
+Summary: Building blocks for Data Engineering
+Author-email: Ashpreet Bedi <ashpreet@phidata.com>
+Project-URL: homepage, https://www.phidata.com
+Project-URL: documentation, https://www.docs.phidata.com
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: aws
+License-File: LICENSE
+
 <h1 align="center">
   phidata
 </h1>
 <p align="center">
     <em>Building Blocks for Data Engineering</em>
 </p>
 
@@ -21,25 +34,26 @@
 <a href="https://github.com/phidatahq/phidata/actions/workflows/test.yml" target="_blank">
     <img src="https://github.com/phidatahq/phidata/actions/workflows/test.yml/badge.svg" alt="test-status">
 </a>
 </p>
 
 ---
 
-### **Phidata is a set of building blocks for data engineering**
+### **A python library of data engineering building blocks**
+
+Python library of OSS data tools, use it deliver high-quality data products on the cheap.
 
-It makes data tools plug-n-play so teams can deliver high-quality, reliable data products
+Honestly our goal is just to save money and run OSS on the cheap. So we run stuff locally using docker and in production on AWS. Because we're running OSS, we're OSS too with a MPL-2.0 license.
 
 ### How it works
 
-- You start with a codebase that has data tools pre-configured
-- Enable the Apps you need - Airflow, Superset, Jupyter, MLFlow
-- Build data products (tables, metrics) in a dev environment running locally on docker
-- Write pipelines in python or SQL. Use GPT-3 to generate boilerplate code
-- Run production on AWS. Infrastructure is also pre-configured
+- Phidata converts infrastructure, tools and data assets into python classes.
+- These classes are then put together to build data platforms, ML Apis, AI Apps, etc.
+- Run your platform locally for development using docker with `phi ws up dev:docker`
+- Run it in production on AWS: `phi ws up prod:aws`
 
 ### Advantages
 
 - Automate the grunt work
 - Recipes for common data tasks
 - Everything is version controlled: Infra, Apps and Workflows
 - Equal `dev` and `production` environments for data development at scale
```

#### html2text {}

```diff
@@ -1,48 +1,55 @@
+Metadata-Version: 2.1 Name: phidata Version: 1.5.0 Summary: Building blocks for
+Data Engineering Author-email: Ashpreet Bedi
+phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
+documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
+File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
       [version] [pythonversion] [downloads] [build-status] [test-status]
---- ### **Phidata is a set of building blocks for data engineering** It makes
-data tools plug-n-play so teams can deliver high-quality, reliable data
-products ### How it works - You start with a codebase that has data tools pre-
-configured - Enable the Apps you need - Airflow, Superset, Jupyter, MLFlow -
-Build data products (tables, metrics) in a dev environment running locally on
-docker - Write pipelines in python or SQL. Use GPT-3 to generate boilerplate
-code - Run production on AWS. Infrastructure is also pre-configured ###
-Advantages - Automate the grunt work - Recipes for common data tasks -
-Everything is version controlled: Infra, Apps and Workflows - Equal `dev` and
-`production` environments for data development at scale - Multiple teams
-working together share code and define dependencies in a pythonic way -
-Formatting (`black`), linting (`ruff`), type-checking (`mypy`) and testing
-(`pytest`) included ### More Information: - **Website**: phidata.com -
-**Documentation**: https://docs.phidata.com - **Chat**: Discord --- ##
-Quickstart Let's build a data product using crypto data. Open the `Terminal`
-and follow along to download sample data and analyze it in a jupyter notebook.
-## Setup Create a python virtual environment ```bash python3 -m venv ~/.venvs/
-dpenv source ~/.venvs/dpenv/bin/activate ``` Install and initialize phidata
-```bash pip install phidata phi init ``` > If you encounter errors, try
-updating pip using `python -m pip install --upgrade pip` ## Create workspace
-**Workspace** is a directory containing the source code for your data platform.
-Run `phi ws init` to create a new workspace. Press Enter to select the default
-name (`data-platform`) and template (`aws-data-platform`) ```bash phi ws init
-``` cd into the new workspace directory ```bash cd data-platform ``` ## Run
-your first workflow The first step of building a data product is collecting the
-data. The `workflows/crypto/prices.py` file contains an example task for
-downloading crypto data locally to a CSV file. Run it using ```bash phi wf run
-crypto/prices ``` Note how we define the output as a `CsvTableLocal` object
-with partitions and pre-write checks ```python # Step 1: Define CsvTableLocal
-for storing data # Path: `storage/tables/crypto_prices` crypto_prices_local =
-CsvTableLocal( name="crypto_prices", database="crypto", partitions=["ds"],
-write_checks=[NotEmpty()], ) ``` Checkout `data-platform/storage/tables/
-crypto_prices` for the CSVs ## Run your first App **Docker** is a great tool
-for testing locally. Your workspace comes pre-configured with a jupyter
-notebook for analyzing data. Install [docker desktop](https://docs.docker.com/
-desktop/install/mac-install/) and after the engine is running, start the
-workspace using ```bash phi ws up ``` Press Enter to confirm. Verify the
-container is running using the docker dashboard or `docker ps` ```bash docker
-ps --format 'table {{.Names}}\t{{.Image}}' NAMES IMAGE jupyter-container
+--- ### **A python library of data engineering building blocks** Python library
+of OSS data tools, use it deliver high-quality data products on the cheap.
+Honestly our goal is just to save money and run OSS on the cheap. So we run
+stuff locally using docker and in production on AWS. Because we're running OSS,
+we're OSS too with a MPL-2.0 license. ### How it works - Phidata converts
+infrastructure, tools and data assets into python classes. - These classes are
+then put together to build data platforms, ML Apis, AI Apps, etc. - Run your
+platform locally for development using docker with `phi ws up dev:docker` - Run
+it in production on AWS: `phi ws up prod:aws` ### Advantages - Automate the
+grunt work - Recipes for common data tasks - Everything is version controlled:
+Infra, Apps and Workflows - Equal `dev` and `production` environments for data
+development at scale - Multiple teams working together share code and define
+dependencies in a pythonic way - Formatting (`black`), linting (`ruff`), type-
+checking (`mypy`) and testing (`pytest`) included ### More Information: -
+**Website**: phidata.com - **Documentation**: https://docs.phidata.com -
+**Chat**: Discord --- ## Quickstart Let's build a data product using crypto
+data. Open the `Terminal` and follow along to download sample data and analyze
+it in a jupyter notebook. ## Setup Create a python virtual environment ```bash
+python3 -m venv ~/.venvs/dpenv source ~/.venvs/dpenv/bin/activate ``` Install
+and initialize phidata ```bash pip install phidata phi init ``` > If you
+encounter errors, try updating pip using `python -m pip install --upgrade pip`
+## Create workspace **Workspace** is a directory containing the source code for
+your data platform. Run `phi ws init` to create a new workspace. Press Enter to
+select the default name (`data-platform`) and template (`aws-data-platform`)
+```bash phi ws init ``` cd into the new workspace directory ```bash cd data-
+platform ``` ## Run your first workflow The first step of building a data
+product is collecting the data. The `workflows/crypto/prices.py` file contains
+an example task for downloading crypto data locally to a CSV file. Run it using
+```bash phi wf run crypto/prices ``` Note how we define the output as a
+`CsvTableLocal` object with partitions and pre-write checks ```python # Step 1:
+Define CsvTableLocal for storing data # Path: `storage/tables/crypto_prices`
+crypto_prices_local = CsvTableLocal( name="crypto_prices", database="crypto",
+partitions=["ds"], write_checks=[NotEmpty()], ) ``` Checkout `data-platform/
+storage/tables/crypto_prices` for the CSVs ## Run your first App **Docker** is
+a great tool for testing locally. Your workspace comes pre-configured with a
+jupyter notebook for analyzing data. Install [docker desktop](https://
+docs.docker.com/desktop/install/mac-install/) and after the engine is running,
+start the workspace using ```bash phi ws up ``` Press Enter to confirm. Verify
+the container is running using the docker dashboard or `docker ps` ```bash
+docker ps --format 'table {{.Names}}\t{{.Image}}' NAMES IMAGE jupyter-container
 phidata/jupyter-aws-dp:dev ``` ## Jupyter UI Open [localhost:8888](http://
 localhost:8888) in a new tab to view the jupyterlab UI. Password: **admin**
 Navigate to `notebooks/examples/crypto_prices.ipynb` and run all cells. ##
 Shutdown Play around and then stop the workspace using ```bash phi ws down ```
 ## Next Checkout the [documentation](https://docs.phidata.com) for more
 information or chat with us on [discord](https://discord.gg/4MtYHHrgA8) ---
```

### Comparing `phidata-1.4.4/phidata/airflow/operators/empty.py` & `phidata-1.5.0/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/airflow/airflow_base.py` & `phidata-1.5.0/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/airflow/airflow_flower.py` & `phidata-1.5.0/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/airflow/airflow_manager.py` & `phidata-1.5.0/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/airflow/airflow_scheduler.py` & `phidata-1.5.0/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/airflow/airflow_webserver.py` & `phidata-1.5.0/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/airflow/airflow_worker.py` & `phidata-1.5.0/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/alertmanager/alertmanager.py` & `phidata-1.5.0/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/amundsen/frontend.py` & `phidata-1.5.0/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/amundsen/metadata.py` & `phidata-1.5.0/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/amundsen/search.py` & `phidata-1.5.0/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/assistant/assistant.py` & `phidata-1.5.0/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/cadvisor/cadvisor.py` & `phidata-1.5.0/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/databox/databox.py` & `phidata-1.5.0/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/db/base_db.py` & `phidata-1.5.0/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/elastic/elastic_app.py` & `phidata-1.5.0/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/elasticsearch/elasticsearch.py` & `phidata-1.5.0/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/grafana/grafana.py` & `phidata-1.5.0/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/group.py` & `phidata-1.5.0/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/jupyter/jupyter_hub.py` & `phidata-1.5.0/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/jupyter/jupyter_lab.py` & `phidata-1.5.0/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/k8s/app.py` & `phidata-1.5.0/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/k8s/dir.py` & `phidata-1.5.0/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/k8s/url.py` & `phidata-1.5.0/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/neo4j/neo4j.py` & `phidata-1.5.0/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/nodeexporter/nodeexporter.py` & `phidata-1.5.0/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/phidata_app.py` & `phidata-1.5.0/phidata/app/phidata_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,16 +276,20 @@
     # Type: CreateStorageClass
     extra_storage_classes: Optional[List[Any]] = None
     # Type: CreateCustomObject
     extra_custom_objects: Optional[List[Any]] = None
     # Type: CreateCustomResourceDefinition
     extra_crds: Optional[List[Any]] = None
 
+    # -*- AWS configuration
+    aws_subnets: Optional[List[str]] = None
+    aws_security_groups: Optional[List[str]] = None
+
     # Other args
-    print_env_on_load: bool = True
+    print_env_on_load: bool = False
     # If True, skip resource creation if active resources with the same name exist.
     use_cache: bool = True
 
     # Extra kwargs used to ensure older versions of phidata don't throw syntax errors
     extra_kwargs: Optional[Dict[str, Any]] = None
 
     # -*- AWS parameters
@@ -316,14 +320,18 @@
         # Type: Optional[Dict[str, DockerResourceGroup]]
         self.docker_resource_groups: Optional[Dict[str, Any]] = None
 
         # Dict of KubernetesResourceGroups
         # Type: Optional[Dict[str, K8sResourceGroup]]
         self.k8s_resource_groups: Optional[Dict[str, Any]] = None
 
+        # Dict of AwsResourceGroups
+        # Type: Optional[Dict[str, AwsResourceGroup]]
+        self.aws_resource_groups: Optional[Dict[str, Any]] = None
+
     @property
     def workspace_root_path(self) -> Optional[Path]:
         return self.args.workspace_root_path if self.args else None
 
     @workspace_root_path.setter
     def workspace_root_path(self, workspace_root_path: Path) -> None:
         if self.args is not None and workspace_root_path is not None:
@@ -557,17 +565,15 @@
     ## Docker functions
     ######################################################
 
     def get_container_restart_policy_docker(self) -> Optional[Dict[str, Any]]:
         return self.args.container_restart_policy_docker if self.args else None
 
     def init_docker_resource_groups(self, docker_build_context: Any) -> None:
-        logger.debug(
-            f"@init_docker_resource_groups not defined for {self.__class__.__name__}"
-        )
+        logger.debug(f"@init_docker_resource_groups not defined for {self.name}")
 
     def get_docker_resource_groups(
         self, docker_build_context: Any
     ) -> Optional[Dict[str, Any]]:
         if self.docker_resource_groups is None:
             self.init_docker_resource_groups(docker_build_context)
         # # Comment out in production
@@ -580,17 +586,15 @@
         return self.docker_resource_groups
 
     ######################################################
     ## K8s functions
     ######################################################
 
     def init_k8s_resource_groups(self, k8s_build_context: Any) -> None:
-        logger.debug(
-            f"@init_docker_resource_groups not defined for {self.__class__.__name__}"
-        )
+        logger.debug(f"@init_docker_resource_groups not defined for {self.name}")
 
     def get_k8s_resource_groups(
         self, k8s_build_context: Any
     ) -> Optional[Dict[str, Any]]:
         if self.k8s_resource_groups is None:
             self.init_k8s_resource_groups(k8s_build_context)
         # # Comment out in production
@@ -599,18 +603,42 @@
         #     for rg_name, rg in self.k8s_resource_groups.items():
         #         logger.debug(
         #             "{}:{}\n{}".format(rg_name, type(rg), rg)
         #         )
         return self.k8s_resource_groups
 
     ######################################################
+    ## AWS functions
+    ######################################################
+
+    def init_aws_resource_groups(self, aws_build_context: Any) -> None:
+        logger.debug(f"@init_aws_resource_groups not defined for {self.name}")
+
+    def get_aws_resource_groups(
+        self, aws_build_context: Any
+    ) -> Optional[Dict[str, Any]]:
+        if self.aws_resource_groups is None:
+            self.init_aws_resource_groups(aws_build_context)
+        # Comment out in production
+        if self.aws_resource_groups:
+            logger.debug("AwsResourceGroups:")
+            for rg_name, rg in self.aws_resource_groups.items():
+                try:
+                    logger.debug("{}\n{}".format(rg_name, rg.json(indent=2)))
+                except Exception:
+                    pass
+        return self.aws_resource_groups
+
+    ######################################################
     ## Helpers
     ######################################################
 
-    def get_container_paths(self) -> Optional[Any]:
+    def get_container_paths(
+        self, add_ws_name_to_container_path: bool = True
+    ) -> Optional[Any]:
         if self.workspace_root_path is None:
             return None
 
         workspace_name = self.workspace_root_path.stem
         if workspace_name is None:
             return None
 
@@ -618,14 +646,16 @@
         if workspace_volume_container_path is None:
             return None
 
         from phidata.types.context import ContainerPathContext
 
         workspace_root_container_path = (
             f"{workspace_volume_container_path}/{workspace_name}"
+            if add_ws_name_to_container_path
+            else workspace_volume_container_path
         )
         container_paths = ContainerPathContext(
             workspace_name=workspace_name,
             workspace_root=workspace_root_container_path,
             workspace_parent=workspace_volume_container_path,
         )
```

### Comparing `phidata-1.4.4/phidata/app/postgres/postgres_db.py` & `phidata-1.5.0/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/prometheus/prometheus.py` & `phidata-1.5.0/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/redis/redis.py` & `phidata-1.5.0/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/server/api_server.py` & `phidata-1.5.0/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/server/app_server.py` & `phidata-1.5.0/phidata/app/server/app_server.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/server/server_base.py` & `phidata-1.5.0/phidata/app/spark/spark_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,43 +4,56 @@
 from phidata.app.phidata_app import PhidataApp, PhidataAppArgs, WorkspaceVolumeType
 from phidata.k8s.enums.service_type import ServiceType
 from phidata.k8s.enums.image_pull_policy import ImagePullPolicy
 from phidata.k8s.enums.restart_policy import RestartPolicy
 from phidata.utils.log import logger
 
 
-class ServerBaseArgs(PhidataAppArgs):
-    name: str = "server"
+class SparkBaseArgs(PhidataAppArgs):
+    name: str = "spark"
     version: str = "1"
     enabled: bool = True
 
     # -*- Image Configuration
-    image_name: str = "phidata/server"
-    image_tag: str = "1.4.1"
+    image_name: str = "phidata/spark"
+    image_tag: str = "3.3.1"
     entrypoint: Optional[Union[str, List]] = None
     command: Optional[Union[str, List]] = None
 
+    # -*- Spark Configuration
+    cores: Optional[int] = None
+    memory: Optional[str] = None
+    driver_port: int = 7077
+    driver_url: Optional[str] = None
+    properties_file: Optional[str] = None
 
-class ServerBase(PhidataApp):
+
+class SparkBase(PhidataApp):
     def __init__(
         self,
-        name: str = "server",
+        name: str = "spark",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/server",
-        image_tag: str = "1.4.1",
+        image_name: str = "phidata/spark",
+        image_tag: str = "3.3.1",
         entrypoint: Optional[Union[str, List]] = None,
         command: Optional[Union[str, List]] = None,
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
+        # -*- Spark Configuration
+        cores: Optional[int] = None,
+        memory: Optional[str] = None,
+        driver_port: int = 7077,
+        driver_url: Optional[str] = None,
+        properties_file: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Overwrite the PYTHONPATH env var,
         # which is usually set to the workspace_root_container_path,
         python_path: Optional[str] = None,
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
@@ -57,28 +70,31 @@
         secrets: Optional[Dict[str, str]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
-        open_container_port: bool = False,
+        open_container_port: bool = True,
         # Port number on the container,
         container_port: int = 8080,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
         container_host_port: int = 8080,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume inside the container,
-        workspace_volume_container_path: str = "/usr/local/server",
+        # Path to mount the workspace volume,
+        # This is the parent directory for the workspace on the container,
+        # i.e. the ws is mounted as a subdir in this dir,
+        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
+        workspace_volume_container_path: str = "/mnt/workspaces",
         # How to mount the workspace volume,
         # Option 1: Mount the workspace from the host machine,
         # If None, use the workspace_root_path,
         # Note: This is the default on DockerContainers. We assume that DockerContainers,
         # are running locally on the user's machine so the local workspace_root_path,
         # is mounted to the workspace_volume_container_path,
         workspace_volume_host_path: Optional[str] = None,
@@ -241,25 +257,30 @@
         print_env_on_load: bool = True,
         # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
         **kwargs,
     ):
         super().__init__()
         try:
-            self.args: ServerBaseArgs = ServerBaseArgs(
+            self.args: SparkBaseArgs = SparkBaseArgs(
                 name=name,
                 version=version,
                 enabled=enabled,
                 image=image,
                 image_name=image_name,
                 image_tag=image_tag,
                 entrypoint=entrypoint,
                 command=command,
                 install_requirements=install_requirements,
                 requirements_file=requirements_file,
+                cores=cores,
+                memory=memory,
+                driver_port=driver_port,
+                driver_url=driver_url,
+                properties_file=properties_file,
                 container_name=container_name,
                 python_path=python_path,
                 add_python_path=add_python_path,
                 container_labels=container_labels,
                 env=env,
                 env_file=env_file,
                 secrets=secrets,
@@ -349,14 +370,22 @@
                 use_cache=use_cache,
                 extra_kwargs=kwargs,
             )
         except Exception as e:
             logger.error(f"Args for {self.name} are not valid")
             raise
 
+    @property
+    def driver_url(self) -> Optional[str]:
+        driver_host = self.get_container_name()
+        driver_port = self.args.driver_port
+        if not driver_host or not driver_port:
+            return None
+        return f"spark://{driver_host}:{driver_port}"
+
     ######################################################
     ## Docker Resources
     ######################################################
 
     def get_docker_rg(self, docker_build_context: Any) -> Optional[Any]:
         app_name = self.args.name
         logger.debug(f"Building {app_name} DockerResourceGroup")
@@ -424,21 +453,38 @@
             WORKSPACES_MOUNT_ENV_VAR: container_paths.workspace_parent,
             WORKSPACE_CONFIG_DIR_ENV_VAR: container_paths.workspace_config_dir,
             "INSTALL_REQUIREMENTS": str(self.args.install_requirements),
             "REQUIREMENTS_FILE_PATH": container_paths.requirements_file,
             "MOUNT_WORKSPACE": str(self.args.mount_workspace),
             # Print env when the container starts
             "PRINT_ENV_ON_LOAD": str(self.args.print_env_on_load),
+            # Spark env vars
+            "SPARK_DRIVER_PORT": str(self.args.driver_port),
+            "SPARK_DRIVER_URL": str(self.args.driver_url)
+            if self.args.driver_url
+            else "",
+            "SPARK_WEBUI_PORT": str(self.args.container_port),
         }
 
         # Set aws env vars
         self.set_aws_env_vars(env_dict=container_env)
 
-        # Set container env using env_dict, env_file or secrets_file
-        self.set_container_env(container_env=container_env)
+        # Update the container env using env_file
+        env_data_from_file = self.get_env_data()
+        if env_data_from_file is not None:
+            container_env.update(env_data_from_file)
+
+        # Update the container env using secrets_file or a secrets backend
+        secret_data_from_file = self.get_secret_data()
+        if secret_data_from_file is not None:
+            container_env.update(secret_data_from_file)
+
+        # Update the container env with user provided env, this overwrites any existing variables
+        if self.args.env is not None and isinstance(self.args.env, dict):
+            container_env.update(self.args.env)
 
         # Container Volumes
         # container_volumes is a dictionary which configures the volumes to mount
         # inside the container. The key is either the host path or a volume name,
         # and the value is a dictionary with 2 keys:
         #   bind - The path to mount the volume inside the container
         #   mode - Either rw to mount the volume read/write, or ro to mount it read-only.
@@ -496,20 +542,35 @@
 
         # if open_container_port = True
         if self.args.open_container_port:
             container_ports[
                 str(self.args.container_port)
             ] = self.args.container_host_port
 
+        container_cmd: List[str]
+        if isinstance(self.args.command, str):
+            container_cmd = self.args.command.split(" ")
+        else:
+            container_cmd = self.args.command
+
+        if self.args.cores is not None:
+            container_cmd.append(f"--cores {str(self.args.cores)}")
+
+        if self.args.memory is not None:
+            container_cmd.append(f"--memory {str(self.args.memory)}")
+
+        if self.args.properties_file is not None:
+            container_cmd.append(f"--properties-file {str(self.args.properties_file)}")
+
         # Create the container
         docker_container = DockerContainer(
             name=self.get_container_name(),
             image=self.get_image_str(),
             entrypoint=self.args.entrypoint,
-            command=self.args.command,
+            command=" ".join(container_cmd),
             detach=self.args.container_detach,
             auto_remove=self.args.container_auto_remove,
             healthcheck=self.args.container_healthcheck,
             hostname=self.args.container_hostname,
             labels=self.args.container_labels,
             environment=container_env,
             network=docker_build_context.network,
```

### Comparing `phidata-1.4.4/phidata/app/spark/spark_base.py` & `phidata-1.5.0/phidata/app/server/server_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,56 +4,52 @@
 from phidata.app.phidata_app import PhidataApp, PhidataAppArgs, WorkspaceVolumeType
 from phidata.k8s.enums.service_type import ServiceType
 from phidata.k8s.enums.image_pull_policy import ImagePullPolicy
 from phidata.k8s.enums.restart_policy import RestartPolicy
 from phidata.utils.log import logger
 
 
-class SparkBaseArgs(PhidataAppArgs):
-    name: str = "spark"
+class ServerBaseArgs(PhidataAppArgs):
+    name: str = "server"
     version: str = "1"
     enabled: bool = True
 
     # -*- Image Configuration
-    image_name: str = "phidata/spark"
-    image_tag: str = "3.3.1"
+    image_name: str = "phidata/server"
+    image_tag: str = "1.5.0"
     entrypoint: Optional[Union[str, List]] = None
     command: Optional[Union[str, List]] = None
 
-    # -*- Spark Configuration
-    cores: Optional[int] = None
-    memory: Optional[str] = None
-    driver_port: int = 7077
-    driver_url: Optional[str] = None
-    properties_file: Optional[str] = None
+    # -*- AWS Configuration
+    ecs_cluster: Optional[Any] = None
+    ecs_launch_type: str = "FARGATE"
+    ecs_task_cpu: str = "256"
+    ecs_task_memory: str = "512"
+    ecs_service_count: int = 1
+    assign_public_ip: bool = True
+    elb: Optional[Any] = None
 
 
-class SparkBase(PhidataApp):
+class ServerBase(PhidataApp):
     def __init__(
         self,
-        name: str = "spark",
+        name: str = "server",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/spark",
-        image_tag: str = "3.3.1",
+        image_name: str = "phidata/server",
+        image_tag: str = "1.5.0",
         entrypoint: Optional[Union[str, List]] = None,
         command: Optional[Union[str, List]] = None,
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
-        # -*- Spark Configuration
-        cores: Optional[int] = None,
-        memory: Optional[str] = None,
-        driver_port: int = 7077,
-        driver_url: Optional[str] = None,
-        properties_file: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Overwrite the PYTHONPATH env var,
         # which is usually set to the workspace_root_container_path,
         python_path: Optional[str] = None,
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
@@ -70,31 +66,28 @@
         secrets: Optional[Dict[str, str]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
-        open_container_port: bool = True,
+        open_container_port: bool = False,
         # Port number on the container,
         container_port: int = 8080,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
         container_host_port: int = 8080,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume,
-        # This is the parent directory for the workspace on the container,
-        # i.e. the ws is mounted as a subdir in this dir,
-        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
-        workspace_volume_container_path: str = "/mnt/workspaces",
+        # Path to mount the workspace volume inside the container,
+        workspace_volume_container_path: str = "/usr/local/server",
         # How to mount the workspace volume,
         # Option 1: Mount the workspace from the host machine,
         # If None, use the workspace_root_path,
         # Note: This is the default on DockerContainers. We assume that DockerContainers,
         # are running locally on the user's machine so the local workspace_root_path,
         # is mounted to the workspace_volume_container_path,
         workspace_volume_host_path: Optional[str] = None,
@@ -249,38 +242,53 @@
         extra_volumes: Optional[List[Any]] = None,
         # Type: CreateStorageClass,
         extra_storage_classes: Optional[List[Any]] = None,
         # Type: CreateCustomObject,
         extra_custom_objects: Optional[List[Any]] = None,
         # Type: CreateCustomResourceDefinition,
         extra_crds: Optional[List[Any]] = None,
+        # -*- AWS configuration,
+        ecs_cluster: Optional[Any] = None,
+        ecs_launch_type: str = "FARGATE",
+        ecs_task_cpu: str = "256",
+        ecs_task_memory: str = "512",
+        ecs_service_count: int = 1,
+        assign_public_ip: bool = True,
+        elb: Optional[Any] = None,
+        aws_subnets: Optional[List[str]] = None,
+        aws_security_groups: Optional[List[str]] = None,
         # Other args,
-        print_env_on_load: bool = True,
+        print_env_on_load: bool = False,
+        skip_create: bool = False,
+        skip_read: bool = False,
+        skip_update: bool = False,
+        recreate_on_update: bool = False,
+        skip_delete: bool = False,
+        wait_for_creation: bool = True,
+        wait_for_update: bool = True,
+        wait_for_deletion: bool = True,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 50,
         # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
         **kwargs,
     ):
         super().__init__()
         try:
-            self.args: SparkBaseArgs = SparkBaseArgs(
+            self.args: ServerBaseArgs = ServerBaseArgs(
                 name=name,
                 version=version,
                 enabled=enabled,
                 image=image,
                 image_name=image_name,
                 image_tag=image_tag,
                 entrypoint=entrypoint,
                 command=command,
                 install_requirements=install_requirements,
                 requirements_file=requirements_file,
-                cores=cores,
-                memory=memory,
-                driver_port=driver_port,
-                driver_url=driver_url,
-                properties_file=properties_file,
                 container_name=container_name,
                 python_path=python_path,
                 add_python_path=add_python_path,
                 container_labels=container_labels,
                 env=env,
                 env_file=env_file,
                 secrets=secrets,
@@ -362,30 +370,41 @@
                 extra_containers=extra_containers,
                 extra_init_containers=extra_init_containers,
                 extra_ports=extra_ports,
                 extra_volumes=extra_volumes,
                 extra_storage_classes=extra_storage_classes,
                 extra_custom_objects=extra_custom_objects,
                 extra_crds=extra_crds,
+                ecs_cluster=ecs_cluster,
+                ecs_launch_type=ecs_launch_type,
+                ecs_task_cpu=ecs_task_cpu,
+                ecs_task_memory=ecs_task_memory,
+                ecs_service_count=ecs_service_count,
+                assign_public_ip=assign_public_ip,
+                elb=elb,
+                aws_subnets=aws_subnets,
+                aws_security_groups=aws_security_groups,
                 print_env_on_load=print_env_on_load,
+                skip_create=skip_create,
+                skip_read=skip_read,
+                skip_update=skip_update,
+                recreate_on_update=recreate_on_update,
+                skip_delete=skip_delete,
+                wait_for_creation=wait_for_creation,
+                wait_for_update=wait_for_update,
+                wait_for_deletion=wait_for_deletion,
+                waiter_delay=waiter_delay,
+                waiter_max_attempts=waiter_max_attempts,
                 use_cache=use_cache,
                 extra_kwargs=kwargs,
             )
         except Exception as e:
             logger.error(f"Args for {self.name} are not valid")
             raise
 
-    @property
-    def driver_url(self) -> Optional[str]:
-        driver_host = self.get_container_name()
-        driver_port = self.args.driver_port
-        if not driver_host or not driver_port:
-            return None
-        return f"spark://{driver_host}:{driver_port}"
-
     ######################################################
     ## Docker Resources
     ######################################################
 
     def get_docker_rg(self, docker_build_context: Any) -> Optional[Any]:
         app_name = self.args.name
         logger.debug(f"Building {app_name} DockerResourceGroup")
@@ -453,38 +472,21 @@
             WORKSPACES_MOUNT_ENV_VAR: container_paths.workspace_parent,
             WORKSPACE_CONFIG_DIR_ENV_VAR: container_paths.workspace_config_dir,
             "INSTALL_REQUIREMENTS": str(self.args.install_requirements),
             "REQUIREMENTS_FILE_PATH": container_paths.requirements_file,
             "MOUNT_WORKSPACE": str(self.args.mount_workspace),
             # Print env when the container starts
             "PRINT_ENV_ON_LOAD": str(self.args.print_env_on_load),
-            # Spark env vars
-            "SPARK_DRIVER_PORT": str(self.args.driver_port),
-            "SPARK_DRIVER_URL": str(self.args.driver_url)
-            if self.args.driver_url
-            else "",
-            "SPARK_WEBUI_PORT": str(self.args.container_port),
         }
 
         # Set aws env vars
         self.set_aws_env_vars(env_dict=container_env)
 
-        # Update the container env using env_file
-        env_data_from_file = self.get_env_data()
-        if env_data_from_file is not None:
-            container_env.update(env_data_from_file)
-
-        # Update the container env using secrets_file or a secrets backend
-        secret_data_from_file = self.get_secret_data()
-        if secret_data_from_file is not None:
-            container_env.update(secret_data_from_file)
-
-        # Update the container env with user provided env, this overwrites any existing variables
-        if self.args.env is not None and isinstance(self.args.env, dict):
-            container_env.update(self.args.env)
+        # Set container env using env_dict, env_file or secrets_file
+        self.set_container_env(container_env=container_env)
 
         # Container Volumes
         # container_volumes is a dictionary which configures the volumes to mount
         # inside the container. The key is either the host path or a volume name,
         # and the value is a dictionary with 2 keys:
         #   bind - The path to mount the volume inside the container
         #   mode - Either rw to mount the volume read/write, or ro to mount it read-only.
@@ -542,35 +544,20 @@
 
         # if open_container_port = True
         if self.args.open_container_port:
             container_ports[
                 str(self.args.container_port)
             ] = self.args.container_host_port
 
-        container_cmd: List[str]
-        if isinstance(self.args.command, str):
-            container_cmd = self.args.command.split(" ")
-        else:
-            container_cmd = self.args.command
-
-        if self.args.cores is not None:
-            container_cmd.append(f"--cores {str(self.args.cores)}")
-
-        if self.args.memory is not None:
-            container_cmd.append(f"--memory {str(self.args.memory)}")
-
-        if self.args.properties_file is not None:
-            container_cmd.append(f"--properties-file {str(self.args.properties_file)}")
-
         # Create the container
         docker_container = DockerContainer(
             name=self.get_container_name(),
             image=self.get_image_str(),
             entrypoint=self.args.entrypoint,
-            command=" ".join(container_cmd),
+            command=self.args.command,
             detach=self.args.container_detach,
             auto_remove=self.args.container_auto_remove,
             healthcheck=self.args.container_healthcheck,
             hostname=self.args.container_hostname,
             labels=self.args.container_labels,
             environment=container_env,
             network=docker_build_context.network,
@@ -1064,7 +1051,238 @@
         k8s_rg = self.get_k8s_rg(k8s_build_context)
         if k8s_rg is not None:
             from collections import OrderedDict
 
             if self.k8s_resource_groups is None:
                 self.k8s_resource_groups = OrderedDict()
             self.k8s_resource_groups[k8s_rg.name] = k8s_rg
+
+    ######################################################
+    ## Aws Resources
+    ######################################################
+
+    def get_aws_rg(self, aws_build_context: Any) -> Optional[Any]:
+        app_name = self.args.name
+        logger.debug(f"Building {app_name} AwsResourceGroup")
+
+        from phidata.constants import (
+            PYTHONPATH_ENV_VAR,
+            PHIDATA_RUNTIME_ENV_VAR,
+            SCRIPTS_DIR_ENV_VAR,
+            STORAGE_DIR_ENV_VAR,
+            META_DIR_ENV_VAR,
+            PRODUCTS_DIR_ENV_VAR,
+            NOTEBOOKS_DIR_ENV_VAR,
+            WORKFLOWS_DIR_ENV_VAR,
+            WORKSPACE_ROOT_ENV_VAR,
+            WORKSPACES_MOUNT_ENV_VAR,
+            WORKSPACE_CONFIG_DIR_ENV_VAR,
+        )
+        from phidata.aws.resource.group import (
+            AwsResourceGroup,
+            EcsCluster,
+            EcsContainer,
+            EcsTaskDefinition,
+            EcsService,
+            LoadBalancer,
+            TargetGroup,
+            Listener,
+            Subnet,
+        )
+        from phidata.types.context import ContainerPathContext
+
+        # Workspace paths
+        if self.workspace_root_path is None:
+            logger.error("Invalid workspace_root_path")
+            return None
+
+        workspace_name = self.workspace_root_path.stem
+        container_paths: Optional[ContainerPathContext] = self.get_container_paths(
+            add_ws_name_to_container_path=False
+        )
+        if container_paths is None:
+            logger.error("Could not build container paths")
+            return None
+        logger.debug(f"Container Paths: {container_paths.json(indent=2)}")
+
+        # Container pythonpath
+        # python_path = self.args.python_path
+        # if python_path is None:
+        #     python_path = "{}{}".format(
+        #         container_paths.workspace_root,
+        #         f":{self.args.add_python_path}" if self.args.add_python_path else "",
+        #     )
+
+        # Container Environment
+        container_env: Dict[str, Any] = {
+            # Env variables used by data workflows and data assets
+            # PYTHONPATH_ENV_VAR: python_path,
+            PHIDATA_RUNTIME_ENV_VAR: "ecs",
+            SCRIPTS_DIR_ENV_VAR: container_paths.scripts_dir,
+            STORAGE_DIR_ENV_VAR: container_paths.storage_dir,
+            META_DIR_ENV_VAR: container_paths.meta_dir,
+            PRODUCTS_DIR_ENV_VAR: container_paths.products_dir,
+            NOTEBOOKS_DIR_ENV_VAR: container_paths.notebooks_dir,
+            WORKFLOWS_DIR_ENV_VAR: container_paths.workflows_dir,
+            WORKSPACE_ROOT_ENV_VAR: container_paths.workspace_root,
+            WORKSPACES_MOUNT_ENV_VAR: container_paths.workspace_parent,
+            WORKSPACE_CONFIG_DIR_ENV_VAR: container_paths.workspace_config_dir,
+            "INSTALL_REQUIREMENTS": str(self.args.install_requirements),
+            "REQUIREMENTS_FILE_PATH": container_paths.requirements_file,
+            "MOUNT_WORKSPACE": str(self.args.mount_workspace),
+            # Print env when the container starts
+            "PRINT_ENV_ON_LOAD": str(self.args.print_env_on_load),
+        }
+
+        # Set aws env vars
+        self.set_aws_env_vars(env_dict=container_env)
+
+        # Set container env using env_dict, env_file or secrets_file
+        self.set_container_env(container_env=container_env)
+
+        # -*- Create ECS cluster
+        ecs_cluster = self.args.ecs_cluster
+        if ecs_cluster is None:
+            ecs_cluster = EcsCluster(
+                name=f"{app_name}-cluster",
+                ecs_cluster_name=app_name,
+                capacity_providers=[self.args.ecs_launch_type],
+                skip_create=self.args.skip_create,
+                skip_delete=self.args.skip_delete,
+                wait_for_creation=self.args.wait_for_creation,
+                wait_for_deletion=self.args.wait_for_deletion,
+            )
+
+        # -*- Create Load Balancer
+        load_balancer = self.args.elb
+        if load_balancer is None:
+            load_balancer = LoadBalancer(
+                name=f"{app_name}-lb",
+                subnets=self.args.aws_subnets,
+                security_groups=self.args.aws_security_groups,
+                skip_create=self.args.skip_create,
+                skip_delete=self.args.skip_delete,
+                wait_for_creation=self.args.wait_for_creation,
+                wait_for_deletion=self.args.wait_for_deletion,
+            )
+
+        # Get VPC ID from subnets
+        vpc_ids = set()
+        for subnet in self.args.aws_subnets:
+            _vpc = Subnet(id=subnet).get_vpc_id()
+            vpc_ids.add(_vpc)
+            if len(vpc_ids) != 1:
+                raise ValueError("Subnets must be in the same VPC")
+        vpc_id = vpc_ids.pop()
+
+        # -*- Create Target Group
+        target_group = TargetGroup(
+            name=f"{app_name}-tg",
+            port=self.get_container_port(),
+            protocol="HTTP",
+            vpc_id=vpc_id,
+            target_type="ip",
+            skip_create=self.args.skip_create,
+            skip_delete=self.args.skip_delete,
+            wait_for_creation=self.args.wait_for_creation,
+            wait_for_deletion=self.args.wait_for_deletion,
+        )
+
+        # -*- Create Listener
+        listener = Listener(
+            name=f"{app_name}-listener",
+            protocol="HTTP",
+            port=80,
+            load_balancer=load_balancer,
+            target_group=target_group,
+            skip_create=self.args.skip_create,
+            skip_delete=self.args.skip_delete,
+            wait_for_creation=self.args.wait_for_creation,
+            wait_for_deletion=self.args.wait_for_deletion,
+        )
+
+        # -*- Create ECS Container
+        ecs_container = EcsContainer(
+            name=app_name,
+            image=self.get_image_str(),
+            port_mappings=[{"containerPort": self.get_container_port()}],
+            command=self.args.command,
+            environment=[{"name": k, "value": v} for k, v in container_env.items()],
+            log_configuration={
+                "logDriver": "awslogs",
+                "options": {
+                    "awslogs-group": app_name,
+                    "awslogs-region": self.aws_region,
+                    "awslogs-create-group": "true",
+                    "awslogs-stream-prefix": app_name,
+                },
+            },
+            skip_create=self.args.skip_create,
+            skip_delete=self.args.skip_delete,
+            wait_for_creation=self.args.wait_for_creation,
+            wait_for_deletion=self.args.wait_for_deletion,
+        )
+
+        # -*- Create ECS Task Definition
+        ecs_task_definition = EcsTaskDefinition(
+            name=f"{app_name}-td",
+            family=app_name,
+            network_mode="awsvpc",
+            cpu=self.args.ecs_task_cpu,
+            memory=self.args.ecs_task_memory,
+            containers=[ecs_container],
+            requires_compatibilities=[self.args.ecs_launch_type],
+            skip_create=self.args.skip_create,
+            skip_delete=self.args.skip_delete,
+            wait_for_creation=self.args.wait_for_creation,
+            wait_for_deletion=self.args.wait_for_deletion,
+        )
+
+        aws_vpc_config = {}
+        if self.args.aws_subnets is not None:
+            aws_vpc_config["subnets"] = self.args.aws_subnets
+        if self.args.aws_security_groups is not None:
+            aws_vpc_config["securityGroups"] = self.args.aws_security_groups
+        if self.args.assign_public_ip:
+            aws_vpc_config["assignPublicIp"] = "ENABLED"
+
+        # -*- Create ECS Service
+        ecs_service = EcsService(
+            name=f"{app_name}-service",
+            desired_count=self.args.ecs_service_count,
+            launch_type=self.args.ecs_launch_type,
+            cluster=ecs_cluster,
+            task_definition=ecs_task_definition,
+            target_group=target_group,
+            target_container_name=ecs_container.name,
+            target_container_port=self.get_container_port(),
+            network_configuration={"awsvpcConfiguration": aws_vpc_config},
+            # Force delete the service.
+            force_delete=True,
+            # Force a new deployment of the service on update.
+            force_new_deployment=True,
+            skip_create=self.args.skip_create,
+            skip_delete=self.args.skip_delete,
+            wait_for_creation=self.args.wait_for_creation,
+            wait_for_deletion=self.args.wait_for_deletion,
+        )
+
+        # -*- Create AwsResourceGroup
+        return AwsResourceGroup(
+            name=app_name,
+            enabled=self.enabled,
+            ecs_clusters=[ecs_cluster],
+            ecs_task_definitions=[ecs_task_definition],
+            ecs_services=[ecs_service],
+            load_balancers=[load_balancer],
+            target_groups=[target_group],
+            listeners=[listener],
+        )
+
+    def init_aws_resource_groups(self, aws_build_context: Any) -> None:
+        aws_rg = self.get_aws_rg(aws_build_context)
+        if aws_rg is not None:
+            from collections import OrderedDict
+
+            if self.aws_resource_groups is None:
+                self.aws_resource_groups = OrderedDict()
+            self.aws_resource_groups[aws_rg.name] = aws_rg
```

### Comparing `phidata-1.4.4/phidata/app/spark/spark_driver.py` & `phidata-1.5.0/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/spark/spark_worker.py` & `phidata-1.5.0/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/superset/superset_base.py` & `phidata-1.5.0/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/superset/superset_init.py` & `phidata-1.5.0/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/superset/superset_webserver.py` & `phidata-1.5.0/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/superset/superset_worker.py` & `phidata-1.5.0/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/superset/superset_worker_beat.py` & `phidata-1.5.0/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/traefik/crds.py` & `phidata-1.5.0/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/traefik/ingress_route.py` & `phidata-1.5.0/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/app/traefik/router.py` & `phidata-1.5.0/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/asset/aws/aws_asset.py` & `phidata-1.5.0/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/asset/data_asset.py` & `phidata-1.5.0/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/asset/local/file.py` & `phidata-1.5.0/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/asset/local/local_asset.py` & `phidata-1.5.0/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/api_client.py` & `phidata-1.5.0/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/athena/query.py` & `phidata-1.5.0/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/create/iam/eks_admin_role.py` & `phidata-1.5.0/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/create/iam/role.py` & `phidata-1.5.0/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/enums/manager_status.py` & `phidata-1.5.0/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/manager.py` & `phidata-1.5.0/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/acm/certificate.py` & `phidata-1.5.0/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/athena/query.py` & `phidata-1.5.0/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/base.py` & `phidata-1.5.0/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/cloudformation/stack.py` & `phidata-1.5.0/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/ec2/subnet.py` & `phidata-1.5.0/phidata/aws/resource/ec2/subnet.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,7 +35,25 @@
             logger.debug(f"AZ for {self.id}: {az}")
             return az
         except ClientError as ce:
             logger.debug(f"ClientError: {ce}")
         except Exception as e:
             print_error(f"Error reading {self.get_resource_type()}: {e}")
         return None
+
+    def get_vpc_id(self, aws_client: Optional[AwsApiClient] = None) -> Optional[str]:
+        # logger.debug(f"Reading {self.get_resource_type()}: {self.get_resource_name()}")
+
+        from botocore.exceptions import ClientError
+
+        client: AwsApiClient = aws_client or self.get_aws_client()
+        service_resource = self.get_service_resource(client)
+        try:
+            subnet = service_resource.Subnet(self.id)
+            vpc_id = subnet.vpc_id
+            logger.debug(f"VPC ID for {self.id}: {vpc_id}")
+            return vpc_id
+        except ClientError as ce:
+            logger.debug(f"ClientError: {ce}")
+        except Exception as e:
+            print_error(f"Error reading {self.get_resource_type()}: {e}")
+        return None
```

### Comparing `phidata-1.4.4/phidata/aws/resource/ec2/volume.py` & `phidata-1.5.0/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/ecs/cluster.py` & `phidata-1.5.0/phidata/aws/resource/ecs/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,7 +136,14 @@
             )
             return True
         except Exception as e:
             print_error(f"{self.get_resource_type()} could not be deleted.")
             print_error("Please try again or delete resources manually.")
             print_error(e)
         return False
+
+    def get_arn(self, aws_client: AwsApiClient) -> Optional[str]:
+        tg = self._read(aws_client)
+        if tg is None:
+            return None
+        tg_arn = tg.get("ListenerArn", None)
+        return tg_arn
```

### Comparing `phidata-1.4.4/phidata/aws/resource/ecs/container.py` & `phidata-1.5.0/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/ecs/service.py` & `phidata-1.5.0/phidata/aws/resource/ecs/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional, Any, Dict, List, Literal, Union
 
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
 from phidata.aws.resource.ecs.cluster import EcsCluster
 from phidata.aws.resource.ecs.task_definition import EcsTaskDefinition
+from phidata.aws.resource.elb.target_group import TargetGroup
 from phidata.utils.cli_console import print_info, print_error
 from phidata.utils.log import logger
 
 
 class EcsService(AwsResource):
     """
     # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html
@@ -34,14 +35,24 @@
     # - string: The family and revision (family:revision ) or full ARN of the task definition.
     # - EcsTaskDefinition
     # If a revision isn't specified, the latest ACTIVE revision is used.
     task_definition: Optional[Union[EcsTaskDefinition, str]] = None
 
     # A load balancer object representing the load balancers to use with your service.
     load_balancers: Optional[List[Dict[str, Any]]] = None
+
+    # We can generate the load_balancers dict using
+    # the target_group, target_container_name and target_container_port
+    # Target group to attach to a service.
+    target_group: Optional[TargetGroup] = None
+    # Target container name for the service.
+    target_container_name: Optional[str] = None
+    target_container_port: Optional[int] = None
+
+    # The details of the service discovery registries to assign to this service.
     service_registries: Optional[List[Dict[str, Any]]] = None
     # The number of instantiations of the specified task definition to place and keep running on your cluster.
     # This is required if schedulingStrategy is REPLICA or isn't specified.
     # If schedulingStrategy is DAEMON then this isn't required.
     desired_count: Optional[int] = None
     # An identifier that you provide to ensure the idempotency of the request. It must be unique and is case-sensitive.
     client_token: Optional[str] = None
@@ -96,16 +107,14 @@
 
         # create a dict of args which are not null, otherwise aws type validation fails
         not_null_args: Dict[str, Any] = {}
 
         cluster_name = self.get_ecs_cluster_name()
         if cluster_name is not None:
             not_null_args["cluster"] = cluster_name
-        if self.load_balancers is not None:
-            not_null_args["loadBalancers"] = self.load_balancers
         if self.service_registries is not None:
             not_null_args["serviceRegistries"] = self.service_registries
         if self.desired_count is not None:
             not_null_args["desiredCount"] = self.desired_count
         if self.client_token is not None:
             not_null_args["clientToken"] = self.client_token
         if self.launch_type is not None:
@@ -137,14 +146,25 @@
         if self.enable_ecsmanaged_tags is not None:
             not_null_args["enableECSManagedTags"] = self.enable_ecsmanaged_tags
         if self.propagate_tags is not None:
             not_null_args["propagateTags"] = self.propagate_tags
         if self.enable_execute_command is not None:
             not_null_args["enableExecuteCommand"] = self.enable_execute_command
 
+        if self.load_balancers is not None:
+            not_null_args["loadBalancers"] = self.load_balancers
+        elif self.target_group is not None and self.target_container_name is not None:
+            not_null_args["loadBalancers"] = [
+                {
+                    "targetGroupArn": self.target_group.get_arn(aws_client),
+                    "containerName": self.target_container_name,
+                    "containerPort": self.target_container_port,
+                }
+            ]
+
         # Register EcsService
         service_client = self.get_service_client(aws_client)
         try:
             create_response = service_client.create_service(
                 serviceName=self.get_ecs_service_name(),
                 taskDefinition=self.get_ecs_task_definition(),
                 **not_null_args,
```

### Comparing `phidata-1.4.4/phidata/aws/resource/ecs/task_definition.py` & `phidata-1.5.0/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/ecs/volume.py` & `phidata-1.5.0/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/eks/addon.py` & `phidata-1.5.0/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/eks/cluster.py` & `phidata-1.5.0/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/eks/fargate_profile.py` & `phidata-1.5.0/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/eks/kubeconfig.py` & `phidata-1.5.0/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/eks/node_group.py` & `phidata-1.5.0/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/elasticache/cluster.py` & `phidata-1.5.0/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-1.5.0/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/emr/cluster.py` & `phidata-1.5.0/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/glue/crawler.py` & `phidata-1.5.0/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/group.py` & `phidata-1.5.0/phidata/aws/resource/group.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 from phidata.aws.resource.acm.certificate import AcmCertificate
 from phidata.aws.resource.cloudformation.stack import CloudFormationStack
 from phidata.aws.resource.ec2.volume import EbsVolume
+from phidata.aws.resource.ec2.subnet import Subnet
 from phidata.aws.resource.ecs.cluster import EcsCluster
 from phidata.aws.resource.ecs.container import EcsContainer
 from phidata.aws.resource.ecs.task_definition import EcsTaskDefinition
 from phidata.aws.resource.ecs.volume import EcsVolume
 from phidata.aws.resource.ecs.service import EcsService
 from phidata.aws.resource.eks.cluster import EksCluster
 from phidata.aws.resource.eks.fargate_profile import EksFargateProfile
 from phidata.aws.resource.eks.node_group import EksNodeGroup
 from phidata.aws.resource.eks.kubeconfig import EksKubeconfig
+from phidata.aws.resource.elb.load_balancer import LoadBalancer
+from phidata.aws.resource.elb.target_group import TargetGroup
+from phidata.aws.resource.elb.listener import Listener
 from phidata.aws.resource.iam.role import IamRole
 from phidata.aws.resource.iam.policy import IamPolicy
 from phidata.aws.resource.glue.crawler import GlueCrawler
 from phidata.aws.resource.s3.bucket import S3Bucket
 from phidata.aws.resource.emr.cluster import EmrCluster
 from phidata.aws.resource.rds.db_cluster import DbCluster
 from phidata.aws.resource.rds.db_instance import DbInstance
@@ -29,14 +33,15 @@
 class AwsResourceGroup(BaseModel):
     """The AwsResourceGroup class contains the data for all AwsResources"""
 
     name: str = "default"
     enabled: bool = True
     weight: int = 100
 
+    subnets: Optional[List[Subnet]] = None
     iam_roles: Optional[List[IamRole]] = None
     iam_policies: Optional[List[IamPolicy]] = None
     acm_certificates: Optional[List[AcmCertificate]] = None
     s3_buckets: Optional[List[S3Bucket]] = None
     cache_clusters: Optional[List[CacheCluster]] = None
     cache_subnet_groups: Optional[List[CacheSubnetGroup]] = None
     db_clusters: Optional[List[DbCluster]] = None
@@ -49,7 +54,10 @@
     cloudformation_stacks: Optional[List[CloudFormationStack]] = None
     eks_cluster: Optional[EksCluster] = None
     eks_kubeconfig: Optional[EksKubeconfig] = None
     eks_fargate_profiles: Optional[List[EksFargateProfile]] = None
     eks_nodegroups: Optional[List[EksNodeGroup]] = None
     crawlers: Optional[List[GlueCrawler]] = None
     emr: Optional[List[EmrCluster]] = None
+    load_balancers: Optional[List[LoadBalancer]] = None
+    target_groups: Optional[List[TargetGroup]] = None
+    listeners: Optional[List[Listener]] = None
```

### Comparing `phidata-1.4.4/phidata/aws/resource/iam/group.py` & `phidata-1.5.0/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/iam/policy.py` & `phidata-1.5.0/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/iam/role.py` & `phidata-1.5.0/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/rds/db_cluster.py` & `phidata-1.5.0/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/rds/db_instance.py` & `phidata-1.5.0/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-1.5.0/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/s3/bucket.py` & `phidata-1.5.0/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/secret/manager.py` & `phidata-1.5.0/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/resource/types.py` & `phidata-1.5.0/phidata/aws/resource/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from collections import OrderedDict
 from typing import Dict, List, Type, Union
 
 from phidata.aws.resource.base import AwsResource
 from phidata.aws.resource.acm.certificate import AcmCertificate
 from phidata.aws.resource.cloudformation.stack import CloudFormationStack
 from phidata.aws.resource.ec2.volume import EbsVolume
+from phidata.aws.resource.ec2.subnet import Subnet
 from phidata.aws.resource.ecs.cluster import EcsCluster
 from phidata.aws.resource.ecs.task_definition import EcsTaskDefinition
 from phidata.aws.resource.eks.cluster import EksCluster
 from phidata.aws.resource.ecs.service import EcsService
 from phidata.aws.resource.eks.fargate_profile import EksFargateProfile
 from phidata.aws.resource.eks.node_group import EksNodeGroup
 from phidata.aws.resource.eks.kubeconfig import EksKubeconfig
+from phidata.aws.resource.elb.load_balancer import LoadBalancer
+from phidata.aws.resource.elb.target_group import TargetGroup
+from phidata.aws.resource.elb.listener import Listener
 from phidata.aws.resource.iam.role import IamRole
 from phidata.aws.resource.iam.policy import IamPolicy
 from phidata.aws.resource.glue.crawler import GlueCrawler
 from phidata.aws.resource.s3.bucket import S3Bucket
 from phidata.aws.resource.emr.cluster import EmrCluster
 from phidata.aws.resource.rds.db_cluster import DbCluster
 from phidata.aws.resource.rds.db_instance import DbInstance
@@ -32,40 +36,48 @@
     EksFargateProfile,
     EksNodeGroup,
     EksKubeconfig,
     IamRole,
     IamPolicy,
     GlueCrawler,
     S3Bucket,
+    Subnet,
     DbSubnetGroup,
     DbCluster,
     DbInstance,
     CacheSubnetGroup,
     CacheCluster,
     EmrCluster,
     EcsCluster,
     EcsTaskDefinition,
     EcsService,
+    LoadBalancer,
+    TargetGroup,
+    Listener,
 ]
 
 # Use this as an ordered list to iterate over all Aws Resource Classes
 # This list is the order in which resources should be installed as well.
 AwsResourceTypeList: List[Type[AwsResource]] = [
+    Subnet,
     IamRole,
     IamPolicy,
     S3Bucket,
     EbsVolume,
     AcmCertificate,
     CloudFormationStack,
     GlueCrawler,
     DbSubnetGroup,
     DbCluster,
     DbInstance,
     CacheSubnetGroup,
     CacheCluster,
+    LoadBalancer,
+    TargetGroup,
+    Listener,
     EcsCluster,
     EcsTaskDefinition,
     EcsService,
     EksCluster,
     EksKubeconfig,
     EksFargateProfile,
     EksNodeGroup,
```

### Comparing `phidata-1.4.4/phidata/aws/resource/utils.py` & `phidata-1.5.0/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/s3/csv_dataset.py` & `phidata-1.5.0/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/s3/dataset.py` & `phidata-1.5.0/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/s3/dataset_base.py` & `phidata-1.5.0/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/s3/object.py` & `phidata-1.5.0/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/aws/worker.py` & `phidata-1.5.0/phidata/aws/worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import OrderedDict
 from typing import Dict, List, Optional
 
 from phidata.aws.args import AwsArgs
+from phidata.app.phidata_app import PhidataApp
 from phidata.aws.api_client import AwsApiClient
 from phidata.aws.resource.base import AwsResource
 from phidata.aws.resource.group import AwsResourceGroup
 from phidata.aws.resource.utils import (
     filter_and_flatten_aws_resource_groups,
 )
 from phidata.utils.cli_console import (
@@ -43,45 +44,122 @@
         app_filter: Optional[str] = None,
     ) -> Optional[Dict[str, AwsResourceGroup]]:
         """
         Build the AwsResourceGroups for the requested apps
         """
         logger.debug("-*- Initializing AwsResourceGroups")
 
+        aws_resource_groups: Optional[Dict[str, AwsResourceGroup]] = None
+
+        aws_apps: Optional[List[PhidataApp]] = self.aws_args.apps
         aws_rgs: Optional[List[AwsResourceGroup]] = self.aws_args.resources
 
-        num_rgs_to_build = len(aws_rgs) if aws_rgs is not None else 0
+        num_apps = len(aws_apps) if aws_apps is not None else 0
+        num_rgs = len(aws_rgs) if aws_rgs is not None else 0
+        num_rgs_to_build = num_apps + num_rgs
         num_rgs_built = 0
 
-        if aws_rgs is not None and isinstance(aws_rgs, list):
-            aws_resource_groups: Dict[str, AwsResourceGroup] = OrderedDict()
+        # Step 1: Convert each PhidataApp to AwsResourceGroup.
+        if aws_apps is not None and isinstance(aws_apps, list):
+            for app in aws_apps:
+                if app.args is None:
+                    logger.error("Args for App {} are None".format(app))
+                    num_rgs_built += 1
+                    continue
+
+                if not app.enabled:
+                    logger.debug(f"{app.name} disabled")
+                    num_rgs_built += 1
+                    continue
+
+                # skip apps not matching app_filter if provided
+                if app_filter is not None:
+                    if app_filter.lower() not in app.name:
+                        logger.debug(f"Skipping {app.name}")
+                        num_rgs_built += 1
+                        continue
+
+                logger.debug("-*- App: {}".format(app.name))
 
+                ######################################################################
+                # NOTE: VERY IMPORTANT TO GET RIGHT
+                # Pass down parameters from K8sArgs -> PhidataApp
+                # The K8sConfig inherits these params from the WorkspaceConfig
+                # 1. Pass down the paths from the WorkspaceConfig
+                # 2. Pass down k8s_env
+                # 3. Pass down common cloud configuration. eg: aws_region, aws_profile
+                # This should match phidata.infra.prep_infra_config.prep_infra_config()
+                ######################################################################
+
+                # -*- Path parameters
+                app.scripts_dir = self.aws_args.scripts_dir
+                app.storage_dir = self.aws_args.storage_dir
+                app.meta_dir = self.aws_args.meta_dir
+                app.products_dir = self.aws_args.products_dir
+                app.notebooks_dir = self.aws_args.notebooks_dir
+                app.workflows_dir = self.aws_args.workflows_dir
+                # The ws_root_path is the ROOT directory for the workspace
+                app.workspace_root_path = self.aws_args.workspace_root_path
+                app.workspace_config_dir = self.aws_args.workspace_config_dir
+                app.workspace_config_file_path = (
+                    self.aws_args.workspace_config_file_path
+                )
+
+                # -*- AWS parameters
+                # only update the params if they are not available on the app.
+                # so we can prefer the app param if provided
+                if app.aws_region is None and self.aws_args.aws_region is not None:
+                    app.aws_region = self.aws_args.aws_region
+                if app.aws_profile is None and self.aws_args.aws_profile is not None:
+                    app.aws_profile = self.aws_args.aws_profile
+                if (
+                    app.aws_config_file is None
+                    and self.aws_args.aws_config_file is not None
+                ):
+                    app.aws_config_file = self.aws_args.aws_config_file
+                if (
+                    app.aws_shared_credentials_file is None
+                    and self.aws_args.aws_shared_credentials_file is not None
+                ):
+                    app.aws_shared_credentials_file = (
+                        self.aws_args.aws_shared_credentials_file
+                    )
+
+                app_rgs: Optional[
+                    Dict[str, AwsResourceGroup]
+                ] = app.get_aws_resource_groups(aws_build_context=self.aws_args)
+                if app_rgs is not None:
+                    if aws_resource_groups is None:
+                        aws_resource_groups = OrderedDict()
+                    aws_resource_groups.update(app_rgs)
+                    num_rgs_built += 1
+
+        # Step 2: Add all AwsResourceGroups to the aws_resource_groups dict
+        if aws_rgs is not None and isinstance(aws_rgs, list):
             for rg in aws_rgs:
                 if not rg.enabled:
                     logger.debug(f"{rg.name} disabled")
                     num_rgs_built += 1
                     continue
 
                 # skip groups not matching app_filter if provided
                 if app_filter is not None:
                     if app_filter.lower() not in rg.name:
                         logger.debug(f"Skipping {rg.name}")
                         num_rgs_built += 1
                         continue
 
                 if isinstance(rg, AwsResourceGroup):
+                    if aws_resource_groups is None:
+                        aws_resource_groups = OrderedDict()
                     aws_resource_groups[rg.name] = rg
                     num_rgs_built += 1
 
-            logger.debug(
-                f"# AwsResourceGroups built: {num_rgs_built}/{num_rgs_to_build}"
-            )
-            return aws_resource_groups
-
-        return None
+        logger.debug(f"# AwsResourceGroups built: {num_rgs_built}/{num_rgs_to_build}")
+        return aws_resource_groups
 
     ######################################################
     ## Create Resources
     ######################################################
 
     def create_resources(
         self,
```

### Comparing `phidata-1.4.4/phidata/checks/check.py` & `phidata-1.5.0/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/checks/not_empty.py` & `phidata-1.5.0/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/constants.py` & `phidata-1.5.0/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/decorators/timer.py` & `phidata-1.5.0/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/decorators/validate_env.py` & `phidata-1.5.0/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/api_client.py` & `phidata-1.5.0/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/args.py` & `phidata-1.5.0/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/config.py` & `phidata-1.5.0/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/enums.py` & `phidata-1.5.0/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/manager.py` & `phidata-1.5.0/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/resource/base.py` & `phidata-1.5.0/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/resource/container.py` & `phidata-1.5.0/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/resource/group.py` & `phidata-1.5.0/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/resource/image.py` & `phidata-1.5.0/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/resource/network.py` & `phidata-1.5.0/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/resource/types.py` & `phidata-1.5.0/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/resource/utils.py` & `phidata-1.5.0/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/resource/volume.py` & `phidata-1.5.0/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/utils/container.py` & `phidata-1.5.0/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/docker/worker.py` & `phidata-1.5.0/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/infra/args.py` & `phidata-1.5.0/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/infra/config.py` & `phidata-1.5.0/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/infra/resource.py` & `phidata-1.5.0/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/api_client.py` & `phidata-1.5.0/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/args.py` & `phidata-1.5.0/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/config.py` & `phidata-1.5.0/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.5.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.5.0/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/apps/v1/deployment.py` & `phidata-1.5.0/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/common/port.py` & `phidata-1.5.0/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/core/v1/config_map.py` & `phidata-1.5.0/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/core/v1/container.py` & `phidata-1.5.0/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/core/v1/namespace.py` & `phidata-1.5.0/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-1.5.0/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-1.5.0/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/core/v1/secret.py` & `phidata-1.5.0/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/core/v1/service.py` & `phidata-1.5.0/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/core/v1/service_account.py` & `phidata-1.5.0/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/core/v1/volume.py` & `phidata-1.5.0/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-1.5.0/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/group.py` & `phidata-1.5.0/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/kubeconfig.py` & `phidata-1.5.0/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-1.5.0/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.5.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.5.0/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-1.5.0/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/enums/api_version.py` & `phidata-1.5.0/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/enums/kind.py` & `phidata-1.5.0/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/enums/manager_status.py` & `phidata-1.5.0/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/enums/pv.py` & `phidata-1.5.0/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/manager.py` & `phidata-1.5.0/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.5.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.5.0/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-1.5.0/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-1.5.0/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/base.py` & `phidata-1.5.0/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/config_map.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/container.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/namespace.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/pod.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/secret.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/service.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/service_account.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/toleration.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/volume.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-1.5.0/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/group.py` & `phidata-1.5.0/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/kubeconfig.py` & `phidata-1.5.0/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-1.5.0/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-1.5.0/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-1.5.0/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.5.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.5.0/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-1.5.0/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/types.py` & `phidata-1.5.0/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/resource/utils.py` & `phidata-1.5.0/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/utils/pod.py` & `phidata-1.5.0/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/k8s/worker.py` & `phidata-1.5.0/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/product/data_product.py` & `phidata-1.5.0/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/table/local/csv.py` & `phidata-1.5.0/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/table/local/local_table.py` & `phidata-1.5.0/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/table/local/parquet.py` & `phidata-1.5.0/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/table/s3/csv.py` & `phidata-1.5.0/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/table/s3/parquet.py` & `phidata-1.5.0/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/table/s3/s3_table.py` & `phidata-1.5.0/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/table/sql/postgres.py` & `phidata-1.5.0/phidata/table/sql/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 
 class PostgresTable(SqlTable):
     def __init__(
         self,
         # Table Name: required
         name: str,
-        # SQLModel for this table: required
-        data_model: Any,
+        # SQLModel for this table
+        data_model: Optional[Any] = None,
         # Database for the table (eg: "public" on postgres)
         database: Optional[str] = None,
         # -*- Table Connection
         # sqlalchemy.engine.(Engine or Connection)
         # Using SQLAlchemy makes it possible to use any DB supported by that library.
         # NOTE: db_engine is required but can be derived using other args.
         db_engine: Optional[Union[Engine, Connection]] = None,
```

### Comparing `phidata-1.4.4/phidata/table/sql/sql_table.py` & `phidata-1.5.0/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/aws/athena/run_query.py` & `phidata-1.5.0/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/aws/emr/create_cluster.py` & `phidata-1.5.0/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/aws/emr/delete_cluster.py` & `phidata-1.5.0/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/aws/glue/start_crawler.py` & `phidata-1.5.0/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/decorator.py` & `phidata-1.5.0/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/download/s3/to_file.py` & `phidata-1.5.0/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/download/url/to_file.py` & `phidata-1.5.0/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/download/url/to_s3.py` & `phidata-1.5.0/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/download/url/to_sql.py` & `phidata-1.5.0/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/plot/sql/query.py` & `phidata-1.5.0/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/python_task.py` & `phidata-1.5.0/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/run/sql/query.py` & `phidata-1.5.0/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/task.py` & `phidata-1.5.0/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/task_relatives.py` & `phidata-1.5.0/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/upload/file/to_s3.py` & `phidata-1.5.0/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/task/upload/file/to_sql.py` & `phidata-1.5.0/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/types/airflow.py` & `phidata-1.5.0/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/types/context.py` & `phidata-1.5.0/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/types/phidata_runtime.py` & `phidata-1.5.0/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/cli_console.py` & `phidata-1.5.0/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/common.py` & `phidata-1.5.0/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/compare.py` & `phidata-1.5.0/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/context.py` & `phidata-1.5.0/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/dttm.py` & `phidata-1.5.0/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/enums.py` & `phidata-1.5.0/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/env_file.py` & `phidata-1.5.0/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/env_var.py` & `phidata-1.5.0/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/filesystem.py` & `phidata-1.5.0/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/log.py` & `phidata-1.5.0/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/prep_infra_config.py` & `phidata-1.5.0/phidata/utils/prep_infra_config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/print_table.py` & `phidata-1.5.0/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/utils/workspace_path.py` & `phidata-1.5.0/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/workflow/decorator.py` & `phidata-1.5.0/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/workflow/workflow.py` & `phidata-1.5.0/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/workflow/workflow_relatives.py` & `phidata-1.5.0/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/workspace/config.py` & `phidata-1.5.0/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata/workspace/settings.py` & `phidata-1.5.0/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-1.4.4/phidata.egg-info/PKG-INFO` & `phidata-1.5.0/phidata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.4.4
+Version: 1.5.0
 Summary: Building blocks for Data Engineering
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://www.phidata.com
 Project-URL: documentation, https://www.docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -34,25 +34,26 @@
 <a href="https://github.com/phidatahq/phidata/actions/workflows/test.yml" target="_blank">
     <img src="https://github.com/phidatahq/phidata/actions/workflows/test.yml/badge.svg" alt="test-status">
 </a>
 </p>
 
 ---
 
-### **Phidata is a set of building blocks for data engineering**
+### **A python library of data engineering building blocks**
 
-It makes data tools plug-n-play so teams can deliver high-quality, reliable data products
+Python library of OSS data tools, use it deliver high-quality data products on the cheap.
+
+Honestly our goal is just to save money and run OSS on the cheap. So we run stuff locally using docker and in production on AWS. Because we're running OSS, we're OSS too with a MPL-2.0 license.
 
 ### How it works
 
-- You start with a codebase that has data tools pre-configured
-- Enable the Apps you need - Airflow, Superset, Jupyter, MLFlow
-- Build data products (tables, metrics) in a dev environment running locally on docker
-- Write pipelines in python or SQL. Use GPT-3 to generate boilerplate code
-- Run production on AWS. Infrastructure is also pre-configured
+- Phidata converts infrastructure, tools and data assets into python classes.
+- These classes are then put together to build data platforms, ML Apis, AI Apps, etc.
+- Run your platform locally for development using docker with `phi ws up dev:docker`
+- Run it in production on AWS: `phi ws up prod:aws`
 
 ### Advantages
 
 - Automate the grunt work
 - Recipes for common data tasks
 - Everything is version controlled: Infra, Apps and Workflows
 - Equal `dev` and `production` environments for data development at scale
```

#### html2text {}

```diff
@@ -1,54 +1,55 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.4.4 Summary: Building blocks for
+Metadata-Version: 2.1 Name: phidata Version: 1.5.0 Summary: Building blocks for
 Data Engineering Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
 documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
       [version] [pythonversion] [downloads] [build-status] [test-status]
---- ### **Phidata is a set of building blocks for data engineering** It makes
-data tools plug-n-play so teams can deliver high-quality, reliable data
-products ### How it works - You start with a codebase that has data tools pre-
-configured - Enable the Apps you need - Airflow, Superset, Jupyter, MLFlow -
-Build data products (tables, metrics) in a dev environment running locally on
-docker - Write pipelines in python or SQL. Use GPT-3 to generate boilerplate
-code - Run production on AWS. Infrastructure is also pre-configured ###
-Advantages - Automate the grunt work - Recipes for common data tasks -
-Everything is version controlled: Infra, Apps and Workflows - Equal `dev` and
-`production` environments for data development at scale - Multiple teams
-working together share code and define dependencies in a pythonic way -
-Formatting (`black`), linting (`ruff`), type-checking (`mypy`) and testing
-(`pytest`) included ### More Information: - **Website**: phidata.com -
-**Documentation**: https://docs.phidata.com - **Chat**: Discord --- ##
-Quickstart Let's build a data product using crypto data. Open the `Terminal`
-and follow along to download sample data and analyze it in a jupyter notebook.
-## Setup Create a python virtual environment ```bash python3 -m venv ~/.venvs/
-dpenv source ~/.venvs/dpenv/bin/activate ``` Install and initialize phidata
-```bash pip install phidata phi init ``` > If you encounter errors, try
-updating pip using `python -m pip install --upgrade pip` ## Create workspace
-**Workspace** is a directory containing the source code for your data platform.
-Run `phi ws init` to create a new workspace. Press Enter to select the default
-name (`data-platform`) and template (`aws-data-platform`) ```bash phi ws init
-``` cd into the new workspace directory ```bash cd data-platform ``` ## Run
-your first workflow The first step of building a data product is collecting the
-data. The `workflows/crypto/prices.py` file contains an example task for
-downloading crypto data locally to a CSV file. Run it using ```bash phi wf run
-crypto/prices ``` Note how we define the output as a `CsvTableLocal` object
-with partitions and pre-write checks ```python # Step 1: Define CsvTableLocal
-for storing data # Path: `storage/tables/crypto_prices` crypto_prices_local =
-CsvTableLocal( name="crypto_prices", database="crypto", partitions=["ds"],
-write_checks=[NotEmpty()], ) ``` Checkout `data-platform/storage/tables/
-crypto_prices` for the CSVs ## Run your first App **Docker** is a great tool
-for testing locally. Your workspace comes pre-configured with a jupyter
-notebook for analyzing data. Install [docker desktop](https://docs.docker.com/
-desktop/install/mac-install/) and after the engine is running, start the
-workspace using ```bash phi ws up ``` Press Enter to confirm. Verify the
-container is running using the docker dashboard or `docker ps` ```bash docker
-ps --format 'table {{.Names}}\t{{.Image}}' NAMES IMAGE jupyter-container
+--- ### **A python library of data engineering building blocks** Python library
+of OSS data tools, use it deliver high-quality data products on the cheap.
+Honestly our goal is just to save money and run OSS on the cheap. So we run
+stuff locally using docker and in production on AWS. Because we're running OSS,
+we're OSS too with a MPL-2.0 license. ### How it works - Phidata converts
+infrastructure, tools and data assets into python classes. - These classes are
+then put together to build data platforms, ML Apis, AI Apps, etc. - Run your
+platform locally for development using docker with `phi ws up dev:docker` - Run
+it in production on AWS: `phi ws up prod:aws` ### Advantages - Automate the
+grunt work - Recipes for common data tasks - Everything is version controlled:
+Infra, Apps and Workflows - Equal `dev` and `production` environments for data
+development at scale - Multiple teams working together share code and define
+dependencies in a pythonic way - Formatting (`black`), linting (`ruff`), type-
+checking (`mypy`) and testing (`pytest`) included ### More Information: -
+**Website**: phidata.com - **Documentation**: https://docs.phidata.com -
+**Chat**: Discord --- ## Quickstart Let's build a data product using crypto
+data. Open the `Terminal` and follow along to download sample data and analyze
+it in a jupyter notebook. ## Setup Create a python virtual environment ```bash
+python3 -m venv ~/.venvs/dpenv source ~/.venvs/dpenv/bin/activate ``` Install
+and initialize phidata ```bash pip install phidata phi init ``` > If you
+encounter errors, try updating pip using `python -m pip install --upgrade pip`
+## Create workspace **Workspace** is a directory containing the source code for
+your data platform. Run `phi ws init` to create a new workspace. Press Enter to
+select the default name (`data-platform`) and template (`aws-data-platform`)
+```bash phi ws init ``` cd into the new workspace directory ```bash cd data-
+platform ``` ## Run your first workflow The first step of building a data
+product is collecting the data. The `workflows/crypto/prices.py` file contains
+an example task for downloading crypto data locally to a CSV file. Run it using
+```bash phi wf run crypto/prices ``` Note how we define the output as a
+`CsvTableLocal` object with partitions and pre-write checks ```python # Step 1:
+Define CsvTableLocal for storing data # Path: `storage/tables/crypto_prices`
+crypto_prices_local = CsvTableLocal( name="crypto_prices", database="crypto",
+partitions=["ds"], write_checks=[NotEmpty()], ) ``` Checkout `data-platform/
+storage/tables/crypto_prices` for the CSVs ## Run your first App **Docker** is
+a great tool for testing locally. Your workspace comes pre-configured with a
+jupyter notebook for analyzing data. Install [docker desktop](https://
+docs.docker.com/desktop/install/mac-install/) and after the engine is running,
+start the workspace using ```bash phi ws up ``` Press Enter to confirm. Verify
+the container is running using the docker dashboard or `docker ps` ```bash
+docker ps --format 'table {{.Names}}\t{{.Image}}' NAMES IMAGE jupyter-container
 phidata/jupyter-aws-dp:dev ``` ## Jupyter UI Open [localhost:8888](http://
 localhost:8888) in a new tab to view the jupyterlab UI. Password: **admin**
 Navigate to `notebooks/examples/crypto_prices.ipynb` and run all cells. ##
 Shutdown Play around and then stop the workspace using ```bash phi ws down ```
 ## Next Checkout the [documentation](https://docs.phidata.com) for more
 information or chat with us on [discord](https://discord.gg/4MtYHHrgA8) ---
```

### Comparing `phidata-1.4.4/phidata.egg-info/SOURCES.txt` & `phidata-1.5.0/phidata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,17 @@
 phidata/app/prometheus/__init__.py
 phidata/app/prometheus/prometheus.py
 phidata/app/redis/__init__.py
 phidata/app/redis/redis.py
 phidata/app/server/__init__.py
 phidata/app/server/api_server.py
 phidata/app/server/app_server.py
+phidata/app/server/fastapi.py
 phidata/app/server/server_base.py
+phidata/app/server/streamlit.py
 phidata/app/spark/__init__.py
 phidata/app/spark/spark_base.py
 phidata/app/spark/spark_driver.py
 phidata/app/spark/spark_worker.py
 phidata/app/superset/__init__.py
 phidata/app/superset/superset_base.py
 phidata/app/superset/superset_init.py
@@ -126,14 +128,18 @@
 phidata/aws/resource/eks/cluster.py
 phidata/aws/resource/eks/fargate_profile.py
 phidata/aws/resource/eks/kubeconfig.py
 phidata/aws/resource/eks/node_group.py
 phidata/aws/resource/elasticache/__init__.py
 phidata/aws/resource/elasticache/cluster.py
 phidata/aws/resource/elasticache/subnet_group.py
+phidata/aws/resource/elb/__init__.py
+phidata/aws/resource/elb/listener.py
+phidata/aws/resource/elb/load_balancer.py
+phidata/aws/resource/elb/target_group.py
 phidata/aws/resource/emr/__init__.py
 phidata/aws/resource/emr/cluster.py
 phidata/aws/resource/glue/__init__.py
 phidata/aws/resource/glue/crawler.py
 phidata/aws/resource/iam/__init__.py
 phidata/aws/resource/iam/group.py
 phidata/aws/resource/iam/policy.py
```

### Comparing `phidata-1.4.4/pyproject.toml` & `phidata-1.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "phidata"
-version = "1.4.4"
+version = "1.5.0"
 description = "Building blocks for Data Engineering"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
   "boto3",
-  "phiterm==1.4.3",
+  "phiterm==1.5.0",
   "pyarrow",
   "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
```

