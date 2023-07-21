# Comparing `tmp/dataset.sh-0.0.1.tar.gz` & `tmp/dataset.sh-1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset.sh-0.0.1.tar", last modified: Fri Jul 21 03:41:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

