# Comparing `tmp/pil-supporter-0.0.10.tar.gz` & `tmp/pil-supporter-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pil-supporter-0.0.10.tar", last modified: Fri Jul 21 03:23:02 2023, max compression
+gzip compressed data, was "pil-supporter-0.0.8.tar", last modified: Sun Mar 12 10:38:42 2023, max compression
```

## Comparing `pil-supporter-0.0.10.tar` & `pil-supporter-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 03:23:02.647036 pil-supporter-0.0.10/
--rw-r--r--   0 root         (0) root         (0)      974 2023-07-21 03:23:02.647036 pil-supporter-0.0.10/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      724 2023-07-21 03:23:01.000000 pil-supporter-0.0.10/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 03:23:02.645036 pil-supporter-0.0.10/pil_supporter/
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-21 03:23:01.000000 pil-supporter-0.0.10/pil_supporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 03:23:02.647036 pil-supporter-0.0.10/pil_supporter/utils/
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-21 03:23:01.000000 pil-supporter-0.0.10/pil_supporter/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2738 2023-07-21 03:23:01.000000 pil-supporter-0.0.10/pil_supporter/utils/draw.py
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-21 03:23:01.000000 pil-supporter-0.0.10/pil_supporter/utils/etc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 03:23:02.646036 pil-supporter-0.0.10/pil_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      974 2023-07-21 03:23:02.000000 pil-supporter-0.0.10/pil_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-21 03:23:02.000000 pil-supporter-0.0.10/pil_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 03:23:02.000000 pil-supporter-0.0.10/pil_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 03:23:02.000000 pil-supporter-0.0.10/pil_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-21 03:23:02.000000 pil-supporter-0.0.10/pil_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 03:23:02.000000 pil-supporter-0.0.10/pil_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 03:23:02.647036 pil-supporter-0.0.10/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      592 2023-07-21 03:23:01.000000 pil-supporter-0.0.10/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:38:42.059975 pil-supporter-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)      914 2023-03-12 10:38:42.059975 pil-supporter-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      645 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:38:42.057975 pil-supporter-0.0.8/pil_supporter/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/pil_supporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:38:42.058975 pil-supporter-0.0.8/pil_supporter/utils/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/pil_supporter/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/pil_supporter/utils/draw.py
+-rw-r--r--   0 root         (0) root         (0)      782 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/pil_supporter/utils/etc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:38:42.058975 pil-supporter-0.0.8/pil_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      914 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/pil_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      315 2023-03-12 10:38:42.000000 pil-supporter-0.0.8/pil_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/pil_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/pil_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/pil_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-12 10:38:42.059975 pil-supporter-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      591 2023-03-12 10:38:41.000000 pil-supporter-0.0.8/setup.py
```

### Comparing `pil-supporter-0.0.10/PKG-INFO` & `pil-supporter-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pil-supporter
-Version: 0.0.10
+Version: 0.0.8
 Summary: Pil supporter
 Home-page: https://github.com/automatethem/pil-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # pil-supporter
 
-https://pypi.org/project/pil-supporter
-<pre>
-pip install pil-supporter
-</pre>
-
 Supported APIs
 <pre>
 import pil_supporter
 
 pil_supporter.utils.draw_rect(image, point1, point2)
 pil_supporter.utils.draw_label(image, text, point, font_color=(255, 255, 255), font_size=28)
 pil_supporter.utils.draw_rect_with_label(image, point1, point2, text, font_color=(255, 255, 255), font_size=28)
 pil_supporter.utils.draw_point(image, point)
 pil_supporter.utils.draw_image(image, image_to_draw, point)
 
 pil_supporter.utils.crop_center(image_file, left, top, right, bottom)
 pil_supporter.utils.create_dummy_image(size, image_file, background_color=(255, 255, 255))
 pil_supporter.utils.read_from_image_file(image_file)
 </pre>
+
+
```

### Comparing `pil-supporter-0.0.10/README.md` & `pil-supporter-0.0.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 # pil-supporter
 
-https://pypi.org/project/pil-supporter
-<pre>
-pip install pil-supporter
-</pre>
-
 Supported APIs
 <pre>
 import pil_supporter
 
 pil_supporter.utils.draw_rect(image, point1, point2)
 pil_supporter.utils.draw_label(image, text, point, font_color=(255, 255, 255), font_size=28)
 pil_supporter.utils.draw_rect_with_label(image, point1, point2, text, font_color=(255, 255, 255), font_size=28)
```

### Comparing `pil-supporter-0.0.10/pil_supporter/utils/draw.py` & `pil-supporter-0.0.8/pil_supporter/utils/draw.py`

 * *Files identical despite different names*

### Comparing `pil-supporter-0.0.10/pil_supporter/utils/etc.py` & `pil-supporter-0.0.8/pil_supporter/utils/etc.py`

 * *Files identical despite different names*

### Comparing `pil-supporter-0.0.10/pil_supporter.egg-info/PKG-INFO` & `pil-supporter-0.0.8/pil_supporter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pil-supporter
-Version: 0.0.10
+Version: 0.0.8
 Summary: Pil supporter
 Home-page: https://github.com/automatethem/pil-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # pil-supporter
 
-https://pypi.org/project/pil-supporter
-<pre>
-pip install pil-supporter
-</pre>
-
 Supported APIs
 <pre>
 import pil_supporter
 
 pil_supporter.utils.draw_rect(image, point1, point2)
 pil_supporter.utils.draw_label(image, text, point, font_color=(255, 255, 255), font_size=28)
 pil_supporter.utils.draw_rect_with_label(image, point1, point2, text, font_color=(255, 255, 255), font_size=28)
 pil_supporter.utils.draw_point(image, point)
 pil_supporter.utils.draw_image(image, image_to_draw, point)
 
 pil_supporter.utils.crop_center(image_file, left, top, right, bottom)
 pil_supporter.utils.create_dummy_image(size, image_file, background_color=(255, 255, 255))
 pil_supporter.utils.read_from_image_file(image_file)
 </pre>
+
+
```

### Comparing `pil-supporter-0.0.10/setup.py` & `pil-supporter-0.0.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='pil-supporter',
-	version='0.0.10',
+	version='0.0.8',
 	description='Pil supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/pil-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

