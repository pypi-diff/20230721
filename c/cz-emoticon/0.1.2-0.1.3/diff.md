# Comparing `tmp/cz_emoticon-0.1.2.tar.gz` & `tmp/cz_emoticon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cz_emoticon-0.1.2.tar", last modified: Sat Jul 15 22:35:00 2023, max compression
+gzip compressed data, was "cz_emoticon-0.1.3.tar", last modified: Thu Jul 20 22:13:35 2023, max compression
```

## Comparing `cz_emoticon-0.1.2.tar` & `cz_emoticon-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 javier    (1000) javier    (1000)        0 2023-07-15 22:35:00.879840 cz_emoticon-0.1.2/
--rw-r--r--   0 javier    (1000) javier    (1000)     3628 2023-07-15 22:35:00.879840 cz_emoticon-0.1.2/PKG-INFO
--rw-r--r--   0 javier    (1000) javier    (1000)     2804 2023-07-15 22:29:13.000000 cz_emoticon-0.1.2/README.md
-drwxr-xr-x   0 javier    (1000) javier    (1000)        0 2023-07-15 22:35:00.879840 cz_emoticon-0.1.2/cz_emoticon.egg-info/
--rw-r--r--   0 javier    (1000) javier    (1000)     3628 2023-07-15 22:35:00.000000 cz_emoticon-0.1.2/cz_emoticon.egg-info/PKG-INFO
--rw-r--r--   0 javier    (1000) javier    (1000)      245 2023-07-15 22:35:00.000000 cz_emoticon-0.1.2/cz_emoticon.egg-info/SOURCES.txt
--rw-r--r--   0 javier    (1000) javier    (1000)        1 2023-07-15 22:35:00.000000 cz_emoticon-0.1.2/cz_emoticon.egg-info/dependency_links.txt
--rw-r--r--   0 javier    (1000) javier    (1000)       58 2023-07-15 22:35:00.000000 cz_emoticon-0.1.2/cz_emoticon.egg-info/entry_points.txt
--rw-r--r--   0 javier    (1000) javier    (1000)       11 2023-07-15 22:35:00.000000 cz_emoticon-0.1.2/cz_emoticon.egg-info/requires.txt
--rw-r--r--   0 javier    (1000) javier    (1000)       12 2023-07-15 22:35:00.000000 cz_emoticon-0.1.2/cz_emoticon.egg-info/top_level.txt
--rw-r--r--   0 javier    (1000) javier    (1000)    13539 2023-07-12 02:37:33.000000 cz_emoticon-0.1.2/cz_emoticon.py
--rw-r--r--   0 javier    (1000) javier    (1000)       38 2023-07-15 22:35:00.879840 cz_emoticon-0.1.2/setup.cfg
--rw-r--r--   0 javier    (1000) javier    (1000)      535 2023-07-15 22:33:42.000000 cz_emoticon-0.1.2/setup.py
+drwxr-xr-x   0 javier    (1000) javier    (1000)        0 2023-07-20 22:13:35.392746 cz_emoticon-0.1.3/
+-rw-r--r--   0 javier    (1000) javier    (1000)     3628 2023-07-20 22:13:35.392746 cz_emoticon-0.1.3/PKG-INFO
+-rw-r--r--   0 javier    (1000) javier    (1000)     2804 2023-07-15 22:29:13.000000 cz_emoticon-0.1.3/README.md
+drwxr-xr-x   0 javier    (1000) javier    (1000)        0 2023-07-20 22:13:35.392746 cz_emoticon-0.1.3/cz_emoticon.egg-info/
+-rw-r--r--   0 javier    (1000) javier    (1000)     3628 2023-07-20 22:13:35.000000 cz_emoticon-0.1.3/cz_emoticon.egg-info/PKG-INFO
+-rw-r--r--   0 javier    (1000) javier    (1000)      245 2023-07-20 22:13:35.000000 cz_emoticon-0.1.3/cz_emoticon.egg-info/SOURCES.txt
+-rw-r--r--   0 javier    (1000) javier    (1000)        1 2023-07-20 22:13:35.000000 cz_emoticon-0.1.3/cz_emoticon.egg-info/dependency_links.txt
+-rw-r--r--   0 javier    (1000) javier    (1000)       58 2023-07-20 22:13:35.000000 cz_emoticon-0.1.3/cz_emoticon.egg-info/entry_points.txt
+-rw-r--r--   0 javier    (1000) javier    (1000)       11 2023-07-20 22:13:35.000000 cz_emoticon-0.1.3/cz_emoticon.egg-info/requires.txt
+-rw-r--r--   0 javier    (1000) javier    (1000)       12 2023-07-20 22:13:35.000000 cz_emoticon-0.1.3/cz_emoticon.egg-info/top_level.txt
+-rw-r--r--   0 javier    (1000) javier    (1000)    13400 2023-07-20 22:07:34.000000 cz_emoticon-0.1.3/cz_emoticon.py
+-rw-r--r--   0 javier    (1000) javier    (1000)       38 2023-07-20 22:13:35.392746 cz_emoticon-0.1.3/setup.cfg
+-rw-r--r--   0 javier    (1000) javier    (1000)      553 2023-07-20 22:12:16.000000 cz_emoticon-0.1.3/setup.py
```

### Comparing `cz_emoticon-0.1.2/PKG-INFO` & `cz_emoticon-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz_emoticon
-Version: 0.1.2
+Version: 0.1.3
 Summary: UNKNOWN
 Home-page: https://github.com/jdbaigorria/cz_emoticon
 Author: Javier Baigorria
 Author-email: jdbaigorria@gmail.com
 License: MIT
 Description: # Emoticon cz
```

### Comparing `cz_emoticon-0.1.2/README.md` & `cz_emoticon-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cz_emoticon-0.1.2/cz_emoticon.egg-info/PKG-INFO` & `cz_emoticon-0.1.3/cz_emoticon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cz-emoticon
-Version: 0.1.2
+Version: 0.1.3
 Summary: UNKNOWN
 Home-page: https://github.com/jdbaigorria/cz_emoticon
 Author: Javier Baigorria
 Author-email: jdbaigorria@gmail.com
 License: MIT
 Description: # Emoticon cz
```

### Comparing `cz_emoticon-0.1.2/cz_emoticon.py` & `cz_emoticon-0.1.3/cz_emoticon.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,18 +324,14 @@
 
         if self.jira_prefix and self.jira_url:
             parsed_message["footer"] = parse_jira_codes(parsed_message["footer"], self.jira_url, self.jira_prefix)
 
         if self.git_repo:
             parsed_message["footer"] = parse_issues(parsed_message["footer"], self.git_repo)
 
-        f = open ('/home/javier/projects/emoticon/holamundo.txt','a')
-        f.write(parsed_message.__repr__() + "\n")
-        f.close()
-
         return parsed_message
     
     def __extract_footer(self, commit: git.GitCommit):
         footer_pattern = r"\((.*?)\)"
         matches = re.findall(footer_pattern, commit.body)
         return ", ".join(matches)
```

### Comparing `cz_emoticon-0.1.2/setup.py` & `cz_emoticon-0.1.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
-with open('README.md') as f:
+with open('README.md', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
 
     name="cz_emoticon",
-    version="0.1.2",
+    version="0.1.3",
     py_modules=["cz_emoticon"],
     license="MIT",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/jdbaigorria/cz_emoticon",
     install_requires=["commitizen"],
     entry_points={"commitizen.plugin": ["cz_emoticon = cz_emoticon:EmoticonCz"]},
```

