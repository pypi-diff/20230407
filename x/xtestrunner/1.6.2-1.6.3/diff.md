# Comparing `tmp/xtestrunner-1.6.2.tar.gz` & `tmp/xtestrunner-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtestrunner-1.6.2.tar", max compression
+gzip compressed data, was "xtestrunner-1.6.3.tar", max compression
```

## Comparing `xtestrunner-1.6.2.tar` & `xtestrunner-1.6.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11567 2022-03-16 14:28:26.157468 xtestrunner-1.6.2/LICENSE
--rw-r--r--   0        0        0     1160 2023-03-11 15:51:23.311769 xtestrunner-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     2342 2023-03-06 16:55:59.681328 xtestrunner-1.6.2/README.md
--rw-r--r--   0        0        0     2107 2023-03-11 15:51:01.700855 xtestrunner-1.6.2/XTestRunner/__init__.py
--rw-r--r--   0        0        0     4300 2022-11-23 16:26:28.416349 xtestrunner-1.6.2/XTestRunner/_dingtalk.py
--rw-r--r--   0        0        0     3221 2023-03-06 16:55:59.683323 xtestrunner-1.6.2/XTestRunner/_email.py
--rw-r--r--   0        0        0     4944 2022-11-23 16:33:04.007983 xtestrunner-1.6.2/XTestRunner/_feishu.py
--rw-r--r--   0        0        0     4251 2023-03-06 16:55:59.684323 xtestrunner-1.6.2/XTestRunner/_weixin.py
--rw-r--r--   0        0        0      875 2022-04-07 16:13:07.194649 xtestrunner-1.6.2/XTestRunner/config.py
--rw-r--r--   0        0        0        0 2022-03-05 09:43:21.583035 xtestrunner-1.6.2/XTestRunner/html/__init__.py
--rw-r--r--   0        0        0     9995 2022-05-07 13:53:25.627622 xtestrunner-1.6.2/XTestRunner/html/heading-en.html
--rw-r--r--   0        0        0     9998 2022-05-07 13:53:25.628656 xtestrunner-1.6.2/XTestRunner/html/heading-zh-CN.html
--rw-r--r--   0        0        0     4431 2022-04-12 14:37:36.417747 xtestrunner-1.6.2/XTestRunner/html/mail.html
--rw-r--r--   0        0        0      442 2022-04-12 14:45:26.407074 xtestrunner-1.6.2/XTestRunner/html/notice_tmp.md
--rw-r--r--   0        0        0     2549 2023-03-06 16:55:59.685323 xtestrunner-1.6.2/XTestRunner/html/report-en.html
--rw-r--r--   0        0        0     2555 2023-03-06 16:55:59.686323 xtestrunner-1.6.2/XTestRunner/html/report-zh-CN.html
--rw-r--r--   0        0        0     5455 2023-03-11 15:34:52.855357 xtestrunner-1.6.2/XTestRunner/html/stylesheet.html
--rw-r--r--   0        0        0     8300 2022-07-28 15:36:31.468348 xtestrunner-1.6.2/XTestRunner/html/template.html
--rw-r--r--   0        0        0        0 2022-03-11 14:28:55.560239 xtestrunner-1.6.2/XTestRunner/htmlrunner/__init__.py
--rw-r--r--   0        0        0     8724 2023-03-11 15:08:38.167810 xtestrunner-1.6.2/XTestRunner/htmlrunner/result.py
--rw-r--r--   0        0        0    19457 2023-03-11 15:30:19.410914 xtestrunner-1.6.2/XTestRunner/htmlrunner/runner.py
--rw-r--r--   0        0        0      478 2022-03-11 15:11:22.626827 xtestrunner-1.6.2/XTestRunner/version.py
--rw-r--r--   0        0        0        0 2022-03-08 14:19:54.668807 xtestrunner-1.6.2/XTestRunner/xmlrunner/__init__.py
--rw-r--r--   0        0        0    26732 2023-03-11 16:23:55.295699 xtestrunner-1.6.2/XTestRunner/xmlrunner/result.py
--rw-r--r--   0        0        0     5587 2023-03-06 16:55:59.691323 xtestrunner-1.6.2/XTestRunner/xmlrunner/runner.py
--rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 xtestrunner-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11567 2022-03-16 14:28:26.157468 xtestrunner-1.6.3/LICENSE
+-rw-r--r--   0        0        0     1160 2023-04-07 16:05:03.752586 xtestrunner-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2342 2023-03-06 16:55:59.681328 xtestrunner-1.6.3/README.md
+-rw-r--r--   0        0        0     2107 2023-04-07 16:00:47.363977 xtestrunner-1.6.3/XTestRunner/__init__.py
+-rw-r--r--   0        0        0     4300 2022-11-23 16:26:28.416349 xtestrunner-1.6.3/XTestRunner/_dingtalk.py
+-rw-r--r--   0        0        0     3571 2023-04-05 03:32:24.218179 xtestrunner-1.6.3/XTestRunner/_email.py
+-rw-r--r--   0        0        0     4944 2022-11-23 16:33:04.007983 xtestrunner-1.6.3/XTestRunner/_feishu.py
+-rw-r--r--   0        0        0     4251 2023-03-06 16:55:59.684323 xtestrunner-1.6.3/XTestRunner/_weixin.py
+-rw-r--r--   0        0        0      875 2022-04-07 16:13:07.194649 xtestrunner-1.6.3/XTestRunner/config.py
+-rw-r--r--   0        0        0        0 2022-03-05 09:43:21.583035 xtestrunner-1.6.3/XTestRunner/html/__init__.py
+-rw-r--r--   0        0        0     9995 2023-04-07 15:55:51.680155 xtestrunner-1.6.3/XTestRunner/html/heading-en.html
+-rw-r--r--   0        0        0     9998 2022-05-07 13:53:25.628656 xtestrunner-1.6.3/XTestRunner/html/heading-zh-CN.html
+-rw-r--r--   0        0        0     4431 2022-04-12 14:37:36.417747 xtestrunner-1.6.3/XTestRunner/html/mail.html
+-rw-r--r--   0        0        0      442 2022-04-12 14:45:26.407074 xtestrunner-1.6.3/XTestRunner/html/notice_tmp.md
+-rw-r--r--   0        0        0     2549 2023-03-06 16:55:59.685323 xtestrunner-1.6.3/XTestRunner/html/report-en.html
+-rw-r--r--   0        0        0     2555 2023-03-06 16:55:59.686323 xtestrunner-1.6.3/XTestRunner/html/report-zh-CN.html
+-rw-r--r--   0        0        0     5455 2023-03-11 15:34:52.855357 xtestrunner-1.6.3/XTestRunner/html/stylesheet.html
+-rw-r--r--   0        0        0     8300 2023-04-07 15:55:51.682151 xtestrunner-1.6.3/XTestRunner/html/template.html
+-rw-r--r--   0        0        0        0 2022-03-11 14:28:55.560239 xtestrunner-1.6.3/XTestRunner/htmlrunner/__init__.py
+-rw-r--r--   0        0        0     8914 2023-04-05 03:32:24.219167 xtestrunner-1.6.3/XTestRunner/htmlrunner/result.py
+-rw-r--r--   0        0        0    19457 2023-03-11 15:30:19.410914 xtestrunner-1.6.3/XTestRunner/htmlrunner/runner.py
+-rw-r--r--   0        0        0      478 2022-03-11 15:11:22.626827 xtestrunner-1.6.3/XTestRunner/version.py
+-rw-r--r--   0        0        0        0 2022-03-08 14:19:54.668807 xtestrunner-1.6.3/XTestRunner/xmlrunner/__init__.py
+-rw-r--r--   0        0        0    26732 2023-03-11 16:23:55.295699 xtestrunner-1.6.3/XTestRunner/xmlrunner/result.py
+-rw-r--r--   0        0        0     5587 2023-03-06 16:55:59.691323 xtestrunner-1.6.3/XTestRunner/xmlrunner/runner.py
+-rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 xtestrunner-1.6.3/PKG-INFO
```

### Comparing `xtestrunner-1.6.2/LICENSE` & `xtestrunner-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/pyproject.toml` & `xtestrunner-1.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "XTestRunner"
-version = "1.6.2"
+version = "1.6.3"
 description = "Modern style test report based on unittest framework."
 authors = ["bugmaster <fnngj@126.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/seldomQA/XTestRunner/"
 repository = "https://github.com/seldomQA/XTestRunner/"
 classifiers = [
```

### Comparing `xtestrunner-1.6.2/README.md` & `xtestrunner-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/__init__.py` & `xtestrunner-1.6.3/XTestRunner/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,10 +38,10 @@
 from ._feishu import FeiShu
 from ._weixin import Weinxin
 from .config import label
 
 
 __author__ = "bugmaster"
 
-__version__ = "1.6.2"
+__version__ = "1.6.3"
 
 __description__ = "Unittest-based HTML test report."
```

### Comparing `xtestrunner-1.6.2/XTestRunner/_dingtalk.py` & `xtestrunner-1.6.3/XTestRunner/_dingtalk.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/_email.py` & `xtestrunner-1.6.3/XTestRunner/_email.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,30 @@
 
 
 class SMTP(object):
     """
     Mail function based on SMTP protocol
     """
 
-    def __init__(self, user, password, host, port=None, ssl=True):
+    def __init__(self, user, password, host, port=None, ssl=True, tls=True):
+        """
+
+        :param user: Email login user name
+        :param password: Email login password
+        :param host: Email service address
+        :param port: Email service post
+        :param ssl: SMTP SSL True/False
+        :param tls: TLS mode True/False
+        """
         self.user = user
         self.password = password
         self.host = host
         self.port = int(port) if port is not None else 465
         self.ssl = ssl
+        self.tls = tls
 
     def sender(self, to=None, subject=None, contents=None, attachments=None):
         if to is None:
             raise ValueError("Please specify the email address to send")
 
         if isinstance(to, str):
             to = [to]
@@ -73,16 +83,17 @@
 
             att = MIMEApplication(open(attachments, 'rb').read())
             att['Content-Type'] = 'application/octet-stream'
             att["Content-Disposition"] = 'attachment; filename="{}"'.format(att_name)
             msg.attach(att)
 
         smtp = smtplib.SMTP_SSL(self.host, self.port) if self.ssl else smtplib.SMTP(self.host, self.port)
-        try:
+        if self.tls is True:
             smtp.starttls()
+        try:
             smtp.login(self.user, self.password)
             smtp.sendmail(self.user, to, msg.as_string())
             print(" 📧 Email sent successfully!!")
         except BaseException as msg:
             print('❌ Email failed to send!!' + msg.__str__())
         finally:
             smtp.quit()
```

### Comparing `xtestrunner-1.6.2/XTestRunner/_feishu.py` & `xtestrunner-1.6.3/XTestRunner/_feishu.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/_weixin.py` & `xtestrunner-1.6.3/XTestRunner/_weixin.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/config.py` & `xtestrunner-1.6.3/XTestRunner/config.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/html/heading-en.html` & `xtestrunner-1.6.3/XTestRunner/html/heading-en.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/html/heading-zh-CN.html` & `xtestrunner-1.6.3/XTestRunner/html/heading-zh-CN.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/html/mail.html` & `xtestrunner-1.6.3/XTestRunner/html/mail.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/html/report-en.html` & `xtestrunner-1.6.3/XTestRunner/html/report-en.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/html/report-zh-CN.html` & `xtestrunner-1.6.3/XTestRunner/html/report-zh-CN.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/html/stylesheet.html` & `xtestrunner-1.6.3/XTestRunner/html/stylesheet.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/html/template.html` & `xtestrunner-1.6.3/XTestRunner/html/template.html`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/htmlrunner/result.py` & `xtestrunner-1.6.3/XTestRunner/htmlrunner/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,23 @@
             self.stdout0 = None
 
         if self.stderr0:
             sys.stderr = self.stderr0
             self.stderr0 = None
 
         if self.logger is not None:
-            self.logger.logger.remove(self.logger_handler_id)
+            try:
+                self.logger.logger.remove(self.logger_handler_id)
+            except ValueError:
+                ...
 
-        return self.output_buffer.getvalue()
+        if self.output_buffer is not None:
+            return self.output_buffer.getvalue()
+        else:
+            return "setUpClass/start_class error."
 
     def stopTest(self, test):
         """
         Usually one of addSuccess, addError or addFailure would have been called.
         But there are some path in unittest that would bypass this.
         We must disconnect stdout in stopTest(), which is guaranteed to be called.
         """
```

### Comparing `xtestrunner-1.6.2/XTestRunner/htmlrunner/runner.py` & `xtestrunner-1.6.3/XTestRunner/htmlrunner/runner.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/xmlrunner/result.py` & `xtestrunner-1.6.3/XTestRunner/xmlrunner/result.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/XTestRunner/xmlrunner/runner.py` & `xtestrunner-1.6.3/XTestRunner/xmlrunner/runner.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.2/PKG-INFO` & `xtestrunner-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtestrunner
-Version: 1.6.2
+Version: 1.6.3
 Summary: Modern style test report based on unittest framework.
 Home-page: https://github.com/seldomQA/XTestRunner/
 License: Apache-2.0
 Author: bugmaster
 Author-email: fnngj@126.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

