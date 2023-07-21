# Comparing `tmp/spluscalib-0.3.3.tar.gz` & `tmp/spluscalib-0.3.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spluscalib-0.3.3.tar", last modified: Fri Jul 21 01:05:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

