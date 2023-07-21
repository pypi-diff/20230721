# Comparing `tmp/RecruitmentCurveFitting-1.1.2-py2.py3-none-any.whl.zip` & `tmp/RecruitmentCurveFitting-1.1.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 106350 bytes, number of entries: 12
+Zip file size: 106507 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    35821 b- defN 23-May-27 05:45 RecruitmentCurveFitting/COPYING
--rw-r--r--  2.0 unx    18750 b- defN 23-May-30 15:02 RecruitmentCurveFitting/CurveFitting.py
+-rw-r--r--  2.0 unx    18938 b- defN 23-Jul-21 16:10 RecruitmentCurveFitting/CurveFitting.py
 -rw-r--r--  2.0 unx    28640 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting/RecruitmentCurves.py
--rw-r--r--  2.0 unx     4252 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting/__init__.py
+-rw-r--r--  2.0 unx     4314 b- defN 23-Jul-21 16:10 RecruitmentCurveFitting/__init__.py
 -rw-r--r--  2.0 unx     7820 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting/__main__.py
 -rw-r--r--  2.0 unx     1491 b- defN 23-May-27 02:43 RecruitmentCurveFitting/example-data1.txt
 -rw-r--r--  2.0 unx     2291 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-data2.txt
 -rw-r--r--  2.0 unx   208425 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-waveforms.csv
--rw-r--r--  2.0 unx     2529 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting-1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1135 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting-1.1.2.dist-info/RECORD
-12 files, 311288 bytes uncompressed, 104410 bytes compressed:  66.5%
+-rw-r--r--  2.0 unx     2650 b- defN 23-Jul-21 16:10 RecruitmentCurveFitting-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-21 16:10 RecruitmentCurveFitting-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-21 16:10 RecruitmentCurveFitting-1.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1135 b- defN 23-Jul-21 16:10 RecruitmentCurveFitting-1.1.3.dist-info/RECORD
+12 files, 311659 bytes uncompressed, 104567 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: RecruitmentCurveFitting/example-data2.txt
 Comment: 
 
 Filename: RecruitmentCurveFitting/example-waveforms.csv
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.2.dist-info/METADATA
+Filename: RecruitmentCurveFitting-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.2.dist-info/WHEEL
+Filename: RecruitmentCurveFitting-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.2.dist-info/top_level.txt
+Filename: RecruitmentCurveFitting-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.2.dist-info/RECORD
+Filename: RecruitmentCurveFitting-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RecruitmentCurveFitting/CurveFitting.py

```diff
@@ -443,14 +443,24 @@
 		return x[ indexOfYMax ], y[ indexOfYMax ]
 
 	@staticmethod
 	def Evaluate( x, *params ): raise TypeError( 'cannot use the abstract base class in this way - subclass must define method self.Evaluate(x, ...) with named parameters' )
 	@staticmethod
 	def Initialize( x, y ): raise TypeError( 'cannot use the abstract base class in this way - subclass must define method self.Initialize(x, y)' )
 
+	@classmethod
+	def AddMethod( cls, func ):
+		"""
+		Use this as a function decorator, to add a function
+		as a new class method.
+		"""
+		setattr( cls, func.__name__, func )
+		return func
+
+
 def SavePDF( filename, figures='all' ):
 	import matplotlib.pyplot as plt
 	if figures == 'all': figures = plt.get_fignums()
 	from matplotlib.backends.backend_pdf import PdfPages
 	with PdfPages( filename ) as pdf:
 		for figure in figures: pdf.savefig( figure )
```

## RecruitmentCurveFitting/__init__.py

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 
 # $BEGIN_RECRUITMENTCURVEFITTING_LICENSE$
 # 
 # This file is part of the RecruitmentCurveFitting project, a Python
 # package for fitting sigmoid and bell-shaped functions to EMG
 # recruitment-curve measurements.
 # 
@@ -24,52 +24,48 @@
 # along with this program. If not, see http://www.gnu.org/licenses/ .
 # 
 # $END_RECRUITMENTCURVEFITTING_LICENSE$
 
 __all__ = [ 'Cite' ]
 import os, sys, ast
 from . import RecruitmentCurves
-__doc__ = RecruitmentCurves.__doc__
+__doc__ = RecruitmentCurves.__doc__  # the main docstring for the Python API is in the RecruitmentCurves submodule
 __all__ += RecruitmentCurves.__all__
 from .RecruitmentCurves import *
 
 CITATION_INFO = """
 If you use this software in your research, your report should cite the article
 in which this approach was introduced, as follows:
 
 - McKinnon ML, Hill NJ, Carp JS, Dellenbach B & Thompson AK (2023).
   Methods for automated delineation and assessment of EMG responses evoked by
   peripheral nerve stimulation in diagnostic and closed-loop therapeutic
-  applications.
-  Journal of Neural Engineering (in press)
+  applications.  Journal of Neural Engineering 20(4):046012.
   https://doi.org/10.1088/1741-2552/ace6fb
-    
+
 The corresponding BibTeX entry is::
 
     @article{mckinnonhill2023,
       author  = {McKinnon, Michael L. and Hill, N. Jeremy and Carp, Jonathan S.
                  and Dellenbach, Blair and Thompson, Aiko K.},
       title   = {Methods for Automated Delineation and Assessment of {EMG}
                  Responses Evoked by Peripheral Nerve Stimulation in Diagnostic
                  and Closed-Loop Therapeutic Applications},
       journal = {Journal of Neural Engineering},
       year    = {2023},
+      month   = {July},
+      date    = {2023-07-21},
+      volume  = {20},
+      number  = {4},
+      pages   = {046012},
       doi     = {10.1088/1741-2552/ace6fb},
       url     = {https://doi.org/10.1088/1741-2552/ace6fb},
     }
 """
 
-"""
-      month   = {TBD},
-      date    = {2023-TBD-TBD},
-      volume  = {TBD},
-      number  = {TBD},
-      pages   = {TBD--TBD},
-"""
-
 def Cite( command=None, prefix='', stream=None ):
 	"""
 =============================================================================
 This is the RecruitmentCurveFitting package version @VERSION@ by Jeremy Hill,
 running in Python @PYVERSION@.
 
 @CITATION_INFO@
```

## Comparing `RecruitmentCurveFitting-1.1.2.dist-info/METADATA` & `RecruitmentCurveFitting-1.1.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecruitmentCurveFitting
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package for fitting sigmoid and bell-shaped functions to EMG recruitment-curve measurements
 Home-page: UNKNOWN
 Author: Jeremy Hill
 Author-email: jezhill@gmail.com
 License: GPL v3+
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, <4
@@ -36,27 +36,31 @@
 
 If you use this software in your research, your report should cite the article
 in which this approach was introduced, as follows:
 
 - McKinnon ML, Hill NJ, Carp JS, Dellenbach B & Thompson AK (2023).
   Methods for automated delineation and assessment of EMG responses evoked by
   peripheral nerve stimulation in diagnostic and closed-loop therapeutic
-  applications.
-  Journal of Neural Engineering (in press)
+  applications.  Journal of Neural Engineering 20(4):046012.
   https://doi.org/10.1088/1741-2552/ace6fb
-    
+
 The corresponding BibTeX entry is::
 
     @article{mckinnonhill2023,
       author  = {McKinnon, Michael L. and Hill, N. Jeremy and Carp, Jonathan S.
                  and Dellenbach, Blair and Thompson, Aiko K.},
       title   = {Methods for Automated Delineation and Assessment of {EMG}
                  Responses Evoked by Peripheral Nerve Stimulation in Diagnostic
                  and Closed-Loop Therapeutic Applications},
       journal = {Journal of Neural Engineering},
       year    = {2023},
+      month   = {July},
+      date    = {2023-07-21},
+      volume  = {20},
+      number  = {4},
+      pages   = {046012},
       doi     = {10.1088/1741-2552/ace6fb},
       url     = {https://doi.org/10.1088/1741-2552/ace6fb},
     }
```

## Comparing `RecruitmentCurveFitting-1.1.2.dist-info/RECORD` & `RecruitmentCurveFitting-1.1.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 RecruitmentCurveFitting/COPYING,sha256=Czg9WmPaZE9ijZnDOXbqZIftiaqlnwsyV5kt6sEXHms,35821
-RecruitmentCurveFitting/CurveFitting.py,sha256=80RF2UuoP9KUl-pydCIwa_FHD9k8-J7OFvefHWRfL2A,18750
+RecruitmentCurveFitting/CurveFitting.py,sha256=zO4CplGAz82mUpaS51q5Xrw9J3AIaKc5U1JJViX8Z78,18938
 RecruitmentCurveFitting/RecruitmentCurves.py,sha256=dLMjlYzPga1Fk02dUcmg5HLCwKZ8YXKy3U39LC1_HRk,28640
-RecruitmentCurveFitting/__init__.py,sha256=UcN47a5WENmUknrgfFhy3bV-XCbiFtfNyMvtxYqjx8w,4252
+RecruitmentCurveFitting/__init__.py,sha256=oszDg6VmgVTP65AuYSLJmmio9B_2T5PUJPOmdIwvpbw,4314
 RecruitmentCurveFitting/__main__.py,sha256=515xY1F8yjh3qF-hpvkFFMnAbFcDeKSTJWkrL3XEhUE,7820
 RecruitmentCurveFitting/example-data1.txt,sha256=FeaYwnAMGemLQKM9Kj1IPi_3fey7gyY9SLOJYttZcXc,1491
 RecruitmentCurveFitting/example-data2.txt,sha256=SBv6zHDxt1YOhylfZSMMHSCsDNwL1brHpTgAdH8esvg,2291
 RecruitmentCurveFitting/example-waveforms.csv,sha256=eWF7HtChJAv5uHfiQ1Pg__l-d9eYKtGWr8PlYp7-kis,208425
-RecruitmentCurveFitting-1.1.2.dist-info/METADATA,sha256=twgs6DgNW0HihY7erMvIfQv-_dUEcX2-W_Tpm5vwJmg,2529
-RecruitmentCurveFitting-1.1.2.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
-RecruitmentCurveFitting-1.1.2.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
-RecruitmentCurveFitting-1.1.2.dist-info/RECORD,,
+RecruitmentCurveFitting-1.1.3.dist-info/METADATA,sha256=0JYF6I1pKzJgLLS8Oi30zlj2CLhHNWVKqIOvR40r6mo,2650
+RecruitmentCurveFitting-1.1.3.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
+RecruitmentCurveFitting-1.1.3.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
+RecruitmentCurveFitting-1.1.3.dist-info/RECORD,,
```

