# Comparing `tmp/spade_client-5.0.4.tar.gz` & `tmp/spade_client-5.2.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spade_client-5.0.4.tar", last modified: Tue Oct  4 17:48:17 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

