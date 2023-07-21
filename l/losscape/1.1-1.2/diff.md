# Comparing `tmp/losscape-1.1.tar.gz` & `tmp/losscape-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.1.tar", last modified: Fri Jul 21 07:10:19 2023, max compression
+gzip compressed data, was "losscape-1.2.tar", last modified: Fri Jul 21 07:21:56 2023, max compression
```

## Comparing `losscape-1.1.tar` & `losscape-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:10:19.579264 losscape-1.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:10:19.579264 losscape-1.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3020 2023-07-18 21:38:11.000000 losscape-1.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:10:19.579264 losscape-1.1/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.1/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.1/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.1/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15665 2023-07-21 06:59:27.000000 losscape-1.1/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.1/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:10:19.579264 losscape-1.1/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 07:10:19.000000 losscape-1.1/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 07:10:19.579264 losscape-1.1/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      399 2023-07-21 07:09:32.000000 losscape-1.1/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:21:56.211571 losscape-1.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:21:56.211571 losscape-1.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3020 2023-07-18 21:38:11.000000 losscape-1.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:21:56.211571 losscape-1.2/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.2/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1380 2023-07-18 10:08:58.000000 losscape-1.2/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.2/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15690 2023-07-21 07:21:10.000000 losscape-1.2/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.2/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 07:21:56.211571 losscape-1.2/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      230 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       36 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-21 07:21:56.000000 losscape-1.2/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-21 07:21:56.211571 losscape-1.2/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      399 2023-07-21 07:21:29.000000 losscape-1.2/setup.py
```

### Comparing `losscape-1.1/README.md` & `losscape-1.2/README.md`

 * *Files identical despite different names*

### Comparing `losscape-1.1/losscape/compute_loss.py` & `losscape-1.2/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.1/losscape/create_directions.py` & `losscape-1.2/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.1/losscape/create_landscape.py` & `losscape-1.2/losscape/create_landscape.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,16 @@
         plt.show()
     
     plt.clf()
 
     if output_vtp:
         _create_vtp(X, Y, losses, log=log_vtp)
 
+    return X, Y, losses
+
 def _set_weights(model, weights, directions, step):
     if len(directions) == 2:
         dx = directions[0]
         dy = directions[1]
         changes = [d0*step[0] + d1*step[1] for (d0, d1) in zip(dx, dy)]
 
     else:
```

### Comparing `losscape-1.1/losscape/train.py` & `losscape-1.2/losscape/train.py`

 * *Files identical despite different names*

