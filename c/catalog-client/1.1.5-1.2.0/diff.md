# Comparing `tmp/catalog_client-1.1.5.tar.gz` & `tmp/catalog_client-1.2.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/catalog_client-1.1.5.tar", last modified: Fri Jun 24 17:35:20 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

