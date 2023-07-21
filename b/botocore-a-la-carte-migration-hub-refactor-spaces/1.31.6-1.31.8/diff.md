# Comparing `tmp/botocore-a-la-carte-migration-hub-refactor-spaces-1.31.6.tar.gz` & `tmp/botocore_a_la_carte_migration_hub_refactor_spaces-1.31.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-migration-hub-refactor-spaces-1.31.6.tar", last modified: Thu Jul 20 01:20:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

