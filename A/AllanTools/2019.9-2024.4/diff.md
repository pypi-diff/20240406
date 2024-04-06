# Comparing `tmp/AllanTools-2019.9.tar.gz` & `tmp/AllanTools-2024.4-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AllanTools-2019.9.tar", last modified: Fri Sep 20 16:54:54 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

