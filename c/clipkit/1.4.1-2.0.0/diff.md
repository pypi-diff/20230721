# Comparing `tmp/clipkit-1.4.1.tar.gz` & `tmp/clipkit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipkit-1.4.1.tar", last modified: Sun Feb 26 23:32:15 2023, max compression
+gzip compressed data, was "clipkit-2.0.0.tar", last modified: Fri Jul 21 17:52:43 2023, max compression
```

## Comparing `clipkit-1.4.1.tar` & `clipkit-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2023-02-26 23:32:15.232237 clipkit-1.4.1/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1078 2020-10-28 23:29:32.000000 clipkit-1.4.1/LICENSE.md
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4988 2023-02-26 23:32:15.232106 clipkit-1.4.1/PKG-INFO
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4284 2023-02-26 23:31:51.000000 clipkit-1.4.1/README.md
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2023-02-26 23:32:15.231236 clipkit-1.4.1/clipkit/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        0 2020-10-04 18:34:57.000000 clipkit-1.4.1/clipkit/__init__.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      124 2020-10-04 18:34:57.000000 clipkit-1.4.1/clipkit/__main__.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1222 2023-02-26 23:31:51.000000 clipkit-1.4.1/clipkit/args_processing.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     3788 2023-02-26 23:31:57.000000 clipkit-1.4.1/clipkit/clipkit.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1454 2020-10-04 18:34:57.000000 clipkit-1.4.1/clipkit/files.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     9397 2023-02-26 23:31:51.000000 clipkit-1.4.1/clipkit/helpers.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     3614 2021-12-07 15:14:07.000000 clipkit-1.4.1/clipkit/modes.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     7640 2023-02-26 23:31:51.000000 clipkit-1.4.1/clipkit/parser.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2259 2023-02-26 23:31:51.000000 clipkit-1.4.1/clipkit/smart_gap_helper.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      437 2023-02-26 23:31:51.000000 clipkit-1.4.1/clipkit/stats.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       21 2023-02-26 23:32:07.000000 clipkit-1.4.1/clipkit/version.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      756 2020-10-04 18:34:57.000000 clipkit-1.4.1/clipkit/warnings.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2285 2023-02-26 23:31:51.000000 clipkit-1.4.1/clipkit/write.py
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2023-02-26 23:32:15.231936 clipkit-1.4.1/clipkit.egg-info/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4988 2023-02-26 23:32:15.000000 clipkit-1.4.1/clipkit.egg-info/PKG-INFO
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      475 2023-02-26 23:32:15.000000 clipkit-1.4.1/clipkit.egg-info/SOURCES.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        1 2023-02-26 23:32:15.000000 clipkit-1.4.1/clipkit.egg-info/dependency_links.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       50 2023-02-26 23:32:15.000000 clipkit-1.4.1/clipkit.egg-info/entry_points.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       46 2023-02-26 23:32:15.000000 clipkit-1.4.1/clipkit.egg-info/requires.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        8 2023-02-26 23:32:15.000000 clipkit-1.4.1/clipkit.egg-info/top_level.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       38 2023-02-26 23:32:15.232278 clipkit-1.4.1/setup.cfg
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1311 2023-02-26 22:41:25.000000 clipkit-1.4.1/setup.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2023-07-21 17:52:43.103650 clipkit-2.0.0/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1078 2020-10-28 23:29:32.000000 clipkit-2.0.0/LICENSE.md
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4977 2023-07-21 17:52:43.103051 clipkit-2.0.0/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4372 2023-07-21 16:57:06.000000 clipkit-2.0.0/README.md
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2023-07-21 17:52:43.099527 clipkit-2.0.0/clipkit/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       25 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/__init__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      124 2020-10-04 18:34:57.000000 clipkit-2.0.0/clipkit/__main__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2012 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/api.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1472 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/args_processing.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5039 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/clipkit.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      103 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/exceptions.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1394 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/files.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     6828 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/helpers.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      193 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/logger.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     3533 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/modes.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2544 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/msa.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     8780 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/parser.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       88 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/settings.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2505 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/smart_gap_helper.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      932 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/stats.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       22 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/version.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      829 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/warnings.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2897 2023-07-21 16:57:06.000000 clipkit-2.0.0/clipkit/write.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2023-07-21 17:52:43.102639 clipkit-2.0.0/clipkit.egg-info/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4977 2023-07-21 17:52:43.000000 clipkit-2.0.0/clipkit.egg-info/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      565 2023-07-21 17:52:43.000000 clipkit-2.0.0/clipkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        1 2023-07-21 17:52:43.000000 clipkit-2.0.0/clipkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       50 2023-07-21 17:52:43.000000 clipkit-2.0.0/clipkit.egg-info/entry_points.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       48 2023-07-21 17:52:43.000000 clipkit-2.0.0/clipkit.egg-info/requires.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        8 2023-07-21 17:52:43.000000 clipkit-2.0.0/clipkit.egg-info/top_level.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       38 2023-07-21 17:52:43.103700 clipkit-2.0.0/setup.cfg
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1225 2023-07-21 16:57:06.000000 clipkit-2.0.0/setup.py
```

### Comparing `clipkit-1.4.1/LICENSE.md` & `clipkit-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clipkit-1.4.1/PKG-INFO` & `clipkit-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: clipkit
-Version: 1.4.1
+Version: 2.0.0
 Summary: Alignment trimming software for phylogenetics.
 Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <p align="center">
   <a href="https://github.com/jlsteenwyk/clipkit">
     <img src="https://raw.githubusercontent.com/JLSteenwyk/ClipKIT/master/docs/_static/img/logo.jpg" alt="Logo" width="400">
@@ -66,24 +64,35 @@
 
 <br />
 
 This documentation covers downloading and installing ClipKIT. Details about each function as well as tutorials for using ClipKIT are available in the [online documentation](https://jlsteenwyk.com/ClipKIT/).
 
 <br />
 
+**Quick Start**
+
+```shell
+# install
+pip install clipkit
+# run
+clipkit input.fa
+```
+
+<br />
+
 **Installation**
 
 **If you are having trouble installing ClipKIT, please contact the lead developer, Jacob L. Steenwyk, via [email](https://jlsteenwyk.com/contact.html) or [twitter](https://twitter.com/jlsteenwyk) to get help.**
 
 To install using *pip*, we strongly recommend building a virtual environment to avoid software dependency issues. To do so, execute the following commands:
 ```shell
 # create virtual environment
-python -m venv .venv
+python -m venv venv
 # activate virtual environment
-source .venv/bin/activate
+source venv/bin/activate
 # install clipkit
 pip install clipkit
 ```
 **Note, the virtual environment must be activated to use *clipkit*.**
 
 After using ClipKIT, you may wish to deactivate your virtual environment and can do so using the following command:
 ```shell
@@ -95,17 +104,17 @@
 
 Similarly, to install from source, we strongly recommend using a virtual environment. To do so, use the following commands:
 ```shell
 # download
 git clone https://github.com/JLSteenwyk/ClipKIT.git
 cd ClipKIT/
 # create virtual environment
-python -m venv .venv
+python -m venv venv
 # activate virtual environment
-source .venv/bin/activate
+source venv/bin/activate
 # install
 make install
 ```
 To deactivate your virtual environment, use the following command:
 ```shell
 # deactivate virtual environment
 deactivate
```

#### html2text {}

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 2.1 Name: clipkit Version: 1.4.1 Summary: Alignment trimming
+Metadata-Version: 2.1 Name: clipkit Version: 2.0.0 Summary: Alignment trimming
 software for phylogenetics. Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk Author-email: jlsteenwyk@gmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Scientific/Engineering Description-Content-Type: text/markdown
-License-File: LICENSE.md
+Python Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
+Engineering Description-Content-Type: text/markdown License-File: LICENSE.md
                                     [Logo]
                      Docs Â· Report_Bug Â· Request_Feature
   [https://img.shields.io/github/actions/workflow/status/JLSteenwyk/ClipKIT/
 ci.yml?branch=master] [https://codecov.io/gh/jlsteenwyk/clipkit/branch/master/
 graph/badge.svg?token=0J49I6441V] [https://img.shields.io/github/contributors/
                    jlsteenwyk/clipkit] [follow_on_Twitter]
                  [https://static.pepy.tech/personalized-badge/
@@ -27,28 +25,30 @@
 al. 2020, PLoS Biology. doi: [10.1371/journal.pbio.3001007](https://
 journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3001007).
 
 ---
 This documentation covers downloading and installing ClipKIT. Details about
 each function as well as tutorials for using ClipKIT are available in the
 [online documentation](https://jlsteenwyk.com/ClipKIT/).
+**Quick Start** ```shell # install pip install clipkit # run clipkit input.fa
+```
 **Installation** **If you are having trouble installing ClipKIT, please contact
 the lead developer, Jacob L. Steenwyk, via [email](https://jlsteenwyk.com/
 contact.html) or [twitter](https://twitter.com/jlsteenwyk) to get help.** To
 install using *pip*, we strongly recommend building a virtual environment to
 avoid software dependency issues. To do so, execute the following commands:
-```shell # create virtual environment python -m venv .venv # activate virtual
-environment source .venv/bin/activate # install clipkit pip install clipkit ```
+```shell # create virtual environment python -m venv venv # activate virtual
+environment source venv/bin/activate # install clipkit pip install clipkit ```
 **Note, the virtual environment must be activated to use *clipkit*.** After
 using ClipKIT, you may wish to deactivate your virtual environment and can do
 so using the following command: ```shell # deactivate virtual environment
 deactivate ```
 Similarly, to install from source, we strongly recommend using a virtual
 environment. To do so, use the following commands: ```shell # download git
 clone https://github.com/JLSteenwyk/ClipKIT.git cd ClipKIT/ # create virtual
-environment python -m venv .venv # activate virtual environment source .venv/
-bin/activate # install make install ``` To deactivate your virtual environment,
-use the following command: ```shell # deactivate virtual environment deactivate
-``` **Note, the virtual environment must be activated to use *clipkit*.**
+environment python -m venv venv # activate virtual environment source venv/bin/
+activate # install make install ``` To deactivate your virtual environment, use
+the following command: ```shell # deactivate virtual environment deactivate ```
+**Note, the virtual environment must be activated to use *clipkit*.**
 To install via anaconda, execute the follwoing command: ``` shell conda install
 -c jlsteenwyk clipkit ``` Visit here for more information: https://
 anaconda.org/jlsteenwyk/clipkit
```

### Comparing `clipkit-1.4.1/README.md` & `clipkit-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,24 +46,35 @@
 
 <br />
 
 This documentation covers downloading and installing ClipKIT. Details about each function as well as tutorials for using ClipKIT are available in the [online documentation](https://jlsteenwyk.com/ClipKIT/).
 
 <br />
 
+**Quick Start**
+
+```shell
+# install
+pip install clipkit
+# run
+clipkit input.fa
+```
+
+<br />
+
 **Installation**
 
 **If you are having trouble installing ClipKIT, please contact the lead developer, Jacob L. Steenwyk, via [email](https://jlsteenwyk.com/contact.html) or [twitter](https://twitter.com/jlsteenwyk) to get help.**
 
 To install using *pip*, we strongly recommend building a virtual environment to avoid software dependency issues. To do so, execute the following commands:
 ```shell
 # create virtual environment
-python -m venv .venv
+python -m venv venv
 # activate virtual environment
-source .venv/bin/activate
+source venv/bin/activate
 # install clipkit
 pip install clipkit
 ```
 **Note, the virtual environment must be activated to use *clipkit*.**
 
 After using ClipKIT, you may wish to deactivate your virtual environment and can do so using the following command:
 ```shell
@@ -75,17 +86,17 @@
 
 Similarly, to install from source, we strongly recommend using a virtual environment. To do so, use the following commands:
 ```shell
 # download
 git clone https://github.com/JLSteenwyk/ClipKIT.git
 cd ClipKIT/
 # create virtual environment
-python -m venv .venv
+python -m venv venv
 # activate virtual environment
-source .venv/bin/activate
+source venv/bin/activate
 # install
 make install
 ```
 To deactivate your virtual environment, use the following command:
 ```shell
 # deactivate virtual environment
 deactivate
```

#### html2text {}

```diff
@@ -17,28 +17,30 @@
 al. 2020, PLoS Biology. doi: [10.1371/journal.pbio.3001007](https://
 journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3001007).
 
 ---
 This documentation covers downloading and installing ClipKIT. Details about
 each function as well as tutorials for using ClipKIT are available in the
 [online documentation](https://jlsteenwyk.com/ClipKIT/).
+**Quick Start** ```shell # install pip install clipkit # run clipkit input.fa
+```
 **Installation** **If you are having trouble installing ClipKIT, please contact
 the lead developer, Jacob L. Steenwyk, via [email](https://jlsteenwyk.com/
 contact.html) or [twitter](https://twitter.com/jlsteenwyk) to get help.** To
 install using *pip*, we strongly recommend building a virtual environment to
 avoid software dependency issues. To do so, execute the following commands:
-```shell # create virtual environment python -m venv .venv # activate virtual
-environment source .venv/bin/activate # install clipkit pip install clipkit ```
+```shell # create virtual environment python -m venv venv # activate virtual
+environment source venv/bin/activate # install clipkit pip install clipkit ```
 **Note, the virtual environment must be activated to use *clipkit*.** After
 using ClipKIT, you may wish to deactivate your virtual environment and can do
 so using the following command: ```shell # deactivate virtual environment
 deactivate ```
 Similarly, to install from source, we strongly recommend using a virtual
 environment. To do so, use the following commands: ```shell # download git
 clone https://github.com/JLSteenwyk/ClipKIT.git cd ClipKIT/ # create virtual
-environment python -m venv .venv # activate virtual environment source .venv/
-bin/activate # install make install ``` To deactivate your virtual environment,
-use the following command: ```shell # deactivate virtual environment deactivate
-``` **Note, the virtual environment must be activated to use *clipkit*.**
+environment python -m venv venv # activate virtual environment source venv/bin/
+activate # install make install ``` To deactivate your virtual environment, use
+the following command: ```shell # deactivate virtual environment deactivate ```
+**Note, the virtual environment must be activated to use *clipkit*.**
 To install via anaconda, execute the follwoing command: ``` shell conda install
 -c jlsteenwyk clipkit ``` Visit here for more information: https://
 anaconda.org/jlsteenwyk/clipkit
```

### Comparing `clipkit-1.4.1/clipkit/modes.py` & `clipkit-2.0.0/clipkit/modes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,102 @@
-import logging
-
 from enum import Enum
+from typing import TYPE_CHECKING
+from .logger import log_file_logger
+
+if TYPE_CHECKING:
+    from Bio.Align import MultipleSeqAlignment
+    from .msa import MSA
 
-logger = logging.getLogger("clipkit.clipkit")
+
+class SiteClassificationType(Enum):
+    parsimony_informative = "parsimony-informative"
+    constant = "constant"
+    singleton = "singleton"
+    other = "other"
 
 
 class TrimmingMode(Enum):
     gappy = "gappy"
     smart_gap = "smart-gap"
     kpi = "kpi"
     kpi_gappy = "kpi-gappy"
     kpi_smart_gap = "kpi-smart-gap"
     kpic = "kpic"
     kpic_gappy = "kpic-gappy"
     kpic_smart_gap = "kpic-smart-gap"
 
 
-def shouldKeep(
+def should_keep_site(
     mode: TrimmingMode,
-    parsimony_informative: bool,
-    constant_site: bool,
+    site_classification_type: "SiteClassificationType",
     gappyness: float,
     gaps: float,
-):
-    """
-    Determine if a site should be kept or not
-    """
+) -> bool:
     if mode == TrimmingMode.kpi_gappy:
-        return gappyness <= gaps and parsimony_informative
+        return (
+            gappyness <= gaps
+            and site_classification_type == SiteClassificationType.parsimony_informative
+        )
     elif mode == TrimmingMode.gappy:
         return gappyness <= gaps
     elif mode == TrimmingMode.kpi:
-        return parsimony_informative
+        return site_classification_type == SiteClassificationType.parsimony_informative
     elif mode == TrimmingMode.kpic:
-        return parsimony_informative or constant_site
+        return (
+            site_classification_type == SiteClassificationType.parsimony_informative
+            or site_classification_type == SiteClassificationType.constant
+        )
     elif mode == TrimmingMode.kpic_gappy:
-        return gappyness <= gaps and (parsimony_informative or constant_site)
+        return gappyness <= gaps and (
+            site_classification_type == SiteClassificationType.parsimony_informative
+            or site_classification_type == SiteClassificationType.constant
+        )
     elif mode == TrimmingMode.smart_gap:
         return round(gappyness, 4) < gaps
     elif mode == TrimmingMode.kpic_smart_gap:
-        return round(gappyness, 4) < gaps and (parsimony_informative or constant_site)
+        return round(gappyness, 4) < gaps and (
+            site_classification_type == SiteClassificationType.parsimony_informative
+            or site_classification_type == SiteClassificationType.constant
+        )
     elif mode == TrimmingMode.kpi_smart_gap:
-        return round(gappyness, 4) < gaps and parsimony_informative
+        return (
+            round(gappyness, 4) < gaps
+            and site_classification_type == SiteClassificationType.parsimony_informative
+        )
 
 
 def trim(
     gappyness: float,
-    parsimony_informative: bool,
-    constant_site: bool,
-    keepD: dict,
-    trimD: dict,
+    site_classification_type: "SiteClassificationType",
+    site_classification_counts: dict,
+    keep_msa: "MSA",
+    trim_msa: "MSA",
     alignment_position: int,
     gaps: float,
-    alignment,
+    alignment: "MultipleSeqAlignment",
     mode: TrimmingMode,
     use_log: bool,
-):
-    """
-    Trims according to the mode kpi-gappy wherein only parismony informative
-    sites are kept. Additionally, sites that are sufficiently gappy are removed
-
-    Arguments
-    ---------
-    argv: gappyness
-        a float value for what fraction of characters are gaps
-    argv: parsimony_informative
-        boolean for whether or not a site is parsimony informative
-    argv: keepD
-        dictionary for sites that will be kept in the resulting alignment
-    argv: trimD
-        dictionary for sites that will be removed from the final alignment
-    argv: i
-        i is the position in the alignment that the loop is currently in
-    argv: gaps
-        gaps threshold to determine if a position is too gappy or not
-    argv: alignment
-        biopython multiple sequence alignment object
-    """
-    # save to keepD
-    if shouldKeep(mode, parsimony_informative, constant_site, gappyness, gaps):
+) -> tuple["MSA", "MSA"]:
+    if should_keep_site(mode, site_classification_type, gappyness, gaps):
+        site_classification_counts[site_classification_type] += 1
         for entry in alignment:
-            keepD[entry.description][alignment_position] = entry.seq._data[alignment_position:alignment_position+1]
+            new_value = entry.seq._data[alignment_position : alignment_position + 1]
+            keep_msa.set_entry_sequence_at_position(
+                entry.description, alignment_position, new_value
+            )
         if use_log:
-            if constant_site:
-                logger.debug(f"{str(alignment_position + 1)} keep Const {gappyness}")
-            elif parsimony_informative:
-                logger.debug(f"{str(alignment_position + 1)} keep PI {gappyness}")
-            else:
-                logger.debug(
-                    f"{str(alignment_position + 1)} keep nConst,nPI {gappyness}"
-                )
-    # save to trimD
+            log_file_logger.debug(
+                f"{str(alignment_position + 1)} keep {site_classification_type.value} {gappyness}"
+            )
     else:
-        for entry in alignment:
-            trimD[entry.description][alignment_position] = entry.seq._data[alignment_position:alignment_position+1]
-        if use_log:
-            if constant_site:
-                logger.debug(f"{str(alignment_position + 1)} trim Const {gappyness}")
-            elif parsimony_informative:
-                logger.debug(f"{str(alignment_position + 1)} trim PI {gappyness}")
-            else:
-                logger.debug(
-                    f"{str(alignment_position + 1)} trim nConst,nPI {gappyness}"
+        if trim_msa is not None:
+            for entry in alignment:
+                new_value = entry.seq._data[alignment_position : alignment_position + 1]
+                trim_msa.set_entry_sequence_at_position(
+                    entry.description, alignment_position, new_value
                 )
+        if use_log:
+            log_file_logger.debug(
+                f"{str(alignment_position + 1)} trim {site_classification_type.value} {gappyness}"
+            )
 
-    return keepD, trimD
+    return keep_msa, trim_msa
```

### Comparing `clipkit-1.4.1/clipkit/parser.py` & `clipkit-2.0.0/clipkit/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import sys
 import textwrap
 
 from argparse import (
     ArgumentParser,
-    RawTextHelpFormatter,
     SUPPRESS,
     RawDescriptionHelpFormatter,
 )
 
 from .helpers import SeqType
-from .modes import TrimmingMode
 from .files import FileFormat
+from .modes import TrimmingMode
 from .version import __version__
 
-def create_parser():
+
+def create_parser() -> ArgumentParser:
     parser = ArgumentParser(
         add_help=False,
         formatter_class=RawDescriptionHelpFormatter,
         usage=SUPPRESS,
         description=textwrap.dedent(
             f"""\
-              _____ _ _       _  _______ _______ 
+              _____ _ _       _  _______ _______  
              / ____| (_)     | |/ /_   _|__   __|
             | |    | |_ _ __ | ' /  | |    | |   
             | |    | | | '_ \|  <   | |    | |   
             | |____| | | |_) | . \ _| |_   | |   
              \_____|_|_| .__/|_|\_\_____|  |_|   
                        | |                       
                        |_|  
@@ -32,37 +32,37 @@
         Version: {__version__}
         Citation: Steenwyk et al. 2020, PLOS Biology. doi: 10.1371/journal.pbio.3001007
         https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3001007
 
         ClipKIT trims multiple sequence alignments and maintains phylogenetically informative sites.
 
         Usage: clipkit <input> [optional arguments]
-        """
+        """  # noqa
         ),
     )
 
     # if no arguments are given, print help and exit
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit()
 
-    ## required arguments
+    # required arguments
     required = parser.add_argument_group(
         "required arguments",
         description=textwrap.dedent(
             """\
         <input>                                     input file
                                                     (must be the first argument)
         """
         ),
     )
 
     required.add_argument("input", type=str, help=SUPPRESS)
 
-    ## optional arguments
+    # optional arguments
     optional = parser.add_argument_group(
         "optional arguments",
         description=textwrap.dedent(
             """\
         -o, --output <output_file_name>             output file name 
                                                     (default: input file named with '.clipkit' suffix)
 
@@ -74,29 +74,35 @@
                     kpi,
                     kpi-smart-gap,
                     kpi-gappy>                      
                                                     
         -g, --gaps <threshold_of_gaps>              specifies gaps threshold
                                                     (default: 0.9)
 
+        -gc, --gap_characters <string_of_gap_chars> specifies gap characters used in input file
+                                                    (default for aa: "-?*XxNn"
+                                                     default for nt: "-?*Xx")
+
         -if, --input_file_format <file_format>      specifies input file format
                                                     (default: auto-detect)    
 
         -s, --sequence_type <nt, aa>                specifies sequence type of input file
                                                     (default: auto-detect)
 
         -of, --output_file_format <file_format>     specifies output file format
                                                     (default: same as input file format)
 
         -l, --log                                   creates a log file
                                                     (input file named with '.log' suffix)
 
         -c, --complementary                         creates complementary alignment of trimmed sequences
                                                     (input file named with '.log' suffix)
- 
+
+        -q, --quiet                                 disables all logging to stdout
+
         -h, --help                                  help message
         -v, --version                               print version
 
         -------------------------------------
         | Detailed explanation of arguments | 
         -------------------------------------
         Modes
@@ -111,14 +117,20 @@
 
         Gaps
             Positions with gappyness greater than threshold will be trimmed. 
             Must be between 0 and 1. (Default: 0.9). This argument is ignored
             when using the kpi and kpic mdoes of trimming as well as an 
             iteration of trimming that uses smart-gap.
 
+        Gap characters
+            Specifies gap characters used in the input file. All gap characters
+            should have a quotes (single or double) surrounding them. For example,
+            "NnXx-?" would specify that "N", "n", "X", "x", "-", and "?" are
+            gap characters.
+
         Sequence type
             Specifies the type of sequences in the input file. Valid options
             include aa or nt for amino acids and nucleotides. This argument
             is case insensitive. This matters for what characters are
             considered gaps. For amino acids, -, ?, *, and X are considered
             gaps. For nucleotide sequences, the same characters are
             considered gaps as well as N.
@@ -135,49 +147,81 @@
             - Column 2 reports if the site was trimmed or kept (trim and keep, respectively),
             - Column 3 reports if the site is a parsimony informative site or not (PI and nPI, respectively), or
               a constant site or not (Const and nConst, respectively), or neither (nConst, nPI)
             - Column 4 reports the gappyness of the the position (number of gaps / entries in alignment)
 
         Complementary
             Creates an alignment file of only the trimmed sequences
-        """
+        """  # noqa
         ),
     )
 
     optional.add_argument(
-        "-o", "--output", help=SUPPRESS, metavar="output"
+        "-q",
+        "--quiet",
+        help=SUPPRESS,
+        action="store_true",
+        required=False,
     )
 
+    optional.add_argument("-o", "--output", help=SUPPRESS, metavar="output")
+
     mode_choices = [mode.value for mode in TrimmingMode]
     optional.add_argument(
-        "-m", "--mode", help=SUPPRESS, nargs="?", choices=mode_choices,
+        "-m",
+        "--mode",
+        help=SUPPRESS,
+        nargs="?",
+        choices=mode_choices,
     )
 
-    seq_type_choices = [seq.value.upper() for seq in SeqType] + [seq.value.lower() for seq in SeqType]
+    seq_type_choices = [seq.value.upper() for seq in SeqType] + [
+        seq.value.lower() for seq in SeqType
+    ]
     optional.add_argument(
-        "-s", "--sequence_type", help=SUPPRESS, nargs="?", choices=seq_type_choices,
+        "-s",
+        "--sequence_type",
+        help=SUPPRESS,
+        nargs="?",
+        choices=seq_type_choices,
     )
 
     optional.add_argument(
-        "-h", "--help", action="help", help=SUPPRESS,
+        "-h",
+        "--help",
+        action="help",
+        help=SUPPRESS,
     )
 
     optional.add_argument(
-        "-v", "--version", action="version", version=f"clipkit {__version__}", help=SUPPRESS,
+        "-v",
+        "--version",
+        action="version",
+        version=f"clipkit {__version__}",
+        help=SUPPRESS,
     )
 
     optional.add_argument(
         "-g",
         "--gaps",
         type=float,
         required=False,
         help=SUPPRESS,
         metavar="fraction of gaps",
     )
 
+    optional.add_argument(
+        "-gc",
+        "--gap_characters",
+        type=str,
+        required=False,
+        help=SUPPRESS,
+        metavar="gap characters",
+    )
+
     file_format_choices = [file_format.value.lower() for file_format in FileFormat]
     optional.add_argument(
         "-if",
         "--input_file_format",
         type=str,
         required=False,
         choices=file_format_choices,
@@ -192,15 +236,23 @@
         required=False,
         choices=file_format_choices,
         help=SUPPRESS,
         metavar="",
     )
 
     optional.add_argument(
-        "-l", "--log", action="store_true", required=False, help=SUPPRESS,
+        "-l",
+        "--log",
+        action="store_true",
+        required=False,
+        help=SUPPRESS,
     )
 
     optional.add_argument(
-        "-c", "--complementary", action="store_true", required=False, help=SUPPRESS,
+        "-c",
+        "--complementary",
+        action="store_true",
+        required=False,
+        help=SUPPRESS,
     )
 
     return parser
```

### Comparing `clipkit-1.4.1/clipkit/smart_gap_helper.py` & `clipkit-2.0.0/clipkit/smart_gap_helper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 from collections import Counter
 
+from Bio.Align import MultipleSeqAlignment
 import numpy as np
+from tqdm import tqdm
+
+from .helpers import report_column_features
+from .logger import logger
 
-from .helpers import get_sequence_at_position_and_report_features
 
 def smart_gap_threshold_determination(
-    alignment, char
+    alignment: MultipleSeqAlignment, gap_chars: list, quiet: bool
 ) -> float:
-    # loop through alignment and determine site-wise gappyness
     alignment_length = alignment.get_alignment_length()
 
     # get distribution of gaps rounded to the fourth decimal place
-    gaps_dist = get_gaps_distribution(alignment, alignment_length, char)
-    
+    gaps_dist = get_gaps_distribution(alignment, alignment_length, gap_chars, quiet)
+
     # count freq of gaps and convert to sorted np array
     gaps_arr = count_and_sort_gaps(gaps_dist)
 
     # calculate gap-to-gap slope
     slopes = gap_to_gap_slope(gaps_arr, alignment_length)
 
-    # find the greatest difference in slopes and set
-    # gaps to y1
+    # find the greatest difference in slopes and set gaps to y1
     return greatest_diff_in_slopes(slopes, gaps_arr)
 
-def greatest_diff_in_slopes(
-    slopes,
-    gaps_arr
-):
+
+def greatest_diff_in_slopes(slopes: list[float], gaps_arr: np.array) -> float:
     diffs = []
     # if there is only one slope, use that value to determine
     # the threshold. Otherwise, calculate the greatest difference
     # in slopes
     if len(slopes) > 1:
         for val0, val1 in zip(slopes, slopes[1:]):
-            diff0 = abs(val0-val1)
+            diff0 = abs(val0 - val1)
             diffs.append(diff0)
     elif len(slopes) == 0:
         return 1
     else:
         diffs = slopes
     return gaps_arr[diffs.index(max(diffs))][0]
 
-def gap_to_gap_slope(
-    gaps_arr, alignment_length
-):
-    sum_sites_current = gaps_arr[0][1]/alignment_length
+
+def gap_to_gap_slope(gaps_arr: np.array, alignment_length: int) -> list[float]:
+    sum_sites_current = gaps_arr[0][1] / alignment_length
     sum_sites_previous = 0
     slopes = []
     for previous, current in zip(gaps_arr, gaps_arr[1:]):
-        sum_sites_previous+=(previous[1]/alignment_length)
-        sum_sites_current+=(current[1]/alignment_length)
-        slopes.append(abs((sum_sites_current-sum_sites_previous)/(current[0] - previous[0])))
+        sum_sites_previous += previous[1] / alignment_length
+        sum_sites_current += current[1] / alignment_length
+        slopes.append(
+            abs((sum_sites_current - sum_sites_previous) / (current[0] - previous[0]))
+        )
     # only use first half of slopes
-    return slopes[:(len(slopes)//2)]
+    return slopes[: (len(slopes) // 2)]
 
-def get_gaps_distribution(alignment, alignment_length: int, char):
+
+def get_gaps_distribution(
+    alignment: MultipleSeqAlignment, alignment_length: int, gap_chars: list, quiet: bool
+) -> list[float]:
     gaps_dist = []
-    for i in range(0, alignment_length):
-        _, gappyness = get_sequence_at_position_and_report_features(alignment, i, char)
+    for i in tqdm(range(0, alignment_length), disable=quiet, postfix="smart-gap"):
+        _, gappyness = report_column_features(alignment, i, gap_chars)
         gappyness = round(gappyness, 4)
         gaps_dist.append(gappyness)
+
     return gaps_dist
 
-def count_and_sort_gaps(gaps_dist: list):
+
+def count_and_sort_gaps(gaps_dist: list) -> list:
     gaps_count = dict(Counter(gaps_dist))
     gaps_arr = np.array(list(gaps_count.items()))
-    return gaps_arr[np.argsort(-gaps_arr[:,0])].tolist()
+    return gaps_arr[np.argsort(-gaps_arr[:, 0])].tolist()
```

### Comparing `clipkit-1.4.1/clipkit/write.py` & `clipkit-2.0.0/clipkit/write.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,122 @@
 import textwrap
 import time
+from .logger import logger
+from .stats import TrimmingStats
 
+from typing import TYPE_CHECKING
 
-def write_processing_aln():
-    """
-    Function to print out processing alignment
-    """
-    print(
+if TYPE_CHECKING:
+    from .files import FileFormat
+    from .helpers import SeqType
+    from .modes import TrimmingMode
+
+
+def write_processing_aln() -> None:
+    logger.info(
         textwrap.dedent(
-            f"""\
+            """\
         
         ------------------------
         | Processing Alignment |
         ------------------------
-    """
+    """  # noqa
         )
     )
 
 
 def write_user_args(
-    inFile, inFileFormat, outFile, outFileFormat, char, gaps, mode, complement, use_log
-):
-    if char.value == "nt":
-        seq_type = "Nucleotides"
+    in_file_name: str,
+    in_file_format: "FileFormat",
+    out_file_name: str,
+    out_file_format: "FileFormat",
+    seq_type: "SeqType",
+    gaps: float,
+    gap_chars: list,
+    mode: "TrimmingMode",
+    complement: bool,
+    use_log: bool,
+) -> None:
+    if seq_type.value == "nt":
+        seq_type_name = "Nucleotides"
     else:
-        seq_type = "Protein"
+        seq_type_name = "Protein"
     """
     Function to print user arguments to stdout
     """
-    print(
+    logger.info(
         textwrap.dedent(
             f"""\
+
     -------------
     | Arguments |
     -------------
-    Input file: {inFile} (format: {inFileFormat.value})
-    Output file: {outFile} (format: {outFileFormat.value})
-    Sequence type: {seq_type}
+    Input file: {in_file_name} (format: {in_file_format.value})
+    Output file: {out_file_name} (format: {out_file_format.value})
+    Sequence type: {seq_type_name}
     Gaps threshold: {gaps}
+    Gap characters: {gap_chars}
     Trimming mode: {mode.value}
     Create complementary output: {complement}
     Create log file: {use_log}
-    """
+    """  # noqa
         )
     )
 
 
-def write_output_files_message(outFile, complement, use_log):
+def write_output_files_message(
+    out_file_name: str, complement: bool, use_log: bool
+) -> None:
     """
     Function to print out that the output files are being written
     """
-    print(
+    logger.info(
         textwrap.dedent(
             f"""\
 
 
         ------------------------
         | Writing output files |
         ------------------------
-        trimmed alignment: {outFile}
-        complement file: {outFile + '.complement' if complement else False}
-        log file: {outFile + '.log' if use_log else False}
+        trimmed alignment: {out_file_name}
+        complement file: {out_file_name + '.complement' if complement else False}
+        log file: {out_file_name + '.log' if use_log else False}
     """
         )
     )
 
 
-def write_output_stats(stats: dict, start_time):
+def write_output_stats(stats: "TrimmingStats", start_time: float) -> None:
     """
     Function to print out output statistics
     """
-    print(
+    logger.info(
         textwrap.dedent(
             f"""\
 
         ---------------------
         | Output Statistics |
         ---------------------
-        Number of sites kept: {stats["output_length"]}
-        Number of sites trimmed: {stats["trimmed_length"]}
+        Number of sites kept: {stats.output_length}
+        Number of sites trimmed: {stats.trimmed_length}
 
-        Percentage of alignment trimmed: {stats["trimmed_percentage"]}%
+        Percentage of alignment trimmed: {stats.trimmed_percentage}%
 
         Execution time: {round(time.time() - start_time, 3)}s
     """
         )
     )
 
-def write_determining_smart_gap_threshold():
+
+def write_determining_smart_gap_threshold() -> None:
     """
     Function to inform using that the smart-gap threshold is being determined
     """
-    print(
+    logger.info(
         textwrap.dedent(
-            f"""\
-
-        Determining smart-gap threshold...
-    """
+            """\
+        -----------------------------------
+        | Determining smart-gap threshold |
+        -----------------------------------
+        """
         )
     )
```

### Comparing `clipkit-1.4.1/clipkit.egg-info/PKG-INFO` & `clipkit-2.0.0/clipkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: clipkit
-Version: 1.4.1
+Version: 2.0.0
 Summary: Alignment trimming software for phylogenetics.
 Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <p align="center">
   <a href="https://github.com/jlsteenwyk/clipkit">
     <img src="https://raw.githubusercontent.com/JLSteenwyk/ClipKIT/master/docs/_static/img/logo.jpg" alt="Logo" width="400">
@@ -66,24 +64,35 @@
 
 <br />
 
 This documentation covers downloading and installing ClipKIT. Details about each function as well as tutorials for using ClipKIT are available in the [online documentation](https://jlsteenwyk.com/ClipKIT/).
 
 <br />
 
+**Quick Start**
+
+```shell
+# install
+pip install clipkit
+# run
+clipkit input.fa
+```
+
+<br />
+
 **Installation**
 
 **If you are having trouble installing ClipKIT, please contact the lead developer, Jacob L. Steenwyk, via [email](https://jlsteenwyk.com/contact.html) or [twitter](https://twitter.com/jlsteenwyk) to get help.**
 
 To install using *pip*, we strongly recommend building a virtual environment to avoid software dependency issues. To do so, execute the following commands:
 ```shell
 # create virtual environment
-python -m venv .venv
+python -m venv venv
 # activate virtual environment
-source .venv/bin/activate
+source venv/bin/activate
 # install clipkit
 pip install clipkit
 ```
 **Note, the virtual environment must be activated to use *clipkit*.**
 
 After using ClipKIT, you may wish to deactivate your virtual environment and can do so using the following command:
 ```shell
@@ -95,17 +104,17 @@
 
 Similarly, to install from source, we strongly recommend using a virtual environment. To do so, use the following commands:
 ```shell
 # download
 git clone https://github.com/JLSteenwyk/ClipKIT.git
 cd ClipKIT/
 # create virtual environment
-python -m venv .venv
+python -m venv venv
 # activate virtual environment
-source .venv/bin/activate
+source venv/bin/activate
 # install
 make install
 ```
 To deactivate your virtual environment, use the following command:
 ```shell
 # deactivate virtual environment
 deactivate
```

#### html2text {}

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 2.1 Name: clipkit Version: 1.4.1 Summary: Alignment trimming
+Metadata-Version: 2.1 Name: clipkit Version: 2.0.0 Summary: Alignment trimming
 software for phylogenetics. Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk Author-email: jlsteenwyk@gmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Scientific/Engineering Description-Content-Type: text/markdown
-License-File: LICENSE.md
+Python Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
+Engineering Description-Content-Type: text/markdown License-File: LICENSE.md
                                     [Logo]
                      Docs Â· Report_Bug Â· Request_Feature
   [https://img.shields.io/github/actions/workflow/status/JLSteenwyk/ClipKIT/
 ci.yml?branch=master] [https://codecov.io/gh/jlsteenwyk/clipkit/branch/master/
 graph/badge.svg?token=0J49I6441V] [https://img.shields.io/github/contributors/
                    jlsteenwyk/clipkit] [follow_on_Twitter]
                  [https://static.pepy.tech/personalized-badge/
@@ -27,28 +25,30 @@
 al. 2020, PLoS Biology. doi: [10.1371/journal.pbio.3001007](https://
 journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3001007).
 
 ---
 This documentation covers downloading and installing ClipKIT. Details about
 each function as well as tutorials for using ClipKIT are available in the
 [online documentation](https://jlsteenwyk.com/ClipKIT/).
+**Quick Start** ```shell # install pip install clipkit # run clipkit input.fa
+```
 **Installation** **If you are having trouble installing ClipKIT, please contact
 the lead developer, Jacob L. Steenwyk, via [email](https://jlsteenwyk.com/
 contact.html) or [twitter](https://twitter.com/jlsteenwyk) to get help.** To
 install using *pip*, we strongly recommend building a virtual environment to
 avoid software dependency issues. To do so, execute the following commands:
-```shell # create virtual environment python -m venv .venv # activate virtual
-environment source .venv/bin/activate # install clipkit pip install clipkit ```
+```shell # create virtual environment python -m venv venv # activate virtual
+environment source venv/bin/activate # install clipkit pip install clipkit ```
 **Note, the virtual environment must be activated to use *clipkit*.** After
 using ClipKIT, you may wish to deactivate your virtual environment and can do
 so using the following command: ```shell # deactivate virtual environment
 deactivate ```
 Similarly, to install from source, we strongly recommend using a virtual
 environment. To do so, use the following commands: ```shell # download git
 clone https://github.com/JLSteenwyk/ClipKIT.git cd ClipKIT/ # create virtual
-environment python -m venv .venv # activate virtual environment source .venv/
-bin/activate # install make install ``` To deactivate your virtual environment,
-use the following command: ```shell # deactivate virtual environment deactivate
-``` **Note, the virtual environment must be activated to use *clipkit*.**
+environment python -m venv venv # activate virtual environment source venv/bin/
+activate # install make install ``` To deactivate your virtual environment, use
+the following command: ```shell # deactivate virtual environment deactivate ```
+**Note, the virtual environment must be activated to use *clipkit*.**
 To install via anaconda, execute the follwoing command: ``` shell conda install
 -c jlsteenwyk clipkit ``` Visit here for more information: https://
 anaconda.org/jlsteenwyk/clipkit
```

### Comparing `clipkit-1.4.1/setup.py` & `clipkit-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 CLASSIFIERS = [
-    'Operating System :: OS Independent',
-    'Intended Audience :: Science/Research',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Topic :: Scientific/Engineering',
+    "Operating System :: OS Independent",
+    "Intended Audience :: Science/Research",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Topic :: Scientific/Engineering",
 ]
 
-REQUIRES = ["biopython>=1.79", "numpy>=1.18", "tqdm>=4.45", "cython"]
+REQUIRES = ["biopython>=1.81", "numpy>=1.24.0", "tqdm>=4.45", "cython"]
 
 setup(
     name="clipkit",
     description="Alignment trimming software for phylogenetics.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jacob L. Steenwyk",
@@ -36,8 +34,8 @@
     include_package_data=True,
     install_requires=REQUIRES,
 )
 
 ## push new version to pypi
 # rm -rf dist
 # python3 setup.py sdist bdist_wheel --universal
-# twine upload dist/* -r pypi
+# twine upload dist/* -r pypi
```

