# Comparing `tmp/openedx-ledger-0.3.0.tar.gz` & `tmp/openedx-ledger-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-ledger-0.3.0.tar", last modified: Thu Apr  6 16:37:09 2023, max compression
+gzip compressed data, was "openedx-ledger-0.3.1.tar", last modified: Fri Apr  7 18:21:56 2023, max compression
```

## Comparing `openedx-ledger-0.3.0.tar` & `openedx-ledger-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:09.576406 openedx-ledger-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-04-06 16:37:09.576406 openedx-ledger-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:09.568405 openedx-ledger-0.3.0/openedx_ledger/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5185 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:09.576406 openedx-ledger-0.3.0/openedx_ledger/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
--rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/migrations/0005_help_text_and_more_indices.py
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/migrations/0006_auto_20230404_1744.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15474 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:09.564405 openedx-ledger-0.3.0/openedx_ledger/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:09.576406 openedx-ledger-0.3.0/openedx_ledger/templates/edx_ledger/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/templates/edx_ledger/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:09.576406 openedx-ledger-0.3.0/openedx_ledger/test_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/test_utils/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/openedx_ledger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:09.576406 openedx-ledger-0.3.0/openedx_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-04-06 16:37:09.000000 openedx-ledger-0.3.0/openedx_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-06 16:37:09.000000 openedx-ledger-0.3.0/openedx_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 16:37:09.000000 openedx-ledger-0.3.0/openedx_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 16:37:09.000000 openedx-ledger-0.3.0/openedx_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-06 16:37:09.000000 openedx-ledger-0.3.0/openedx_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-06 16:37:09.000000 openedx-ledger-0.3.0/openedx_ledger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:09.576406 openedx-ledger-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-06 16:37:09.580406 openedx-ledger-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 16:37:09.576406 openedx-ledger-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4515 2023-04-06 16:37:06.000000 openedx-ledger-0.3.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.214021 openedx-ledger-0.3.1/openedx_ledger/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2696 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5185 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/openedx_ledger/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0006_auto_20230404_1744.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15474 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.214021 openedx-ledger-0.3.1/openedx_ledger/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/openedx_ledger/templates/edx_ledger/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/templates/edx_ledger/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/openedx_ledger/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/test_utils/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.214021 openedx-ledger-0.3.1/openedx_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4515 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/tests/test_models.py
```

### Comparing `openedx-ledger-0.3.0/CHANGELOG.rst` & `openedx-ledger-0.3.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/LICENSE.txt` & `openedx-ledger-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/PKG-INFO` & `openedx-ledger-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.3.0
+Version: 0.3.1
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openedx-ledger-0.3.0/README.rst` & `openedx-ledger-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/admin.py` & `openedx-ledger-0.3.1/openedx_ledger/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,38 @@
     def balance(self, obj):
         """
         Passthrough function to calculate the ledger balance.
         """
         return obj.balance()
 
 
+@admin.register(models.ExternalFulfillmentProvider)
+class ExternalFulfillmentProviderAdmin(SimpleHistoryAdmin):
+    """
+    Admin configuration for the ExternalFulfillmentProvider model.
+    """
+    class Meta:
+        """
+        Metaclass for ExternalFulfillmentProviderAdmin.
+        """
+
+        model = models.ExternalFulfillmentProvider
+        fields = '__all__'
+
+    search_fields = ('name', 'slug',)
+    list_display = ('name', 'slug',)
+
+
+class ExternalTransactionReferenceInlineAdmin(admin.TabularInline):
+    """
+    Inline admin configuration for the ExternalTransactionReference model.
+    """
+    model = models.ExternalTransactionReference
+
+
 @admin.register(models.Transaction)
 class TransactionAdmin(SimpleHistoryAdmin):
     """
     Admin configuration for the Transaction model.
     """
 
     class Meta:
@@ -51,23 +75,24 @@
         Metaclass for TransactionAdmin.
         """
 
         model = models.Transaction
         fields = '__all__'
 
     search_fields = ('content_key', 'lms_user_id', 'uuid', 'external_reference__external_reference_id',)
-    _all_fields = [field.name for field in models.Transaction._meta.get_fields()]
+    _all_fields = [field.name for field in models.Transaction._meta.get_fields() if field.name != 'external_reference']
     list_display = ('uuid', 'idempotency_key', 'quantity', 'state',)
     if can_modify():
         readonly_fields = (
             'created',
             'modified',
         )
     else:
         readonly_fields = _all_fields
+    inlines = [ExternalTransactionReferenceInlineAdmin]
 
 
 @admin.register(models.Reversal)
 class ReversalAdmin(SimpleHistoryAdmin):
     """
     Admin configuration for the Reversal model.
     """
```

### Comparing `openedx-ledger-0.3.0/openedx_ledger/api.py` & `openedx-ledger-0.3.1/openedx_ledger/api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/migrations/0001_initial.py` & `openedx-ledger-0.3.1/openedx_ledger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py` & `openedx-ledger-0.3.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/migrations/0003_field_updates_20230216_1605.py` & `openedx-ledger-0.3.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py` & `openedx-ledger-0.3.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/migrations/0005_help_text_and_more_indices.py` & `openedx-ledger-0.3.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/migrations/0006_auto_20230404_1744.py` & `openedx-ledger-0.3.1/openedx_ledger/migrations/0006_auto_20230404_1744.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/models.py` & `openedx-ledger-0.3.1/openedx_ledger/models.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/templates/edx_ledger/base.html` & `openedx-ledger-0.3.1/openedx_ledger/templates/edx_ledger/base.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/test_utils/factories.py` & `openedx-ledger-0.3.1/openedx_ledger/test_utils/factories.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger/utils.py` & `openedx-ledger-0.3.1/openedx_ledger/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/openedx_ledger.egg-info/PKG-INFO` & `openedx-ledger-0.3.1/openedx_ledger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.3.0
+Version: 0.3.1
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openedx-ledger-0.3.0/openedx_ledger.egg-info/SOURCES.txt` & `openedx-ledger-0.3.1/openedx_ledger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/requirements/constraints.txt` & `openedx-ledger-0.3.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/setup.py` & `openedx-ledger-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/tests/test_api.py` & `openedx-ledger-0.3.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.0/tests/test_models.py` & `openedx-ledger-0.3.1/tests/test_models.py`

 * *Files identical despite different names*

