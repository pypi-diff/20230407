# Comparing `tmp/igwn-alert-0.2.3.tar.gz` & `tmp/igwn-alert-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igwn-alert-0.2.3.tar", last modified: Thu Sep 22 18:55:43 2022, max compression
+gzip compressed data, was "igwn-alert-0.3.0.tar", last modified: Fri Apr  7 19:31:54 2023, max compression
```

## Comparing `igwn-alert-0.2.3.tar` & `igwn-alert-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-09-22 18:55:43.554556 igwn-alert-0.2.3/
--rwxr-xr-x   0 alex      (1010) admin       (80)    35147 2022-07-18 11:00:03.000000 igwn-alert-0.2.3/COPYING
--rwxr-xr-x   0 alex      (1010) admin       (80)       67 2022-07-18 11:00:03.000000 igwn-alert-0.2.3/MANIFEST.in
--rw-r--r--   0 alex      (1010) admin       (80)     1440 2022-09-22 18:55:43.554614 igwn-alert-0.2.3/PKG-INFO
--rwxr-xr-x   0 alex      (1010) admin       (80)      412 2022-07-18 11:00:03.000000 igwn-alert-0.2.3/README.md
-drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-09-22 18:55:43.553414 igwn-alert-0.2.3/igwn_alert/
--rwxr-xr-x   0 alex      (1010) admin       (80)      826 2022-07-18 11:00:03.000000 igwn-alert-0.2.3/igwn_alert/__init__.py
--rwxr-xr-x   0 alex      (1010) admin       (80)    12792 2022-08-02 02:42:05.000000 igwn-alert-0.2.3/igwn_alert/client.py
-drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-09-22 18:55:43.554459 igwn-alert-0.2.3/igwn_alert/tests/
--rw-r--r--   0 alex      (1010) admin       (80)      770 2022-07-18 11:00:03.000000 igwn-alert-0.2.3/igwn_alert/tests/__init__.py
--rw-r--r--   0 alex      (1010) admin       (80)      730 2022-07-18 11:00:03.000000 igwn-alert-0.2.3/igwn_alert/tests/conftest.py
--rw-r--r--   0 alex      (1010) admin       (80)    16033 2022-09-22 18:44:53.000000 igwn-alert-0.2.3/igwn_alert/tests/test_igwn_alert.py
--rwxr-xr-x   0 alex      (1010) admin       (80)     4639 2022-09-22 18:55:16.000000 igwn-alert-0.2.3/igwn_alert/tool.py
--rwxr-xr-x   0 alex      (1010) admin       (80)       22 2022-09-22 18:44:53.000000 igwn-alert-0.2.3/igwn_alert/version.py
-drwxr-xr-x   0 alex      (1010) admin       (80)        0 2022-09-22 18:55:43.553968 igwn-alert-0.2.3/igwn_alert.egg-info/
--rw-r--r--   0 alex      (1010) admin       (80)     1440 2022-09-22 18:55:43.000000 igwn-alert-0.2.3/igwn_alert.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1010) admin       (80)      433 2022-09-22 18:55:43.000000 igwn-alert-0.2.3/igwn_alert.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1010) admin       (80)        1 2022-09-22 18:55:43.000000 igwn-alert-0.2.3/igwn_alert.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1010) admin       (80)       53 2022-09-22 18:55:43.000000 igwn-alert-0.2.3/igwn_alert.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1010) admin       (80)       63 2022-09-22 18:55:43.000000 igwn-alert-0.2.3/igwn_alert.egg-info/requires.txt
--rw-r--r--   0 alex      (1010) admin       (80)       11 2022-09-22 18:55:43.000000 igwn-alert-0.2.3/igwn_alert.egg-info/top_level.txt
--rwxr-xr-x   0 alex      (1010) admin       (80)      203 2022-09-22 18:55:43.554819 igwn-alert-0.2.3/setup.cfg
--rwxr-xr-x   0 alex      (1010) admin       (80)     2786 2022-09-22 18:44:53.000000 igwn-alert-0.2.3/setup.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2023-04-07 19:31:54.959182 igwn-alert-0.3.0/
+-rwxr-xr-x   0 alex      (1010) admin       (80)    35147 2022-07-18 11:00:03.000000 igwn-alert-0.3.0/COPYING
+-rwxr-xr-x   0 alex      (1010) admin       (80)       67 2022-07-18 11:00:03.000000 igwn-alert-0.3.0/MANIFEST.in
+-rw-r--r--   0 alex      (1010) admin       (80)     1421 2023-04-07 19:31:54.959246 igwn-alert-0.3.0/PKG-INFO
+-rwxr-xr-x   0 alex      (1010) admin       (80)      412 2022-07-18 11:00:03.000000 igwn-alert-0.3.0/README.md
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2023-04-07 19:31:54.957567 igwn-alert-0.3.0/igwn_alert/
+-rwxr-xr-x   0 alex      (1010) admin       (80)      826 2022-07-18 11:00:03.000000 igwn-alert-0.3.0/igwn_alert/__init__.py
+-rwxr-xr-x   0 alex      (1010) admin       (80)    13733 2023-02-02 20:45:38.000000 igwn-alert-0.3.0/igwn_alert/client.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2023-04-07 19:31:54.959066 igwn-alert-0.3.0/igwn_alert/tests/
+-rw-r--r--   0 alex      (1010) admin       (80)      770 2022-07-18 11:00:03.000000 igwn-alert-0.3.0/igwn_alert/tests/__init__.py
+-rw-r--r--   0 alex      (1010) admin       (80)      730 2022-07-18 11:00:03.000000 igwn-alert-0.3.0/igwn_alert/tests/conftest.py
+-rw-r--r--   0 alex      (1010) admin       (80)    16033 2023-04-07 19:26:54.000000 igwn-alert-0.3.0/igwn_alert/tests/test_igwn_alert.py
+-rwxr-xr-x   0 alex      (1010) admin       (80)     5257 2023-02-02 20:45:38.000000 igwn-alert-0.3.0/igwn_alert/tool.py
+-rwxr-xr-x   0 alex      (1010) admin       (80)       22 2023-04-07 19:26:54.000000 igwn-alert-0.3.0/igwn_alert/version.py
+drwxr-xr-x   0 alex      (1010) admin       (80)        0 2023-04-07 19:31:54.958401 igwn-alert-0.3.0/igwn_alert.egg-info/
+-rw-r--r--   0 alex      (1010) admin       (80)     1421 2023-04-07 19:31:54.000000 igwn-alert-0.3.0/igwn_alert.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1010) admin       (80)      433 2023-04-07 19:31:54.000000 igwn-alert-0.3.0/igwn_alert.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1010) admin       (80)        1 2023-04-07 19:31:54.000000 igwn-alert-0.3.0/igwn_alert.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1010) admin       (80)       52 2023-04-07 19:31:54.000000 igwn-alert-0.3.0/igwn_alert.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1010) admin       (80)      102 2023-04-07 19:31:54.000000 igwn-alert-0.3.0/igwn_alert.egg-info/requires.txt
+-rw-r--r--   0 alex      (1010) admin       (80)       11 2023-04-07 19:31:54.000000 igwn-alert-0.3.0/igwn_alert.egg-info/top_level.txt
+-rwxr-xr-x   0 alex      (1010) admin       (80)      203 2023-04-07 19:31:54.959497 igwn-alert-0.3.0/setup.cfg
+-rwxr-xr-x   0 alex      (1010) admin       (80)     2847 2023-04-07 19:26:54.000000 igwn-alert-0.3.0/setup.py
```

### Comparing `igwn-alert-0.2.3/COPYING` & `igwn-alert-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `igwn-alert-0.2.3/PKG-INFO` & `igwn-alert-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: igwn-alert
-Version: 0.2.3
+Version: 0.3.0
 Summary: IGWN Alert Network
 Home-page: https://lscsoft.docs.ligo.org/igwn-alert/
 Maintainer: Alexander Pace, Duncan Meacher
 Maintainer-email: alexander.pace@ligo.org, duncan.meacher@ligo.org
 License: GPLv3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/igwn-alert/issues
 Project-URL: Documentation, https://lscsoft.docs.ligo.org/igwn-alert/
 Project-URL: Source Code, https://git.ligo.org/lscsoft/igwn-alert
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -23,8 +22,7 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 License-File: COPYING
 
 The IGWN Alert System (igwn-alert) is a prototype notification service built on Apache Kafka, using the publish-subscribe (pubsub) protocol. It is a higher-level modification of SCIMMA's hop-client to streamline receiving and responding to alerts from GraceDB.
-
```

### Comparing `igwn-alert-0.2.3/igwn_alert/__init__.py` & `igwn-alert-0.3.0/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `igwn-alert-0.2.3/igwn_alert/client.py` & `igwn-alert-0.3.0/igwn_alert/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 log = logging.getLogger(__name__)
 
 DEFAULT_SERVER = 'kafka://kafka.scimma.org/'
 DEFAULT_PORT = 9092
 DEFAULT_GROUP = 'gracedb'
 DEFAULT_BATCH_SIZE = 1
-DEFAULT_BATCH_TIMEOUT = timedelta(seconds=0.05)
+DEFAULT_BATCH_TIMEOUT = timedelta(seconds=0.2)
 
 
 class client(Stream):
     """A hop-scotch client configured for igwn_alerts from GraceDB
 
     Parameters
     ----------
@@ -56,18 +56,29 @@
         A :code:`hop.auth.Auth` object.
     authfile : str (optional)
         Path to hop :code:`auth.toml`
     noauth : bool (optional)
         Set to `True` for unauthenticated session
     group : str (optional)
         GraceDB group (e.g., `gracedb`, `gracedb-playground`)
+    consumer_group : str (optional)
+        The consumer group ID to use for consuming messages. This can be used
+        across sessions to avoid missed messages as well as allowing
+        load-balancing of messages across multiple consumers assigned to the
+        same consumer group. If not set, one will be randomly generated.
     server : str (optional)
         The server host (i.e., kafka://.....)
     port : int (optional)
         The server port
+    batch_size : int (optional)
+        The number of messages to request per batch. Higher values
+        may be more efficient, but may add latency
+    batch_timeout : timedelta (optional)
+        How long the client waits to gather a full batch of messages.
+        Higher values may be more efficient, but may add latency
 
     Example
     -------
 
     Here is an example for listing topics:
 
     .. code-block:: python
@@ -87,16 +98,16 @@
         client = IGWNAlertClient(group='gracedb-test')
         topics = ['superevent', 'cbc_gstlal']
         client.listen(process_alert, topics)
 
     """
 
     def __init__(self, username=None, password=None, auth=None, authfile=None,
-                 noauth=False, group=None, server=None, port=None,
-                 batch_size=None, batch_timeout=None):
+                 noauth=False, group=None, consumer_group=None, server=None,
+                 port=None, batch_size=None, batch_timeout=None):
 
         # Set up variables:
         if server:
             self.server = server
         else:
             self.server = DEFAULT_SERVER
 
@@ -116,14 +127,16 @@
             self.batch_size = DEFAULT_BATCH_SIZE
 
         if batch_timeout:
             self.batch_timeout = batch_timeout
         else:
             self.batch_timeout = DEFAULT_BATCH_TIMEOUT
 
+        self.consumer_group = consumer_group
+
         # Construct the base url prefix for this session.
 
         self.base_url_prefix = self._construct_base_url()
 
         # Initiate the session dict:
         self.sessions = {}
 
@@ -218,15 +231,16 @@
             if isinstance(topic, str):
                 topic = [topic]
             listen_topics = topic
         else:
             listen_topics = self.get_topics()
 
         try:
-            with self.open(self._construct_topic_url(listen_topics), "r") as s:
+            url = self._construct_topic_url(listen_topics)
+            with self.open(url, "r", group_id=self.consumer_group) as s:
                 for payload, metadata in s.read(
                         metadata=True,
                         batch_size=self.batch_size,
                         batch_timeout=self.batch_timeout):
                     # Fix in case message is in new format:
                     if isinstance(payload, JSONBlob):
                         payload = payload.content
@@ -355,16 +369,20 @@
             group = self.group_prefix
 
         # Get the dict of topics from the server. convert the keys to a list.
         # Note: self.auth currently returns a list. FIXME: for now return the
         # first item in the list. Assumes only one credential, i guess.
 
         lt = hop.list_topics
-        all_topics = list(lt.list_topics(url=self.server,
-                          auth=self.auth[0]).keys())
+        if not self.auth:
+            all_topics = list(lt.list_topics(url=self.server,
+                              auth=self.auth).keys())
+        else:
+            all_topics = list(lt.list_topics(url=self.server,
+                              auth=self.auth[0]).keys())
 
         return [topic.split('.')[1] for topic in all_topics if
                 group + '.' in topic]
 
     def get_subscriptions(self):
         """
         Get a list of your subscriptions.
```

### Comparing `igwn-alert-0.2.3/igwn_alert/tests/__init__.py` & `igwn-alert-0.3.0/igwn_alert/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `igwn-alert-0.2.3/igwn_alert/tests/conftest.py` & `igwn-alert-0.3.0/igwn_alert/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `igwn-alert-0.2.3/igwn_alert/tests/test_igwn_alert.py` & `igwn-alert-0.3.0/igwn_alert/tests/test_igwn_alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     print(response)
     return response
 
 
 # Test the version number
 def test_version():
     from igwn_alert import __version__
-    assert __version__ == '0.2.3'
+    assert __version__ == '0.3.0'
 
 
 # Test an unauthorized session
 def test_no_auth():
     tc = test_client(noauth=True)
     assert tc.auth is None
```

### Comparing `igwn-alert-0.2.3/igwn_alert/tool.py` & `igwn-alert-0.3.0/igwn_alert/tool.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,17 +26,23 @@
 
 # Version string
 VERSION_STRING = "igwn-alert client {0}".format(__version__)
 
 
 def parser():
     parser = argparse.ArgumentParser(prog='igwn-alert')
+    parser.add_argument('-a', '--auth', default='true',
+                        choices=['true', 'false'],
+                        help='Use autentication true or false')
     parser.add_argument('-g', '--group', default=DEFAULT_GROUP,
                         help='GraceDB group name (e.g., gracedb, '
                              'gracedb-playground)')
+    parser.add_argument('-c', '--consumer-group',
+                        help='Consumer group ID to use for consuming '
+                             'messages across sessions')
     parser.add_argument('-l', '--log', help='Log level', default='error',
                         choices='critical error warning info debug'.split())
     parser.add_argument('-n', '--netrc',
                         help='netrc file (default: read from NETRC '
                         'environment variable or ~/.netrc)')
     parser.add_argument('-s', '--server', default=DEFAULT_SERVER,
                         help='igwn-alert server hostname')
@@ -77,16 +83,23 @@
 
 def main(args=None):
     opts = parser().parse_args(args)
 
     if opts.log is not None:
         logging.basicConfig(level=opts.log.upper())
 
-    lv = client(server=opts.server,
-                group=opts.group)
+    if opts.auth == 'true':
+        lv = client(server=opts.server,
+                    group=opts.group,
+                    consumer_group=opts.consumer_group)
+    else:
+        lv = client(noauth=True,
+                    server=opts.server,
+                    group=opts.group,
+                    consumer_group=opts.consumer_group)
 
     try:
         if opts.action == 'listen':
             lv.listen(callback=None, topic=[*opts.topics])
         if opts.action == 'topics':
             print("Topics for group {0} associated with the current "
                   "credential:".format(opts.group))
```

### Comparing `igwn-alert-0.2.3/igwn_alert.egg-info/PKG-INFO` & `igwn-alert-0.3.0/igwn_alert.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: igwn-alert
-Version: 0.2.3
+Version: 0.3.0
 Summary: IGWN Alert Network
 Home-page: https://lscsoft.docs.ligo.org/igwn-alert/
 Maintainer: Alexander Pace, Duncan Meacher
 Maintainer-email: alexander.pace@ligo.org, duncan.meacher@ligo.org
 License: GPLv3+
 Project-URL: Bug Tracker, https://git.ligo.org/lscsoft/igwn-alert/issues
 Project-URL: Documentation, https://lscsoft.docs.ligo.org/igwn-alert/
 Project-URL: Source Code, https://git.ligo.org/lscsoft/igwn-alert
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -23,8 +22,7 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 License-File: COPYING
 
 The IGWN Alert System (igwn-alert) is a prototype notification service built on Apache Kafka, using the publish-subscribe (pubsub) protocol. It is a higher-level modification of SCIMMA's hop-client to streamline receiving and responding to alerts from GraceDB.
-
```

### Comparing `igwn-alert-0.2.3/setup.py` & `igwn-alert-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #
 
 from setuptools import (
     setup,
     find_packages,
 )
 
-version = "0.2.3"
+version = "0.3.0"
 
 setup(
     # metadata
     name="igwn-alert",
     version=version,
     maintainer="Alexander Pace, Duncan Meacher",
     maintainer_email=(
@@ -64,18 +64,20 @@
         "Topic :: Scientific/Engineering :: Astronomy",
         "Topic :: Scientific/Engineering :: Physics",
     ],
     # requirements
     python_requires=">=3.6",
     setup_requires=["setuptools"],
     install_requires=[
-        "setuptools",
-        "hop-client>=0.6.0",
-        "confluent-kafka>=1.7.0",
+        "adc-streaming>=2.3.0",
+        "confluent-kafka>=2.0.0",
+        "hop-client>=0.7.0",
+        "pyopenssl>=23.0.0",
         "safe-netrc",
+        "setuptools",
     ],
     # contents
     entry_points={
         'console_scripts': [
             'igwn-alert=igwn_alert.tool:main',
         ],
     },
```

