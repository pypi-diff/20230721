# Comparing `tmp/kwutil-0.1.1.tar.gz` & `tmp/kwutil-0.2.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwutil-0.1.1.tar", last modified: Sun Jun 11 01:12:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

