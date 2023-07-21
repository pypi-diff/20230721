# Comparing `tmp/bioconsertinc-1.0.2.tar.gz` & `tmp/bioconsertinc-1.0.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioconsertinc-1.0.2.tar", last modified: Sun Jul  9 21:35:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

