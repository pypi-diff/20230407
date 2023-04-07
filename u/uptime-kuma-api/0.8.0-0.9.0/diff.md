# Comparing `tmp/uptime_kuma_api-0.8.0.tar.gz` & `tmp/uptime_kuma_api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uptime_kuma_api-0.8.0.tar", last modified: Wed Jan  4 21:54:31 2023, max compression
+gzip compressed data, was "dist/uptime_kuma_api-0.9.0.tar", last modified: Tue Jan 17 20:39:01 2023, max compression
```

## Comparing `uptime_kuma_api-0.8.0.tar` & `uptime_kuma_api-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/
--rw-r--r--   0 lucas     (1000) users      (985)     1067 2022-08-02 11:14:16.000000 uptime_kuma_api-0.8.0/LICENSE
--rw-r--r--   0 lucas     (1000) users      (985)     3151 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/PKG-INFO
--rw-r--r--   0 lucas     (1000) users      (985)     1584 2023-01-04 21:54:03.000000 uptime_kuma_api-0.8.0/README.md
--rw-r--r--   0 lucas     (1000) users      (985)       38 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/setup.cfg
--rw-r--r--   0 lucas     (1000) users      (985)     1858 2022-09-07 09:55:07.000000 uptime_kuma_api-0.8.0/setup.py
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/
--rw-r--r--   0 lucas     (1000) users      (985)      541 2022-12-27 20:21:19.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/__init__.py
--rw-r--r--   0 lucas     (1000) users      (985)      142 2023-01-04 21:54:03.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/__version__.py
--rw-r--r--   0 lucas     (1000) users      (985)   114359 2023-01-01 12:28:18.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/api.py
--rw-r--r--   0 lucas     (1000) users      (985)      276 2022-12-16 20:42:20.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/auth_method.py
--rw-r--r--   0 lucas     (1000) users      (985)      169 2022-12-16 20:42:20.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/docker_type.py
--rw-r--r--   0 lucas     (1000) users      (985)    25248 2023-01-04 21:54:03.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/docstrings.py
--rw-r--r--   0 lucas     (1000) users      (985)      618 2022-12-27 13:49:50.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/event.py
--rw-r--r--   0 lucas     (1000) users      (985)      142 2022-12-16 20:42:20.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/exceptions.py
--rw-r--r--   0 lucas     (1000) users      (985)      324 2022-12-16 20:42:20.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/incident_style.py
--rw-r--r--   0 lucas     (1000) users      (985)      470 2022-12-28 14:09:19.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/maintenance_strategy.py
--rw-r--r--   0 lucas     (1000) users      (985)      705 2022-12-27 12:48:20.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/monitor_type.py
--rw-r--r--   0 lucas     (1000) users      (985)    10922 2023-01-04 21:54:03.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/notification_providers.py
--rw-r--r--   0 lucas     (1000) users      (985)      336 2022-12-27 13:47:50.000000 uptime_kuma_api-0.8.0/uptime_kuma_api/proxy_protocol.py
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/uptime_kuma_api.egg-info/
--rw-r--r--   0 lucas     (1000) users      (985)     3151 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/uptime_kuma_api.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1000) users      (985)      631 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/uptime_kuma_api.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1000) users      (985)        1 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/uptime_kuma_api.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1000) users      (985)       41 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/uptime_kuma_api.egg-info/requires.txt
--rw-r--r--   0 lucas     (1000) users      (985)       16 2023-01-04 21:54:31.000000 uptime_kuma_api-0.8.0/uptime_kuma_api.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/
+-rw-r--r--   0 lucas     (1000) users      (985)     1067 2023-01-17 20:03:37.000000 uptime_kuma_api-0.9.0/LICENSE
+-rw-r--r--   0 lucas     (1000) users      (985)     3151 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/PKG-INFO
+-rw-r--r--   0 lucas     (1000) users      (985)     1584 2023-01-17 19:52:46.000000 uptime_kuma_api-0.9.0/README.md
+-rw-r--r--   0 lucas     (1000) users      (985)       38 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/setup.cfg
+-rw-r--r--   0 lucas     (1000) users      (985)     1858 2022-09-07 09:55:07.000000 uptime_kuma_api-0.9.0/setup.py
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/
+-rw-r--r--   0 lucas     (1000) users      (985)      541 2022-12-27 20:21:19.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/__init__.py
+-rw-r--r--   0 lucas     (1000) users      (985)      142 2023-01-17 20:03:37.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/__version__.py
+-rw-r--r--   0 lucas     (1000) users      (985)   114396 2023-01-17 19:52:38.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/api.py
+-rw-r--r--   0 lucas     (1000) users      (985)      276 2022-12-16 20:42:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/auth_method.py
+-rw-r--r--   0 lucas     (1000) users      (985)      169 2022-12-16 20:42:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/docker_type.py
+-rw-r--r--   0 lucas     (1000) users      (985)    26782 2023-01-17 19:52:38.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/docstrings.py
+-rw-r--r--   0 lucas     (1000) users      (985)      618 2022-12-27 13:49:50.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/event.py
+-rw-r--r--   0 lucas     (1000) users      (985)      142 2022-12-16 20:42:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/exceptions.py
+-rw-r--r--   0 lucas     (1000) users      (985)      324 2022-12-16 20:42:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/incident_style.py
+-rw-r--r--   0 lucas     (1000) users      (985)      470 2022-12-28 14:09:19.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/maintenance_strategy.py
+-rw-r--r--   0 lucas     (1000) users      (985)      705 2022-12-27 12:48:20.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/monitor_type.py
+-rw-r--r--   0 lucas     (1000) users      (985)    11175 2023-01-17 19:52:38.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/notification_providers.py
+-rw-r--r--   0 lucas     (1000) users      (985)      336 2022-12-27 13:47:50.000000 uptime_kuma_api-0.9.0/uptime_kuma_api/proxy_protocol.py
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/
+-rw-r--r--   0 lucas     (1000) users      (985)     3151 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1000) users      (985)      631 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1000) users      (985)        1 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1000) users      (985)       41 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1000) users      (985)       16 2023-01-17 20:39:01.000000 uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/top_level.txt
```

### Comparing `uptime_kuma_api-0.8.0/LICENSE` & `uptime_kuma_api-0.9.0/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Lucas Held
+Copyright (c) 2023 Lucas Held
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `uptime_kuma_api-0.8.0/PKG-INFO` & `uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uptime_kuma_api
-Version: 0.8.0
+Name: uptime-kuma-api
+Version: 0.9.0
 Summary: A python wrapper for the Uptime Kuma WebSocket API
 Home-page: https://github.com/lucasheld/uptime-kuma-api
 Author: Lucas Held
 Author-email: lucasheld@hotmail.de
 License: MIT
 Description: # uptime-kuma-api
         
@@ -12,15 +12,15 @@
         ---
         uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
         
         This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
         
         Python version 3.6+ is required.
         
-        Supported Uptime Kuma versions: 1.17.0 - 1.19.3
+        Supported Uptime Kuma versions: 1.17.0 - 1.19.5
         
         Installation
         ---
         uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
         
         You can install it using pip:
```

### Comparing `uptime_kuma_api-0.8.0/README.md` & `uptime_kuma_api-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ---
 uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
 
 This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
 
 Python version 3.6+ is required.
 
-Supported Uptime Kuma versions: 1.17.0 - 1.19.3
+Supported Uptime Kuma versions: 1.17.0 - 1.19.5
 
 Installation
 ---
 uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
 
 You can install it using pip:
```

### Comparing `uptime_kuma_api-0.8.0/setup.py` & `uptime_kuma_api-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-0.8.0/uptime_kuma_api/__init__.py` & `uptime_kuma_api-0.9.0/uptime_kuma_api/__init__.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-0.8.0/uptime_kuma_api/api.py` & `uptime_kuma_api-0.9.0/uptime_kuma_api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     intervalDay: int = 1,
     weekdays: list = None,
     daysOfMonth: list = None,
     timeRange: list = None
 ) -> dict:
     if not dateRange:
         dateRange = [
-            datetime.date.today().strftime("%Y-%m-%d 00:00")
+            datetime.date.today().strftime("%Y-%m-%d 00:00:00")
         ]
     if not timeRange:
         timeRange = [
             {
                 "hours": 2,
                 "minutes": 0,
             }, {
@@ -334,14 +334,15 @@
         intervalDay=dict(
             min=1,
             max=3650,
         )
     )
     _check_argument_conditions(conditions, kwargs)
 
+
 class UptimeKumaApi(object):
     """This class is used to communicate with Uptime Kuma.
 
     Example::
 
     Import UptimeKumaApi from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
 
@@ -2153,15 +2154,15 @@
     ) -> dict:
         """
         Set settings.
 
         :param str, optional password: Password, defaults to None
         :param bool, optional checkUpdate: Show update if available, defaults to True
         :param bool, optional checkBeta: Also check beta release, defaults to False
-        :param int, optional keepDataPeriodDays: Keep monitor history data for X days., defaults to 180
+        :param int, optional keepDataPeriodDays: Keep monitor history data for X days. Set to 0 for infinite retention., defaults to 180
         :param str, optional serverTimezone: Server Timezone, defaults to ""
         :param str, optional entryPage: Entry Page, defaults to "dashboard"
         :param bool, optional searchEngineIndex: Search Engine Visibility, defaults to False
         :param str, optional primaryBaseURL: Primary Base URL, defaults to ""
         :param str, optional steamAPIKey: Steam API Key. For monitoring a Steam Game Server you need a Steam Web-API key., defaults to ""
         :param bool, optional dnsCache: True to enable DNS Cache. It may be not working in some IPv6 environments, disable it if you encounter any issues., defaults to False
         :param list, optional tlsExpiryNotifyDays: TLS Certificate Expiry. HTTPS Monitors trigger notification when TLS certificate expires in., defaults to None
```

### Comparing `uptime_kuma_api-0.8.0/uptime_kuma_api/docstrings.py` & `uptime_kuma_api-0.9.0/uptime_kuma_api/docstrings.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,17 +116,25 @@
         :param str, optional recieverId: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`
         :param str, optional pagerdutyAutoResolve: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`
         :param str, optional pagerdutyIntegrationUrl: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`
         :param str, optional pagerdutyPriority: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`
         :param str, optional pagerdutyIntegrationKey: Notification option for ``type`` :attr:`~.NotificationType.PAGERDUTY`
         :param str, optional promosmsLogin: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`
         :param str, optional promosmsPassword: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`
-        :param str, optional promosmsPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`
-        :param str, optional promosmsSMSType: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`
+        :param str, optional promosmsPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`. Phone number (for Polish recipient You can skip area codes).
+        :param str, optional promosmsSMSType: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`.
+        
+            Available values are:
+            
+            - ``0``: SMS FLASH - Message will automatically show on recipient device. Limited only to Polish recipients.
+            - ``1``: SMS ECO - cheap but slow and often overloaded. Limited only to Polish recipients.
+            - ``3``: SMS FULL - Premium tier of SMS, You can use your Sender Name (You need to register name first). Reliable for alerts.
+            - ``4``: SMS SPEED - Highest priority in system. Very quick and reliable but costly (about twice of SMS FULL price).
         :param str, optional promosmsSenderName: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`
+        :param bool, optional promosmsAllowLongSMS: Notification option for ``type`` :attr:`~.NotificationType.PROMOSMS`. Allow long SMS.
         :param str, optional pushbulletAccessToken: Notification option for ``type`` :attr:`~.NotificationType.PUSHBULLET`
         :param str, optional pushdeerKey: Notification option for ``type`` :attr:`~.NotificationType.PUSHDEER`
         :param str, optional pushoveruserkey: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
         :param str, optional pushoverapptoken: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
         :param str, optional pushoversounds: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
         :param str, optional pushoverpriority: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
         :param str, optional pushovertitle: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`
@@ -207,21 +215,42 @@
         :param str, optional ntfypassword: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
         :param str, optional ntfytopic: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
         :param int, optional ntfyPriority: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
         :param str, optional ntfyIcon: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
         :param str, optional ntfyserverurl: Notification option for ``type`` :attr:`~.NotificationType.NTFY`
         :param bool, optional smseagleEncoding: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. True to send messages in unicode.
         :param int, optional smseaglePriority: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Message priority (0-9, default = 0).
-        :param str, optional smseagleRecipientType: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Recipient type. Available values are "smseagle-to" (Phone number(s)), "smseagle-group" (Phonebook group name(s)) and "smseagle-contact" (Phonebook contact name(s)).
+        :param str, optional smseagleRecipientType: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Recipient type.
+        
+            Available values are:
+            
+            - ``smseagle-to``: Phone number(s)
+            - ``smseagle-group``: Phonebook group name(s)
+            - ``smseagle-contact``: Phonebook contact name(s)
         :param str, optional smseagleToken: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. API Access token.
         :param str, optional smseagleRecipient: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Recipient(s) (multiple must be separated with comma).
         :param str, optional smseagleUrl: Notification option for ``type`` :attr:`~.NotificationType.SMSEAGLE`. Your SMSEagle device URL.
         :param str, optional webhookUrl: Notification option for ``type`` :attr:`~.NotificationType.ZOHOCLIQ`
         :param str, optional kookGuildID: Notification option for ``type`` :attr:`~.NotificationType.KOOK`
         :param str, optional kookBotToken: Notification option for ``type`` :attr:`~.NotificationType.KOOK`
+        :param str, optional splunkAutoResolve: Notification option for ``type`` :attr:`~.NotificationType.SPLUNK`. Auto resolve or acknowledged.
+        
+            Available values are:
+            
+            - ``0``: do nothing
+            - ``ACKNOWLEDGEMENT``: auto acknowledged
+            - ``RECOVERY``: auto resolve
+        :param str, optional splunkSeverity: Notification option for ``type`` :attr:`~.NotificationType.SPLUNK`. Severity.
+        
+            Available values are:
+            
+            - ``INFO``
+            - ``WARNING``
+            - ``CRITICAL``
+        :param str, optional splunkRestURL: Notification option for ``type`` :attr:`~.NotificationType.SPLUNK`. Splunk Rest URL.
     """
 
 
 def proxy_docstring(mode) -> str:
     return f"""
         :param ProxyProtocol{", optional" if mode == "edit" else ""} protocol: Proxy Protocol
         :param str{", optional" if mode == "edit" else ""} host: Proxy Server
```

### Comparing `uptime_kuma_api-0.8.0/uptime_kuma_api/event.py` & `uptime_kuma_api-0.9.0/uptime_kuma_api/event.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-0.8.0/uptime_kuma_api/monitor_type.py` & `uptime_kuma_api-0.9.0/uptime_kuma_api/monitor_type.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-0.8.0/uptime_kuma_api/notification_providers.py` & `uptime_kuma_api-0.9.0/uptime_kuma_api/notification_providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,17 @@
 
     ZOHOCLIQ = "ZohoCliq"
     """ZohoCliq"""
 
     KOOK = "Kook"
     """Kook"""
 
+    SPLUNK = "Splunk"
+    """Splunk"""
+
 
 notification_provider_options = {
     NotificationType.ALERTA: dict(
         alertaApiEndpoint=dict(
             type="str"
         ),
         alertaApiKey=dict(type="str"),
@@ -232,14 +235,15 @@
     ),
     NotificationType.PROMOSMS: dict(
         promosmsLogin=dict(type="str"),
         promosmsPassword=dict(type="str"),
         promosmsPhoneNumber=dict(type="str"),
         promosmsSMSType=dict(type="str"),
         promosmsSenderName=dict(type="str"),
+        promosmsAllowLongSMS=dict(type="bool"),
     ),
     NotificationType.PUSHBULLET: dict(
         pushbulletAccessToken=dict(type="str"),
     ),
     NotificationType.PUSHDEER: dict(
         pushdeerKey=dict(type="str"),
     ),
@@ -386,14 +390,19 @@
     NotificationType.ZOHOCLIQ: dict(
         webhookUrl=dict(type="str")
     ),
     NotificationType.KOOK: dict(
         kookGuildID=dict(type="str"),
         kookBotToken=dict(type="str")
     ),
+    NotificationType.SPLUNK: dict(
+        splunkAutoResolve=dict(type="str"),
+        splunkSeverity=dict(type="str"),
+        splunkRestURL=dict(type="str")
+    )
 }
 
 notification_provider_conditions = dict(
     gotifyPriority=dict(
         min=0,
         max=10
     ),
```

### Comparing `uptime_kuma_api-0.8.0/uptime_kuma_api.egg-info/PKG-INFO` & `uptime_kuma_api-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uptime-kuma-api
-Version: 0.8.0
+Name: uptime_kuma_api
+Version: 0.9.0
 Summary: A python wrapper for the Uptime Kuma WebSocket API
 Home-page: https://github.com/lucasheld/uptime-kuma-api
 Author: Lucas Held
 Author-email: lucasheld@hotmail.de
 License: MIT
 Description: # uptime-kuma-api
         
@@ -12,15 +12,15 @@
         ---
         uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
         
         This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
         
         Python version 3.6+ is required.
         
-        Supported Uptime Kuma versions: 1.17.0 - 1.19.3
+        Supported Uptime Kuma versions: 1.17.0 - 1.19.5
         
         Installation
         ---
         uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
         
         You can install it using pip:
```

### Comparing `uptime_kuma_api-0.8.0/uptime_kuma_api.egg-info/SOURCES.txt` & `uptime_kuma_api-0.9.0/uptime_kuma_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

