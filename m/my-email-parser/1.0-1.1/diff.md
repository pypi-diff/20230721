# Comparing `tmp/my_email_parser-1.0.tar.gz` & `tmp/my_email_parser-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_email_parser-1.0.tar", last modified: Fri Jul 21 09:33:08 2023, max compression
+gzip compressed data, was "my_email_parser-1.1.tar", last modified: Fri Jul 21 09:43:53 2023, max compression
```

## Comparing `my_email_parser-1.0.tar` & `my_email_parser-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 09:33:08.512369 my_email_parser-1.0/
--rw-rw-rw-   0        0        0      501 2023-07-21 09:33:08.512369 my_email_parser-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-21 09:33:08.512369 my_email_parser-1.0/my_email_parser.egg-info/
--rw-rw-rw-   0        0        0      501 2023-07-21 09:33:08.000000 my_email_parser-1.0/my_email_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-21 09:33:08.000000 my_email_parser-1.0/my_email_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 09:33:08.000000 my_email_parser-1.0/my_email_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-21 09:33:08.000000 my_email_parser-1.0/my_email_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 09:33:08.000000 my_email_parser-1.0/my_email_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      666 2023-07-21 09:29:14.000000 my_email_parser-1.0/settingup.py
--rw-rw-rw-   0        0        0       42 2023-07-21 09:33:08.512369 my_email_parser-1.0/setup.cfg
--rw-rw-rw-   0        0        0      306 2023-07-21 08:40:39.000000 my_email_parser-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 09:43:53.179197 my_email_parser-1.1/
+-rw-rw-rw-   0        0        0       60 2023-07-21 09:43:53.178284 my_email_parser-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-21 09:43:53.174564 my_email_parser-1.1/my_email_parser.egg-info/
+-rw-rw-rw-   0        0        0       60 2023-07-21 09:43:53.000000 my_email_parser-1.1/my_email_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-21 09:43:53.000000 my_email_parser-1.1/my_email_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:43:53.000000 my_email_parser-1.1/my_email_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-21 09:43:53.000000 my_email_parser-1.1/my_email_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 09:43:53.000000 my_email_parser-1.1/my_email_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      202 2023-07-21 09:43:15.000000 my_email_parser-1.1/settingup.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 09:43:53.179197 my_email_parser-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      306 2023-07-21 08:40:39.000000 my_email_parser-1.1/setup.py
```

