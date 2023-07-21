# Comparing `tmp/Pathway-1.3.tar.gz` & `tmp/Pathway-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pathway-1.3.tar", last modified: Sun Jan 17 03:38:38 2010, max compression, from Unix
+gzip compressed data, was "Pathway-1.3.1.tar", last modified: Mon Jan 18 02:26:07 2010, max compression, from Unix
```

## Comparing `Pathway-1.3.tar` & `Pathway-1.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 matthew    (500) matthew    (500)        0 2010-01-17 03:38:38.000000 Pathway-1.3/
--rw-r--r--   0 matthew    (500) matthew    (500)     1053 2009-12-15 15:29:27.000000 Pathway-1.3/LICENSE
--rw-r--r--   0 matthew    (500) matthew    (500)     1278 2010-01-17 03:38:02.000000 Pathway-1.3/setup.py
--rw-r--r--   0 matthew    (500) matthew    (500)     1234 2010-01-17 03:38:38.000000 Pathway-1.3/PKG-INFO
--rw-r--r--   0 matthew    (500) matthew    (500)    13871 2010-01-17 03:37:09.000000 Pathway-1.3/pathway.py
--rw-r--r--   0 matthew    (500) matthew    (500)     1313 2010-01-03 19:12:24.000000 Pathway-1.3/README
+drwxr-xr-x   0 matthew    (500) matthew    (500)        0 2010-01-18 02:26:07.000000 Pathway-1.3.1/
+-rw-r--r--   0 matthew    (500) matthew    (500)     1053 2009-12-15 15:29:27.000000 Pathway-1.3.1/LICENSE
+-rw-r--r--   0 matthew    (500) matthew    (500)     1280 2010-01-18 02:25:05.000000 Pathway-1.3.1/setup.py
+-rw-r--r--   0 matthew    (500) matthew    (500)     1236 2010-01-18 02:26:07.000000 Pathway-1.3.1/PKG-INFO
+-rw-r--r--   0 matthew    (500) matthew    (500)    13871 2010-01-18 02:24:51.000000 Pathway-1.3.1/pathway.py
+-rw-r--r--   0 matthew    (500) matthew    (500)     1313 2010-01-03 19:12:24.000000 Pathway-1.3.1/README
```

### Comparing `Pathway-1.3/LICENSE` & `Pathway-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Pathway-1.3/setup.py` & `Pathway-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Topic :: System :: Filesystems'
 ]
 
 setup(
     name='Pathway',
-    version='1.3',
+    version='1.3.1',
     description='A library for interacting with the filesystem',
     long_description=info,
     author='LeafStorm',
     author_email='leafstormrush@gmail.com',
     py_modules=['pathway'],
     provides=['pathway'],
     classifiers=classifiers
```

### Comparing `Pathway-1.3/PKG-INFO` & `Pathway-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Pathway
-Version: 1.3
+Version: 1.3.1
 Summary: A library for interacting with the filesystem
 Home-page: UNKNOWN
 Author: LeafStorm
 Author-email: leafstormrush@gmail.com
 License: UNKNOWN
 Description: Pathway is a module for interacting with the filesystem in a clean,
         object-oriented manner. For example, instead of::
```

### Comparing `Pathway-1.3/pathway.py` & `Pathway-1.3.1/pathway.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,28 +387,28 @@
         os.rename(self.path, newpath)
         self.path = newpath
         if self._stats:
             self._restat()
     
     def copy(self, dest, overwrite=True, meta=True):
         if isinstance(dest, Folder):
-            dest = dest[self.basename,]
+            dest = dest + self.basename
         elif p.isdir(dest):
             dest = p.join(dest, self.basename)
         if (not overwrite) and p.exists(dest):
             raise WouldNotOverwriteError(dest)
         if meta:
             shutil.copy2(self.path, dest)
         else:
             shutil.copy(self.path, dest)
     
     if hasattr(os, 'symlink'):
         def symlink(self, dest, overwrite=True):
             if isinstance(dest, Folder):
-                dest = dest[self.basename,]
+                dest = dest + self.basename
             elif p.isdir(dest):
                 dest = p.join(dest, self.basename)
             if (not overwrite) and p.exists(dest):
                 raise WouldNotOverwriteError(dest)
             os.symlink(self.path, dest)
 
     @property
```

### Comparing `Pathway-1.3/README` & `Pathway-1.3.1/README`

 * *Files identical despite different names*

