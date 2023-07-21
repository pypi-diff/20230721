# Comparing `tmp/mkdocs-risonia-theme-0.1.7.tar.gz` & `tmp/mkdocs_risonia_theme-0.1.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-risonia-theme-0.1.7.tar", last modified: Sun May 28 20:47:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

