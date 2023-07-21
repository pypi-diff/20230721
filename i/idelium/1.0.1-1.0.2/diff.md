# Comparing `tmp/idelium-1.0.1.tar.gz` & `tmp/idelium-1.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idelium-1.0.1.tar", last modified: Wed Jul  5 12:54:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

