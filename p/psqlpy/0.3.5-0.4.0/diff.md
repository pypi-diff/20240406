# Comparing `tmp/psqlpy-0.3.5.tar.gz` & `tmp/psqlpy-0.4.0-cp39-none-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

