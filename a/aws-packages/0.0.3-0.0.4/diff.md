# Comparing `tmp/aws_packages-0.0.3.tar.gz` & `tmp/aws_packages-0.0.4-cp310-none-win32.whl.zip`

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

