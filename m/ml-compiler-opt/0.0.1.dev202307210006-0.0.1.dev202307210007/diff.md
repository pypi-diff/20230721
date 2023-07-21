# Comparing `tmp/ml-compiler-opt-0.0.1.dev202307210006.tar.gz` & `tmp/ml_compiler_opt-0.0.1.dev202307210007-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-compiler-opt-0.0.1.dev202307210006.tar", last modified: Fri Jul 21 00:06:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

