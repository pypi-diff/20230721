# Comparing `tmp/swiftly-windows-0.0.8.tar.gz` & `tmp/swiftly-windows-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-windows-0.0.8.tar", last modified: Tue Jul 18 21:15:02 2023, max compression
+gzip compressed data, was "swiftly-windows-0.0.9.tar", last modified: Tue Jul 18 21:19:04 2023, max compression
```

## Comparing `swiftly-windows-0.0.8.tar` & `swiftly-windows-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:15:02.310908 swiftly-windows-0.0.8/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-18 20:18:06.000000 swiftly-windows-0.0.8/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 21:15:02.310775 swiftly-windows-0.0.8/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:15:02.309292 swiftly-windows-0.0.8/scripts/
--rw-r--r--   0 brainspoof   (501) staff       (20)     6142 2023-07-18 21:14:13.000000 swiftly-windows-0.0.8/scripts/swiftly.bat
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-18 21:15:02.310950 swiftly-windows-0.0.8/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      169 2023-07-18 21:14:57.000000 swiftly-windows-0.0.8/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:15:02.310110 swiftly-windows-0.0.8/swiftly_windows/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:18:06.000000 swiftly-windows-0.0.8/swiftly_windows/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-18 20:18:06.000000 swiftly-windows-0.0.8/swiftly_windows/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-18 20:18:06.000000 swiftly-windows-0.0.8/swiftly_windows/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3299 2023-07-18 20:18:06.000000 swiftly-windows-0.0.8/swiftly_windows/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2172 2023-07-18 20:18:06.000000 swiftly-windows-0.0.8/swiftly_windows/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-18 20:18:06.000000 swiftly-windows-0.0.8/swiftly_windows/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:15:02.310583 swiftly-windows-0.0.8/swiftly_windows.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 21:15:02.000000 swiftly-windows-0.0.8/swiftly_windows.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      352 2023-07-18 21:15:02.000000 swiftly-windows-0.0.8/swiftly_windows.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-18 21:15:02.000000 swiftly-windows-0.0.8/swiftly_windows.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       16 2023-07-18 21:15:02.000000 swiftly-windows-0.0.8/swiftly_windows.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:19:04.165955 swiftly-windows-0.0.9/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-18 20:18:06.000000 swiftly-windows-0.0.9/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 21:19:04.165814 swiftly-windows-0.0.9/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:19:04.164047 swiftly-windows-0.0.9/scripts/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     6143 2023-07-18 21:18:52.000000 swiftly-windows-0.0.9/scripts/swiftly.bat
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-18 21:19:04.165999 swiftly-windows-0.0.9/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      169 2023-07-18 21:19:01.000000 swiftly-windows-0.0.9/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:19:04.165071 swiftly-windows-0.0.9/swiftly_windows/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:18:06.000000 swiftly-windows-0.0.9/swiftly_windows/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-18 20:18:06.000000 swiftly-windows-0.0.9/swiftly_windows/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-18 20:18:06.000000 swiftly-windows-0.0.9/swiftly_windows/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3299 2023-07-18 20:18:06.000000 swiftly-windows-0.0.9/swiftly_windows/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2172 2023-07-18 20:18:06.000000 swiftly-windows-0.0.9/swiftly_windows/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-18 20:18:06.000000 swiftly-windows-0.0.9/swiftly_windows/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:19:04.165645 swiftly-windows-0.0.9/swiftly_windows.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 21:19:04.000000 swiftly-windows-0.0.9/swiftly_windows.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      352 2023-07-18 21:19:04.000000 swiftly-windows-0.0.9/swiftly_windows.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-18 21:19:04.000000 swiftly-windows-0.0.9/swiftly_windows.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       16 2023-07-18 21:19:04.000000 swiftly-windows-0.0.9/swiftly_windows.egg-info/top_level.txt
```

### Comparing `swiftly-windows-0.0.8/LICENSE` & `swiftly-windows-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-windows-0.0.8/scripts/swiftly.bat` & `swiftly-windows-0.0.9/scripts/swiftly.bat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-@echo on
+@echo off
 REM Disable echo
 
 REM Check if the first argument is 'init', 'makeapp', 'run', 'install', 'uninstall', or 'push'
 IF NOT "%~1"=="init" IF NOT "%~1"=="makeapp" IF NOT "%~1"=="run" IF NOT "%~1"=="install" IF NOT "%~1"=="uninstall" IF NOT "%~1"=="push" (
     echo Invalid command.
     exit /b
 )
@@ -135,15 +135,15 @@
         echo Requirements installed
 
         call pip install swiftly-windows --upgrade > NUL 2>&1
         pip freeze > %PROJECT_VENV_LOCATION%\..\requirements.txt
         echo  All checks completed swiftly
     )
 
-    echo ✨ Project '%PROJECT_NAME%' initiated successfully :)
+    echo ☆ Project '%PROJECT_NAME%' initiated successfully :)
 
 :makeapp
     REM Call Python function with arguments
     echo '%~1'
     echo '%PROJECT_VENV_LOCATION%'
     python -c "from swiftly_windows.makeapp import makeapp; makeapp('%~1', r'%PROJECT_VENV_LOCATION%')" > NUL
     TIMEOUT /T 1 /NOBREAK > NUL
```

### Comparing `swiftly-windows-0.0.8/swiftly_windows/gitignore.py` & `swiftly-windows-0.0.9/swiftly_windows/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-windows-0.0.8/swiftly_windows/init.py` & `swiftly-windows-0.0.9/swiftly_windows/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-windows-0.0.8/swiftly_windows/makeapp.py` & `swiftly-windows-0.0.9/swiftly_windows/makeapp.py`

 * *Files identical despite different names*

