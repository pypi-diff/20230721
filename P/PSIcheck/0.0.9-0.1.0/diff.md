# Comparing `tmp/PSIcheck-0.0.9.tar.gz` & `tmp/PSIcheck-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PSIcheck-0.0.9.tar", last modified: Tue Jul 18 07:00:30 2023, max compression
+gzip compressed data, was "PSIcheck-0.1.0.tar", last modified: Fri Jul 21 04:36:11 2023, max compression
```

## Comparing `PSIcheck-0.0.9.tar` & `PSIcheck-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 07:00:30.004214 PSIcheck-0.0.9/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 07:00:29.994243 PSIcheck-0.0.9/PKG-INFO
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 07:00:29.640404 PSIcheck-0.0.9/PSIcheck/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      477 2022-09-23 05:47:24.000000 PSIcheck-0.0.9/PSIcheck/__init__.py
--rwxrwxrwx   0 edith     (1000) edith     (1000)      772 2023-07-18 07:00:14.000000 PSIcheck-0.0.9/PSIcheck/get_parser.py
--rwxrwxrwx   0 edith     (1000) edith     (1000)     9040 2022-11-29 13:40:30.000000 PSIcheck-0.0.9/PSIcheck/screen_for_magPro.py
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 07:00:29.939827 PSIcheck-0.0.9/PSIcheck.egg-info/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/PKG-INFO
--rwxrwxrwx   0 edith     (1000) edith     (1000)      276 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/SOURCES.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)        1 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/dependency_links.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       43 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/entry_points.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       21 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/requires.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)        9 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/top_level.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       38 2023-07-18 07:00:30.006127 PSIcheck-0.0.9/setup.cfg
--rwxrwxrwx   0 edith     (1000) edith     (1000)     1028 2023-07-18 07:00:07.000000 PSIcheck-0.0.9/setup.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-21 04:36:11.057057 PSIcheck-0.1.0/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-21 04:36:11.041538 PSIcheck-0.1.0/PKG-INFO
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-21 04:36:10.604153 PSIcheck-0.1.0/PSIcheck/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      477 2022-09-23 05:47:24.000000 PSIcheck-0.1.0/PSIcheck/__init__.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      772 2023-07-21 04:33:19.000000 PSIcheck-0.1.0/PSIcheck/get_parser.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     9038 2023-07-21 04:35:40.000000 PSIcheck-0.1.0/PSIcheck/screen_for_magPro.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-21 04:36:10.963102 PSIcheck-0.1.0/PSIcheck.egg-info/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-21 04:36:10.000000 PSIcheck-0.1.0/PSIcheck.egg-info/PKG-INFO
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      276 2023-07-21 04:36:10.000000 PSIcheck-0.1.0/PSIcheck.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)        1 2023-07-21 04:36:10.000000 PSIcheck-0.1.0/PSIcheck.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       43 2023-07-21 04:36:10.000000 PSIcheck-0.1.0/PSIcheck.egg-info/entry_points.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       21 2023-07-21 04:36:10.000000 PSIcheck-0.1.0/PSIcheck.egg-info/requires.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)        9 2023-07-21 04:36:10.000000 PSIcheck-0.1.0/PSIcheck.egg-info/top_level.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       38 2023-07-21 04:36:11.057057 PSIcheck-0.1.0/setup.cfg
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     1028 2023-07-21 04:33:10.000000 PSIcheck-0.1.0/setup.py
```

### Comparing `PSIcheck-0.0.9/PSIcheck/get_parser.py` & `PSIcheck-0.1.0/PSIcheck/get_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
              epilog=f"""
 {CBOLD}Usage：{CEND}
 
     {CRED}$ {CGREEN}PSIcheck{CEND} PsiResultPath
 
 Runjia Ji, 2023
 """)
-    parser.add_argument('-v', '--version', action='version', version='%(prog)s 0.0.9', help='show PSIcheck version number and exit')
+    parser.add_argument('-v', '--version', action='version', version='%(prog)s 0.1.0', help='show PSIcheck version number and exit')
     parser.add_argument('PsiResultPath', type=str, help='directory stores PSI-Blast results')
     parser.add_argument('-gbk','--GenbankFilesPath', type=str, help='directory stores Genbank files')
 
     args = parser.parse_args()
     return args
```

### Comparing `PSIcheck-0.0.9/PSIcheck/screen_for_magPro.py` & `PSIcheck-0.1.0/PSIcheck/screen_for_magPro.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     namelist_tmp = []
     fullname_tmp = []
     acclist_tmp = []
     evallist_tmp = []
     for i in range(len(list_)-1):
         if 'Query=' in list_[i]:
             if ('Query=' not in list_[i+1]) & ('blank' not in list_[i+1]):
-                id = re.search('LOCUSTAG_[0-9]+', list_[i]).group()
+                id = re.search('Query=\ (.*)', list_[i]).group(1)
                 idlist.append(id)
                 gname = list_[i].replace('Query=','').split('_LOCUSTAG')[0]
                 gnamelist.append(gname)
                 if namelist_tmp:
                     namelist.append(namelist_tmp)
                 if acclist_tmp:
                     acclist.append(acclist_tmp)
```

### Comparing `PSIcheck-0.0.9/setup.py` & `PSIcheck-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PSIcheck',
-    version='0.0.9',
+    version='0.1.0',
     description="check PSI-Blast result",
     author='Runjia Ji',
     author_email='jirunjia@gmail.com',
     # py_modules=["magcluster", 'args', 'capture_args', 'maga', 'magm', 'magsc', 'main'],
     # package_dir={'': 'src'},
     packages=find_packages(),
     classifiers=[
```

