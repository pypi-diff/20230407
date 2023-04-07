# Comparing `tmp/emmet-api-0.51.6.tar.gz` & `tmp/emmet-api-0.51.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.51.6.tar", last modified: Mon Mar 27 22:32:46 2023, max compression
+gzip compressed data, was "emmet-api-0.51.7.tar", last modified: Fri Apr  7 21:37:44 2023, max compression
```

## Comparing `emmet-api-0.51.6.tar` & `emmet-api-0.51.7.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-27 22:32:41.000000 emmet-api-0.51.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-27 22:32:46.815571 emmet-api-0.51.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-27 22:32:41.000000 emmet-api-0.51.6/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.787571 emmet-api-0.51.6/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/routes/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/routes/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/routes/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/routes/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.795571 emmet-api-0.51.6/emmet/api/routes/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.799571 emmet-api-0.51.6/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/tasks/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/mpcules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/mpcules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.803571 emmet-api-0.51.6/emmet/api/routes/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet/api/routes/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-27 22:32:41.000000 emmet-api-0.51.6/emmet/api/routes/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.807571 emmet-api-0.51.6/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-27 22:32:46.000000 emmet-api-0.51.6/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-03-27 22:32:46.000000 emmet-api-0.51.6/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 22:32:46.000000 emmet-api-0.51.6/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 22:32:46.000000 emmet-api-0.51.6/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-27 22:32:46.000000 emmet-api-0.51.6/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 22:32:46.000000 emmet-api-0.51.6/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-03-27 22:32:41.000000 emmet-api-0.51.6/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-03-27 22:32:41.000000 emmet-api-0.51.6/mpcule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-03-27 22:32:41.000000 emmet-api-0.51.6/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 22:32:46.819571 emmet-api-0.51.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-27 22:32:41.000000 emmet-api-0.51.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-27 22:32:41.000000 emmet-api-0.51.6/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/_general_store/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/chemenv/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.811571 emmet-api-0.51.6/tests/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/mpcules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/mpcules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/mpcules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/mpcules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/mpcules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/mpcules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/mpcules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/tasks/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/mpcules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/mpcules/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:46.815571 emmet-api-0.51.6/tests/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-27 22:32:41.000000 emmet-api-0.51.6/tests/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-07 21:37:40.000000 emmet-api-0.51.7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 21:37:44.140530 emmet-api-0.51.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-07 21:37:40.000000 emmet-api-0.51.7/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.112529 emmet-api-0.51.7/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.120529 emmet-api-0.51.7/emmet/api/routes/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/mpcules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/mpcules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/mpcules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/mpcules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/mpcules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/mpcules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/mpcules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.124529 emmet-api-0.51.7/emmet/api/routes/mpcules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/mpcules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/mpcules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/tasks/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/mpcules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/mpcules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/mpcules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.128529 emmet-api-0.51.7/emmet/api/routes/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.132530 emmet-api-0.51.7/emmet/api/routes/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.132530 emmet-api-0.51.7/emmet/api/routes/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.132530 emmet-api-0.51.7/emmet/api/routes/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.132530 emmet-api-0.51.7/emmet/api/routes/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-07 21:37:40.000000 emmet-api-0.51.7/emmet/api/routes/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.132530 emmet-api-0.51.7/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 21:37:43.000000 emmet-api-0.51.7/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-04-07 21:37:44.000000 emmet-api-0.51.7/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:37:43.000000 emmet-api-0.51.7/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:37:43.000000 emmet-api-0.51.7/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-07 21:37:43.000000 emmet-api-0.51.7/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 21:37:43.000000 emmet-api-0.51.7/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-07 21:37:40.000000 emmet-api-0.51.7/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-07 21:37:40.000000 emmet-api-0.51.7/mpcule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.132530 emmet-api-0.51.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-04-07 21:37:40.000000 emmet-api-0.51.7/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:37:44.140530 emmet-api-0.51.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-07 21:37:40.000000 emmet-api-0.51.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-07 21:37:40.000000 emmet-api-0.51.7/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.132530 emmet-api-0.51.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.132530 emmet-api-0.51.7/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.132530 emmet-api-0.51.7/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/_general_store/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/chemenv/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/mpcules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/mpcules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/mpcules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/mpcules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/mpcules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.136530 emmet-api-0.51.7/tests/mpcules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/mpcules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/tasks/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/mpcules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/mpcules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:44.140530 emmet-api-0.51.7/tests/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-07 21:37:40.000000 emmet-api-0.51.7/tests/xas/test_query_operators.py
```

### Comparing `emmet-api-0.51.6/Dockerfile` & `emmet-api-0.51.7/Dockerfile`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-FROM materialsproject/devops:python-3.916.5 as base
+FROM materialsproject/devops:python-3.1010.1 as base
+RUN apt-get update && apt-get install -y --no-install-recommends libopenblas-dev libjpeg62 && apt-get clean
 
 FROM base as builder
 RUN apt-get update && apt-get install -y --no-install-recommends gcc git g++ cmake make libsnappy-dev wget && apt-get clean
 ENV PATH /root/.local/bin:$PATH
 WORKDIR /emmet-api
 ENV PIP_FLAGS "--user --no-cache-dir --compile"
 COPY requirements/deployment.txt ./requirements.txt
@@ -13,15 +14,15 @@
 COPY setup.py .
 ARG API_VERSION
 RUN SETUPTOOLS_SCM_PRETEND_VERSION=${API_VERSION} pip install $PIP_FLAGS --no-deps .
 RUN wget -q https://raw.githubusercontent.com/vishnubob/wait-for-it/master/wait-for-it.sh && \
     chmod +x wait-for-it.sh && mv wait-for-it.sh /root/.local/bin/
 
 FROM base
-COPY --from=builder /root/.local/lib/python3.9/site-packages /root/.local/lib/python3.9/site-packages
+COPY --from=builder /root/.local/lib/python3.10/site-packages /root/.local/lib/python3.10/site-packages
 COPY --from=builder /root/.local/bin /root/.local/bin
 COPY --from=builder /usr/lib/x86_64-linux-gnu/libsnappy* /usr/lib/x86_64-linux-gnu/
 COPY --from=builder /emmet-api /emmet-api
 WORKDIR /emmet-api
 ARG VERSION
 ENV PATH=/root/.local/bin:$PATH \
     PYTHONUNBUFFERED=1 \
@@ -34,14 +35,16 @@
     MAX_REQUESTS_JITTER=10000 \
     DD_TRACE_HOST=localhost:8126 \
     DD_SERVICE=next-gen-api \
     DD_ENV=prod \
     DD_VERSION=$VERSION
 
 COPY app.py .
+COPY material_resources.py .
+COPY mpcule_resources.py .
 COPY start.sh .
 RUN chmod +x start.sh
 
 LABEL com.datadoghq.ad.logs='[{"source": "gunicorn", "service": "next-gen-api"}]'
 
 EXPOSE 10001 20001
 CMD wait-for-it.sh $DD_TRACE_HOST -q -s -t 60 -- ./start.sh
```

### Comparing `emmet-api-0.51.6/emmet/api/core/api.py` & `emmet-api-0.51.7/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.51.7/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.51.7/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/core/documentation.py` & `emmet-api-0.51.7/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/core/global_header.py` & `emmet-api-0.51.7/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/core/settings.py` & `emmet-api-0.51.7/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.51.7/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.51.7/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.51.7/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.51.7/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/absorption/resources.py` & `emmet-api-0.51.7/emmet/api/routes/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/alloys/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/alloys/resources.py` & `emmet-api-0.51.7/emmet/api/routes/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/bonds/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/bonds/resources.py` & `emmet-api-0.51.7/emmet/api/routes/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/charge_density/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/charge_density/resources.py` & `emmet-api-0.51.7/emmet/api/routes/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/chemenv/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/chemenv/resources.py` & `emmet-api-0.51.7/emmet/api/routes/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/dielectric/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/dielectric/resources.py` & `emmet-api-0.51.7/emmet/api/routes/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/dois/resources.py` & `emmet-api-0.51.7/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/elasticity/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/elasticity/resources.py` & `emmet-api-0.51.7/emmet/api/routes/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/electrodes/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/electrodes/resources.py` & `emmet-api-0.51.7/emmet/api/routes/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/electrodes/utils.py` & `emmet-api-0.51.7/emmet/api/routes/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/electronic_structure/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/electronic_structure/resources.py` & `emmet-api-0.51.7/emmet/api/routes/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/eos/resources.py` & `emmet-api-0.51.7/emmet/api/routes/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/fermi/resources.py` & `emmet-api-0.51.7/emmet/api/routes/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/grain_boundary/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/grain_boundary/resources.py` & `emmet-api-0.51.7/emmet/api/routes/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/magnetism/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/magnetism/resources.py` & `emmet-api-0.51.7/emmet/api/routes/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/materials/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/materials/resources.py` & `emmet-api-0.51.7/emmet/api/routes/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/materials/utils.py` & `emmet-api-0.51.7/emmet/api/routes/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/molecules/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/molecules/resources.py` & `emmet-api-0.51.7/emmet/api/routes/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcomplete/query_operator.py` & `emmet-api-0.51.7/emmet/api/routes/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcomplete/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/association/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/bonds/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/bonds/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/molecules/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/molecules/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/orbitals/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/orbitals/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/partial_charges/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/partial_spins/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/redox/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/redox/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/summary/hint_scheme.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/summary/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/summary/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/tasks/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/tasks/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/thermo/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/thermo/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/utils.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/mpcules/vibrations/resources.py` & `emmet-api-0.51.7/emmet/api/routes/mpcules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/oxidation_states/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/oxidation_states/resources.py` & `emmet-api-0.51.7/emmet/api/routes/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/phonon/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/phonon/resources.py` & `emmet-api-0.51.7/emmet/api/routes/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/piezo/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/piezo/resources.py` & `emmet-api-0.51.7/emmet/api/routes/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/provenance/resources.py` & `emmet-api-0.51.7/emmet/api/routes/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/robocrys/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/robocrys/resources.py` & `emmet-api-0.51.7/emmet/api/routes/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/similarity/resources.py` & `emmet-api-0.51.7/emmet/api/routes/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/substrates/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/substrates/resources.py` & `emmet-api-0.51.7/emmet/api/routes/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/summary/hint_scheme.py` & `emmet-api-0.51.7/emmet/api/routes/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/summary/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/summary/resources.py` & `emmet-api-0.51.7/emmet/api/routes/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/surface_properties/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/surface_properties/resources.py` & `emmet-api-0.51.7/emmet/api/routes/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/synthesis/data_adaptor.py` & `emmet-api-0.51.7/emmet/api/routes/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/synthesis/data_adaptor_synpro.py` & `emmet-api-0.51.7/emmet/api/routes/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/synthesis/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/synthesis/resources.py` & `emmet-api-0.51.7/emmet/api/routes/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/synthesis/utils.py` & `emmet-api-0.51.7/emmet/api/routes/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/tasks/hint_scheme.py` & `emmet-api-0.51.7/emmet/api/routes/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/tasks/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/tasks/resources.py` & `emmet-api-0.51.7/emmet/api/routes/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/tasks/utils.py` & `emmet-api-0.51.7/emmet/api/routes/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/thermo/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/thermo/resources.py` & `emmet-api-0.51.7/emmet/api/routes/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/xas/query_operators.py` & `emmet-api-0.51.7/emmet/api/routes/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet/api/routes/xas/resources.py` & `emmet-api-0.51.7/emmet/api/routes/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.51.7/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/material_resources.py` & `emmet-api-0.51.7/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/mpcule_resources.py` & `emmet-api-0.51.7/mpcule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/requirements/deployment.txt` & `emmet-api-0.51.7/requirements/deployment.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=emmet/emmet-api/requirements/deployment.txt --resolver=backtracking emmet/emmet-api/setup.py python/requirements.txt
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
@@ -11,23 +11,23 @@
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -44,52 +44,52 @@
     # via matplotlib
 cryptography==40.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (emmet/emmet-api/setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.51.3
+emmet-core[all]==0.50.0
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via cattrs
 fastapi==0.95.0
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==20.1.0
     # via emmet-api (emmet/emmet-api/setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
-importlib-metadata==6.1.0
-    # via flask
-importlib-resources==5.12.0
-    # via matplotlib
+importlib-metadata==6.0.1
+    # via opentelemetry-api
 inflect==6.0.2
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -128,23 +128,23 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.30.10
+mp-api==0.30.11
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 numpy==1.21.6
     # via
     #   -r python/requirements.txt
     #   contourpy
@@ -155,33 +155,36 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
+    #   plotly
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   -r python/requirements.txt
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -204,15 +207,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -225,15 +228,15 @@
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
 requests==2.28.2
     # via
@@ -249,15 +252,15 @@
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.0
     # via boto3
 scikit-learn==1.2.2
     # via matminer
-scipy==1.9.1
+scipy==1.10.1
     # via
     #   -r python/requirements.txt
     #   pymatgen
     #   robocrys
     #   scikit-learn
 seekpath==2.0.1
     # via emmet-core
@@ -303,33 +306,32 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.5.0
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
-    #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (emmet/emmet-api/setup.py)
 werkzeug==2.2.3
     # via flask
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/macos-latest_py3.10.txt` & `emmet-api-0.51.7/requirements/ubuntu-latest_py3.8.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -44,16 +44,18 @@
     # via matplotlib
 cryptography==40.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
     # via
     #   emmet-api (setup.py)
@@ -64,28 +66,36 @@
     # via cattrs
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
+importlib-metadata==6.0.1
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
 inflect==6.0.2
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -130,15 +140,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 numpy==1.24.2
     # via
     #   contourpy
     #   maggma
@@ -148,32 +158,37 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
+    #   plotly
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-plotly==5.13.1
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+plotly==5.14.0
     # via pymatgen
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -196,15 +211,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -217,15 +232,15 @@
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
 requests==2.28.2
     # via
@@ -294,26 +309,37 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.5.0
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+    #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.2.3
     # via flask
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
+zipp==3.15.0
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.51.7/requirements/macos-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -56,16 +56,18 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
@@ -78,42 +80,50 @@
     # via
     #   cattrs
     #   pytest
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.6
+filelock==3.10.7
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.25.5
+griffe==0.26.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
+importlib-metadata==6.0.1
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via matplotlib
 inflect==6.0.2
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -188,15 +198,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.20.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2022.9.9
     # via
@@ -218,15 +228,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.7.0
     # via pre-commit
 numpy==1.24.2
     # via
@@ -238,40 +248,43 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
+    #   plotly
     #   pytest
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via emmet-api (setup.py)
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -304,15 +317,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymdown-extensions==9.10
     # via
     #   mkdocs-material
     #   mkdocstrings
@@ -336,15 +349,15 @@
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
@@ -429,27 +442,32 @@
 tornado==6.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.28.11.16
+types-requests==2.28.11.17
     # via emmet-api (setup.py)
-types-setuptools==67.6.0.5
+types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.9
+types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
+    #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -460,12 +478,18 @@
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.2.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
+zipp==3.15.0
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/macos-latest_py3.11.txt` & `emmet-api-0.51.7/requirements/macos-latest_py3.10.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.11.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -44,46 +44,52 @@
     # via matplotlib
 cryptography==40.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
+exceptiongroup==1.1.1
+    # via cattrs
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
+importlib-metadata==6.0.1
+    # via opentelemetry-api
 inflect==6.0.2
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -128,15 +134,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 numpy==1.24.2
     # via
     #   contourpy
     #   maggma
@@ -146,32 +152,35 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
+    #   plotly
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -194,15 +203,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -215,15 +224,15 @@
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
 requests==2.28.2
     # via
@@ -233,14 +242,16 @@
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
 ruamel-yaml==0.17.21
     # via
     #   pymatgen
     #   robocrys
+ruamel-yaml-clib==0.2.7
+    # via ruamel-yaml
 s3transfer==0.6.0
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
@@ -294,22 +305,28 @@
     #   pymatgen
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.2.3
     # via flask
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.51.7/requirements/macos-latest_py3.11_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -56,16 +56,18 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
@@ -74,42 +76,44 @@
     #   mp-api
 envier==0.4.0
     # via ddtrace
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.6
+filelock==3.10.7
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.25.5
+griffe==0.26.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
+importlib-metadata==6.0.1
+    # via opentelemetry-api
 inflect==6.0.2
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -184,15 +188,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.20.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2022.9.9
     # via
@@ -214,15 +218,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.7.0
     # via pre-commit
 numpy==1.24.2
     # via
@@ -234,40 +238,43 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
+    #   plotly
     #   pytest
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via emmet-api (setup.py)
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -300,15 +307,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymdown-extensions==9.10
     # via
     #   mkdocs-material
     #   mkdocstrings
@@ -332,15 +339,15 @@
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
@@ -418,27 +425,29 @@
 tornado==6.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.28.11.16
+types-requests==2.28.11.17
     # via emmet-api (setup.py)
-types-setuptools==67.6.0.5
+types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.9
+types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -449,12 +458,16 @@
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.2.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/macos-latest_py3.8.txt` & `emmet-api-0.51.7/requirements/macos-latest_py3.8.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -44,16 +44,18 @@
     # via matplotlib
 cryptography==40.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
     # via
     #   emmet-api (setup.py)
@@ -64,30 +66,32 @@
     # via cattrs
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
-importlib-metadata==6.1.0
-    # via flask
+importlib-metadata==6.0.1
+    # via
+    #   flask
+    #   opentelemetry-api
 importlib-resources==5.12.0
     # via
     #   jsonschema
     #   matplotlib
 inflect==6.0.2
     # via robocrys
 itsdangerous==2.1.2
@@ -136,15 +140,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 numpy==1.24.2
     # via
     #   contourpy
     #   maggma
@@ -154,34 +158,37 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
+    #   plotly
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -204,15 +211,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -225,15 +232,15 @@
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
 requests==2.28.2
     # via
@@ -309,24 +316,28 @@
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.2.3
     # via flask
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `emmet-api-0.51.6/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.51.7/requirements/macos-latest_py3.8_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -56,16 +56,18 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
@@ -78,47 +80,48 @@
     # via
     #   cattrs
     #   pytest
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.6
+filelock==3.10.7
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.25.5
+griffe==0.26.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
-importlib-metadata==6.1.0
+importlib-metadata==6.0.1
     # via
     #   flask
     #   markdown
     #   mkdocs
+    #   opentelemetry-api
 importlib-resources==5.12.0
     # via
     #   jsonschema
     #   matplotlib
 inflect==6.0.2
     # via robocrys
 iniconfig==2.0.0
@@ -197,15 +200,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.20.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2022.9.9
     # via
@@ -227,15 +230,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.7.0
     # via pre-commit
 numpy==1.24.2
     # via
@@ -247,42 +250,45 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
+    #   plotly
     #   pytest
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via emmet-api (setup.py)
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -315,15 +321,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymdown-extensions==9.10
     # via
     #   mkdocs-material
     #   mkdocstrings
@@ -347,15 +353,15 @@
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
@@ -440,30 +446,32 @@
 tornado==6.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.28.11.16
+types-requests==2.28.11.17
     # via emmet-api (setup.py)
-types-setuptools==67.6.0.5
+types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.9
+types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
     #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -474,14 +482,16 @@
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.2.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `emmet-api-0.51.6/requirements/macos-latest_py3.9.txt` & `emmet-api-0.51.7/requirements/macos-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -44,16 +44,18 @@
     # via matplotlib
 cryptography==40.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
     # via
     #   emmet-api (setup.py)
@@ -64,30 +66,32 @@
     # via cattrs
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
-importlib-metadata==6.1.0
-    # via flask
+importlib-metadata==6.0.1
+    # via
+    #   flask
+    #   opentelemetry-api
 importlib-resources==5.12.0
     # via matplotlib
 inflect==6.0.2
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -134,15 +138,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 numpy==1.24.2
     # via
     #   contourpy
     #   maggma
@@ -152,32 +156,35 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
+    #   plotly
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -200,15 +207,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -221,15 +228,15 @@
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
 requests==2.28.2
     # via
@@ -305,24 +312,28 @@
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.2.3
     # via flask
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `emmet-api-0.51.6/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.51.7/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -56,16 +56,18 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
@@ -78,49 +80,52 @@
     # via
     #   cattrs
     #   pytest
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.6
+filelock==3.10.7
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.25.5
+griffe==0.26.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
-importlib-metadata==6.1.0
+importlib-metadata==6.0.1
     # via
     #   flask
     #   markdown
     #   mkdocs
+    #   opentelemetry-api
 importlib-resources==5.12.0
-    # via matplotlib
+    # via
+    #   jsonschema
+    #   matplotlib
 inflect==6.0.2
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -195,15 +200,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.20.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2022.9.9
     # via
@@ -225,15 +230,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.7.0
     # via pre-commit
 numpy==1.24.2
     # via
@@ -245,40 +250,45 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
+    #   plotly
     #   pytest
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via emmet-api (setup.py)
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -311,15 +321,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymdown-extensions==9.10
     # via
     #   mkdocs-material
     #   mkdocstrings
@@ -343,15 +353,15 @@
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
@@ -436,30 +446,32 @@
 tornado==6.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.28.11.16
+types-requests==2.28.11.17
     # via emmet-api (setup.py)
-types-setuptools==67.6.0.5
+types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.9
+types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
     #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -470,14 +482,16 @@
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.2.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `emmet-api-0.51.6/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.51.7/requirements/ubuntu-latest_py3.10.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -44,16 +44,18 @@
     # via matplotlib
 cryptography==40.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
     # via
     #   emmet-api (setup.py)
@@ -64,28 +66,30 @@
     # via cattrs
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
+importlib-metadata==6.0.1
+    # via opentelemetry-api
 inflect==6.0.2
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -130,15 +134,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 numpy==1.24.2
     # via
     #   contourpy
     #   maggma
@@ -148,32 +152,35 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
+    #   plotly
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -196,15 +203,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -217,15 +224,15 @@
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
 requests==2.28.2
     # via
@@ -298,22 +305,28 @@
     #   pymatgen
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.2.3
     # via flask
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.51.7/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -56,16 +56,18 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
@@ -78,42 +80,50 @@
     # via
     #   cattrs
     #   pytest
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.6
+filelock==3.10.7
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.25.5
+griffe==0.26.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
+importlib-metadata==6.0.1
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via matplotlib
 inflect==6.0.2
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -188,15 +198,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.20.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2022.9.9
     # via
@@ -218,15 +228,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.7.0
     # via pre-commit
 numpy==1.24.2
     # via
@@ -238,40 +248,43 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
+    #   plotly
     #   pytest
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via emmet-api (setup.py)
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -304,15 +317,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymdown-extensions==9.10
     # via
     #   mkdocs-material
     #   mkdocstrings
@@ -336,15 +349,15 @@
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
@@ -429,27 +442,32 @@
 tornado==6.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.28.11.16
+types-requests==2.28.11.17
     # via emmet-api (setup.py)
-types-setuptools==67.6.0.5
+types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.9
+types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
+    #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -460,12 +478,18 @@
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.2.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
+zipp==3.15.0
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.51.7/requirements/ubuntu-latest_py3.11.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -44,16 +44,18 @@
     # via matplotlib
 cryptography==40.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
     # via
     #   emmet-api (setup.py)
@@ -62,28 +64,30 @@
     # via ddtrace
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
+importlib-metadata==6.0.1
+    # via opentelemetry-api
 inflect==6.0.2
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -128,15 +132,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 numpy==1.24.2
     # via
     #   contourpy
     #   maggma
@@ -146,32 +150,35 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
+    #   plotly
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -194,15 +201,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -215,15 +222,15 @@
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
 requests==2.28.2
     # via
@@ -294,22 +301,28 @@
     #   pymatgen
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.2.3
     # via flask
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.51.7/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -56,16 +56,18 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
@@ -74,42 +76,44 @@
     #   mp-api
 envier==0.4.0
     # via ddtrace
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.6
+filelock==3.10.7
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.25.5
+griffe==0.26.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
+importlib-metadata==6.0.1
+    # via opentelemetry-api
 inflect==6.0.2
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -184,15 +188,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.20.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2022.9.9
     # via
@@ -214,15 +218,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.7.0
     # via pre-commit
 numpy==1.24.2
     # via
@@ -234,40 +238,43 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
+    #   plotly
     #   pytest
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via emmet-api (setup.py)
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -300,15 +307,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymdown-extensions==9.10
     # via
     #   mkdocs-material
     #   mkdocstrings
@@ -332,15 +339,15 @@
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
@@ -418,27 +425,29 @@
 tornado==6.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.28.11.16
+types-requests==2.28.11.17
     # via emmet-api (setup.py)
-types-setuptools==67.6.0.5
+types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.9
+types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -449,12 +458,16 @@
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.2.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.51.7/requirements/macos-latest_py3.11.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt
+#    pip-compile --output-file=requirements/macos-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -44,54 +44,50 @@
     # via matplotlib
 cryptography==40.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.1
-    # via cattrs
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
-importlib-metadata==6.1.0
-    # via flask
-importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+importlib-metadata==6.0.1
+    # via opentelemetry-api
 inflect==6.0.2
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -136,15 +132,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 numpy==1.24.2
     # via
     #   contourpy
     #   maggma
@@ -154,34 +150,35 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
+    #   plotly
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -204,15 +201,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -225,15 +222,15 @@
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
 requests==2.28.2
     # via
@@ -243,16 +240,14 @@
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
 ruamel-yaml==0.17.21
     # via
     #   pymatgen
     #   robocrys
-ruamel-yaml-clib==0.2.7
-    # via ruamel-yaml
 s3transfer==0.6.0
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
@@ -302,33 +297,32 @@
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
 typing-extensions==4.5.0
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
-    #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.2.3
     # via flask
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.51.7/requirements/macos-latest_py3.10_extras.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -56,16 +56,18 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
@@ -78,51 +80,44 @@
     # via
     #   cattrs
     #   pytest
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.6
+filelock==3.10.7
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.25.5
+griffe==0.26.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
-importlib-metadata==6.1.0
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+importlib-metadata==6.0.1
+    # via opentelemetry-api
 inflect==6.0.2
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -197,15 +192,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.20.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2022.9.9
     # via
@@ -227,15 +222,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.7.0
     # via pre-commit
 numpy==1.24.2
     # via
@@ -247,42 +242,43 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
+    #   plotly
     #   pytest
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via emmet-api (setup.py)
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -315,15 +311,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymdown-extensions==9.10
     # via
     #   mkdocs-material
     #   mkdocstrings
@@ -347,15 +343,15 @@
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
@@ -440,30 +436,29 @@
 tornado==6.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.28.11.16
+types-requests==2.28.11.17
     # via emmet-api (setup.py)
-types-setuptools==67.6.0.5
+types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.9
+types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
-    #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -474,16 +469,16 @@
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.2.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.51.7/requirements/ubuntu-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -44,16 +44,18 @@
     # via matplotlib
 cryptography==40.0.1
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
     # via
     #   emmet-api (setup.py)
@@ -64,30 +66,32 @@
     # via cattrs
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
-importlib-metadata==6.1.0
-    # via flask
+importlib-metadata==6.0.1
+    # via
+    #   flask
+    #   opentelemetry-api
 importlib-resources==5.12.0
     # via matplotlib
 inflect==6.0.2
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -134,15 +138,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 numpy==1.24.2
     # via
     #   contourpy
     #   maggma
@@ -152,32 +156,35 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
+    #   plotly
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -200,15 +207,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -221,15 +228,15 @@
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   botocore
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
 requests==2.28.2
     # via
@@ -305,24 +312,28 @@
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.2.3
     # via flask
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
     # via
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `emmet-api-0.51.6/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.51.7/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
 anyio==3.6.2
     # via starlette
 attrs==22.2.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
     #   pytest
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.99
+boto3==1.26.106
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.99
+botocore==1.29.106
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.0
+bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via
@@ -56,16 +56,18 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.10.1
+ddtrace==1.11.0
     # via emmet-api (setup.py)
+deprecated==1.2.13
+    # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
 emmet-core[all]==0.50.0
@@ -78,49 +80,44 @@
     # via
     #   cattrs
     #   pytest
 fastapi==0.95.0
     # via
     #   emmet-api (setup.py)
     #   maggma
-filelock==3.10.6
+filelock==3.10.7
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
 flask==2.2.3
     # via mongogrant
-fonttools==4.39.2
+fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.25.5
+griffe==0.26.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.22
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
-importlib-metadata==6.1.0
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-importlib-resources==5.12.0
-    # via matplotlib
+importlib-metadata==6.0.1
+    # via opentelemetry-api
 inflect==6.0.2
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -195,15 +192,15 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.20.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==0.8.3
+mkdocstrings-python==0.9.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2022.9.9
     # via
@@ -225,15 +222,15 @@
     # via emmet-api (setup.py)
 mypy-extensions==1.0.0
     # via
     #   emmet-api (setup.py)
     #   mypy
 natsort==8.3.1
     # via mkdocs-awesome-pages-plugin
-networkx==3.0
+networkx==3.1
     # via
     #   pymatgen
     #   robocrys
 nodeenv==1.7.0
     # via pre-commit
 numpy==1.24.2
     # via
@@ -245,40 +242,43 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-orjson==3.8.8
+opentelemetry-api==1.17.0
+    # via ddtrace
+orjson==3.8.9
     # via maggma
 packaging==23.0
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
+    #   plotly
     #   pytest
 palettable==3.3.0
     # via pymatgen
-pandas==1.5.3
+pandas==2.0.0
     # via
     #   matminer
     #   pymatgen
 paramiko==3.1.0
     # via sshtunnel
-pillow==9.4.0
+pillow==9.5.0
     # via matplotlib
 platformdirs==3.2.0
     # via virtualenv
-plotly==5.13.1
+plotly==5.14.0
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.2.1
+pre-commit==3.2.2
     # via emmet-api (setup.py)
 protobuf==4.22.1
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
@@ -311,15 +311,15 @@
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
-pymatgen-analysis-alloys==0.0.5
+pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
 pymdown-extensions==9.10
     # via
     #   mkdocs-material
     #   mkdocstrings
@@ -343,15 +343,15 @@
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
     #   pandas
-pytz==2023.2
+pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via
     #   mkdocs
     #   mkdocs-markdownextradata-plugin
     #   pre-commit
     #   pybtex
@@ -436,30 +436,29 @@
 tornado==6.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.28.11.16
+types-requests==2.28.11.17
     # via emmet-api (setup.py)
-types-setuptools==67.6.0.5
+types-setuptools==67.6.0.7
     # via emmet-api (setup.py)
-types-urllib3==1.26.25.9
+types-urllib3==1.26.25.10
     # via types-requests
 typing-extensions==4.5.0
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
-    #   starlette
+tzdata==2023.3
+    # via pandas
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
@@ -470,16 +469,16 @@
     # via mkdocs
 wcmatch==8.4.1
     # via mkdocs-awesome-pages-plugin
 werkzeug==2.2.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
+wrapt==1.15.0
+    # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.51.6/setup.py` & `emmet-api-0.51.7/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/_consumer/test_query_operators.py` & `emmet-api-0.51.7/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/_general_store/test_query_operators.py` & `emmet-api-0.51.7/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/bonds/test_query_operators.py` & `emmet-api-0.51.7/tests/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/charge_density/test_query_operators.py` & `emmet-api-0.51.7/tests/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/chemenv/test_query_operators.py` & `emmet-api-0.51.7/tests/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/core/test_mapi.py` & `emmet-api-0.51.7/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/dielectric/test_query_operators.py` & `emmet-api-0.51.7/tests/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/elasticity/test_query_operators.py` & `emmet-api-0.51.7/tests/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/electrodes/test_query_operators.py` & `emmet-api-0.51.7/tests/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/electrodes/test_utils.py` & `emmet-api-0.51.7/tests/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/electronic_structure/test_query_operators.py` & `emmet-api-0.51.7/tests/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/grain_boundary/test_query_operators.py` & `emmet-api-0.51.7/tests/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/magnetism/test_query_operators.py` & `emmet-api-0.51.7/tests/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/materials/test_query_operators.py` & `emmet-api-0.51.7/tests/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/materials/test_utils.py` & `emmet-api-0.51.7/tests/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/molecules/test_query_operators.py` & `emmet-api-0.51.7/tests/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/mpcomplete/test_query_operators.py` & `emmet-api-0.51.7/tests/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/mpcules/bonds/test_query_operators.py` & `emmet-api-0.51.7/tests/mpcules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/mpcules/molecules/test_query_operators.py` & `emmet-api-0.51.7/tests/mpcules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/mpcules/orbitals/test_query_operators.py` & `emmet-api-0.51.7/tests/mpcules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/mpcules/redox/test_query_operators.py` & `emmet-api-0.51.7/tests/mpcules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/mpcules/summary/test_query_operators.py` & `emmet-api-0.51.7/tests/mpcules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/mpcules/tasks/test_query_operators.py` & `emmet-api-0.51.7/tests/mpcules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/mpcules/thermo/test_query_operators.py` & `emmet-api-0.51.7/tests/mpcules/thermo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/oxidation_states/test_query_operators.py` & `emmet-api-0.51.7/tests/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/piezo/test_query_operators.py` & `emmet-api-0.51.7/tests/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/robocrys/test_query_operators.py` & `emmet-api-0.51.7/tests/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/substrates/test_query_operators.py` & `emmet-api-0.51.7/tests/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/summary/test_query_operators.py` & `emmet-api-0.51.7/tests/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/surface_properties/test_query_operators.py` & `emmet-api-0.51.7/tests/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/synthesis/test_adaptor.py` & `emmet-api-0.51.7/tests/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/synthesis/test_adaptor_synpro.py` & `emmet-api-0.51.7/tests/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/synthesis/test_query_operators.py` & `emmet-api-0.51.7/tests/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/synthesis/test_utils.py` & `emmet-api-0.51.7/tests/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/tasks/test_query_operators.py` & `emmet-api-0.51.7/tests/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/tasks/test_utils.py` & `emmet-api-0.51.7/tests/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.6/tests/xas/test_query_operators.py` & `emmet-api-0.51.7/tests/xas/test_query_operators.py`

 * *Files identical despite different names*

