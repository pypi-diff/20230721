# Comparing `tmp/iktomi-0.8.tar.gz` & `tmp/iktomi-0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iktomi-0.8.tar", last modified: Thu Dec  2 14:14:38 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

