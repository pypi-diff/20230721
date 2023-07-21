# Comparing `tmp/ipymafs-0.0.1.tar.gz` & `tmp/ipymafs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymafs-0.0.1.tar", max compression
+gzip compressed data, was "ipymafs-0.0.2.tar", max compression
```

## Comparing `ipymafs-0.0.1.tar` & `ipymafs-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       20 2023-07-17 18:25:07.232927 ipymafs-0.0.1/README.md
--rw-r--r--   0        0        0      213 2023-07-17 18:26:31.717089 ipymafs-0.0.1/ipymafs/__init__.py
--rw-r--r--   0        0        0  3976013 2023-07-17 18:25:30.252805 ipymafs-0.0.1/ipymafs/static/style.css
--rw-r--r--   0        0        0   568165 2023-07-17 18:25:30.252302 ipymafs-0.0.1/ipymafs/static/widget.js
--rw-r--r--   0        0        0      407 2023-07-17 18:32:11.985091 ipymafs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 ipymafs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      373 2023-07-21 14:03:23.255986 ipymafs-0.0.2/README.md
+-rw-r--r--   0        0        0      263 2023-07-21 14:06:39.413892 ipymafs-0.0.2/ipymafs/__init__.py
+-rw-r--r--   0        0        0     2236 2023-07-21 14:06:12.814221 ipymafs-0.0.2/ipymafs/static/widget.css
+-rw-r--r--   0        0        0  1655253 2023-07-21 14:06:12.814350 ipymafs-0.0.2/ipymafs/static/widget.js
+-rw-r--r--   0        0        0      362 2023-07-21 14:02:15.438827 ipymafs-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 ipymafs-0.0.2/PKG-INFO
```

