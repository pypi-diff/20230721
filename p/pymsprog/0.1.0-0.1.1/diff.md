# Comparing `tmp/pymsprog-0.1.0.tar.gz` & `tmp/pymsprog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymsprog-0.1.0.tar", max compression
+gzip compressed data, was "pymsprog-0.1.1.tar", max compression
```

## Comparing `pymsprog-0.1.0.tar` & `pymsprog-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0        0 2023-03-13 14:29:39.519974 pymsprog-0.1.0/README.md
--rw-r--r--   0        0        0    32688 2023-03-13 15:58:22.881101 pymsprog-0.1.0/pymsprog/__init__.py
--rw-r--r--   0        0        0      415 2023-03-13 15:41:42.871827 pymsprog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 pymsprog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5497 2023-07-21 15:07:18.010896 pymsprog-0.1.1/README.md
+-rw-r--r--   0        0        0     6148 2023-07-21 14:08:33.945772 pymsprog-0.1.1/pymsprog/.DS_Store
+-rw-r--r--   0        0        0     2414 2023-07-21 14:08:20.046467 pymsprog-0.1.1/pymsprog/.ipynb_checkpoints/pymsprog_tutorial-checkpoint.ipynb
+-rw-r--r--   0        0        0    57826 2023-07-21 15:27:12.699736 pymsprog-0.1.1/pymsprog/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-21 15:38:54.349254 pymsprog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 pymsprog-0.1.1/PKG-INFO
```

