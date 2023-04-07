# Comparing `tmp/tmu-0.7.1.tar.gz` & `tmp/tmu-0.7.9-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmu-0.7.1.tar", last modified: Wed Jan 11 10:54:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

