# Comparing `tmp/pyxll_jupyter-0.4.1-py3-none-any.whl.zip` & `tmp/pyxll_jupyter-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,26 @@
-Zip file size: 43360 bytes, number of entries: 22
+Zip file size: 46247 bytes, number of entries: 24
 -rw-rw-rw-  2.0 fat      496 b- defN 20-Sep-14 16:14 pyxll_jupyter/__init__.py
--rw-rw-rw-  2.0 fat    23073 b- defN 23-May-15 15:16 pyxll_jupyter/kernel.py
+-rw-rw-rw-  2.0 fat    23270 b- defN 23-Jul-12 10:48 pyxll_jupyter/kernel.py
 -rw-rw-rw-  2.0 fat     9105 b- defN 23-Jan-26 10:15 pyxll_jupyter/magic.py
--rw-rw-rw-  2.0 fat    30195 b- defN 23-May-16 14:06 pyxll_jupyter/onedrive.py
--rw-rw-rw-  2.0 fat    11056 b- defN 23-May-15 15:17 pyxll_jupyter/pyxll.py
--rw-rw-rw-  2.0 fat       50 b- defN 23-Jan-26 10:15 pyxll_jupyter/kernel_managers/__init__.py
+-rw-rw-rw-  2.0 fat    30207 b- defN 23-Jul-21 11:07 pyxll_jupyter/onedrive.py
+-rw-rw-rw-  2.0 fat    12765 b- defN 23-Jul-21 11:07 pyxll_jupyter/pyxll.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-12 10:47 pyxll_jupyter/kernel_managers/__init__.py
 -rw-rw-rw-  2.0 fat     4196 b- defN 23-May-15 14:48 pyxll_jupyter/kernel_managers/extipy.py
+-rw-rw-rw-  2.0 fat     1708 b- defN 23-Jul-21 11:07 pyxll_jupyter/kernel_managers/labkm.py
+-rw-rw-rw-  2.0 fat     1986 b- defN 23-Jul-21 11:07 pyxll_jupyter/kernel_managers/nbkm.py
 -rw-rw-rw-  2.0 fat       43 b- defN 23-Jan-26 10:15 pyxll_jupyter/provisioning/__init__.py
 -rw-rw-rw-  2.0 fat     1816 b- defN 23-Apr-25 14:52 pyxll_jupyter/provisioning/existing.py
 -rw-rw-rw-  2.0 fat     5704 b- defN 21-Jul-27 09:57 pyxll_jupyter/resources/browser.png
 -rw-rw-rw-  2.0 fat     4436 b- defN 20-Sep-14 08:15 pyxll_jupyter/resources/jupyter.png
 -rw-rw-rw-  2.0 fat     1658 b- defN 21-Jul-27 09:57 pyxll_jupyter/resources/ribbon.xml
 -rw-rw-rw-  2.0 fat       64 b- defN 21-Jul-27 09:57 pyxll_jupyter/widgets/__init__.py
--rw-rw-rw-  2.0 fat     4786 b- defN 21-Jul-27 09:57 pyxll_jupyter/widgets/browser.py
--rw-rw-rw-  2.0 fat     1856 b- defN 22-Jan-12 15:35 pyxll_jupyter/widgets/jupyter.py
--rw-rw-rw-  2.0 fat     3302 b- defN 22-Jan-12 15:35 pyxll_jupyter/widgets/qtimports.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-16 14:12 pyxll_jupyter-0.4.1.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     5262 b- defN 23-May-16 14:12 pyxll_jupyter-0.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-16 14:12 pyxll_jupyter-0.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      187 b- defN 23-May-16 14:12 pyxll_jupyter-0.4.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-16 14:12 pyxll_jupyter-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1937 b- defN 23-May-16 14:12 pyxll_jupyter-0.4.1.dist-info/RECORD
-22 files, 110415 bytes uncompressed, 40174 bytes compressed:  63.6%
+-rw-rw-rw-  2.0 fat     6557 b- defN 23-Jul-12 10:21 pyxll_jupyter/widgets/browser.py
+-rw-rw-rw-  2.0 fat     2340 b- defN 23-Jul-12 10:22 pyxll_jupyter/widgets/jupyter.py
+-rw-rw-rw-  2.0 fat     3302 b- defN 23-Jul-21 11:07 pyxll_jupyter/widgets/qtimports.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-21 11:13 pyxll_jupyter-0.5.0.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     7411 b- defN 23-Jul-21 11:13 pyxll_jupyter-0.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 11:13 pyxll_jupyter-0.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      187 b- defN 23-Jul-21 11:13 pyxll_jupyter-0.5.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-21 11:13 pyxll_jupyter-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2125 b- defN 23-Jul-21 11:13 pyxll_jupyter-0.5.0.dist-info/RECORD
+24 files, 120569 bytes uncompressed, 42759 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -15,14 +15,20 @@
 
 Filename: pyxll_jupyter/kernel_managers/__init__.py
 Comment: 
 
 Filename: pyxll_jupyter/kernel_managers/extipy.py
 Comment: 
 
+Filename: pyxll_jupyter/kernel_managers/labkm.py
+Comment: 
+
+Filename: pyxll_jupyter/kernel_managers/nbkm.py
+Comment: 
+
 Filename: pyxll_jupyter/provisioning/__init__.py
 Comment: 
 
 Filename: pyxll_jupyter/provisioning/existing.py
 Comment: 
 
 Filename: pyxll_jupyter/resources/browser.png
@@ -42,26 +48,26 @@
 
 Filename: pyxll_jupyter/widgets/jupyter.py
 Comment: 
 
 Filename: pyxll_jupyter/widgets/qtimports.py
 Comment: 
 
-Filename: pyxll_jupyter-0.4.1.dist-info/LICENSE.md
+Filename: pyxll_jupyter-0.5.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: pyxll_jupyter-0.4.1.dist-info/METADATA
+Filename: pyxll_jupyter-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: pyxll_jupyter-0.4.1.dist-info/WHEEL
+Filename: pyxll_jupyter-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyxll_jupyter-0.4.1.dist-info/entry_points.txt
+Filename: pyxll_jupyter-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyxll_jupyter-0.4.1.dist-info/top_level.txt
+Filename: pyxll_jupyter-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyxll_jupyter-0.4.1.dist-info/RECORD
+Filename: pyxll_jupyter-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyxll_jupyter/kernel.py

```diff
@@ -24,17 +24,19 @@
 import sys
 import os
 import re
 
 # Command line args for the different Jupyter subcommands
 _subcommand_jupyter_args = {
     "notebook": [
-        "--NotebookApp.kernel_manager_class=pyxll_jupyter.kernel_managers.ExternalIPythonKernelManager"
+        "--NotebookApp.kernel_manager_class=pyxll_jupyter.kernel_managers.nbkm.ExternalMappingKernelManager",
+        "--KernelProvisionerFactory.default_provisioner_name=pyxll-provisioner"
     ],
     "lab": [
+        "--ServerApp.kernel_manager_class=pyxll_jupyter.kernel_managers.labkm.ExternalMappingKernelManager",
         "--KernelProvisionerFactory.default_provisioner_name=pyxll-provisioner"
     ]
 }
 
 # Query args to add to the URL to open the client
 _subcommand_query_params = {
     "notebook": [],
```

## pyxll_jupyter/onedrive.py

```diff
@@ -3,15 +3,15 @@
 https://gist.githubusercontent.com/guwidoe/038398b6be1b16c458365716a921814d/raw/5bf858b2939e21e2b5731562bfb81768d7bfdb55/GetLocalOneDrivePath.bas.vb
 
 Note: The variable names used in this file don't conform with the style
 used in the rest of this project and it is not well structured.
 This is intentional to make comparing this code with the original VB code easier.
 """
 
-b"""
+r"""
 'Attribute VB_Name = "GetLocalOneDrivePath"
 ' Cross-platform VBA Function to get the local path of OneDrive/SharePoint
 ' synchronized Microsoft Office files (Works on Windows and on macOS)
 '
 ' Author: Guido Witt-Dorring
 ' Created: 2022/07/01
 ' Updated: 2023/04/09
@@ -325,25 +325,25 @@
     clpPath = Path(os.environ["LOCALAPPDATA"], "Microsoft", "Office", "CLP")
 
     oneDriveSettDirs = []
     for settPath in settPaths:
         if settPath.exists() and settPath.is_dir():
             for dirName in settPath.iterdir():
                   if dirName.is_dir() \
-                  and (dirName.name == "Personal" or re.match("^Business\d+$", dirName.name)):
+                  and (dirName.name == "Personal" or re.match(r"^Business\d+$", dirName.name)):
                         oneDriveSettDirs.append(dirName)
 
     requiredFiles = []
     for vDir in oneDriveSettDirs:
          for fileName in vDir.iterdir():
               if fileName.is_file() and (
-                re.match("^([\da-f]{16}|([\da-f]{8}-[\da-f]{4}-[\da-f]{4}-[\da-f]{4}-[\da-f]{12}))\.(ini|dat)$", fileName.name, re.I) \
-                or re.match("^ClientPolicy.*\.ini$", fileName.name, re.I) \
-                or re.match("^GroupFolders.ini$", fileName.name, re.I) \
-                or re.match("^global.ini$", fileName.name, re.I)):
+                re.match(r"^([\da-f]{16}|([\da-f]{8}-[\da-f]{4}-[\da-f]{4}-[\da-f]{4}-[\da-f]{12}))\.(ini|dat)$", fileName.name, re.I) \
+                or re.match(r"^ClientPolicy.*\.ini$", fileName.name, re.I) \
+                or re.match(r"^GroupFolders.ini$", fileName.name, re.I) \
+                or re.match(r"^global.ini$", fileName.name, re.I)):
                    requiredFiles.append(fileName)
 
     # This part should ensure perfect accuracy despite the mount point cache
     # while sacrificing almost no performance at all by querying FileDateTimes.
     if not rebuild_cache:
         for vFile in requiredFiles:
             if lastCacheUpdate is None or vFile.stat().st_mtime > lastCacheUpdate:
@@ -384,15 +384,15 @@
         if not globalIni.exists():
             continue
         
         # Get the cid from the global.ini file
         cid = None
         with open(globalIni, "rt", encoding="utf-16le") as fh:
             for line in fh.readlines():
-                match = re.match("cid\s*=\s*([\da-f]{16}|(?:[\da-f]{8}-[\da-f]{4}-[\da-f]{4}-[\da-f]{4}-[\da-f]{12}))", line, re.I)
+                match = re.match(r"cid\s*=\s*([\da-f]{16}|(?:[\da-f]{8}-[\da-f]{4}-[\da-f]{4}-[\da-f]{4}-[\da-f]{12}))", line, re.I)
                 if match:
                         cid = match.group(1)
                         break
             else:
                 continue
         
         dirName = vDir.name
@@ -409,15 +409,15 @@
                 if i > 0:
                     email = fileName.name[:i-1]
                     break
 
         # Read all the ClientPloicy*.ini files:
         cliPolColl = {}
         for fileName in vDir.iterdir():
-            if re.match("^ClientPolicy.*\.ini", fileName.name, re.I):
+            if re.match(r"^ClientPolicy.*\.ini", fileName.name, re.I):
                 cliPol = cliPolColl[fileName.name] = {}
                 with open(fileName, "rt", encoding="utf-16le") as fh:
                     for line in fh.readlines():
                         if "=" in line:
                             tag, s = re.split(r"\s*=\s*", line.strip(), 1)
                             if tag == "DavUrlNamespace":
                                 cliPol[tag] = s
@@ -429,17 +429,17 @@
 
         # Read cid.dat file (assume we'll have enough memory to read it all in)
         odFolders = {}
         with open(datFile, "rb") as fh:
             s = fh.read()
 
         if re.match("Personal", vDir.name, re.I):
-            folderIdPattern = re.compile("^[a-z0-9]{16}!\d{3}.*$", re.I)
+            folderIdPattern = re.compile(r"^[a-z0-9]{16}!\d{3}.*$", re.I)
         else:
-            folderIdPattern = re.compile("^[a-z0-9]{32}$", re.I)
+            folderIdPattern = re.compile(r"^[a-z0-9]{32}$", re.I)
 
         for vItem in range(16, 0, -8):
             i = s.find(sig2, vItem)               # Search pattern in cid.dat
             while i > vItem and i < len(s) - 168: # and confirm with another
                 if s[i-vItem:i-vItem+1] == sig1:  # one
                     i = i + 8
                     n = s.find(vbNullByte, i) - i
@@ -459,15 +459,15 @@
                         odFolders[folderID] = (parentID, folderName)
 
                 # Find next sig2 in cid.dat
                 i = s.find(sig2, i+1)
 
         # Read cid.ini file
         with open(iniFile, "rt", encoding="utf-16le") as fh:
-            if re.match("^Business\d+$", dirName, re.I):
+            if re.match(r"^Business\d+$", dirName, re.I):
                 # Settings files for a business OD account
                 # Max 9 Business OneDrive accounts can be signed in at a time.
                 libNrToWebColl = {}
                 locToWebColl = {}
                 mainMount = ""
                 for line in fh.readlines():
                     line = line.strip()
@@ -552,15 +552,15 @@
 
                             locRoot = Path(mainMount) / s
                             locToWebColl[locRoot] = (locRoot, webRoot, email, mainSyncID, mainSyncFind, dirName)
 
             elif dirName == "Personal":  # Settings files for a personal OD account
                 # Only one Personal OneDrive account can be signed in at a time.
                 for line in fh.readlines():  # Loop should exit at first line
-                    if re.match("^Library\s+=\s.*$", line, re.I):
+                    if re.match(r"^Library\s+=\s.*$", line, re.I):
                         parts = re.split("\"", line)
                         locRoot = parts[3]
                         syncFind = locRoot
                         syncID = re.split(r"\s+", parts[4])[2]
                         break
 
                 # This file may be missing if the personal OD was logged out of the OneDrive app
@@ -575,15 +575,15 @@
                 if not groupFoldersIni.exists():
                     continue
 
                 cid = None
                 with open(groupFoldersIni, "rt", encoding="utf-16le") as gfh:
                     for line in gfh.readlines():
                         line = line.rstrip()
-                        if re.match("^.*_BaseUri\s+=\s+.*%$", line, re.I):
+                        if re.match(r"^.*_BaseUri\s+=\s+.*%$", line, re.I):
                             cid = line.rsplit("/", 1)[1][:16]
                             folderID = line.split("_", 1)[0]
                             locToWebColl[Path(locRoot) / odFolders[folderID][1]] = (
                                 Path(locRoot) / odFolders[folderID][1], 
                                 f"{webRoot}/{cid}/{line[len(folderID) + 9:]}",
                                 email,
                                 syncID,
```

## pyxll_jupyter/pyxll.py

```diff
@@ -150,17 +150,53 @@
     :param notebook_path: Path of Jupyter notebook to open.
     """
     from pyxll import create_ctp
 
     # Get the Qt Application
     app = _get_qt_app()
 
-    # Create the Jupyter web browser widget
+    
+    # Get the browser args from the config
+    cfg = get_config()
+
+    private_browser = False
+    if cfg.has_option("JUPYTER", "private_browser"):
+        try:
+            private_browser = bool(int(cfg.get("JUPYTER", "private_browser")))
+        except:
+            raise ValueError(f"Unexpected value for JUPYTER.private_browser '{cfg.get('JUPYTER', 'private_browser')}'")
+
+    allow_cookies = True
+    if cfg.has_option("JUPYTER", "allow_cookies"):
+        try:
+            allow_cookies = bool(int(cfg.get("JUPYTER", "allow_cookies")))
+        except:
+            raise ValueError(f"Unexpected value for JUPYTER.allow_cookies '{cfg.get('JUPYTER', 'allow_cookies')}'")
+
+    storage_path = None
+    if cfg.has_option("JUPYTER", "storage_path"):
+        storage_path = cfg.get("JUPYTER", "storage_path")
+        if not os.path.exists(storage_path) or not os.path.isdir(storage_path):
+            raise ValueError(f"Invalid JUPYTER.storage_path '{storage_path}'")
+
+    cache_path = None
+    if cfg.has_option("JUPYTER", "cache_path"):
+        cache_path = cfg.get("JUPYTER", "cache_path")
+        if not os.path.exists(cache_path) or not os.path.isdir(cache_path):
+            raise ValueError(f"Invalid JUPYTER.cache_path '{cache_path}'")
+
+    # Get the notebook args
     kwargs = _get_notebook_kwargs(initial_path=initial_path, notebook_path=notebook_path)
-    widget = JupyterQtWidget(**kwargs)
+
+    # Create the Jupyter web browser widget
+    widget = JupyterQtWidget(private_browser=private_browser,
+                             allow_cookies=allow_cookies,
+                             storage_path=storage_path,
+                             cache_path=cache_path,
+                             **kwargs)
 
     # Show it in a CTP
     create_ctp(widget, width=800)
 
 
 def open_jupyter_notebook_in_browser(*args, initial_path=None, notebook_path=None):
     """Ribbon action function for opening the Jupyter notebook in a web browser.
@@ -226,47 +262,50 @@
     except:
         app = _get_qt_app()
         QMessageBox.warning(None, "Error", "Error setting selection in Excel")
         _log.error("Error setting selection in Excel", exc_info=True)
 
 
 @xl_macro
-def OpenJupyterNotebook(path=None):
+def OpenJupyterNotebook(path=None, browser=False):
     """
     Open a Jupyter notebook in a new task pane.
 
     :param path: Path to Jupyter notebook file or directory.
+    :param browser: Set to true to open in a browser instead of a task pane.
     :return: True on success
     """
     try:
-        if path is not None:
+        if path:
             if not os.path.isabs(path):
                 # Try and get the absolute path relative to the active workbook
                 xl = xl_app(com_package="win32com")
                 wb = xl.ActiveWorkbook
                 if wb is not None and wb.FullName and os.path.exists(wb.FullName):
                     abs_path = os.path.join(os.path.dirname(wb.FullName), path)
                     if os.path.exists(abs_path):
                         path = abs_path
             if not os.path.exists(path):
                 raise RuntimeError(f"Path '{path}' not found.")
 
         initial_path = None
         notebook_path = None
-        if path is not None:
+        if path:
             if os.path.isdir(path):
                 initial_path = path
             elif os.path.isfile(path):
                 notebook_path = path
             else:
-                raise RuntimeError(f"Something is wrong with {path}")
+                raise RuntimeError(f"Something is wrong with the path '{path}'.")
+
+        open_jupyter = open_jupyter_notebook_in_browser if browser else open_jupyter_notebook
 
         # Use schedule_call to actually open the notebook since if this was called
         # from a Workbook.Open macro Excel may not yet be ready to open a CTP.
-        schedule_call(partial(open_jupyter_notebook,
+        schedule_call(partial(open_jupyter,
                                 initial_path=initial_path,
                                 notebook_path=notebook_path))
 
         return True
     except Exception as e:
         xlcAlert(f"Error opening Jupyter notebook: {e}")
         raise
```

## pyxll_jupyter/kernel_managers/__init__.py

```diff
@@ -1,4 +0,0 @@
-00000000: 6672 6f6d 202e 6578 7469 7079 2069 6d70  from .extipy imp
-00000010: 6f72 7420 4578 7465 726e 616c 4950 7974  ort ExternalIPyt
-00000020: 686f 6e4b 6572 6e65 6c4d 616e 6167 6572  honKernelManager
-00000030: 0d0a                                     ..
```

## pyxll_jupyter/widgets/browser.py

```diff
@@ -7,27 +7,53 @@
 
 or
 
 pip install PySide2
 """
 from .qtimports import *
 import logging
+import warnings
 _log = logging.getLogger(__name__)
 
 
 class Browser(QWidget):
     """Tabbed browser widget."""
 
     closed = Signal()
 
-    def __init__(self, parent=None, scale=None):
+    def __init__(self,
+                 parent=None,
+                 scale=None,
+                 private_browser=False,
+                 allow_cookies=True,
+                 cache_path=None,
+                 storage_path=None):
         super().__init__(parent)
-        self.profile = QWebEngineProfile()
         self.tabs = []
 
+        storage_name = "pyxll-jupyter"
+        if private_browser:
+            _log.debug("Using private browser mode.")
+            storage_name = None
+
+        self.profile = QWebEngineProfile(storage_name)
+
+        if allow_cookies:
+            _log.debug(f"Setting browser cookies policy to 'AllowPersistentCookies'.")
+            self.profile.setPersistentCookiesPolicy(QWebEngineProfile.PersistentCookiesPolicy.AllowPersistentCookies)
+
+        if cache_path is not None:
+            self.profile.setCachePath(cache_path)
+
+        if storage_path is not None:
+            self.profile.setPersistentStoragePath(storage_path)
+
+        _log.debug(f"Browser cache path is {self.profile.cachePath()}.")
+        _log.debug(f"Browser persistent storage path is {self.profile.persistentStoragePath()}.")
+
         layout = QVBoxLayout()
         layout.setSpacing(0)
         layout.setContentsMargins(0, 0, 0, 0)
 
         self.tab_widget = TabWidget(self, self.profile, scale=scale)
         self.tab_widget.closed.connect(self.close)
 
@@ -95,15 +121,15 @@
 
     def closeEvent(self, event):
         self.closed.emit()
 
     def create_tab(self, url=None):
         view = WebView(self)
         self.tabs.append(view)
-        page = QWebEnginePage(self.profile, view)
+        page = WebEnginePage(self.profile, view)
         view.setPage(page)
 
         if self.scale:
             view.setZoomFactor(self.scale)
 
         self.addTab(view, "Loading...")
         view.resize(self.currentWidget().size())
@@ -150,14 +176,33 @@
             index = self.indexOf(view)
             if index != -1:
                 self.closeTab(index)
 
         page.windowCloseRequested.connect(close_requested)
 
 
+
+class WebEnginePage(QWebEnginePage):
+
+    def javaScriptConsoleMessage(self, level, message, lineNumber, sourceID):
+        """Log JavaScript errors to the Python log."""
+        pylevel = logging.ERROR
+        try:
+            if level == QWebEnginePage.JavaScriptConsoleMessageLevel.InfoMessageLevel:
+                pylevel = logging.INFO
+            elif level == QWebEnginePage.JavaScriptConsoleMessageLevel.WarningMessageLevel:
+                pylevel = logging.WARNING
+        except AttributeError:
+            warnings.warn("QWebEnginePage.JavaScriptConsoleMessageLevel attribute not found")
+
+        if pylevel >= logging.WARNING:
+            message = f"JavaScript Error (line {lineNumber}, source {sourceID}): {message}"
+        _log.log(pylevel, message)
+
+
 class WebView(QWebEngineView):
     """QWebEngineView that implements 'createWindow' so that
     all new windows are opened in a new tab.
 
     :param owner: QTabWidget containing this view.
     """
```

## pyxll_jupyter/widgets/jupyter.py

```diff
@@ -9,37 +9,50 @@
 import ctypes
 
 _log = logging.getLogger(__name__)
 
 
 class JupyterQtWidget(QWidget):
 
-    def __init__(self, parent=None, scale=None, **kwargs):
+    def __init__(self,
+                 parent=None,
+                 scale=None,
+                 private_browser=False,
+                 allow_cookies=True,
+                 cache_path=None,
+                 storage_path=None,
+                 **kwargs):
         super().__init__(parent)
 
         # proc gets set to the subprocess when the jupyter is started
         self.proc = None
 
         # Get the scale from the window DPI if using Qt5
         if scale is None:
             qt_version = int(qVersion().split(".", 1)[0])
             if qt_version < 6:
                 LOGPIXELSX = 88
                 hwnd = self.winId()
                 if isinstance(hwnd, str):
                     hwnd = int(hwnd, 16 if hwnd.startswith("0x") else 10)
-                hwnd = ctypes.c_size_t(hwnd)
+                hwnd = ctypes.c_size_t(int(hwnd))
                 screen = ctypes.windll.user32.GetDC(hwnd)
                 try:
                     scale = ctypes.windll.gdi32.GetDeviceCaps(screen, LOGPIXELSX) / 96.0
                 finally:
                     ctypes.windll.user32.ReleaseDC(hwnd, screen)
 
         # Create the browser widget
-        self.browser = Browser(self, scale=scale)
+        self.browser = Browser(self,
+                               scale=scale,
+                               private_browser=private_browser,
+                               allow_cookies=allow_cookies,
+                               cache_path=cache_path,
+                               storage_path=storage_path)
+
         self.browser.closed.connect(self.close)
 
         # Add the browser to the widgets layout
         layout = QVBoxLayout()
         layout.addWidget(self.browser)
         self.setLayout(layout)
```

## Comparing `pyxll_jupyter-0.4.1.dist-info/LICENSE.md` & `pyxll_jupyter-0.5.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pyxll_jupyter-0.4.1.dist-info/RECORD` & `pyxll_jupyter-0.5.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 pyxll_jupyter/__init__.py,sha256=mdO9kpbRcBx_UPSU8Zyk6vWvvZnWk-Eand3_Q7ns8RI,496
-pyxll_jupyter/kernel.py,sha256=QkZpm7OIhKSdXAwQzqlVU1JUOcC4oFYYtQvjEYoo9oU,23073
+pyxll_jupyter/kernel.py,sha256=G78VElQfvPugAddbeKVqFPW53Ip6iNhPU9MzSbceHI0,23270
 pyxll_jupyter/magic.py,sha256=KMd_yLfBT6fT-A0EgHGdKJs54hwDmomy6_cQDkmguKo,9105
-pyxll_jupyter/onedrive.py,sha256=97eEScYIsRdHjsH6Iq19ziigg_N9l5NTrvHjN8DgWmo,30195
-pyxll_jupyter/pyxll.py,sha256=rOG_udjC94Fy7XOixklGtrUx-b6Zr9pbncvyq-B2jTo,11056
-pyxll_jupyter/kernel_managers/__init__.py,sha256=BGLY9OvRJSMCQwhpiz7NVG6DL2XeJIE1agExSBFVrH0,50
+pyxll_jupyter/onedrive.py,sha256=GMawVaNo4CsNqfK4ME5FjZhKDaCbLqQaWIa0Os8HqhM,30207
+pyxll_jupyter/pyxll.py,sha256=dDLdCu1tqu-zoop1YVc96U_kaL_SRcRwxNyJVlLj-V0,12765
+pyxll_jupyter/kernel_managers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyxll_jupyter/kernel_managers/extipy.py,sha256=brHXOVCDKFgTfAHORXljrPdPkY9YLMJpKJ4BsM4rlCg,4196
+pyxll_jupyter/kernel_managers/labkm.py,sha256=i1grdPa3syz7rwqP4yRxnQQ8Szz5WMZMzYORcV1bmyU,1708
+pyxll_jupyter/kernel_managers/nbkm.py,sha256=Sus1KuhnIj_XheieKl7g8Q3l_0OitrTJT9EGHEQAOFk,1986
 pyxll_jupyter/provisioning/__init__.py,sha256=SSQgCsR_Jfjwk3FgHRRbIicdnXb2NBXY5q9eya5f_JU,43
 pyxll_jupyter/provisioning/existing.py,sha256=N4ZFoxeyg0zdglNwnDm9KlU1GQ2YxH-cIiSqy_YzHsM,1816
 pyxll_jupyter/resources/browser.png,sha256=fFQoWhmOzguG-mzOSfQw1aBgu54zM7RcUrO8dC1qD60,5704
 pyxll_jupyter/resources/jupyter.png,sha256=H6BglrUs-6rd-Y4kOZxelx4G3cg0yDKbRZNtTQf4KV0,4436
 pyxll_jupyter/resources/ribbon.xml,sha256=w5jIm_Z77Gb7K_NXPMrV1YixcvYEvZIUvt0EPp0zaV8,1658
 pyxll_jupyter/widgets/__init__.py,sha256=1eX2naiOVjgOqQ8UxsKYX1_c_IRAGK7FU-YBSjdGzWs,64
-pyxll_jupyter/widgets/browser.py,sha256=yUiiAl_G2TuZi_bz9Eovt7ViK6Z2NMsHYzvHsakqd-Q,4786
-pyxll_jupyter/widgets/jupyter.py,sha256=cRI2_sWYZBUN5zLtOwj3ozHz934pSrtVTv5Y1GwwphY,1856
+pyxll_jupyter/widgets/browser.py,sha256=0IOUenNgQIzesMi8L2oOylw95rTLifBLQonSiQQAgrw,6557
+pyxll_jupyter/widgets/jupyter.py,sha256=fOKlE2CUVxvxXZG3RYGKSdC0J2jWxWvGx4D_tOTUXoI,2340
 pyxll_jupyter/widgets/qtimports.py,sha256=gHzHDEC-48Q2VIEdD-_PUFws9lNQatESTpjQAqpJNxo,3302
-pyxll_jupyter-0.4.1.dist-info/LICENSE.md,sha256=_Lv_zhFvdAlSe69UkLShEwwRh7pdMDdjzRZcnxMRj2I,1087
-pyxll_jupyter-0.4.1.dist-info/METADATA,sha256=aNh86pySVAIvHl8sgKuTJLRKkQzKoHH4HZ0kU-I7pDc,5262
-pyxll_jupyter-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyxll_jupyter-0.4.1.dist-info/entry_points.txt,sha256=i_TC66oleWSd3gOkTNbNHU6oIqzvfszSGhiU8UNcI9U,187
-pyxll_jupyter-0.4.1.dist-info/top_level.txt,sha256=O8yEET2io_Bn_UyxBhokmuBOysbyrxVg2jGa1OVWQ8M,14
-pyxll_jupyter-0.4.1.dist-info/RECORD,,
+pyxll_jupyter-0.5.0.dist-info/LICENSE.md,sha256=_Lv_zhFvdAlSe69UkLShEwwRh7pdMDdjzRZcnxMRj2I,1087
+pyxll_jupyter-0.5.0.dist-info/METADATA,sha256=dkGiafggpmT-_wt44MNzD6HZWQTb0N8V9g_JtDKAxKM,7411
+pyxll_jupyter-0.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyxll_jupyter-0.5.0.dist-info/entry_points.txt,sha256=i_TC66oleWSd3gOkTNbNHU6oIqzvfszSGhiU8UNcI9U,187
+pyxll_jupyter-0.5.0.dist-info/top_level.txt,sha256=O8yEET2io_Bn_UyxBhokmuBOysbyrxVg2jGa1OVWQ8M,14
+pyxll_jupyter-0.5.0.dist-info/RECORD,,
```

