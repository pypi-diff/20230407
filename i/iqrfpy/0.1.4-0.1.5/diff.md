# Comparing `tmp/iqrfpy-0.1.4.tar.gz` & `tmp/iqrfpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqrfpy-0.1.4.tar", last modified: Thu Apr  6 11:30:07 2023, max compression
+gzip compressed data, was "iqrfpy-0.1.5.tar", last modified: Fri Apr  7 16:12:51 2023, max compression
```

## Comparing `iqrfpy-0.1.4.tar` & `iqrfpy-0.1.5.tar`

### file list

```diff
@@ -1,193 +1,194 @@
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      309 2023-03-12 10:44:36.000000 iqrfpy-0.1.4/.editorconfig
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      113 2023-03-27 06:23:13.000000 iqrfpy-0.1.4/.gitignore
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      937 2023-03-22 19:16:00.000000 iqrfpy-0.1.4/.gitlab-ci.yml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      203 2023-03-22 19:16:00.000000 iqrfpy-0.1.4/.pylintrc
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2023-03-24 07:47:59.000000 iqrfpy-0.1.4/LICENSE
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      663 2023-03-25 07:04:37.000000 iqrfpy-0.1.4/Makefile
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        9 2023-03-07 12:47:49.000000 iqrfpy-0.1.4/README.md
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      671 2023-04-06 07:28:51.000000 iqrfpy-0.1.4/example.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.268975 iqrfpy-0.1.4/examples/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2081 2023-03-25 07:08:59.000000 iqrfpy-0.1.4/examples/response_factories.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.268975 iqrfpy-0.1.4/iqrfpy/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       44 2023-04-06 11:28:53.000000 iqrfpy-0.1.4/iqrfpy/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.268975 iqrfpy-0.1.4/iqrfpy/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5379 2023-03-24 10:38:31.000000 iqrfpy-0.1.4/iqrfpy/enums/Commands.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4646 2023-03-24 10:31:05.000000 iqrfpy-0.1.4/iqrfpy/enums/MessageTypes.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       90 2023-03-24 10:27:58.000000 iqrfpy-0.1.4/iqrfpy/enums/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      708 2023-03-24 10:49:19.000000 iqrfpy-0.1.4/iqrfpy/enums/peripherals.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.268975 iqrfpy-0.1.4/iqrfpy/messages/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       61 2023-03-24 07:14:54.000000 iqrfpy-0.1.4/iqrfpy/messages/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.268975 iqrfpy-0.1.4/iqrfpy/messages/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2263 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/IRequest.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-08 11:54:48.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.268975 iqrfpy-0.1.4/iqrfpy/messages/requests/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:27.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      988 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/AddrInfo.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2461 2023-04-02 10:26:37.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/AuthorizeBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1434 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/Backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2161 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/BondNode.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1008 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/BondedDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1010 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/ClearAllBonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1024 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1812 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/Discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1506 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/RemoveBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1668 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/Restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1429 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/SetDpaParams.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2006 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/SetHops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1912 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/SetMID.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4590 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/SmartConnect.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2023-03-16 15:28:35.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:18.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:26.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:21.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:40.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/generic/Raw.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/generic/RawHdp.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:21.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:15.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:11.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:37.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      949 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/node/Read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:41:43.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:14.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:31.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:31.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:27.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/requests/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:32.000000 iqrfpy-0.1.4/iqrfpy/messages/requests/uart/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     8146 2023-04-02 10:45:04.000000 iqrfpy-0.1.4/iqrfpy/messages/response_factory.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2202 2023-03-24 12:37:34.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/AsyncResponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1932 2023-03-24 12:38:06.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/Confirmation.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6896 2023-03-24 12:50:58.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/IResponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-17 10:12:06.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:04.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2144 2023-03-24 12:33:06.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/AddrInfo.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2229 2023-03-24 12:31:46.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/AuthorizeBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2075 2023-03-24 12:36:12.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/Backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2189 2023-03-24 12:33:30.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/BondNode.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2145 2023-03-24 12:33:06.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/BondedDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1808 2023-03-24 12:33:46.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/ClearAllBonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2201 2023-03-24 12:35:05.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2049 2023-03-24 12:35:05.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/Discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2053 2023-03-24 12:35:05.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/RemoveBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1683 2023-03-24 12:35:05.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/Restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2193 2023-03-24 12:35:05.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/SetDpaParams.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2241 2023-03-24 12:35:21.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/SetHops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1677 2023-03-24 12:35:48.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/SetMID.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2221 2023-03-24 12:35:48.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/SmartConnect.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      983 2023-03-24 07:27:46.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:58.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:01.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:56.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:43.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:27.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:23.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:19.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:14.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2492 2023-03-24 12:33:06.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/node/Read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:49.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:52.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:05.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:09.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:32.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/messages/responses/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:37.000000 iqrfpy-0.1.4/iqrfpy/messages/responses/uart/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/transports/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      300 2023-03-22 19:16:00.000000 iqrfpy-0.1.4/iqrfpy/transports/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2133 2023-04-06 09:43:24.000000 iqrfpy-0.1.4/iqrfpy/transports/itransport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2076 2023-03-24 09:57:48.000000 iqrfpy-0.1.4/iqrfpy/transports/mqtt_transport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3788 2023-03-24 09:57:48.000000 iqrfpy-0.1.4/iqrfpy/transports/udp_transport.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/iqrfpy/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       50 2023-03-24 11:33:36.000000 iqrfpy-0.1.4/iqrfpy/utils/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    19524 2023-03-25 06:51:06.000000 iqrfpy-0.1.4/iqrfpy/utils/common.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      343 2023-03-24 11:01:36.000000 iqrfpy-0.1.4/iqrfpy/utils/enums.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.268975 iqrfpy-0.1.4/iqrfpy.egg-info/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-06 11:30:07.000000 iqrfpy-0.1.4/iqrfpy.egg-info/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6091 2023-04-06 11:30:07.000000 iqrfpy-0.1.4/iqrfpy.egg-info/SOURCES.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2023-04-06 11:30:07.000000 iqrfpy-0.1.4/iqrfpy.egg-info/dependency_links.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2023-04-06 11:30:07.000000 iqrfpy-0.1.4/iqrfpy.egg-info/requires.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2023-04-06 11:30:07.000000 iqrfpy-0.1.4/iqrfpy.egg-info/top_level.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      138 2023-03-24 09:25:00.000000 iqrfpy-0.1.4/pyproject.toml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       85 2023-03-24 07:40:43.000000 iqrfpy-0.1.4/requirements.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1162 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/setup.cfg
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      102 2023-03-22 19:16:00.000000 iqrfpy-0.1.4/test_requirements.txt
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.272975 iqrfpy-0.1.4/tests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-07 12:49:34.000000 iqrfpy-0.1.4/tests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/tests/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1241 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/enums/Peripherals_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/tests/messages/
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/tests/messages/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1292 2023-03-18 09:19:32.000000 iqrfpy-0.1.4/tests/messages/requests/IRequest_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/tests/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      869 2023-03-18 09:24:49.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/AddrInfoRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4015 2023-04-02 10:26:13.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2194 2023-03-18 09:44:00.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/BackupRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3758 2023-03-18 09:50:37.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/BondNodeRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      903 2023-03-18 09:24:46.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/BondedDevicesRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      904 2023-03-18 09:57:38.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      925 2023-03-18 09:59:43.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3445 2023-03-18 10:11:35.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/DiscoveryRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2322 2023-03-18 10:17:19.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/RemoveBondRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4241 2023-03-18 10:45:18.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/RestoreRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2257 2023-03-18 10:55:51.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3672 2023-03-18 11:08:56.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/SetHopsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3511 2023-03-18 11:37:09.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/SetMIDRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11030 2023-03-19 07:20:25.000000 iqrfpy-0.1.4/tests/messages/requests/coordinator/SmartConnectRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4549 2023-03-25 07:00:13.000000 iqrfpy-0.1.4/tests/messages/response_factory_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/tests/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2161 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/AsyncResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1280 2023-03-24 12:50:58.000000 iqrfpy-0.1.4/tests/messages/responses/Confirmation_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/tests/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4324 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/AddrInfoResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4513 2023-04-02 10:41:56.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4764 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/BackupResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4390 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/BondNodeResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4211 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/BondedDevicesResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3154 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4343 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3784 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/DiscoveryResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3794 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/RemoveNodeResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3054 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/RestoreResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3930 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4490 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/SetHopsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3052 2023-03-24 10:31:41.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/SetMIDResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4486 2023-03-24 10:47:04.000000 iqrfpy-0.1.4/tests/messages/responses/coordinator/SmartConnectResponse_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-06 11:30:07.276975 iqrfpy-0.1.4/tests/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    15855 2023-03-25 06:53:49.000000 iqrfpy-0.1.4/tests/utils/Common_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       78 2023-03-22 19:16:00.000000 iqrfpy-0.1.4/tox.ini
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      309 2023-03-12 10:44:36.000000 iqrfpy-0.1.5/.editorconfig
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      113 2023-03-27 06:23:13.000000 iqrfpy-0.1.5/.gitignore
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      937 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/.gitlab-ci.yml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      203 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/.pylintrc
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2023-03-24 07:47:59.000000 iqrfpy-0.1.5/LICENSE
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      663 2023-03-25 07:04:37.000000 iqrfpy-0.1.5/Makefile
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        9 2023-03-07 12:47:49.000000 iqrfpy-0.1.5/README.md
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      671 2023-04-06 07:28:51.000000 iqrfpy-0.1.5/example.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.678399 iqrfpy-0.1.5/examples/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2081 2023-03-25 07:08:59.000000 iqrfpy-0.1.5/examples/response_factories.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.678399 iqrfpy-0.1.5/iqrfpy/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       44 2023-04-07 16:12:26.000000 iqrfpy-0.1.5/iqrfpy/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5379 2023-03-24 10:38:31.000000 iqrfpy-0.1.5/iqrfpy/enums/Commands.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4646 2023-03-24 10:31:05.000000 iqrfpy-0.1.5/iqrfpy/enums/MessageTypes.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       90 2023-03-24 10:27:58.000000 iqrfpy-0.1.5/iqrfpy/enums/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      708 2023-03-24 10:49:19.000000 iqrfpy-0.1.5/iqrfpy/enums/peripherals.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4173 2023-04-07 15:58:03.000000 iqrfpy-0.1.5/iqrfpy/exceptions.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       61 2023-03-24 07:14:54.000000 iqrfpy-0.1.5/iqrfpy/messages/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2370 2023-04-07 15:07:14.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/IRequest.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-08 11:54:48.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:27.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      988 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/AddrInfo.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2617 2023-04-07 15:11:45.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/AuthorizeBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1521 2023-04-07 15:13:22.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2268 2023-04-07 15:14:15.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/BondNode.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1008 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/BondedDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1010 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/ClearAllBonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1024 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1922 2023-04-07 15:14:51.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1593 2023-04-07 15:15:04.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/RemoveBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1778 2023-04-07 15:15:27.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1429 2023-04-07 15:16:51.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetDpaParams.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2116 2023-04-07 15:17:08.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetHops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2022 2023-04-07 15:17:22.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetMID.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4922 2023-04-07 15:18:37.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SmartConnect.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2023-03-16 15:28:35.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/dali/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:18.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/dali/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:26.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:21.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:40.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/generic/Raw.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/generic/RawHdp.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:21.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/io/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:15.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:11.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/ledr/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/light/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:37.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/light/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      949 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/node/Read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:41:43.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/node/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:14.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/os/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:31.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:31.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:27.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:32.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/uart/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     8216 2023-04-07 15:00:59.000000 iqrfpy-0.1.5/iqrfpy/messages/response_factory.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2202 2023-03-24 12:37:34.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/AsyncResponse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2074 2023-04-07 15:36:21.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/Confirmation.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3269 2023-04-07 15:34:42.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/IResponse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-17 10:12:06.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:04.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2238 2023-04-07 15:21:57.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/AddrInfo.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2323 2023-04-07 15:23:07.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/AuthorizeBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2169 2023-04-07 15:23:36.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2283 2023-04-07 15:24:18.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/BondNode.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2230 2023-04-07 15:23:59.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/BondedDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1902 2023-04-07 15:24:33.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/ClearAllBonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2286 2023-04-07 15:24:47.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2143 2023-04-07 15:25:03.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2147 2023-04-07 15:25:14.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/RemoveBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1777 2023-04-07 15:25:30.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2287 2023-04-07 15:26:28.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetDpaParams.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2335 2023-04-07 15:26:40.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetHops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1771 2023-04-07 15:26:51.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetMID.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2315 2023-04-07 15:27:01.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SmartConnect.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      983 2023-03-24 07:27:46.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/dali/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:58.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/dali/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:01.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:56.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:43.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:27.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/io/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:23.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:19.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/ledr/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/light/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:14.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/light/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2578 2023-04-07 15:29:01.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/node/Read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:49.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/node/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:52.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/os/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:05.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:09.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:32.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:37.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/uart/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/transports/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      300 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/iqrfpy/transports/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2133 2023-04-06 09:43:24.000000 iqrfpy-0.1.5/iqrfpy/transports/itransport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2076 2023-03-24 09:57:48.000000 iqrfpy-0.1.5/iqrfpy/transports/mqtt_transport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3788 2023-03-24 09:57:48.000000 iqrfpy-0.1.5/iqrfpy/transports/udp_transport.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       50 2023-03-24 11:33:36.000000 iqrfpy-0.1.5/iqrfpy/utils/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    20336 2023-04-07 15:58:34.000000 iqrfpy-0.1.5/iqrfpy/utils/common.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      343 2023-03-24 11:01:36.000000 iqrfpy-0.1.5/iqrfpy/utils/enums.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy.egg-info/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6112 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/requires.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/top_level.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      138 2023-03-24 09:25:00.000000 iqrfpy-0.1.5/pyproject.toml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       85 2023-03-24 07:40:43.000000 iqrfpy-0.1.5/requirements.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1162 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/setup.cfg
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      102 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/test_requirements.txt
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-07 12:49:34.000000 iqrfpy-0.1.5/tests/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1241 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/enums/Peripherals_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1292 2023-03-18 09:19:32.000000 iqrfpy-0.1.5/tests/messages/requests/IRequest_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/requests/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      869 2023-03-18 09:24:49.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/AddrInfoRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4015 2023-04-02 10:26:13.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2194 2023-03-18 09:44:00.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/BackupRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3758 2023-03-18 09:50:37.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/BondNodeRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      903 2023-03-18 09:24:46.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/BondedDevicesRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      904 2023-03-18 09:57:38.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      925 2023-03-18 09:59:43.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3445 2023-03-18 10:11:35.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/DiscoveryRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2322 2023-03-18 10:17:19.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/RemoveBondRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4241 2023-03-18 10:45:18.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/RestoreRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2257 2023-03-18 10:55:51.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3672 2023-03-18 11:08:56.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/SetHopsRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3511 2023-03-18 11:37:09.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/SetMIDRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11030 2023-03-19 07:20:25.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/SmartConnectRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4826 2023-04-07 16:08:13.000000 iqrfpy-0.1.5/tests/messages/response_factory_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2161 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/AsyncResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1280 2023-03-24 12:50:58.000000 iqrfpy-0.1.5/tests/messages/responses/Confirmation_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/responses/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4324 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/AddrInfoResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4513 2023-04-02 10:41:56.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4764 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/BackupResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4390 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/BondNodeResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4211 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/BondedDevicesResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3154 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4343 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3784 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/DiscoveryResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3794 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/RemoveNodeResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3054 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/RestoreResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3930 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4490 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/SetHopsResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3052 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/SetMIDResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4486 2023-03-24 10:47:04.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/SmartConnectResponse_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    16222 2023-04-07 16:02:36.000000 iqrfpy-0.1.5/tests/utils/Common_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       78 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/tox.ini
```

### Comparing `iqrfpy-0.1.4/.gitlab-ci.yml` & `iqrfpy-0.1.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/LICENSE` & `iqrfpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/Makefile` & `iqrfpy-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/PKG-INFO` & `iqrfpy-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/microrisc/libiqrf-python
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Keywords: iqrf,dpa
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iqrfpy-0.1.4/example.py` & `iqrfpy-0.1.5/example.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/examples/response_factories.py` & `iqrfpy-0.1.5/examples/response_factories.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/enums/Commands.py` & `iqrfpy-0.1.5/iqrfpy/enums/Commands.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/enums/MessageTypes.py` & `iqrfpy-0.1.5/iqrfpy/enums/MessageTypes.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/enums/peripherals.py` & `iqrfpy-0.1.5/iqrfpy/enums/peripherals.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/IRequest.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/IRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from abc import ABC, abstractmethod
 from typing import List, Optional, Union
 from uuid import uuid4
 from iqrfpy.utils.common import Common
 from iqrfpy.enums.Commands import Command
 from iqrfpy.enums.MessageTypes import MessageType
 from iqrfpy.enums.peripherals import Peripheral
+from iqrfpy.exceptions import RequestNadrInvalidError, RequestHwpidInvalidError
 
 __all__ = ['IRequest']
 
 
 @typechecked
 class IRequest(ABC):
     __slots__ = '_nadr', '_pnum', '_pcmd', '_m_type', '_hwpid', '_pdata', '_msgid', '_params'
@@ -26,17 +27,17 @@
         self._m_type: Optional[str] = m_type.value if m_type is not None else m_type
         self._msgid: str = msgid
         self._params: Optional[dict] = params if params is not None else {}
         self._validate_base()
 
     def _validate_base(self) -> None:
         if self._nadr < 0 or self._nadr > 239:
-            raise ValueError('NADR should be between 0 and 239.')
+            raise RequestNadrInvalidError('NADR should be between 0 and 239.')
         if self._hwpid < 0 or self._hwpid > 65535:
-            raise ValueError('HWPID should be between 0 and 65535.')
+            raise RequestHwpidInvalidError('HWPID should be between 0 and 65535.')
 
     @abstractmethod
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate_base()
         dpa: List[int] = [0, self._nadr, self._pnum, self._pcmd, self._hwpid & 0xFF, (self._hwpid >> 8) & 0xFF]
         if self._pdata is not None:
             dpa.extend(self._pdata)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/AddrInfo.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/AddrInfo.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/AuthorizeBond.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/AuthorizeBond.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import dataclass
 from typeguard import typechecked
 from uuid import uuid4
 from typing import List, Union
 from iqrfpy.enums.Commands import CoordinatorRequestCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['AuthorizeBondRequest', 'AuthorizeBondParams']
 
 
 @dataclass(slots=True)
@@ -34,22 +35,22 @@
             msgid=msgid
         ),
         self._nodes: List[AuthorizeBondParams] = nodes
         self._validate()
 
     def _validate(self) -> None:
         if len(self._nodes) == 0:
-            raise ValueError('At least one pair of requested address and MID is required.')
+            raise RequestParameterInvalidValueError('At least one pair of requested address and MID is required.')
         if len(self._nodes) > 11:
-            raise ValueError('Request can carry at most 11 pairs of address and MID.')
+            raise RequestParameterInvalidValueError('Request can carry at most 11 pairs of address and MID.')
         for node in self._nodes:
             if node.reqAddr < 1 or node.reqAddr > 239:
-                raise ValueError('Requested address value should be between 1 and 239.')
+                raise RequestParameterInvalidValueError('Requested address value should be between 1 and 239.')
             if node.mid < 0 or node.mid > 0xFFFFFFFF:
-                raise ValueError('MID value should be an unsigned 32bit integer.')
+                raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
 
     def set_nodes(self, nodes: List[AuthorizeBondParams]) -> None:
         self._nodes = nodes
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate()
         pdata = []
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/Backup.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetDpaParams.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 from __future__ import annotations
 from typeguard import typechecked
+from enum import IntEnum
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.Commands import CoordinatorRequestCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
-__all__ = ['BackupRequest']
+__all__ = ['SetDpaParamsRequest', 'DpaParam']
 
 
 @typechecked
-class BackupRequest(IRequest):
-    __slots__ = '_index'
+class DpaParam(IntEnum):
+    LAST_RSSI = 0
+    VOLTAGE = 1
+    SYSTEM = 2
+    USER_SPECIFIED = 3
 
-    def __init__(self, index: int = 0, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+
+@typechecked
+class SetDpaParamsRequest(IRequest):
+    __slots__ = '_dpa_param'
+
+    def __init__(self, dpa_param: DpaParam, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
             nadr=0,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorRequestCommands.BACKUP,
-            m_type=CoordinatorMessages.BACKUP,
+            pcmd=CoordinatorRequestCommands.SET_DPA_PARAMS,
+            m_type=CoordinatorMessages.SET_DPA_PARAMS,
             hwpid=hwpid,
             msgid=msgid
         )
-        self._index = index
-        self._validate()
-
-    def _validate(self) -> None:
-        if self._index < 0 or self._index > 255:
-            raise ValueError('Index value should be between 0 and 255.')
+        self._dpa_param = dpa_param
 
-    def set_index(self, index: int) -> None:
-        self._index = index
+    def set_dpa_param(self, dpa_param: DpaParam) -> None:
+        self._dpa_param = dpa_param
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
-        self._validate()
-        self._pdata = [self._index]
+        self._pdata = [self._dpa_param]
         return super().to_dpa(mutable=mutable)
 
     def to_json(self) -> dict:
-        self._validate()
-        self._params = {'index': self._index}
+        self._params = {'dpaParam': self._dpa_param}
         return super().to_json()
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/BondNode.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/BondNode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.Commands import CoordinatorRequestCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['BondNodeRequest']
 
 
 @typechecked
@@ -29,18 +30,18 @@
         self._bonding_test_retries = bonding_test_retries
         self._validate()
 
     def _validate(self) -> None:
         if self._req_addr == 240 and self._bonding_test_retries == 0:
             return
         if self._req_addr < 0 or self._req_addr > 239:
-            raise ValueError('Address value should be between 0 and 239. Value 240 is allowed in combination with \
-            bonding test retries value 0.')
+            raise RequestParameterInvalidValueError('Address value should be between 0 and 239. Value 240 is allowed \
+            combination with bonding test retries value 0.')
         if self._bonding_test_retries < 0 or self._bonding_test_retries > 255:
-            raise ValueError('Bonding test retries value should be between 0 and 255.')
+            raise RequestParameterInvalidValueError('Bonding test retries value should be between 0 and 255.')
 
     def set_req_addr(self, req_addr: int) -> None:
         self._req_addr = req_addr
 
     def set_bonding_test_retries(self, bonding_test_retries: int) -> None:
         self._bonding_test_retries = bonding_test_retries
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/BondedDevices.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/BondedDevices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/ClearAllBonds.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/ClearAllBonds.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/Discovery.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Discovery.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.Commands import CoordinatorRequestCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['DiscoveryRequest']
 
 
 @typechecked
@@ -26,17 +27,17 @@
         )
         self._tx_power = tx_power
         self._max_addr = max_addr
         self._validate()
 
     def _validate(self) -> None:
         if self._tx_power < 0 or self._tx_power > 7:
-            raise ValueError('TX power value should be between 0 and 7.')
+            raise RequestParameterInvalidValueError('TX power value should be between 0 and 7.')
         if self._max_addr < 0 or self._max_addr > 239:
-            raise ValueError('Max address value should be between 0 and 239.')
+            raise RequestParameterInvalidValueError('Max address value should be between 0 and 239.')
 
     def set_tx_power(self, tx_power: int) -> None:
         self._tx_power = tx_power
 
     def set_max_addr(self, max_addr: int) -> None:
         self._max_addr = max_addr
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/RemoveBond.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/RemoveBond.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.Commands import CoordinatorRequestCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['RemoveBondRequest']
 
 
 @typechecked
@@ -25,15 +26,15 @@
             msgid=msgid
         )
         self._bond_addr = bond_addr
         self._validate()
 
     def _validate(self) -> None:
         if self._bond_addr < 1 or self._bond_addr > 239:
-            raise ValueError('Bond address value should be between 1 and 239.')
+            raise RequestParameterInvalidValueError('Bond address value should be between 1 and 239.')
 
     def set_bond_addr(self, bond_addr: int) -> None:
         self._bond_addr = bond_addr
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate()
         self._pdata = [self._bond_addr]
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/Restore.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Restore.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import List, Union
 from iqrfpy.enums.Commands import CoordinatorRequestCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['RestoreRequest']
 
 
 @typechecked
@@ -25,17 +26,17 @@
             msgid=msgid
         )
         self._network_data = network_data
         self._validate()
 
     def _validate(self) -> None:
         if not Common.values_in_byte_range(self._network_data):
-            raise ValueError('Network data block values should be between 0 and 255.')
+            raise RequestParameterInvalidValueError('Network data block values should be between 0 and 255.')
         if len(self._network_data) != 49:
-            raise ValueError('Network data should be 49 blocks long.')
+            raise RequestParameterInvalidValueError('Network data should be 49 blocks long.')
 
     def set_network_data(self, network_data: List[int]) -> None:
         self._network_data = network_data
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate()
         self._pdata = self._network_data
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/SetDpaParams.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/node/Read.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,31 @@
 from __future__ import annotations
 from typeguard import typechecked
-from enum import IntEnum
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.Commands import NodeRequestCommands
+from iqrfpy.enums.MessageTypes import NodeMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
-__all__ = ['SetDpaParamsRequest', 'DpaParam']
+__all__ = ['ReadRequest']
 
 
 @typechecked
-class DpaParam(IntEnum):
-    LAST_RSSI = 0
-    VOLTAGE = 1
-    SYSTEM = 2
-    USER_SPECIFIED = 3
+class ReadRequest(IRequest):
 
-
-@typechecked
-class SetDpaParamsRequest(IRequest):
-    __slots__ = '_dpa_param'
-
-    def __init__(self, dpa_param: DpaParam, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, nadr: int, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorRequestCommands.SET_DPA_PARAMS,
-            m_type=CoordinatorMessages.SET_DPA_PARAMS,
+            nadr=nadr,
+            pnum=EmbedPeripherals.NODE,
+            pcmd=NodeRequestCommands.READ,
+            m_type=NodeMessages.READ,
             hwpid=hwpid,
             msgid=msgid
         )
-        self._dpa_param = dpa_param
-
-    def set_dpa_param(self, dpa_param: DpaParam) -> None:
-        self._dpa_param = dpa_param
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
-        self._pdata = [self._dpa_param]
         return super().to_dpa(mutable=mutable)
 
     def to_json(self) -> dict:
-        self._params = {'dpaParam': self._dpa_param}
         return super().to_json()
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/SetHops.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetHops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.Commands import CoordinatorRequestCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['SetHopsRequest']
 
 
 @typechecked
@@ -26,17 +27,17 @@
         )
         self._request_hops = request_hops
         self._response_hops = response_hops
         self._validate()
 
     def _validate(self) -> None:
         if (self._request_hops < 0 or self._request_hops > 239) and self._request_hops != 255:
-            raise ValueError('Request hops value should be between 0 and 239, or 255.')
+            raise RequestParameterInvalidValueError('Request hops value should be between 0 and 239, or 255.')
         if (self._response_hops < 1 or self._response_hops > 239) and self._response_hops != 255:
-            raise ValueError('Response hops value should be between 1 and 239, or 255.')
+            raise RequestParameterInvalidValueError('Response hops value should be between 1 and 239, or 255.')
 
     def set_request_hops(self, request_hops: int) -> None:
         self._request_hops = request_hops
 
     def set_response_hops(self, response_hops: int) -> None:
         self._response_hops = response_hops
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/SetMID.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetMID.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
 from iqrfpy.enums.Commands import CoordinatorRequestCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['SetMIDRequest']
 
 
 @typechecked
@@ -26,17 +27,17 @@
         )
         self._bond_addr = bond_addr
         self._mid = mid
         self._validate()
 
     def _validate(self) -> None:
         if self._bond_addr < 1 or self._bond_addr > 239:
-            raise ValueError('Bond address value should be between 1 and 239.')
+            raise RequestParameterInvalidValueError('Bond address value should be between 1 and 239.')
         if self._mid < 0 or self._mid > 0xFFFFFFFF:
-            raise ValueError('MID value should be an unsigned 32bit integer.')
+            raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
 
     def set_bond_addr(self, bond_addr: int) -> None:
         self._bond_addr = bond_addr
 
     def set_mid(self, mid: int) -> None:
         self._mid = mid
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/SmartConnect.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SmartConnect.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import List, Union
 from iqrfpy.enums.Commands import CoordinatorRequestCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['SmartConnectRequest']
 
 
 @typechecked
@@ -31,37 +32,38 @@
         self._mid = mid
         self._virtual_device_address = virtual_device_address
         self._validate()
 
     def _validate(self) -> None:
         if self._req_addr == Common.IQMESH_TEMP_ADDR:
             if self._bonding_test_retries != 0:
-                raise ValueError('Bonding test value must be zero if requested address is set to 254.')
+                raise RequestParameterInvalidValueError('Bonding test value must be zero if requested address \
+                set to 254.')
             if len(self._ibk) != 32:
-                raise ValueError('IBK should be a string of 32 hex characters.')
+                raise RequestParameterInvalidValueError('IBK should be a string of 32 hex characters.')
             # if set(self._ibk) - set('0'):
-            #    raise ValueError('IBK values must be zero if requested address is set to 254.')
+            #    raise RequestParameterInvalidValueError('IBK values must be zero if requested address is set to 254.')
             if self._mid != 0:
-                raise ValueError('MID value must be zero if requested address is set to 254.')
+                raise RequestParameterInvalidValueError('MID value must be zero if requested address is set to 254.')
             if self._virtual_device_address != 0:
-                raise ValueError('VRN value must be zero if requested address is set to 254.')
+                raise RequestParameterInvalidValueError('VRN value must be zero if requested address is set to 254.')
             return
         if self._req_addr < 1 or self._req_addr > 239:
-            raise ValueError('Requested address value should be between 1 and 239, or 254.')
+            raise RequestParameterInvalidValueError('Requested address value should be between 1 and 239, or 254.')
         if self._bonding_test_retries < 0 or self._bonding_test_retries > 255:
-            raise ValueError('Bonding test retries value should be between 0 and 255.')
+            raise RequestParameterInvalidValueError('Bonding test retries value should be between 0 and 255.')
         if len(self._ibk) != 32:
-            raise ValueError('IBK should be a string of 32 hex characters.')
+            raise RequestParameterInvalidValueError('IBK should be a string of 32 hex characters.')
         if not Common.is_hex_string(self._ibk):
-            raise ValueError('IBK string should only contain hexadecimal characters.')
+            raise RequestParameterInvalidValueError('IBK string should only contain hexadecimal characters.')
         if self._mid < 0 or self._mid > 0xFFFFFFFF:
-            raise ValueError('MID value should be an unsigned 32bit integer.')
+            raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
         if (self._virtual_device_address < 1 or self._virtual_device_address > 239) \
                 and self._virtual_device_address != 255:
-            raise ValueError('VRN value should be between 1 and 239, or 255.')
+            raise RequestParameterInvalidValueError('VRN value should be between 1 and 239, or 255.')
 
     def set_req_addr(self, req_addr: int) -> None:
         self._req_addr = req_addr
 
     def set_bonding_test_retries(self, bonding_test_retries: int) -> None:
         self._bonding_test_retries = bonding_test_retries
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/requests/coordinator/__init__.py` & `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/response_factory.py` & `iqrfpy-0.1.5/iqrfpy/messages/response_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
 from ..enums.MessageTypes import *
 from .responses.AsyncResponse import AsyncResponse
 from .responses.Confirmation import Confirmation
 from .responses.IResponse import IResponse
 from .responses.coordinator import *
 from ..utils.common import Common
+from ..exceptions import UnsupportedMessageTypeError
 
 __all__ = [
     'ResponseFactory',
     '_get_factory_from_mtype',
     'AsyncResponseFactory',
     'ConfirmationFactory',
     'CoordinatorAddrInfoFactory',
@@ -216,8 +217,8 @@
         CoordinatorMessages.SET_HOPS: CoordinatorSetHopsFactory(),
         CoordinatorMessages.SET_MID: CoordinatorSetMIDFactory(),
         CoordinatorMessages.SMART_CONNECT: CoordinatorSmartConnectFactory(),
     }
 
     if mtype in factories:
         return factories[mtype]
-    raise ValueError(f'Unknown or unsupported message type: {mtype}')
+    raise UnsupportedMessageTypeError(f'Unknown or unsupported message type: {mtype}')
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/AsyncResponse.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/AsyncResponse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/Confirmation.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/Confirmation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from typing import Optional
 from iqrfpy.enums.Commands import Command
 from iqrfpy.enums.peripherals import Peripheral
+from iqrfpy.exceptions import DpaConfirmationPacketError, DpaConfirmationPacketLengthError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.responses.IResponse import IResponseGetterMixin
 
 __all__ = ['Confirmation']
 
 
 class Confirmation(IResponseGetterMixin):
@@ -34,17 +35,17 @@
 
     def get_timeslot(self) -> int:
         return self._timeslot
 
     @staticmethod
     def from_dpa(dpa: bytes) -> Confirmation:
         if len(dpa) != 11:
-            raise ValueError('Invalid DPA confirmation packet length.')
+            raise DpaConfirmationPacketLengthError('Invalid DPA confirmation packet length.')
         if dpa[6] != 0xFF:
-            raise ValueError('Not a DPA confirmation packet.')
+            raise DpaConfirmationPacketError('Invalid DPA confirmation packet error code.')
         pnum = Common.pnum_from_dpa(dpa[2])
         pcmd = Common.request_pcmd_from_dpa(pnum, dpa[3])
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         result = {'requestHops': dpa[8], 'responseHops': dpa[10], 'timeslot': dpa[9]}
         return Confirmation(nadr=dpa[0], pnum=pnum, pcmd=pcmd, hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7],
                             result=result)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/AddrInfo.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/AddrInfo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
 __all__ = ['AddrInfoResponse']
 
 
 @typechecked
 class AddrInfoResponse(IResponseGetterMixin):
@@ -41,15 +42,15 @@
     def from_dpa(dpa: bytes) -> AddrInfoResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
             if len(dpa) != 10:
-                raise ValueError('Invalid dpa length')
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
             result = {'devNr': dpa[8], 'did': dpa[9]}
         return AddrInfoResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[7], result=result)
 
     @staticmethod
     def from_json(json: dict) -> AddrInfoResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/AuthorizeBond.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/RemoveBond.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,56 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
-__all__ = ['AuthorizeBondResponse']
+__all__ = ['RemoveBondResponse']
 
 
 @typechecked
-class AuthorizeBondResponse(IResponseGetterMixin):
-    __slots__ = '_bond_addr', '_dev_nr'
+class RemoveBondResponse(IResponseGetterMixin):
+    __slots__ = '_dev_nr'
 
     def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
             nadr=0,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.AUTHORIZE_BOND,
-            m_type=CoordinatorMessages.AUTHORIZE_BOND,
+            pcmd=CoordinatorResponseCommands.REMOVE_BOND,
+            m_type=CoordinatorMessages.REMOVE_BOND,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
         if rcode == 0:
-            self._bond_addr = result['bondAddr']
             self._dev_nr = result['devNr']
 
-    def get_bond_addr(self) -> int:
-        return self._bond_addr
-
     def get_dev_nr(self) -> int:
         return self._dev_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> AuthorizeBondResponse:
+    def from_dpa(dpa: bytes) -> RemoveBondResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
-            if len(dpa) != 10:
-                raise ValueError('Invalid dpa length')
-            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
-        return AuthorizeBondResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+            if len(dpa) != 9:
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
+            result = {'devNr': dpa[8]}
+        return RemoveBondResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
 
     @staticmethod
-    def from_json(json: dict) -> AuthorizeBondResponse:
+    def from_json(json: dict) -> RemoveBondResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
         result = Common.result_from_json(json) if rcode == 0 else None
-        return AuthorizeBondResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        return RemoveBondResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/Backup.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Backup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import List, Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
 __all__ = ['BackupResponse']
 
 
 @typechecked
 class BackupResponse(IResponseGetterMixin):
@@ -37,15 +38,15 @@
     def from_dpa(dpa: bytes) -> BackupResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
             if len(dpa) != 57:
-                raise ValueError('Invalid dpa length')
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
             result = {'networkData': list(dpa[8:])}
         return BackupResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
 
     @staticmethod
     def from_json(json: dict) -> BackupResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/BondNode.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/BondNode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
 __all__ = ['BondNodeResponse']
 
 
 @typechecked
 class BondNodeResponse(IResponseGetterMixin):
@@ -41,15 +42,15 @@
     def from_dpa(dpa: bytes) -> BondNodeResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
             if len(dpa) != 10:
-                raise ValueError('Invalid dpa length')
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
             result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
         return BondNodeResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
 
     @staticmethod
     def from_json(json: dict) -> BondNodeResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/BondedDevices.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/AuthorizeBond.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 from __future__ import annotations
 from typeguard import typechecked
-from typing import List, Optional
+from typing import Optional
+from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 
-__all__ = ['BondedDevicesResponse']
+__all__ = ['AuthorizeBondResponse']
 
 
 @typechecked
-class BondedDevicesResponse(IResponseGetterMixin):
-    __slots__ = '_bonded'
+class AuthorizeBondResponse(IResponseGetterMixin):
+    __slots__ = '_bond_addr', '_dev_nr'
 
     def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
             nadr=0,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.BONDED_DEVICES,
-            m_type=CoordinatorMessages.BONDED_DEVICES,
+            pcmd=CoordinatorResponseCommands.AUTHORIZE_BOND,
+            m_type=CoordinatorMessages.AUTHORIZE_BOND,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
         if rcode == 0:
-            self._bonded = result['bondedDevices']
+            self._bond_addr = result['bondAddr']
+            self._dev_nr = result['devNr']
+
+    def get_bond_addr(self) -> int:
+        return self._bond_addr
 
-    def get_bonded(self) -> List[int]:
-        return self._bonded
+    def get_dev_nr(self) -> int:
+        return self._dev_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> BondedDevicesResponse:
+    def from_dpa(dpa: bytes) -> AuthorizeBondResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
-            if len(dpa) != 40:
-                raise ValueError('Response packet incomplete.')
-            result = {'bondedDevices': Common.bitmap_to_nodes(list(dpa[8:]))}
-        return BondedDevicesResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[7], result=result)
+            if len(dpa) != 10:
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
+            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
+        return AuthorizeBondResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
 
     @staticmethod
-    def from_json(json: dict) -> BondedDevicesResponse:
+    def from_json(json: dict) -> AuthorizeBondResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
         result = Common.result_from_json(json) if rcode == 0 else None
-        return BondedDevicesResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        return AuthorizeBondResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/ClearAllBonds.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/ClearAllBonds.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
 __all__ = ['ClearAllBondsResponse']
 
 
 @typechecked
 class ClearAllBondsResponse(IResponseGetterMixin):
@@ -28,15 +29,15 @@
         )
 
     @staticmethod
     def from_dpa(dpa: bytes) -> ClearAllBondsResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         if len(dpa) != 8:
-            raise ValueError('Invalid dpa length')
+            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
         return ClearAllBondsResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=None)
 
     @staticmethod
     def from_json(json: dict) -> ClearAllBondsResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import List, Optional
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 
 __all__ = ['DiscoveredDevicesResponse']
 
 
 @typechecked
@@ -37,15 +38,15 @@
     def from_dpa(dpa: bytes) -> DiscoveredDevicesResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
             if len(dpa) != 40:
-                raise ValueError('Response packet incomplete.')
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
             result = {'discoveredDevices': Common.bitmap_to_nodes(list(dpa[8:]))}
         return DiscoveredDevicesResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[7], result=result)
 
     @staticmethod
     def from_json(json: dict) -> DiscoveredDevicesResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/Discovery.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Restore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,45 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
-__all__ = ['DiscoveryResponse']
+__all__ = ['RestoreResponse']
 
 
 @typechecked
-class DiscoveryResponse(IResponseGetterMixin):
-    __slots__ = '_disc_nr'
+class RestoreResponse(IResponseGetterMixin):
 
     def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
             nadr=0,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.DISCOVERY,
-            m_type=CoordinatorMessages.DISCOVERY,
+            pcmd=CoordinatorResponseCommands.RESTORE,
+            m_type=CoordinatorMessages.RESTORE,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
-            self._disc_nr = result['discNr']
-
-    def get_disc_nr(self) -> int:
-        return self._disc_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> DiscoveryResponse:
+    def from_dpa(dpa: bytes) -> RestoreResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
-        result = None
-        if rcode == 0:
-            if len(dpa) != 9:
-                raise ValueError('Invalid dpa length')
-            result = {'discNr': dpa[8]}
-        return DiscoveryResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+        if len(dpa) != 8:
+            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
+        return RestoreResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=None)
 
     @staticmethod
-    def from_json(json: dict) -> DiscoveryResponse:
+    def from_json(json: dict) -> RestoreResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
-        return DiscoveryResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        return RestoreResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/RemoveBond.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetMID.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,45 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
-__all__ = ['RemoveBondResponse']
+__all__ = ['SetMIDResponse']
 
 
 @typechecked
-class RemoveBondResponse(IResponseGetterMixin):
-    __slots__ = '_dev_nr'
+class SetMIDResponse(IResponseGetterMixin):
 
     def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
             nadr=0,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.REMOVE_BOND,
-            m_type=CoordinatorMessages.REMOVE_BOND,
+            pcmd=CoordinatorResponseCommands.SET_MID,
+            m_type=CoordinatorMessages.SET_MID,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
-            self._dev_nr = result['devNr']
-
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> RemoveBondResponse:
+    def from_dpa(dpa: bytes) -> SetMIDResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
-        result = None
-        if rcode == 0:
-            if len(dpa) != 9:
-                raise ValueError('Invalid dpa length')
-            result = {'devNr': dpa[8]}
-        return RemoveBondResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+        if len(dpa) != 8:
+            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
+        return SetMIDResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=None)
 
     @staticmethod
-    def from_json(json: dict) -> RemoveBondResponse:
+    def from_json(json: dict) -> SetMIDResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
-        return RemoveBondResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        return SetMIDResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/Restore.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SmartConnect.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
-__all__ = ['RestoreResponse']
+__all__ = ['SmartConnectResponse']
 
 
 @typechecked
-class RestoreResponse(IResponseGetterMixin):
+class SmartConnectResponse(IResponseGetterMixin):
+    __slots__ = '_bond_addr', '_dev_nr'
 
     def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
             nadr=0,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.RESTORE,
-            m_type=CoordinatorMessages.RESTORE,
+            pcmd=CoordinatorResponseCommands.SMART_CONNECT,
+            m_type=CoordinatorMessages.SMART_CONNECT,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
+        if rcode == 0:
+            self._bond_addr = result['bondAddr']
+            self._dev_nr = result['devNr']
+
+    def get_bond_addr(self) -> int:
+        return self._bond_addr
+
+    def get_dev_nr(self) -> int:
+        return self._dev_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> RestoreResponse:
+    def from_dpa(dpa: bytes) -> SmartConnectResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        if len(dpa) != 8:
-            raise ValueError('Invalid dpa length')
-        return RestoreResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=None)
+        rcode = dpa[6]
+        result = None
+        if rcode == 0:
+            if len(dpa) != 10:
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
+            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
+        return SmartConnectResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
 
     @staticmethod
-    def from_json(json: dict) -> RestoreResponse:
+    def from_json(json: dict) -> SmartConnectResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        return RestoreResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
+        result = Common.result_from_json(json) if rcode == 0 else None
+        return SmartConnectResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/SetDpaParams.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetDpaParams.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.messages.requests.coordinator.SetDpaParams import DpaParam
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
 __all__ = ['SetDpaParamsResponse']
 
 
 @typechecked
 class SetDpaParamsResponse(IResponseGetterMixin):
@@ -38,15 +39,15 @@
     def from_dpa(dpa: bytes) -> SetDpaParamsResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
             if len(dpa) != 9:
-                raise ValueError('Invalid dpa length')
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
             result = {'prevDpaParam': dpa[8]}
         return SetDpaParamsResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
 
     @staticmethod
     def from_json(json: dict) -> SetDpaParamsResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/SetHops.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetHops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 from iqrfpy.enums.Commands import CoordinatorResponseCommands
 from iqrfpy.enums.MessageTypes import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
 __all__ = ['SetHopsResponse']
 
 
 @typechecked
 class SetHopsResponse(IResponseGetterMixin):
@@ -41,15 +42,15 @@
     def from_dpa(dpa: bytes) -> SetHopsResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
             if len(dpa) != 10:
-                raise ValueError('Invalid dpa length')
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
             result = {'requestHops': dpa[8], 'responseHops': dpa[9]}
         return SetHopsResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
 
     @staticmethod
     def from_json(json: dict) -> SetHopsResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/SmartConnect.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/node/Read.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 from __future__ import annotations
-from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.Commands import NodeResponseCommands
+from iqrfpy.enums.MessageTypes import NodeMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
-__all__ = ['SmartConnectResponse']
+__all__ = ['ReadResponse']
 
 
-@typechecked
-class SmartConnectResponse(IResponseGetterMixin):
-    __slots__ = '_bond_addr', '_dev_nr'
+class ReadResponse(IResponseGetterMixin):
+    __slots__ = '_ntw_addr', '_ntw_vrn', '_ntw_zin', '_ntw_did', '_ntw_pvrn', '_ntw_useraddr', '_ntw_id', \
+        '_ntw_vrnfnz', '_ntw_cfg', '_flags'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.SMART_CONNECT,
-            m_type=CoordinatorMessages.SMART_CONNECT,
+            nadr=nadr,
+            pnum=EmbedPeripherals.NODE,
+            pcmd=NodeResponseCommands.READ,
+            m_type=NodeMessages.READ,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
         if rcode == 0:
-            self._bond_addr = result['bondAddr']
-            self._dev_nr = result['devNr']
-
-    def get_bond_addr(self) -> int:
-        return self._bond_addr
-
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
+            self._ntw_addr = result['ntwADDR']
+            self._ntw_vrn = result['ntwVRN']
+            self._ntw_zin = result['ntwZIN']
+            self._ntw_did = result['ntwDID']
+            self._ntw_pvrn = result['ntwPVRN']
+            self._ntw_useraddr = result['ntwUSERADDRESS']
+            self._ntw_id = result['ntwID']
+            self._ntw_vrnfnz = result['ntwVRNFNZ']
+            self._ntw_cfg = result['ntwCFG']
+            self._flags = result['flags']
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> SmartConnectResponse:
+    def from_dpa(dpa: bytes) -> ReadResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
             if len(dpa) != 10:
-                raise ValueError('Invalid dpa length')
-            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
-        return SmartConnectResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
+            result = {
+
+            }
+        return ReadResponse(nadr=dpa[0], hwpid=hwpid, rcode=rcode, dpa_value=dpa[7], result=result)
 
     @staticmethod
-    def from_json(json: dict) -> SmartConnectResponse:
+    def from_json(json: dict) -> ReadResponse:
+        nadr = Common.nadr_from_json(json)
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
         result = Common.result_from_json(json) if rcode == 0 else None
-        return SmartConnectResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        return ReadResponse(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, result=result)
```

### Comparing `iqrfpy-0.1.4/iqrfpy/messages/responses/coordinator/__init__.py` & `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/transports/itransport.py` & `iqrfpy-0.1.5/iqrfpy/transports/itransport.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/transports/mqtt_transport.py` & `iqrfpy-0.1.5/iqrfpy/transports/mqtt_transport.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/transports/udp_transport.py` & `iqrfpy-0.1.5/iqrfpy/transports/udp_transport.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/iqrfpy/utils/common.py` & `iqrfpy-0.1.5/iqrfpy/utils/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 import math
 from typing import List
 from typeguard import typechecked
 from iqrfpy.enums.Commands import *
 from iqrfpy.enums.MessageTypes import *
 from iqrfpy.enums.peripherals import *
+from iqrfpy.exceptions import InvalidPeripheralValueError, InvalidPeripheralCommandValueError, \
+    JsonMsgidMissingError, JsonMTypeMissingError, JsonNadrMissingError, JsonHwpidMissingError, JsonRCodeMissingError, \
+    JsonDpaValueMissingError, JsonResultMissingError, JsonStatusMissingError, UnsupportedMessageTypeError, \
+    UnsupportedPeripheralError, UnsupportedPeripheralCommandError
 
 
 @typechecked
 class Common:
     """
     Common class provides static methods for handling, modification and extraction of information
     from DPA and Daemon API JSON messages.
@@ -117,20 +121,20 @@
         Raises
         ------
         ValueError
             Raised if pnum value is not between 0 and 255
             Raised if pnum is not a recognized peripheral value
         """
         if pnum < 0 or pnum > 255:
-            raise ValueError('Argument value out of range 0-255.')
+            raise InvalidPeripheralValueError('Peripheral value out of range 0-255.')
         if EmbedPeripherals.has_value(pnum):
             return EmbedPeripherals(pnum)
         if Standards.has_value(pnum):
             return Standards(pnum)
-        raise ValueError('Unknown or unsupported peripheral.')
+        raise UnsupportedPeripheralError('Unknown or unsupported peripheral.')
 
     @staticmethod
     def request_pcmd_from_dpa(pnum: Peripheral, pcmd: int) -> Command:
         """
         Return request command based on DPA peripheral and command data byte.
 
         Parameters
@@ -150,17 +154,17 @@
         ValueError
             Raised if pcmd is a negative value
             Raised if pcmd is not a value between 0 and 127
             Raised if peripheral is not a recognized peripheral value
             Raised if pcmd is not a recognized peripheral command
         """
         if pcmd < 0:
-            raise ValueError('Negative argument values are not allowed.')
+            raise InvalidPeripheralCommandValueError('Negative peripheral command values are not allowed.')
         if pcmd > Common.PNUM_MAX:
-            raise ValueError('Argument value exceeds maximum allowed value of 127.')
+            raise InvalidPeripheralCommandValueError('Peripheral command value exceeds maximum allowed value of 127.')
         commands = None
         match pnum:
             case EmbedPeripherals.COORDINATOR:
                 commands = CoordinatorRequestCommands
             case EmbedPeripherals.NODE:
                 commands = NodeRequestCommands
             case EmbedPeripherals.OS:
@@ -190,15 +194,15 @@
             case Standards.SENSOR:
                 commands = SensorRequestCommands
             case Standards.LIGHT:
                 commands = LightRequestCommands
 
         if commands is not None and commands.has_value(pcmd):
             return commands(pcmd)
-        raise ValueError('Unknown or unsupported peripheral command.')
+        raise UnsupportedPeripheralCommandError('Unknown or unsupported peripheral command.')
 
     @staticmethod
     def response_pcmd_from_dpa(pnum: Peripheral, pcmd: int) -> Command:
         """
         Return response command based on DPA peripheral and command data byte.
 
         Parameters
@@ -218,17 +222,17 @@
         ValueError
             Raised if pcmd is a negative value
             Raised if pcmd is not a value between 128 and 255
             Raised if peripheral is not a recognized peripheral value
             Raised if pcmd is not a recognized peripheral command
         """
         if pcmd < 0:
-            raise ValueError('Negative argument values are not allowed.')
+            raise InvalidPeripheralCommandValueError('Negative peripheral command values are not allowed.')
         if pcmd <= Common.PNUM_MAX or pcmd > 255:
-            raise ValueError('Response command should be value between 128 and 255.')
+            raise InvalidPeripheralCommandValueError('Response peripheral command should be value between 128 and 255.')
         commands = None
         match pnum:
             case EmbedPeripherals.COORDINATOR:
                 commands = CoordinatorResponseCommands
             case EmbedPeripherals.NODE:
                 commands = NodeResponseCommands
             case EmbedPeripherals.OS:
@@ -258,15 +262,15 @@
             case Standards.SENSOR:
                 commands = SensorResponseCommands
             case Standards.LIGHT:
                 commands = LightResponseCommands
 
         if commands is not None and commands.has_value(pcmd):
             return commands(pcmd)
-        raise ValueError('Unknown or unsupported peripheral command.')
+        raise UnsupportedPeripheralCommandError('Unknown or unsupported peripheral command.')
 
     @staticmethod
     def mtype_from_dpa_response(pnum: int, pcmd: int) -> MessageType:
         per = Common.pnum_from_dpa(pnum)
         match per:
             case EmbedPeripherals.COORDINATOR:
                 match pcmd:
@@ -293,17 +297,19 @@
                     case CoordinatorResponseCommands.SET_HOPS:
                         return CoordinatorMessages.SET_HOPS
                     case CoordinatorResponseCommands.SET_MID:
                         return CoordinatorMessages.SET_MID
                     case CoordinatorResponseCommands.SMART_CONNECT:
                         return CoordinatorMessages.SMART_CONNECT
                     case _:
-                        raise ValueError(f'Unknown or unsupported coordinator peripheral command: {pcmd}.')
+                        raise UnsupportedPeripheralCommandError(
+                            f'Unknown or unsupported coordinator peripheral command: {pcmd}.'
+                        )
             case _:
-                raise ValueError(f'Unknown or unsupported peripheral: {pnum}.')
+                raise UnsupportedPeripheralError(f'Unknown or unsupported peripheral: {pnum}.')
 
     # json
 
     @staticmethod
     def msgid_from_json(json: dict) -> str:
         """
         Return response msgid from Daemon API JSON response.
@@ -322,15 +328,15 @@
         ------
         ValueError
             Raised if Daemon API response does not contain the msgId key
         """
         try:
             return json['data']['msgId']
         except KeyError as err:
-            raise ValueError(f'Object does not contain property {str(err)}') from err
+            raise JsonMsgidMissingError(f'Object does not contain property {str(err)}') from err
 
     @staticmethod
     def mtype_str_from_json(json: dict) -> str:
         """
         Return mtype from Daemon API JSON response.
 
         Parameters
@@ -347,15 +353,15 @@
         ------
         ValueError
             Raised if Daemon API response does not contain the mType key
         """
         try:
             return json['mType']
         except KeyError as err:
-            raise ValueError(f'Object does not contain property {str(err)}') from err
+            raise JsonMTypeMissingError(f'Object does not contain property {str(err)}') from err
 
     @staticmethod
     def nadr_from_json(json: dict) -> int:
         """
         Return response nadr from Daemon API JSON response.
 
         Parameters
@@ -367,15 +373,15 @@
         ------
         ValueError
             Raised if Daemon API response does not contain the nAdr key
         """
         try:
             return json['data']['rsp']['nAdr']
         except KeyError as err:
-            raise ValueError(f'Object does not contain property {str(err)}') from err
+            raise JsonNadrMissingError(f'Object does not contain property {str(err)}') from err
 
     @staticmethod
     def hwpid_from_json(json: dict) -> int:
         """
         Return response hwpid from Daemon API JSON response.
 
         Parameters
@@ -387,15 +393,15 @@
         ------
         ValueError
             Raised if Daemon API response does not contain the hwpId key
         """
         try:
             return json['data']['rsp']['hwpId']
         except KeyError as err:
-            raise ValueError(f'Object does not contain property {str(err)}') from err
+            raise JsonHwpidMissingError(f'Object does not contain property {str(err)}') from err
 
     @staticmethod
     def rcode_from_json(json: dict) -> int:
         """
         Return response rcode from Daemon API JSON response.
 
         Parameters
@@ -407,15 +413,15 @@
         ------
         ValueError
             Raised if Daemon API response does not contain the rcode key
         """
         try:
             return json['data']['rsp']['rCode']
         except KeyError as err:
-            raise ValueError(f'Object does not contain property {str(err)}') from err
+            raise JsonRCodeMissingError(f'Object does not contain property {str(err)}') from err
 
     @staticmethod
     def dpa_value_from_json(json: dict) -> int:
         """
         Return response DPA value from Daemon API JSON response.
 
         Parameters
@@ -427,15 +433,15 @@
         ------
         ValueError
             Raised if Daemon API response does not contain the dpaVal key
         """
         try:
             return json['data']['rsp']['dpaVal']
         except KeyError as err:
-            raise ValueError(f'Object does not contain property {str(err)}') from err
+            raise JsonDpaValueMissingError(f'Object does not contain property {str(err)}') from err
 
     @staticmethod
     def result_from_json(json: dict) -> dict:
         """
         Return response result from Daemon API JSON response.
 
         Parameters
@@ -447,15 +453,15 @@
         ------
         ValueError
             Raised if Daemon API response does not contain the result key
         """
         try:
             return json['data']['rsp']['result']
         except KeyError as err:
-            raise ValueError(f'Object does not contain property {str(err)}') from err
+            raise JsonResultMissingError(f'Object does not contain property {str(err)}') from err
 
     @staticmethod
     def status_from_json(json: dict) -> int:
         """
         Return response status from Daemon API JSON response.
 
         Parameters
@@ -467,25 +473,25 @@
         ------
         ValueError
             Raised if Daemon API response does not contain the status key
         """
         try:
             return json['data']['status']
         except KeyError as err:
-            raise ValueError(f'Object does not contain property {str(err)}') from err
+            raise JsonStatusMissingError(f'Object does not contain property {str(err)}') from err
 
     @staticmethod
     def string_to_mtype(string: str):
         messages = [GenericMessages, ExplorationMessages, CoordinatorMessages, NodeMessages, OSMessages, EEPROMMessages,
                     EEEPROMMessages, RAMMessages, LEDRMessages, LEDGMessages, IOMessages, ThermometerMessages,
                     UartMessages, FrcMessages, DALIMessages, BinaryOutputMessages, SensorMessages, LightMessages]
         for item in messages:
             if item.has_value(string):
                 return item(string)
-        raise ValueError(f'Unknown or unsupported message type.')
+        raise UnsupportedMessageTypeError(f'Unknown or unsupported message type.')
 
     # general
 
     @staticmethod
     def bitmap_to_nodes(bitmap: List[int]) -> List[int]:
         """
         Convert node bitmap to list of nodes.
```

### Comparing `iqrfpy-0.1.4/iqrfpy.egg-info/PKG-INFO` & `iqrfpy-0.1.5/iqrfpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/microrisc/libiqrf-python
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Keywords: iqrf,dpa
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iqrfpy-0.1.4/iqrfpy.egg-info/SOURCES.txt` & `iqrfpy-0.1.5/iqrfpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 test_requirements.txt
 tox.ini
 examples/response_factories.py
 iqrfpy/__init__.py
+iqrfpy/exceptions.py
 iqrfpy.egg-info/PKG-INFO
 iqrfpy.egg-info/SOURCES.txt
 iqrfpy.egg-info/dependency_links.txt
 iqrfpy.egg-info/requires.txt
 iqrfpy.egg-info/top_level.txt
 iqrfpy/enums/Commands.py
 iqrfpy/enums/MessageTypes.py
```

### Comparing `iqrfpy-0.1.4/setup.cfg` & `iqrfpy-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/enums/Peripherals_test.py` & `iqrfpy-0.1.5/tests/enums/Peripherals_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/IRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/IRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/AddrInfoRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/AddrInfoRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/BackupRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/BackupRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/BondNodeRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/BondNodeRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/BondedDevicesRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/BondedDevicesRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/DiscoveryRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/DiscoveryRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/RemoveBondRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/RemoveBondRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/RestoreRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/RestoreRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/SetHopsRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/SetHopsRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/SetMIDRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/SetMIDRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/requests/coordinator/SmartConnectRequest_test.py` & `iqrfpy-0.1.5/tests/messages/requests/coordinator/SmartConnectRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/response_factory_test.py` & `iqrfpy-0.1.5/tests/messages/response_factory_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 from parameterized import parameterized
 from iqrfpy.enums.MessageTypes import *
+from iqrfpy.exceptions import JsonMsgidMissingError, JsonMTypeMissingError, UnsupportedMessageTypeError
 from iqrfpy.messages.response_factory import *
 from iqrfpy.messages.responses.AsyncResponse import AsyncResponse
 from iqrfpy.messages.responses.Confirmation import Confirmation
 from iqrfpy.messages.responses.coordinator import *
 
 
 class ResponseFactoryTestCase(unittest.TestCase):
@@ -111,14 +112,15 @@
             }
         }, SetHopsResponse]
     ])
     def test_response_from_json_ok(self, _, json, expected):
         self.assertIsInstance(ResponseFactory.get_response_from_json(json=json), expected)
 
     @parameterized.expand([
-        [{}],
-        [{'data': {'req': {}}}],
+        [{'data': {'req': {}}}, JsonMsgidMissingError],
+        [{'data': {'msgId': 'test'}}, JsonMTypeMissingError],
+        [{'mType': 'unsupported', 'data': {'msgId': 'test'}}, UnsupportedMessageTypeError],
     ])
-    def test_response_from_json_invalid(self, json):
-        with self.assertRaises(ValueError):
+    def test_response_from_json_invalid(self, json, exception):
+        with self.assertRaises(exception):
             ResponseFactory.get_response_from_json(json=json)
```

### Comparing `iqrfpy-0.1.4/tests/messages/responses/AsyncResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/AsyncResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/Confirmation_test.py` & `iqrfpy-0.1.5/tests/messages/responses/Confirmation_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/AddrInfoResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/AddrInfoResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/BackupResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/BackupResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/BondNodeResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/BondNodeResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/BondedDevicesResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/BondedDevicesResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/DiscoveryResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/DiscoveryResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/RemoveNodeResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/RemoveNodeResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/RestoreResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/RestoreResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/SetHopsResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/SetHopsResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/SetMIDResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/SetMIDResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/messages/responses/coordinator/SmartConnectResponse_test.py` & `iqrfpy-0.1.5/tests/messages/responses/coordinator/SmartConnectResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.4/tests/utils/Common_test.py` & `iqrfpy-0.1.5/tests/utils/Common_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from parameterized import parameterized
 import unittest
 from iqrfpy.utils.common import *
 from iqrfpy.enums.Commands import *
 from iqrfpy.enums.MessageTypes import *
 from iqrfpy.enums.peripherals import *
+from iqrfpy.exceptions import JsonMsgidMissingError, JsonDpaValueMissingError, JsonHwpidMissingError, \
+    JsonMTypeMissingError, JsonNadrMissingError, JsonRCodeMissingError, JsonResultMissingError, \
+    JsonStatusMissingError, UnsupportedMessageTypeError
 
 
 class CommonTestCase(unittest.TestCase):
 
     def setUp(self):
         self.request = {
             'mType': 'iqrfEmbedLedr_Set',
@@ -210,15 +213,15 @@
         )
 
     @parameterized.expand([
         [{}],
         [{'data': {'req': {}}}]
     ])
     def test_msgid_from_json_missing_key(self, value):
-        with self.assertRaises(ValueError):
+        with self.assertRaises(JsonMsgidMissingError):
             Common.msgid_from_json(value)
 
     # mtype_str_from_json tests
 
     def test_mtype_str_from_json_ok(self):
         self.assertEqual(
             Common.mtype_str_from_json(self.response),
@@ -226,15 +229,15 @@
         )
 
     @parameterized.expand([
         [{}],
         [{'data': {'req': {}}}]
     ])
     def test_mtype_str_from_json_missing_key(self, value):
-        with self.assertRaises(ValueError):
+        with self.assertRaises(JsonMTypeMissingError):
             Common.mtype_str_from_json(value)
 
     # nadr_from_json tests
 
     def test_nadr_from_json_ok(self):
         expected = 1
         self.assertEqual(
@@ -243,15 +246,15 @@
         )
 
     @parameterized.expand([
         [{}],
         [{'data': {'req': {}}}]
     ])
     def test_nadr_from_json_missing_key(self, value):
-        with self.assertRaises(ValueError):
+        with self.assertRaises(JsonNadrMissingError):
             Common.nadr_from_json(value)
 
     # hwpid_from_json tests
 
     def test_hwpid_from_json_ok(self):
         expected = 2
         self.assertEqual(
@@ -260,15 +263,15 @@
         )
 
     @parameterized.expand([
         [{}],
         [{'data': {'req': {}}}]
     ])
     def test_hwpid_from_json_missing_key(self, value):
-        with self.assertRaises(ValueError):
+        with self.assertRaises(JsonHwpidMissingError):
             Common.hwpid_from_json(value)
 
     # rcode_from_json tests
 
     def test_rcode_from_json_ok(self):
         expected = 0
         self.assertEqual(
@@ -277,15 +280,15 @@
         )
 
     @parameterized.expand([
         [{}],
         [{'data': {'req': {}}}]
     ])
     def test_rcode_from_json_missing_key(self, value):
-        with self.assertRaises(ValueError):
+        with self.assertRaises(JsonRCodeMissingError):
             Common.rcode_from_json(value)
 
     # dpa_value_from_json tests
 
     def test_dpa_value_from_json_ok(self):
         expected = 75
         self.assertEqual(
@@ -294,15 +297,15 @@
         )
 
     @parameterized.expand([
         [{}],
         [{'data': {'req': {}}}]
     ])
     def test_dpa_value_from_json_missing_key(self, value):
-        with self.assertRaises(ValueError):
+        with self.assertRaises(JsonDpaValueMissingError):
             Common.dpa_value_from_json(value)
 
     # result_from_json tests
 
     def test_result_from_json_ok(self):
         expected = {}
         self.assertEqual(
@@ -311,30 +314,30 @@
         )
 
     @parameterized.expand([
         [{}],
         [{'data': {'req': {}}}]
     ])
     def test_result_from_json_missing_key(self, value):
-        with self.assertRaises(ValueError):
+        with self.assertRaises(JsonResultMissingError):
             Common.result_from_json(value)
 
     def test_status_from_json_ok(self):
         expected = 0
         self.assertEqual(
             Common.status_from_json(self.response),
             expected
         )
 
     @parameterized.expand([
         [{}],
         [{'data': {'req': {}}}]
     ])
     def test_status_from_json_missing_key(self, value):
-        with self.assertRaises(ValueError):
+        with self.assertRaises(JsonStatusMissingError):
             Common.status_from_json(value)
 
     # string_to_mtype tests
 
     @parameterized.expand([
         ['Raw', 'iqrfRaw', GenericMessages.RAW],
         ['AddrInfo', 'iqrfEmbedCoordinator_AddrInfo', CoordinatorMessages.ADDR_INFO],
@@ -342,15 +345,15 @@
         ['LightEnumerate', 'iqrfLight_Enumerate', LightMessages.ENUMERATE]
     ])
     def test_string_to_mtype_ok(self, _, string, expected):
         self.assertEqual(Common.string_to_mtype(string), expected)
 
     @parameterized.expand(['test', 'unknown', 'iqrfEmbedCoordinator_Nonexistent'])
     def test_string_to_mtype_unknown(self, string):
-        with self.assertRaises(ValueError):
+        with self.assertRaises(UnsupportedMessageTypeError):
             Common.string_to_mtype(string)
 
     # bitmap_to_nodes tests
 
     @parameterized.expand([
         ['empty', [], []],
         ['single', [0x0e], [1, 2, 3]],
```

