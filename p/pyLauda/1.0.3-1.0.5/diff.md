# Comparing `tmp/pyLauda-1.0.3.tar.gz` & `tmp/pyLauda-1.0.5-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLauda-1.0.3.tar", last modified: Fri Jun 23 04:13:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

