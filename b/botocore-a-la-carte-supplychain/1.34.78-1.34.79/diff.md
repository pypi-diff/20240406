# Comparing `tmp/botocore-a-la-carte-supplychain-1.34.78.tar.gz` & `tmp/botocore_a_la_carte_supplychain-1.34.79-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-supplychain-1.34.78.tar", last modified: Fri Apr  5 01:00:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
