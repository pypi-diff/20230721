# Comparing `tmp/aiopegelonline-0.0.2.tar.gz` & `tmp/aiopegelonline-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopegelonline-0.0.2.tar", last modified: Fri Jul 21 15:03:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

