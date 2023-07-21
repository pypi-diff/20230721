# Comparing `tmp/pyobs_fli-1.1.0b2.tar.gz` & `tmp/pyobs_fli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_fli-1.1.0b2.tar", max compression
+gzip compressed data, was "pyobs_fli-1.1.1.tar", max compression
```

## Comparing `pyobs_fli-1.1.0b2.tar` & `pyobs_fli-1.1.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1099 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/LICENSE
--rw-r--r--   0        0        0     1124 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/build.py
--rw-r--r--   0        0        0     1584 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/lib/Makefile
--rw-r--r--   0        0        0    32439 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/lib/docxx.sty
--rw-r--r--   0        0        0    20171 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/lib/libfli-camera-parport.c
--rw-r--r--   0        0        0     4533 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/lib/libfli-camera-parport.h
--rw-r--r--   0        0        0    74000 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/lib/libfli-camera-usb.c
--rw-r--r--   0        0        0     7336 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/lib/libfli-camera-usb.h
--rw-r--r--   0        0        0    25687 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/lib/libfli-camera.c
--rw-r--r--   0        0        0     4946 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/lib/libfli-camera.h
--rw-r--r--   0        0        0     2136 2022-11-17 10:47:13.611055 pyobs_fli-1.1.0b2/lib/libfli-debug.h
--rw-r--r--   0        0        0    37241 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli-filter-focuser.c
--rw-r--r--   0        0        0     2860 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli-filter-focuser.h
--rw-r--r--   0        0        0     8859 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli-libfli.h
--rw-r--r--   0        0        0     6443 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli-mem.c
--rw-r--r--   0        0        0     2260 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli-mem.h
--rw-r--r--   0        0        0     2495 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli-raw.c
--rw-r--r--   0        0        0     1998 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli-raw.h
--rw-r--r--   0        0        0    47939 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli.c
--rw-r--r--   0        0        0     1316 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli.dxx
--rw-r--r--   0        0        0    12631 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/libfli.h
--rw-r--r--   0        0        0     4986 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/bsd/libfli-usb-sys.c
--rw-r--r--   0        0        0     3273 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/libfli-debug.c
--rw-r--r--   0        0        0     2190 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/libfli-parport.h
--rw-r--r--   0        0        0     4976 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/libfli-serial.c
--rw-r--r--   0        0        0     1995 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/libfli-serial.h
--rw-r--r--   0        0        0     9827 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/libfli-sys.c
--rw-r--r--   0        0        0     3677 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/libfli-sys.h
--rw-r--r--   0        0        0     2751 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/libfli-usb.c
--rw-r--r--   0        0        0     3147 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/libfli-usb.h
--rw-r--r--   0        0        0     4415 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/linux/fli_ioctl.h
--rw-r--r--   0        0        0     3231 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/linux/fliusb_ioctl.h
--rw-r--r--   0        0        0     3390 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/linux/libfli-parport.c
--rw-r--r--   0        0        0     6278 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/linux/libfli-usb-sys.c
--rw-r--r--   0        0        0    27919 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/osx/libfli-usb-sys.c
--rw-r--r--   0        0        0     5792 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/unix/osx/libfli-usb-sys.h
--rw-r--r--   0        0        0     4742 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli-debug.c
--rw-r--r--   0        0        0     2027 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli-parport.h
--rw-r--r--   0        0        0     3690 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli-serial.c
--rw-r--r--   0        0        0     1967 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli-serial.h
--rw-r--r--   0        0        0     2746 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli-sys.h
--rw-r--r--   0        0        0     8430 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli-usb.c
--rw-r--r--   0        0        0     5643 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli-usb.h
--rw-r--r--   0        0        0    12024 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli-windows-parport.c
--rw-r--r--   0        0        0    31829 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli-windows.c
--rw-r--r--   0        0        0     1683 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli.def
--rw-r--r--   0        0        0     2282 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli.rc
--rw-r--r--   0        0        0     2381 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli.sln
--rw-r--r--   0        0        0    14624 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli.vcproj
--rw-r--r--   0        0        0     1668 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/libfli64.def
--rw-r--r--   0        0        0      386 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/lib/windows/resource.h
--rw-r--r--   0        0        0      160 2022-11-17 10:47:13.615055 pyobs_fli-1.1.0b2/pyobs_fli/__init__.py
--rw-r--r--   0        0        0     3309 2022-11-17 10:47:13.619055 pyobs_fli-1.1.0b2/pyobs_fli/flibase.py
--rw-r--r--   0        0        0    10262 2022-11-17 10:47:13.619055 pyobs_fli-1.1.0b2/pyobs_fli/flicamera.py
--rw-r--r--   0        0        0    11865 2022-11-17 10:47:13.619055 pyobs_fli-1.1.0b2/pyobs_fli/flidriver.pyx
--rw-r--r--   0        0        0     3878 2022-11-17 10:47:13.619055 pyobs_fli-1.1.0b2/pyobs_fli/flifilterwheel.py
--rw-r--r--   0        0        0     9561 2022-11-17 10:47:13.619055 pyobs_fli-1.1.0b2/pyobs_fli/libfli.pxd
--rw-r--r--   0        0        0      669 2022-11-17 10:47:13.619055 pyobs_fli-1.1.0b2/pyproject.toml
--rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 pyobs_fli-1.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1299 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/build.py
+-rw-r--r--   0        0        0     1584 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/lib/Makefile
+-rw-r--r--   0        0        0    32439 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/lib/docxx.sty
+-rw-r--r--   0        0        0    20171 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/lib/libfli-camera-parport.c
+-rw-r--r--   0        0        0     4533 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/lib/libfli-camera-parport.h
+-rw-r--r--   0        0        0    74000 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/lib/libfli-camera-usb.c
+-rw-r--r--   0        0        0     7336 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/lib/libfli-camera-usb.h
+-rw-r--r--   0        0        0    25687 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/lib/libfli-camera.c
+-rw-r--r--   0        0        0     4946 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/lib/libfli-camera.h
+-rw-r--r--   0        0        0     2136 2023-07-21 12:16:14.993778 pyobs_fli-1.1.1/lib/libfli-debug.h
+-rw-r--r--   0        0        0    37241 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli-filter-focuser.c
+-rw-r--r--   0        0        0     2860 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli-filter-focuser.h
+-rw-r--r--   0        0        0     8859 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli-libfli.h
+-rw-r--r--   0        0        0     6443 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli-mem.c
+-rw-r--r--   0        0        0     2260 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli-mem.h
+-rw-r--r--   0        0        0     2495 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli-raw.c
+-rw-r--r--   0        0        0     1998 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli-raw.h
+-rw-r--r--   0        0        0    47939 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli.c
+-rw-r--r--   0        0        0     1316 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli.dxx
+-rw-r--r--   0        0        0    12631 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/libfli.h
+-rw-r--r--   0        0        0     4986 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/bsd/libfli-usb-sys.c
+-rw-r--r--   0        0        0     3273 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/libfli-debug.c
+-rw-r--r--   0        0        0     2190 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/libfli-parport.h
+-rw-r--r--   0        0        0     4976 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/libfli-serial.c
+-rw-r--r--   0        0        0     1995 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/libfli-serial.h
+-rw-r--r--   0        0        0     9827 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/libfli-sys.c
+-rw-r--r--   0        0        0     3677 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/libfli-sys.h
+-rw-r--r--   0        0        0     2751 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/libfli-usb.c
+-rw-r--r--   0        0        0     3147 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/libfli-usb.h
+-rw-r--r--   0        0        0     4415 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/linux/fli_ioctl.h
+-rw-r--r--   0        0        0     3231 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/linux/fliusb_ioctl.h
+-rw-r--r--   0        0        0     3390 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/linux/libfli-parport.c
+-rw-r--r--   0        0        0     6278 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/linux/libfli-usb-sys.c
+-rw-r--r--   0        0        0    27919 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/osx/libfli-usb-sys.c
+-rw-r--r--   0        0        0     5792 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/unix/osx/libfli-usb-sys.h
+-rw-r--r--   0        0        0     4742 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli-debug.c
+-rw-r--r--   0        0        0     2027 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli-parport.h
+-rw-r--r--   0        0        0     3690 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli-serial.c
+-rw-r--r--   0        0        0     1967 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli-serial.h
+-rw-r--r--   0        0        0     2746 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli-sys.h
+-rw-r--r--   0        0        0     8430 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli-usb.c
+-rw-r--r--   0        0        0     5643 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli-usb.h
+-rw-r--r--   0        0        0    12024 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli-windows-parport.c
+-rw-r--r--   0        0        0    31829 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli-windows.c
+-rw-r--r--   0        0        0     1683 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli.def
+-rw-r--r--   0        0        0     2282 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli.rc
+-rw-r--r--   0        0        0     2381 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli.sln
+-rw-r--r--   0        0        0    14624 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli.vcproj
+-rw-r--r--   0        0        0     1668 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/libfli64.def
+-rw-r--r--   0        0        0      386 2023-07-21 12:16:14.997778 pyobs_fli-1.1.1/lib/windows/resource.h
+-rw-r--r--   0        0        0      160 2023-07-21 12:16:15.001778 pyobs_fli-1.1.1/pyobs_fli/__init__.py
+-rw-r--r--   0        0        0     3309 2023-07-21 12:16:15.001778 pyobs_fli-1.1.1/pyobs_fli/flibase.py
+-rw-r--r--   0        0        0    10262 2023-07-21 12:16:15.001778 pyobs_fli-1.1.1/pyobs_fli/flicamera.py
+-rw-r--r--   0        0        0    11866 2023-07-21 12:16:15.001778 pyobs_fli-1.1.1/pyobs_fli/flidriver.pyx
+-rw-r--r--   0        0        0     3936 2023-07-21 12:16:15.001778 pyobs_fli-1.1.1/pyobs_fli/flifilterwheel.py
+-rw-r--r--   0        0        0     9561 2023-07-21 12:16:15.001778 pyobs_fli-1.1.1/pyobs_fli/libfli.pxd
+-rw-r--r--   0        0        0      667 2023-07-21 12:16:15.001778 pyobs_fli-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 pyobs_fli-1.1.1/PKG-INFO
```

### Comparing `pyobs_fli-1.1.0b2/LICENSE` & `pyobs_fli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/build.py` & `pyobs_fli-1.1.1/build.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import shutil
+
 from setuptools import Extension, Distribution
 import numpy
 from Cython.Build import cythonize
 from Cython.Distutils.build_ext import new_build_ext as cython_build_ext
 
 
 def build() -> None:
@@ -32,13 +34,17 @@
             "cmdclass": {
                 "build_ext": cython_build_ext,
             },
         }
     )
 
     distribution.run_command("build_ext")
+
+    # copy to source
     build_ext_cmd = distribution.get_command_obj("build_ext")
-    build_ext_cmd.copy_extensions_to_source()
+    for ext in build_ext_cmd.extensions:
+        filename = build_ext_cmd.get_ext_filename(ext.name)
+        shutil.copyfile(os.path.join(build_ext_cmd.build_lib, filename), filename)
 
 
 if __name__ == "__main__":
     build()
```

### Comparing `pyobs_fli-1.1.0b2/lib/Makefile` & `pyobs_fli-1.1.1/lib/Makefile`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/docxx.sty` & `pyobs_fli-1.1.1/lib/docxx.sty`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-camera-parport.c` & `pyobs_fli-1.1.1/lib/libfli-camera-parport.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-camera-parport.h` & `pyobs_fli-1.1.1/lib/libfli-camera-parport.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-camera-usb.c` & `pyobs_fli-1.1.1/lib/libfli-camera-usb.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-camera-usb.h` & `pyobs_fli-1.1.1/lib/libfli-camera-usb.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-camera.c` & `pyobs_fli-1.1.1/lib/libfli-camera.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-camera.h` & `pyobs_fli-1.1.1/lib/libfli-camera.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-debug.h` & `pyobs_fli-1.1.1/lib/libfli-debug.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-filter-focuser.c` & `pyobs_fli-1.1.1/lib/libfli-filter-focuser.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-filter-focuser.h` & `pyobs_fli-1.1.1/lib/libfli-filter-focuser.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-libfli.h` & `pyobs_fli-1.1.1/lib/libfli-libfli.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-mem.c` & `pyobs_fli-1.1.1/lib/libfli-mem.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-mem.h` & `pyobs_fli-1.1.1/lib/libfli-mem.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-raw.c` & `pyobs_fli-1.1.1/lib/libfli-raw.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli-raw.h` & `pyobs_fli-1.1.1/lib/libfli-raw.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli.c` & `pyobs_fli-1.1.1/lib/libfli.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli.dxx` & `pyobs_fli-1.1.1/lib/libfli.dxx`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/libfli.h` & `pyobs_fli-1.1.1/lib/libfli.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/bsd/libfli-usb-sys.c` & `pyobs_fli-1.1.1/lib/unix/bsd/libfli-usb-sys.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/libfli-debug.c` & `pyobs_fli-1.1.1/lib/unix/libfli-debug.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/libfli-parport.h` & `pyobs_fli-1.1.1/lib/unix/libfli-parport.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/libfli-serial.c` & `pyobs_fli-1.1.1/lib/unix/libfli-serial.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/libfli-serial.h` & `pyobs_fli-1.1.1/lib/unix/libfli-serial.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/libfli-sys.c` & `pyobs_fli-1.1.1/lib/unix/libfli-sys.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/libfli-sys.h` & `pyobs_fli-1.1.1/lib/unix/libfli-sys.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/libfli-usb.c` & `pyobs_fli-1.1.1/lib/unix/libfli-usb.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/libfli-usb.h` & `pyobs_fli-1.1.1/lib/unix/libfli-usb.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/linux/fli_ioctl.h` & `pyobs_fli-1.1.1/lib/unix/linux/fli_ioctl.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/linux/fliusb_ioctl.h` & `pyobs_fli-1.1.1/lib/unix/linux/fliusb_ioctl.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/linux/libfli-parport.c` & `pyobs_fli-1.1.1/lib/unix/linux/libfli-parport.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/linux/libfli-usb-sys.c` & `pyobs_fli-1.1.1/lib/unix/linux/libfli-usb-sys.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/osx/libfli-usb-sys.c` & `pyobs_fli-1.1.1/lib/unix/osx/libfli-usb-sys.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/unix/osx/libfli-usb-sys.h` & `pyobs_fli-1.1.1/lib/unix/osx/libfli-usb-sys.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli-debug.c` & `pyobs_fli-1.1.1/lib/windows/libfli-debug.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli-parport.h` & `pyobs_fli-1.1.1/lib/windows/libfli-parport.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli-serial.c` & `pyobs_fli-1.1.1/lib/windows/libfli-serial.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli-serial.h` & `pyobs_fli-1.1.1/lib/windows/libfli-serial.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli-sys.h` & `pyobs_fli-1.1.1/lib/windows/libfli-sys.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli-usb.c` & `pyobs_fli-1.1.1/lib/windows/libfli-usb.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli-usb.h` & `pyobs_fli-1.1.1/lib/windows/libfli-usb.h`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli-windows-parport.c` & `pyobs_fli-1.1.1/lib/windows/libfli-windows-parport.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli-windows.c` & `pyobs_fli-1.1.1/lib/windows/libfli-windows.c`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli.def` & `pyobs_fli-1.1.1/lib/windows/libfli.def`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli.rc` & `pyobs_fli-1.1.1/lib/windows/libfli.rc`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli.sln` & `pyobs_fli-1.1.1/lib/windows/libfli.sln`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli.vcproj` & `pyobs_fli-1.1.1/lib/windows/libfli.vcproj`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/lib/windows/libfli64.def` & `pyobs_fli-1.1.1/lib/windows/libfli64.def`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/pyobs_fli/flibase.py` & `pyobs_fli-1.1.1/pyobs_fli/flibase.py`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/pyobs_fli/flicamera.py` & `pyobs_fli-1.1.1/pyobs_fli/flicamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/pyobs_fli/flidriver.pyx` & `pyobs_fli-1.1.1/pyobs_fli/flidriver.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from enum import Enum
 from typing import Tuple, List
 
 import numpy as np
 cimport numpy as np
 np.import_array()
 
-from libfli cimport *
+from .libfli cimport *
 
 
 DeviceInfo = namedtuple('DeviceInfo', ['domain', 'filename', 'name'])
 
 
 class FliTemperature(Enum):
     """Enumeration for temperature sensors."""
```

### Comparing `pyobs_fli-1.1.0b2/pyobs_fli/flifilterwheel.py` & `pyobs_fli-1.1.1/pyobs_fli/flifilterwheel.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,11 +125,11 @@
 
         Args:
             namespaces: If given, only return FITS headers for the given namespaces.
 
         Returns:
             Dictionary containing FITS headers.
         """
-        pass
+        return {"FILTER": (await self.get_filter(), "Current filter")}
 
 
 __all__ = ["FliFilterWheel"]
```

### Comparing `pyobs_fli-1.1.0b2/pyobs_fli/libfli.pxd` & `pyobs_fli-1.1.1/pyobs_fli/libfli.pxd`

 * *Files identical despite different names*

### Comparing `pyobs_fli-1.1.0b2/pyproject.toml` & `pyobs_fli-1.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "pyobs-fli"
-version = "1.1.0b2"
+version = "1.1.1"
 description = "pyobs module for FLI cameras"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 include = ['lib']
 
 [tool.poetry.build]
 script = "build.py"
 generate-setup-file = false
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.9,<3.12"
 astropy = "^5.0"
 numpy = "^1.21"
 pyobs-core = "^1.0"
 
 [tool.poetry.dev-dependencies]
 black = "^21.12b0"
 pre-commit = "^2.16"
 sphinx-rtd-theme = "^1.0"
 Sphinx = "^4.4"
-Cython = "^0.29"
+cython = "^3.0.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "Cython>=0.29.0", "numpy>=1.21.0", "setuptools"]
+requires = ["poetry-core>=1.0.0", "Cython>=3.0.0", "numpy>=1.21.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

