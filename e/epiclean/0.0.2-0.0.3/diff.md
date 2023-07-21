# Comparing `tmp/epiclean-0.0.2.tar.gz` & `tmp/epiclean-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epiclean-0.0.2.tar", last modified: Tue Nov 29 05:35:57 2022, max compression
+gzip compressed data, was "epiclean-0.0.3.tar", last modified: Fri Jul 21 16:05:14 2023, max compression
```

## Comparing `epiclean-0.0.2.tar` & `epiclean-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shreyaskolpe   (501) staff       (20)        0 2022-11-29 05:35:57.739984 epiclean-0.0.2/
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)     1056 2022-05-27 15:43:46.000000 epiclean-0.0.2/LICENSE
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)      873 2022-11-29 05:35:57.740117 epiclean-0.0.2/PKG-INFO
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)      276 2022-11-29 05:15:41.000000 epiclean-0.0.2/README.md
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)       86 2022-11-29 05:09:16.000000 epiclean-0.0.2/pyproject.toml
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)      723 2022-11-29 05:35:57.740795 epiclean-0.0.2/setup.cfg
-drwxr-xr-x   0 shreyaskolpe   (501) staff       (20)        0 2022-11-29 05:35:57.735146 epiclean-0.0.2/src/
-drwxr-xr-x   0 shreyaskolpe   (501) staff       (20)        0 2022-11-29 05:35:57.738465 epiclean-0.0.2/src/epiclean/
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)        0 2022-05-27 15:47:26.000000 epiclean-0.0.2/src/epiclean/__init__.py
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)      850 2022-11-29 05:29:24.000000 epiclean-0.0.2/src/epiclean/clean_epigraphia.py
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)     1716 2022-11-29 05:29:46.000000 epiclean-0.0.2/src/epiclean/cleaner.py
-drwxr-xr-x   0 shreyaskolpe   (501) staff       (20)        0 2022-11-29 05:35:57.739735 epiclean-0.0.2/src/epiclean.egg-info/
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)      873 2022-11-29 05:35:57.000000 epiclean-0.0.2/src/epiclean.egg-info/PKG-INFO
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)      268 2022-11-29 05:35:57.000000 epiclean-0.0.2/src/epiclean.egg-info/SOURCES.txt
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)        1 2022-11-29 05:35:57.000000 epiclean-0.0.2/src/epiclean.egg-info/dependency_links.txt
--rw-r--r--   0 shreyaskolpe   (501) staff       (20)        9 2022-11-29 05:35:57.000000 epiclean-0.0.2/src/epiclean.egg-info/top_level.txt
+drwxr-xr-x   0 shreyaskolpe   (501) staff       (20)        0 2023-07-21 16:05:14.548959 epiclean-0.0.3/
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)     1056 2022-05-27 15:43:46.000000 epiclean-0.0.3/LICENSE
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)     1371 2023-07-21 16:05:14.549119 epiclean-0.0.3/PKG-INFO
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)      773 2023-07-21 16:02:47.000000 epiclean-0.0.3/README.md
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)       86 2022-11-29 05:09:16.000000 epiclean-0.0.3/pyproject.toml
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)      723 2023-07-21 16:05:14.549774 epiclean-0.0.3/setup.cfg
+drwxr-xr-x   0 shreyaskolpe   (501) staff       (20)        0 2023-07-21 16:05:14.542239 epiclean-0.0.3/src/
+drwxr-xr-x   0 shreyaskolpe   (501) staff       (20)        0 2023-07-21 16:05:14.547086 epiclean-0.0.3/src/epiclean/
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)        0 2022-05-27 15:47:26.000000 epiclean-0.0.3/src/epiclean/__init__.py
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)      991 2023-07-21 15:53:31.000000 epiclean-0.0.3/src/epiclean/clean_epigraphia.py
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)     2097 2023-07-21 15:53:39.000000 epiclean-0.0.3/src/epiclean/cleaner.py
+drwxr-xr-x   0 shreyaskolpe   (501) staff       (20)        0 2023-07-21 16:05:14.548681 epiclean-0.0.3/src/epiclean.egg-info/
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)     1371 2023-07-21 16:05:14.000000 epiclean-0.0.3/src/epiclean.egg-info/PKG-INFO
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)      268 2023-07-21 16:05:14.000000 epiclean-0.0.3/src/epiclean.egg-info/SOURCES.txt
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)        1 2023-07-21 16:05:14.000000 epiclean-0.0.3/src/epiclean.egg-info/dependency_links.txt
+-rw-r--r--   0 shreyaskolpe   (501) staff       (20)        9 2023-07-21 16:05:14.000000 epiclean-0.0.3/src/epiclean.egg-info/top_level.txt
```

### Comparing `epiclean-0.0.2/LICENSE` & `epiclean-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `epiclean-0.0.2/setup.cfg` & `epiclean-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = epiclean
-version = 0.0.2
+version = 0.0.3
 author = Shreyas Kolpe
 author_email = shreyas10.kolpe@gmail.com
 description = A package for data cleaning inscriptions in Epigraphia Carnatica
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ShreyasKolpe/epigraphia-data-cleaning/tree/main/automation
 project_urls =
```

### Comparing `epiclean-0.0.2/src/epiclean/cleaner.py` & `epiclean-0.0.3/src/epiclean/cleaner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import argparse
 from clean_epigraphia import processor
 
 # This file is the command line tool to make use of processor
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("-lang", help="script/language of text. Supports kn (Kannada)", required=True, choices=('kn', ))
+    parser.add_argument("-a", help="whether to find and replace ā. Boolean", action='store_true', default=False)
     parser.add_argument("-e", help="whether to find and replace ē. Boolean", action='store_true', default=False)
     parser.add_argument("-o", help="whether to find and replace ō. Boolean", action='store_true', default=False)
-    parser.add_argument("-s", help="whether to find and replace the sequence śrī. Boolean", action='store_true', default=False)
+    parser.add_argument("-s", help="whether to find and replace ś and Ś. Boolean", action='store_true', default=False)
+    parser.add_argument("-sri", help="whether to find and replace the sequence śrī. Boolean", action='store_true', default=False)
     parser.add_argument("-n", help="whether to find and replace consonant clusters involving anunasika", action='store_true', default=False)
     parser.add_argument("-jn", help="whether to find and replace (probable) ñ", action='store_true', default=False)
+    parser.add_argument("-m", help="whether to find and replace (probable) ṁ", action='store_true', default=False)
     parser.add_argument("-f", help="path of file containing unclean text")
     parser.add_argument("-i", help="for providing text in(command)line. Don't forget to enclose in double quotes")
     args = parser.parse_args()
     input = None
     if args.f:
         with open(args.f, 'r') as file:
             input = file.read()
@@ -23,17 +26,17 @@
         print("One of -f or -i must be specified")
         exit(1)
 
     if not input:
         print("input is null")
         exit(1)
 
-    output = processor(input, args.lang, args.e, args.o, args.s, args.n, args.jn)
+    output = processor(input, args.lang, args.a, args.e, args.o, args.s, args.sri, args.n, args.jn, args.m)
     if not output:
         print("An error occurred. Aborting")
         exit(1)
 
     if args.f:
         with open("output.txt", 'w') as file:
             file.write(output)
     else:
-        print(output)
+        print(output)
```

