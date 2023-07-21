# Comparing `tmp/nextflowpy-0.6.1-py3-none-any.whl.zip` & `tmp/nextflowpy-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 29087 bytes, number of entries: 14
--rw-r--r--  2.0 unx      312 b- defN 23-Jul-07 18:58 nextflow/__init__.py
+Zip file size: 29110 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      312 b- defN 23-Jul-21 10:13 nextflow/__init__.py
 -rw-r--r--  2.0 unx     8731 b- defN 23-Jul-07 18:57 nextflow/command.py
 -rw-r--r--  2.0 unx      148 b- defN 23-Feb-09 15:42 nextflow/exceptions.py
 -rw-r--r--  2.0 unx     9133 b- defN 22-Oct-31 17:04 nextflow/execution.py
 -rw-r--r--  2.0 unx     1155 b- defN 23-May-24 20:50 nextflow/io.py
 -rw-r--r--  2.0 unx     3862 b- defN 23-Apr-07 01:28 nextflow/log.py
--rw-r--r--  2.0 unx     3190 b- defN 23-May-24 20:50 nextflow/models.py
+-rw-r--r--  2.0 unx     3228 b- defN 23-Jul-21 10:15 nextflow/models.py
 -rw-r--r--  2.0 unx     7652 b- defN 22-Oct-31 17:06 nextflow/pipeline.py
 -rw-r--r--  2.0 unx     6989 b- defN 22-Oct-31 17:04 nextflow/utils.py
--rw-r--r--  2.0 unx    35148 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    11829 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1079 b- defN 23-Jul-07 19:03 nextflowpy-0.6.1.dist-info/RECORD
-14 files, 89329 bytes uncompressed, 27321 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx    35148 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11967 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1079 b- defN 23-Jul-21 10:35 nextflowpy-0.6.2.dist-info/RECORD
+14 files, 89505 bytes uncompressed, 27344 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: nextflow/pipeline.py
 Comment: 
 
 Filename: nextflow/utils.py
 Comment: 
 
-Filename: nextflowpy-0.6.1.dist-info/LICENSE
+Filename: nextflowpy-0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: nextflowpy-0.6.1.dist-info/METADATA
+Filename: nextflowpy-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: nextflowpy-0.6.1.dist-info/WHEEL
+Filename: nextflowpy-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: nextflowpy-0.6.1.dist-info/top_level.txt
+Filename: nextflowpy-0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: nextflowpy-0.6.1.dist-info/RECORD
+Filename: nextflowpy-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nextflow/__init__.py

```diff
@@ -1,11 +1,11 @@
 from shutil import which
 from .exceptions import NextflowNotInstalledError
 from .command import run, run_and_poll
 
 __author__ = "Sam Ireland"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 if not which("nextflow"):
     raise NextflowNotInstalledError(
         "Nextflow is either not installed, not in PATH, or is not executable."
     )
```

## nextflow/models.py

```diff
@@ -78,25 +78,26 @@
 
     @property
     def full_path(self):
         """The full absolute path to the process execution.
         
         :rtype: ``pathlib.Path``"""
 
-        if not self.path: return ""
+        if not self.path: return None
         return Path(self.execution.path, "work", self.path)
     
 
     def input_data(self, include_path=True):
         """A list of files passed to the process execution as inputs.
         
         :param bool include_path: if ``False``, only filenames returned.
         :type: ``list``"""
         
         inputs = []
+        if not self.path: return []
         run = get_file_text(self.full_path / ".command.run")
         stage = re.search(r"nxf_stage\(\)((.|\n|\r)+?)}", run)
         if not stage: return []
         contents = stage[1]
         inputs = re.findall(r"ln -s (.+?) ", contents)
         if include_path:
             return inputs
```

## Comparing `nextflowpy-0.6.1.dist-info/LICENSE` & `nextflowpy-0.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nextflowpy-0.6.1.dist-info/METADATA` & `nextflowpy-0.6.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextflowpy
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python wrapper around Nextflow.
 Home-page: https://github.com/goodwright/nextflow.py
 Author: Sam Ireland
 Author-email: sam@goodwright.com
 License: GPLv3+
 Keywords: nextflow bioinformatics pipeline
 Platform: UNKNOWN
@@ -111,15 +111,15 @@
 
     >>> pipeline = nextflow.run("pipelines/my-pipeline.nf")
 
 This will return an ``Execution`` object, which represents the pipeline
 execution that just took place (see below for details on this object). You can
 customise the execution with various options:
 
-    >>> execution = pipeline.run(run_path="./rundir", params={"param1": "123"}, profiles=["docker", "test"], version="22.0.1", configs=["env.config"])
+    >>> execution = pipeline.run("my-pipeline.nf", run_path="./rundir", params={"param1": "123"}, profiles=["docker", "test"], version="22.0.1", configs=["env.config"])
 
 * ``run_path`` - The location to run the pipeline from, which by default is just the current working directory.
 
 * ``params`` - A dictionary of parameters to pass to the pipeline as command. In the above example, this would run the pipeline with ``--param1=123``.
 
 * ``profiles`` - A list of Nextflow profiles to use when running the pipeline. These are defined in the ``nextflow.config`` file, and can be used to configure things like the executor to use, or the container engine to use. In the above example, this would run the pipeline with ``-profile docker,test``.
 
@@ -244,18 +244,26 @@
    'published' via some channel, and those which weren't. It is not possible to
    distinguish these once execution is complete, so nextflow.py reports all
    output files, not just those which are 'published'.
 
 Changelog
 ---------
 
+Release 0.6.2
+~~~~~~~~~~~~~
+
+`21st July, 2023`
+
+* Fixed issue in handling no path for process execution input data.
+
+
 Release 0.6.1
 ~~~~~~~~~~~~~
 
-`7 July, 2023`
+`7th July, 2023`
 
 * Added option to specify timezone to Nextflow.
 
 
 Release 0.6.0
 ~~~~~~~~~~~~~
```

## Comparing `nextflowpy-0.6.1.dist-info/RECORD` & `nextflowpy-0.6.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-nextflow/__init__.py,sha256=4Vhw_FLq67wnFF2oGLff-WYhIaEcBd6reTx--D83eR4,312
+nextflow/__init__.py,sha256=vCuuDX0NgDbWo0-DPycL5t-sawl2kNPAJTWqph-eVnA,312
 nextflow/command.py,sha256=bHJ382e43utvSwJUnJhzeEGUcN0Ahx7Fy7HPpTLXrTs,8731
 nextflow/exceptions.py,sha256=ktaEfdLca9Bk52CtJoKYMkGaXLrQ9dZVfYh0QtSC9lk,148
 nextflow/execution.py,sha256=j_wsEuqyZafY3BapmhQBkxAmEJsnq9X-a8ADW3Bs0LA,9133
 nextflow/io.py,sha256=8BuYCRGfsI8_oGRkeY3hjTcT4CC_8eFk21Db-Zo5UIk,1155
 nextflow/log.py,sha256=uuL2bMUmuh2iplkfnX6Ch-LgDiWEcZLNxPvEO761yyU,3862
-nextflow/models.py,sha256=v64scmkKaXpidcLcMZSucpDeGVBBFMZmMaZIng_Vu-0,3190
+nextflow/models.py,sha256=Q57ZRefj1EsNwdILanWpg_KriNgIvq6za4xLoxqAUfI,3228
 nextflow/pipeline.py,sha256=XUCsUtcGW3Ou6resfZJIWGkc5rfAq4gAY-jmZ4md9xo,7652
 nextflow/utils.py,sha256=7jSVHEc57_dZb8ZUNVrpUxIQTs3cp7wLQU9R-r-K6OE,6989
-nextflowpy-0.6.1.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-nextflowpy-0.6.1.dist-info/METADATA,sha256=30xzdG-8ahwEwiY_G5lDUOozQXI14bb0Dn-88_PokPE,11829
-nextflowpy-0.6.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-nextflowpy-0.6.1.dist-info/top_level.txt,sha256=uD97_QD0Jwq__urXtKK-PQMFxiAjWT-y63C2Oi_lad0,9
-nextflowpy-0.6.1.dist-info/RECORD,,
+nextflowpy-0.6.2.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+nextflowpy-0.6.2.dist-info/METADATA,sha256=kSBtb34x7dT2hTcS06-4lCWoX3h5B6JRoeS4V-k7Ztg,11967
+nextflowpy-0.6.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+nextflowpy-0.6.2.dist-info/top_level.txt,sha256=uD97_QD0Jwq__urXtKK-PQMFxiAjWT-y63C2Oi_lad0,9
+nextflowpy-0.6.2.dist-info/RECORD,,
```

