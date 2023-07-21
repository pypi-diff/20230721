# Comparing `tmp/langful-0.37-py3-none-any.whl.zip` & `tmp/langful-0.38-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5561 bytes, number of entries: 7
+Zip file size: 5620 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-06 06:25 langful/__init__.py
--rw-rw-rw-  2.0 fat    10023 b- defN 23-Jul-20 12:41 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3050 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/RECORD
-7 files, 14933 bytes uncompressed, 4631 bytes compressed:  69.0%
+-rw-rw-rw-  2.0 fat    10241 b- defN 23-Jul-21 02:54 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-21 03:18 langful-0.38.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-Jul-21 03:18 langful-0.38.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 03:18 langful-0.38.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-21 03:18 langful-0.38.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      528 b- defN 23-Jul-21 03:18 langful-0.38.dist-info/RECORD
+7 files, 15151 bytes uncompressed, 4690 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.37.dist-info/LICENSE
+Filename: langful-0.38.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.37.dist-info/METADATA
+Filename: langful-0.38.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.37.dist-info/WHEEL
+Filename: langful-0.38.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.37.dist-info/top_level.txt
+Filename: langful-0.38.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.37.dist-info/RECORD
+Filename: langful-0.38.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -14,15 +14,15 @@
     import re
     ret = {}
     for line in lang_file.split( "\n" ) :
         text = re.split( "([^#^=^\\s]+|)(\\s+=\\s+|\\s+=|=\\s+|=|)([^#^\\n]+|)" , line )
         index = 0
         for value in text :
             if "=" in value :
-                ret[ "".join( text[ :index ] ) ] = "".join( text[ index + 1: ] )
+                ret[ "".join( text[ :index ] ) ] = "".join( text[ index + 1 : ] )
                 break
             index += 1
     return ret
 
 def to_lang( dict_file : dict ) -> str :
     """
     .json -> .lang
@@ -56,49 +56,110 @@
     return code.replace( "-" , "_" ).lower()
 
 class lang :
     """
     # lang
     """
 
-    def __setitem__( self , key , value ) -> None :
+    @property
+    def locales( self ) -> list :
         """
-        set
+        locales
         """
-        self.set( key , value )
+        return list( self.types.keys() )
 
-    def __delitem__( self , key ) -> None :
+    @property
+    def locale( self ) -> str :
         """
-        remove
+        choose locale
         """
-        self.remove( key )
+        for locale in [ self.use_locale , self.system_locale , self.default_locale ] :
+            if locale and locale in self.locales :
+                return locale
+        raise KeyError( f"no such locale '{ self.system_locale }' or '{ self.default_locale }'" )
+
+    @property
+    def language( self ) -> dict :
+        """
+        get now language
+        """
+        return self.lang_get( self.locale )
+
+    @property
+    def lang( self ) -> dict :
+        """
+        same to language function
+        """
+        return self.language
+
+    @property
+    def langs( self ) -> dict :
+        """
+        same to languages variable
+        """
+        return self.languages
+
+    @property
+    def type( self ) -> str :
+        """
+        get type, ".json" or ".lang"
+        """
+        return self.types[ self.locale ]
 
     def __getitem__( self , key ) -> str :
         """
-        get
+        get the value in language variable
         """
         return self.get( key )
 
+    def __setitem__( self , key , value ) -> None :
+        """
+        set the value in languages[ locale ]
+        """
+        self.set( key , value )
+
+    def __delitem__( self , key ) -> None :
+        """
+        remove the value in languages[ locale ]
+        """
+        self.remove( key )
+
     def __call__( self ) -> None :
         """
-        init
+        init function
         """
         self.init()
 
+    def __str__( self ) -> str :
+        """
+        to string
+        """
+        return json.dumps( self.languages , indent = 4 , ensure_ascii = False , separators = self.separators )
+
     def __len__( self ) -> int :
-        return len( self.languages )
+        """
+        how many item in language variable
+        """
+        return len( self.language )
+
+    def __bool__( self ) -> bool :
+        """
+        is system locale in languages dictionary
+        """
+        return self.system_locale in self.languages
 
     def __init__( self , lang_dir : str | dict = "lang" , default_locale : str = "en_us" , json_first : bool = True ) -> None :
         """
         lang_dir: lang files dir, if use dict to set that to a dictionary or False
         default_locale: default locale
         json_first: is load json file first
         """
         self.system_locale = getdefaultlocale()
         self.default_locale = default_locale
+        self.separators = [ " ," , ": " ]
         self.json_first = json_first
         self.replace_letter = "%"
         self.lang_dir = lang_dir
         self.use_locale = None
         self.is_file = False
         self.languages = {}
         self.types = {}
@@ -160,68 +221,14 @@
         set type to file
         """
         if not os.path.exists( path ) :
             os.makedirs( path )
         self.lang_dir = path
         self.is_file = True
 
-    @property
-    def locales( self ) -> list :
-        """
-        locales
-        """
-        return list( self.types.keys() )
-
-    @property
-    def locale( self ) -> str :
-        """
-        choose locale
-        """
-        for locale in [ self.use_locale , self.system_locale , self.default_locale ] :
-            if locale and locale in self.locales :
-                return locale
-        raise KeyError( f"no such locale '{ self.system_locale }' or '{ self.default_locale }'" )
-
-    @property
-    def language( self ) -> dict :
-        """
-        get now language
-        """
-        return self.lang_get( self.locale )
-
-    @property
-    def lang( self ) -> dict :
-        """
-        same to language function
-        """
-        return self.language
-
-    @property
-    def langs( self ) -> dict :
-        """
-        same to languages variable
-        """
-        return self.languages
-
-    @property
-    def type( self ) -> str :
-        """
-        get type, ".json" or ".lang"
-        """
-        return self.types[ self.locale ]
-
-    def replace_letter_get( self , replace_letter : str = None ) -> str :
-        """
-        get replace letter, usually use in function
-        """
-        if replace_letter :
-            return replace_letter
-        else :
-            return self.replace_letter
-
     def locale_get( self , locale : str = None ) -> str :
         """
         get locale, usually use in function
         """
         if locale :
             return locale
         else :
@@ -289,33 +296,33 @@
         args = to_list( args )
         ret = self.lang_get( self.locale_get( locale ) )
         for locale_key in args :
             for key , value in self.lang_get( locale_key ).items() :
                 ret[ key ] = value
         return ret
 
-    def save( self , separators : list = [ " ," , ": " ] ) -> dict :
+    def save( self ) -> dict :
         """
         save file when is_file variable is true
         """
         if self.is_file :
             for key , value in self.languages.items() :
                 suffix = self.types[ key ]
                 with open( os.path.join( self.lang_dir , key + suffix ) , "w" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
-                        json.dump( value , file , indent = 4 , separators = separators , ensure_ascii = False )
+                        json.dump( value , file , indent = 4 , separators = self.separators , ensure_ascii = False )
                     elif suffix == ".lang" :
                         file.write( to_lang( value ) )
         return self.languages
 
-    def replace( self , key : str = None , args : str | list  = None , locale : str = None , replace_letter : str = None ) -> str :
+    def replace( self , key : str = None , args : str | list  = None , locale : str = None ) -> str :
         """
         replace
         """
-        replace_letter = self.replace_letter_get( replace_letter )
+        replace_letter = self.replace_letter
         locale = self.locale_get( locale )
         args = to_list( args )
         index = 0
         ret = ""
         for text in self.get( key , locale ) :
             if text == replace_letter :
                 if len( ret ) and ret[ -1 ] == "\\" :
```

## Comparing `langful-0.37.dist-info/LICENSE` & `langful-0.38.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.37.dist-info/METADATA` & `langful-0.38.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.37
+Version: 0.38
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >= 3.6
+Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align = "center" >
     <h1>langful</h1>
     <a href = "https://pypi.org/project/langful" >
         <img alt = "PyPI version" src = "https://img.shields.io/pypi/v/langful?color=blue" >
     </a>
     <a href = "https://www.python.org" >
-        <img alt = "Python version" src = "https://img.shields.io/badge/python-3.6+-blue" >
+        <img alt = "Python version" src = "https://img.shields.io/badge/python-3.9+-blue" >
     </a>
     <a href = "https://opensource.org/license/mit" >
         <img alt = "license" src = "https://img.shields.io/badge/license-MIT-blue" >
     </a>
     <a href = "https://github.com/cueavy/langful" >
         <img alt = "Github stars" src = "https://img.shields.io/github/stars/cueavy/langful?color=blue" >
     </a>
```

