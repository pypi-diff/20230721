# Comparing `tmp/pdfcrowd-5.8.0.tar.gz` & `tmp/pdfcrowd-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfcrowd-5.8.0.tar", last modified: Mon Sep  5 13:18:04 2022, max compression
+gzip compressed data, was "pdfcrowd-5.9.0.tar", last modified: Mon Oct  3 10:16:40 2022, max compression
```

## Comparing `pdfcrowd-5.8.0.tar` & `pdfcrowd-5.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2022-09-05 13:18:04.309289 pdfcrowd-5.8.0/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1076 2021-12-06 13:05:19.000000 pdfcrowd-5.8.0/LICENSE
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      677 2022-09-05 13:18:04.309289 pdfcrowd-5.8.0/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1071 2022-07-15 07:03:21.000000 pdfcrowd-5.8.0/README.md
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      333 2022-09-05 13:14:47.000000 pdfcrowd-5.8.0/html2image
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      331 2022-09-05 13:14:47.000000 pdfcrowd-5.8.0/html2pdf
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      334 2022-09-05 13:14:47.000000 pdfcrowd-5.8.0/image2image
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      332 2022-09-05 13:14:47.000000 pdfcrowd-5.8.0/image2pdf
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      331 2022-09-05 13:14:47.000000 pdfcrowd-5.8.0/pdf2html
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      330 2022-09-05 13:14:47.000000 pdfcrowd-5.8.0/pdf2pdf
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2022-09-05 13:18:04.309289 pdfcrowd-5.8.0/pdfcrowd.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      677 2022-09-05 13:18:04.000000 pdfcrowd-5.8.0/pdfcrowd.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      247 2022-09-05 13:18:04.000000 pdfcrowd-5.8.0/pdfcrowd.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2022-09-05 13:18:04.000000 pdfcrowd-5.8.0/pdfcrowd.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2022-09-05 13:18:04.000000 pdfcrowd-5.8.0/pdfcrowd.egg-info/top_level.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)   304705 2022-09-05 13:16:20.000000 pdfcrowd-5.8.0/pdfcrowd.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      108 2022-09-05 13:18:04.309289 pdfcrowd-5.8.0/setup.cfg
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2238 2022-09-05 13:16:20.000000 pdfcrowd-5.8.0/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2022-10-03 10:16:40.788875 pdfcrowd-5.9.0/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1076 2021-12-06 13:05:19.000000 pdfcrowd-5.9.0/LICENSE
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      677 2022-10-03 10:16:40.788875 pdfcrowd-5.9.0/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1071 2022-07-15 07:03:21.000000 pdfcrowd-5.9.0/README.md
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      333 2022-10-03 10:12:23.000000 pdfcrowd-5.9.0/html2image
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      331 2022-10-03 10:12:23.000000 pdfcrowd-5.9.0/html2pdf
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      334 2022-10-03 10:12:23.000000 pdfcrowd-5.9.0/image2image
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      332 2022-10-03 10:12:23.000000 pdfcrowd-5.9.0/image2pdf
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      331 2022-10-03 10:12:23.000000 pdfcrowd-5.9.0/pdf2html
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      330 2022-10-03 10:12:23.000000 pdfcrowd-5.9.0/pdf2pdf
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2022-10-03 10:16:40.788875 pdfcrowd-5.9.0/pdfcrowd.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      677 2022-10-03 10:16:40.000000 pdfcrowd-5.9.0/pdfcrowd.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      247 2022-10-03 10:16:40.000000 pdfcrowd-5.9.0/pdfcrowd.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2022-10-03 10:16:40.000000 pdfcrowd-5.9.0/pdfcrowd.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2022-10-03 10:16:40.000000 pdfcrowd-5.9.0/pdfcrowd.egg-info/top_level.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)   305275 2022-10-03 10:14:00.000000 pdfcrowd-5.9.0/pdfcrowd.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      108 2022-10-03 10:16:40.792875 pdfcrowd-5.9.0/setup.cfg
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2238 2022-10-03 10:14:00.000000 pdfcrowd-5.9.0/setup.py
```

### Comparing `pdfcrowd-5.8.0/LICENSE` & `pdfcrowd-5.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfcrowd-5.8.0/PKG-INFO` & `pdfcrowd-5.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfcrowd
-Version: 5.8.0
+Version: 5.9.0
 Summary: A client library for the Pdfcrowd API.
 Home-page: https://pdfcrowd.com/api/
 Author: Pdfcrowd Team
 Author-email: support@pdfcrowd.com
 License: License :: OSI Approved :: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pdfcrowd-5.8.0/README.md` & `pdfcrowd-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pdfcrowd-5.8.0/pdfcrowd.egg-info/PKG-INFO` & `pdfcrowd-5.9.0/pdfcrowd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfcrowd
-Version: 5.8.0
+Version: 5.9.0
 Summary: A client library for the Pdfcrowd API.
 Home-page: https://pdfcrowd.com/api/
 Author: Pdfcrowd Team
 Author-email: support@pdfcrowd.com
 License: License :: OSI Approved :: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pdfcrowd-5.8.0/pdfcrowd.py` & `pdfcrowd-5.9.0/pdfcrowd.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import re
 import argparse
 import sys
 import os
 import ssl
 import time
 
-__version__ = '5.8.0'
+__version__ = '5.9.0'
 
 # ======================================
 # === PDFCrowd legacy version client ===
 # ======================================
 
 if PYTHON_3:
     # constants for Client.setPageLayout()
@@ -694,15 +694,15 @@
 
 # =====================================
 # === PDFCrowd cloud version client ===
 # =====================================
 
 HOST = os.environ.get('PDFCROWD_HOST', 'api.pdfcrowd.com')
 MULTIPART_BOUNDARY = '----------ThIs_Is_tHe_bOUnDary_$'
-CLIENT_VERSION = '5.8.0'
+CLIENT_VERSION = '5.9.0'
 
 def get_utf8_string(string):
     if PYTHON_3:
         # get Python3 string
         try:
             return string.decode()
         except AttributeError:
@@ -787,25 +787,26 @@
     def __init__(self, user_name, api_key):
         self.user_name = user_name
         self.api_key = api_key
 
         self._reset_response_data()
         self.setProxy(None, None, None, None)
         self.setUseHttp(False)
-        self.setUserAgent('pdfcrowd_python_client/5.8.0 (https://pdfcrowd.com)')
+        self.setUserAgent('pdfcrowd_python_client/5.9.0 (https://pdfcrowd.com)')
 
         self.retry_count = 1
         self.converter_version = '20.10'
 
     def _reset_response_data(self):
         self.debug_log_url = None
         self.credits = 999999
         self.consumed_credits = 0
         self.job_id = ''
         self.page_count = 0
+        self.total_page_count = 0
         self.output_size = 0
         self.retry = 0
 
     def post(self, fields, files, raw_data, out_stream = None):
         body = encode_multipart_post_data(fields, files, raw_data)
         content_type = 'multipart/form-data; boundary=' + MULTIPART_BOUNDARY
         return self._do_post(body, content_type, out_stream)
@@ -863,14 +864,15 @@
             response = conn.getresponse()
 
             self.debug_log_url = response.getheader('X-Pdfcrowd-Debug-Log', '')
             self.credits = int(response.getheader('X-Pdfcrowd-Remaining-Credits', 999999))
             self.consumed_credits = int(response.getheader('X-Pdfcrowd-Consumed-Credits', 0))
             self.job_id = response.getheader('X-Pdfcrowd-Job-Id', '')
             self.page_count = int(response.getheader('X-Pdfcrowd-Pages', 0))
+            self.total_page_count = int(response.getheader('X-Pdfcrowd-Total-Pages', 0))
             self.output_size = int(response.getheader('X-Pdfcrowd-Output-Size', 0))
 
             if (os.environ.get('PDFCROWD_UNIT_TEST_MODE') and
                 self.retry_count > self.retry):
                 raise Error('test 502', 502)
 
             if response.status > 299:
@@ -933,14 +935,17 @@
 
     def getJobId(self):
         return self.job_id
 
     def getPageCount(self):
         return self.page_count
 
+    def getTotalPageCount(self):
+        return self.total_page_count
+
     def getOutputSize(self):
         return self.output_size
 
     def getConverterVersion(self):
         return self.converter_version
 
 # generated code
@@ -1946,19 +1951,19 @@
         self.fields['auto_detect_element_to_convert'] = value
         return self
 
     def setReadabilityEnhancements(self, enhancements):
         """
         The input HTML is automatically enhanced to improve the readability.
 
-        enhancements - Allowed values are none, readability-v1, readability-v2, readability-v3.
+        enhancements - Allowed values are none, readability-v1, readability-v2, readability-v3, readability-v4.
         return - The converter object.
         """
-        if not re.match('(?i)^(none|readability-v1|readability-v2|readability-v3)$', enhancements):
-            raise Error(create_invalid_value_message(enhancements, "setReadabilityEnhancements", "html-to-pdf", 'Allowed values are none, readability-v1, readability-v2, readability-v3.', "set_readability_enhancements"), 470);
+        if not re.match('(?i)^(none|readability-v1|readability-v2|readability-v3|readability-v4)$', enhancements):
+            raise Error(create_invalid_value_message(enhancements, "setReadabilityEnhancements", "html-to-pdf", 'Allowed values are none, readability-v1, readability-v2, readability-v3, readability-v4.', "set_readability_enhancements"), 470);
         
         self.fields['readability_enhancements'] = get_utf8_string(enhancements)
         return self
 
     def setViewportWidth(self, width):
         """
         Set the viewport width in pixels. The viewport is the user's visible area of the page.
@@ -2462,19 +2467,26 @@
         Get the job id.
         return - The unique job identifier.
         """
         return self.helper.getJobId()
 
     def getPageCount(self):
         """
-        Get the total number of pages in the output document.
+        Get the number of pages in the output document.
         return - The page count.
         """
         return self.helper.getPageCount()
 
+    def getTotalPageCount(self):
+        """
+        Get the total number of pages in the original output document, including the pages excluded by setPrintPageRange().
+        return - The total page count.
+        """
+        return self.helper.getTotalPageCount()
+
     def getOutputSize(self):
         """
         Get the size of the output in bytes.
         return - The count of bytes.
         """
         return self.helper.getOutputSize()
 
@@ -3179,19 +3191,19 @@
         self.fields['auto_detect_element_to_convert'] = value
         return self
 
     def setReadabilityEnhancements(self, enhancements):
         """
         The input HTML is automatically enhanced to improve the readability.
 
-        enhancements - Allowed values are none, readability-v1, readability-v2, readability-v3.
+        enhancements - Allowed values are none, readability-v1, readability-v2, readability-v3, readability-v4.
         return - The converter object.
         """
-        if not re.match('(?i)^(none|readability-v1|readability-v2|readability-v3)$', enhancements):
-            raise Error(create_invalid_value_message(enhancements, "setReadabilityEnhancements", "html-to-image", 'Allowed values are none, readability-v1, readability-v2, readability-v3.', "set_readability_enhancements"), 470);
+        if not re.match('(?i)^(none|readability-v1|readability-v2|readability-v3|readability-v4)$', enhancements):
+            raise Error(create_invalid_value_message(enhancements, "setReadabilityEnhancements", "html-to-image", 'Allowed values are none, readability-v1, readability-v2, readability-v3, readability-v4.', "set_readability_enhancements"), 470);
         
         self.fields['readability_enhancements'] = get_utf8_string(enhancements)
         return self
 
     def setScreenshotWidth(self, width):
         """
         Set the output image width in pixels.
@@ -4369,15 +4381,15 @@
         Get the job id.
         return - The unique job identifier.
         """
         return self.helper.getJobId()
 
     def getPageCount(self):
         """
-        Get the total number of pages in the output document.
+        Get the number of pages in the output document.
         return - The page count.
         """
         return self.helper.getPageCount()
 
     def getOutputSize(self):
         """
         Get the size of the output in bytes.
@@ -5188,15 +5200,15 @@
         Get the job id.
         return - The unique job identifier.
         """
         return self.helper.getJobId()
 
     def getPageCount(self):
         """
-        Get the total number of pages in the output document.
+        Get the number of pages in the output document.
         return - The page count.
         """
         return self.helper.getPageCount()
 
     def getOutputSize(self):
         """
         Get the size of the output in bytes.
@@ -5572,15 +5584,15 @@
                             help = 'Wait for the specified element in a source document. The element is specified by one or more CSS selectors. The element is searched for in the main document and all iframes. If the element is not found, the conversion fails. Your API license defines the maximum wait time by "Max Delay" parameter. One or more CSS selectors separated by commas. The string must not be empty.'
 )
         parser.add_argument('-auto-detect-element-to-convert',
                             action = 'store_true',
                             help = 'The main HTML element for conversion is detected automatically.'
 )
         parser.add_argument('-readability-enhancements',
-                            help = 'The input HTML is automatically enhanced to improve the readability. Allowed values are none, readability-v1, readability-v2, readability-v3. Default is none.'
+                            help = 'The input HTML is automatically enhanced to improve the readability. Allowed values are none, readability-v1, readability-v2, readability-v3, readability-v4. Default is none.'
 )
         parser.add_argument('-viewport-width',
                             help = 'Set the viewport width in pixels. The viewport is the user\'s visible area of the page. The value must be in the range 96-65000. Default is 1024.'
 )
         parser.add_argument('-viewport-height',
                             help = 'Set the viewport height in pixels. The viewport is the user\'s visible area of the page. If the input HTML uses lazily loaded images, try using a large value that covers the entire height of the HTML, e.g. 100000. Must be a positive integer number. Default is 768.'
 )
@@ -5887,15 +5899,15 @@
                             help = 'Wait for the specified element in a source document. The element is specified by one or more CSS selectors. The element is searched for in the main document and all iframes. If the element is not found, the conversion fails. Your API license defines the maximum wait time by "Max Delay" parameter. One or more CSS selectors separated by commas. The string must not be empty.'
 )
         parser.add_argument('-auto-detect-element-to-convert',
                             action = 'store_true',
                             help = 'The main HTML element for conversion is detected automatically.'
 )
         parser.add_argument('-readability-enhancements',
-                            help = 'The input HTML is automatically enhanced to improve the readability. Allowed values are none, readability-v1, readability-v2, readability-v3. Default is none.'
+                            help = 'The input HTML is automatically enhanced to improve the readability. Allowed values are none, readability-v1, readability-v2, readability-v3, readability-v4. Default is none.'
 )
         parser.add_argument('-screenshot-width',
                             help = 'Set the output image width in pixels. The value must be in the range 96-65000. Default is 1024.'
 )
         parser.add_argument('-screenshot-height',
                             help = 'Set the output image height in pixels. If it is not specified, actual document height is used. Must be a positive integer number.'
 )
```

### Comparing `pdfcrowd-5.8.0/setup.py` & `pdfcrowd-5.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 py_modules=['pdfcrowd']
 
 setup(name='pdfcrowd',
-      version='5.8.0',
+      version='5.9.0',
       description="A client library for the Pdfcrowd API.",
       url='https://pdfcrowd.com/api/',
       license="License :: OSI Approved :: MIT License",
       author='Pdfcrowd Team',
       author_email='support@pdfcrowd.com',
       long_description="""
 The Pdfcrowd API lets you easily convert between HTML, PDF and various image formats.
```

