# Comparing `tmp/pvipy-0.3.0.tar.gz` & `tmp/pvipy-0.4.0.tar.gz`

## Comparing `pvipy-0.3.0.tar` & `pvipy-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,46 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pvipy-0.3.0/whatsnew.txt
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/basics1.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/browse_for_targets.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/gui1.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/linknode1.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/list_objects1.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/list_objects2.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/list_objects3.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/logger1.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/logger2.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/modules1.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/modules2.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/modules3.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/set_ip_address.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/simple1.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pvipy-0.3.0/examples/simple2.py
--rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Connection.py
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Cpu.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Device.py
--rw-r--r--   0        0        0   108627 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Error.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Line.py
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Module.py
--rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Object.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Station.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Task.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/Variable.py
--rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/VariableType.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/include/__init__.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/include/common_h.py
--rw-r--r--   0        0        0    16521 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/include/pvi_h.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/utils/BrDataObjectFile.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/utils/BrFile.py
--rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/utils/BrLoggerFile.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pvipy-0.3.0/pvi/utils/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pvipy-0.3.0/tests/test1.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pvipy-0.3.0/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pvipy-0.3.0/LICENSE
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 pvipy-0.3.0/README.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pvipy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 pvipy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pvipy-0.4.0/whatsnew.txt
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/basics1.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/browse_for_targets.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/gui1.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/linknode1.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects1.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects2.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects3.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects4.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects5.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/list_objects6.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/logger1.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/logger2.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/logger3.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/modules1.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/modules2.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/modules3.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/set_ip_address.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/simple1.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/simple2.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 pvipy-0.4.0/examples/simple3.py
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Connection.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Cpu.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Device.py
+-rw-r--r--   0        0        0   108627 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Error.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Line.py
+-rw-r--r--   0        0        0    10176 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Module.py
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Object.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Station.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Task.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/Variable.py
+-rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/VariableType.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/include/__init__.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/include/common_h.py
+-rw-r--r--   0        0        0    16521 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/include/pvi_h.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/utils/BrDataObjectFile.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/utils/BrFile.py
+-rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/utils/BrLoggerFile.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pvipy-0.4.0/pvi/utils/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pvipy-0.4.0/tests/test1.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pvipy-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pvipy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 pvipy-0.4.0/README.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pvipy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 pvipy-0.4.0/PKG-INFO
```

### Comparing `pvipy-0.3.0/examples/basics1.py` & `pvipy-0.4.0/examples/basics1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/browse_for_targets.py` & `pvipy-0.4.0/examples/browse_for_targets.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/gui1.py` & `pvipy-0.4.0/examples/gui1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/linknode1.py` & `pvipy-0.4.0/examples/linknode1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/list_objects1.py` & `pvipy-0.4.0/examples/list_objects1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/list_objects2.py` & `pvipy-0.4.0/examples/list_objects2.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/list_objects3.py` & `pvipy-0.4.0/examples/list_objects3.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/logger1.py` & `pvipy-0.4.0/examples/logger1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/logger2.py` & `pvipy-0.4.0/examples/logger2.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/modules1.py` & `pvipy-0.4.0/examples/modules1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/modules2.py` & `pvipy-0.4.0/examples/modules2.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/modules3.py` & `pvipy-0.4.0/examples/modules3.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/set_ip_address.py` & `pvipy-0.4.0/examples/set_ip_address.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/simple1.py` & `pvipy-0.4.0/examples/simple1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/examples/simple2.py` & `pvipy-0.4.0/examples/simple2.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/Connection.py` & `pvipy-0.4.0/pvi/Connection.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/Cpu.py` & `pvipy-0.4.0/pvi/Cpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from .include import *
 from .Object import PviObject
 from .Error import PviError
 
 
 # ----------------------------------------------------------------------------------
 class Cpu(PviObject):
+
     def __init__( self, parent, name, **objectDescriptor ):
         if parent._type != T_POBJ_TYPE.POBJ_DEVICE and parent._type != T_POBJ_TYPE.POBJ_STATION:
             raise PviError(12009, self )                    
         super().__init__( parent, 'POBJ_CPU', name, **objectDescriptor) 
         self._downloaded = None
         self._progress = None  
   
@@ -141,25 +142,56 @@
             raise PviError( self._result, self )
 
 
     @property
     def modules(self):
         """     
         Cpu.modules : list of str
-        get a list a modules 
+        get a list of all modules 
         """
         s = create_string_buffer(b'\000' * 4096)   
         self._result = PviRead( self._linkID, POBJ_ACC_LIST_MODULE, None, 0, byref(s), sizeof(s) )
         if self._result == 0:
             s = str(s, 'ascii').rstrip('\x00')
             return s.split('\t')
         else:
             raise PviError(self._result, self)
 
 
+    @property
+    def tasks(self):
+        """     
+        Cpu.tasks : list of str
+        get a list of all tasks
+        """
+        s = create_string_buffer(b'\000' * 4096)   
+        self._result = PviRead( self._linkID, POBJ_ACC_LIST_TASK, None, 0, byref(s), sizeof(s) )
+        if self._result == 0:
+            s = str(s, 'ascii').rstrip('\x00')
+            return s.split('\t')
+        else:
+            raise PviError(self._result, self)
+
+
+    @property
+    def variables(self):
+        """     
+        Cpu.variables : list of str
+        get a list of global variables
+        """
+        s = create_string_buffer(b'\000' * 65536)   
+        self._result = PviRead( self._linkID, POBJ_ACC_LIST_PVAR, None, 0, byref(s), sizeof(s) )
+        if( self._result == 0 ):
+            s = str(s, 'ascii').rstrip('\x00')
+            variables = [v.split(' ')[0] for v in s.split('\t')]
+            return variables
+        else:
+            raise PviError(self._result, self)
+
+
     @property       
     def status(self) -> dict:
         """
         Cpu.status
         read the CPU status
         """
         st = super().status
```

### Comparing `pvipy-0.3.0/pvi/Device.py` & `pvipy-0.4.0/pvi/Device.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/Error.py` & `pvipy-0.4.0/pvi/Error.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/Line.py` & `pvipy-0.4.0/pvi/Line.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/Module.py` & `pvipy-0.4.0/pvi/Module.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
                 xmlTree = ET.fromstring(s)
                 loggerVersion = xmlTree.attrib.get('Version', '1000').encode('ascii')
                 s = create_string_buffer(b'DN=10000000 VI=' + loggerVersion )   
                 self._result = PviReadArgumentRequest( self._linkID, POBJ_ACC_LN_XML_LOGM_DATA, byref(s), sizeof(s), PVI_HMSG_NIL, SET_PVIFUNCTION, 0 )            
                 if self._result:
                     raise PviError(self._result)           
             elif self._result == 12058: # access not aupported ?
-                s = create_string_buffer(b'DN=10000000')
+                s = create_string_buffer(b'DN=100000') # maximum possible is undocumented.
                 self._result = PviReadArgumentRequest( self._linkID, POBJ_ACC_MOD_DATA, byref(s), sizeof(s), PVI_HMSG_NIL, SET_PVIFUNCTION, 0    ) 
                 if self._result:
                     raise PviError(self._result)           
             else:
                 raise PviError(self._result)
         else:
             s = create_string_buffer(bytes(arguments, 'ascii'))
```

### Comparing `pvipy-0.3.0/pvi/Object.py` & `pvipy-0.4.0/pvi/Object.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,24 +171,25 @@
 
 
     @property
     def externalObjects(self):
         """     
         PviObject.externalObjects : list of dict
         get a list of external objects
+        # only available with ANSL, not with INA2000
         """    
         s = create_string_buffer(b'\000' * 65536)   
-        self.result = PviRead( self._linkID, POBJ_ACC_LIST_EXTERN, None, 0, byref(s), sizeof(s) )
-        if self.result == 0:
+        self._result = PviRead( self._linkID, POBJ_ACC_LIST_EXTERN, None, 0, byref(s), sizeof(s) )
+        if self._result == 0:
             s = str(s, 'ascii').rstrip('\x00')
             li1 = [r.split(' OT=') for r in s.split('\t')]
             li2 = [{ 'name': r[0], 'type' : r[1] } for r in li1]
             return li2
-        else:
-            return []
+        else: 
+            raise PviError(self._result, self)
 
 
     @property       
     def status(self) -> dict:
         """
         PviObject.status
         read the object's status ()
```

### Comparing `pvipy-0.3.0/pvi/Station.py` & `pvipy-0.4.0/pvi/Station.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/Task.py` & `pvipy-0.4.0/pvi/Task.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,10 +56,26 @@
         Task: stop task
         '''
         s = create_string_buffer(b"ST=Stop")
         self._result = PviWrite( self._linkID, POBJ_ACC_STATUS, byref(s), sizeof(s), None, 0 )
         if self._result != 0:
             raise PviError(self._result, self)                  
 
+    @property
+    def variables(self):
+        """     
+        Task.variables : list of str
+        get a list of local variables
+        """
+        s = create_string_buffer(b'\000' * 65536)   
+        self._result = PviRead( self._linkID, POBJ_ACC_LIST_PVAR, None, 0, byref(s), sizeof(s) )
+        if( self._result == 0 ):
+            s = str(s, 'ascii').rstrip('\x00')
+            variables = [v.split(' ')[0] for v in s.split('\t')]
+            return variables
+        else:
+            raise PviError(self._result, self)
+
+
     def __repr__(self):
         return f"Task( name={self._name}, linkID={self._linkID} )"
```

### Comparing `pvipy-0.3.0/pvi/Variable.py` & `pvipy-0.4.0/pvi/Variable.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/VariableType.py` & `pvipy-0.4.0/pvi/VariableType.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/__init__.py` & `pvipy-0.4.0/pvi/__init__.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/include/common_h.py` & `pvipy-0.4.0/pvi/include/common_h.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/include/pvi_h.py` & `pvipy-0.4.0/pvi/include/pvi_h.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/utils/BrDataObjectFile.py` & `pvipy-0.4.0/pvi/utils/BrDataObjectFile.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/utils/BrFile.py` & `pvipy-0.4.0/pvi/utils/BrFile.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/pvi/utils/BrLoggerFile.py` & `pvipy-0.4.0/pvi/utils/BrLoggerFile.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/tests/test1.py` & `pvipy-0.4.0/tests/test1.py`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/.gitignore` & `pvipy-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/LICENSE` & `pvipy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pvipy-0.3.0/README.md` & `pvipy-0.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -37,29 +37,51 @@
 ## Start here
 ### [simple1.py](examples/simple1.py) (ANSL)
 this simple example just registers a variable, reads its value and then exit after a few seconds
 
 ### [simple2.py](examples/simple2.py) (ANSL)
 this simple example just registers a variable for reading and another for writing. In fact we switch on the 'coffee machine' and watch its temperature ...
 
+### [simple3.py](examples/simple3.py) (INA2000)
+this simple example just registers a variable for reading and another for writing. In fact we switch on the 'coffee machine' and watch its temperature ...
+This is similar to simple2.py but we use a control running AR 3.x. ANSL is not available here and we change to good old INA2000
+
+
 ## Basics
 ### [basics1.py](examples/basics1.py) (ANSL)
 shows reading and writing of basic data types
 
 ## Create Lists of objects
 ### [list_objects1.py](examples/list_objects1.py) (ANSL)
 this example lists objects with 'global scope' (modules, task and global variables)
-from 'coffe machine' cpu and returns status information about them
+from 'coffee machine' cpu and returns status information about them
 
 ### [list_objects2.py](examples/list_objects2.py) (ANSL)
 this example lists global and local variables and their content
 
 ### [list_objects3.py](examples/list_objects3.py) (ANSL)
 this example lists all local variables of a specific task and their content
 
+### [list_objects4.py](examples/list_objects4.py) (INA2000)
+this example lists objects with 'global scope' (modules, task and global variables)
+from 'coffee machine' cpu and returns status information about them
+
+This is similar to list_objects1.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+### [list_objects5.py](examples/list_objects5.py) (INA2000)
+this example lists global and local variables and their content
+
+This is similar to list_objects2.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+### [list_objects6.py](examples/list_objects6.py) (INA2000)
+this example lists all local variables of a specific task and their content
+
+This is similar to list_objects3.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+
 ## Handling modules
 ### [modules1.py](examples/modules1.py) (ANSL)
 this simple example creates a module on CPU by downloading a bytestream and checks if it exists
 
 ### [modules2.py](examples/modules2.py) (ANSL)
 this simple example creates a module on CPU by downloading a bytestream and afterwards uploads it again
 
@@ -70,14 +92,19 @@
 
 ### [logger1.py](examples/logger1.py) (ANSL)
 this example uploads some loggers from CPU
 
 ### [logger2.py](examples/logger2.py) 
 extract all logger from a systemdump container and save them as csv
 
+### [logger3.py](examples/logger3.py) (INA2000)
+this example uploads some loggers from CPU
+
+This is similar to logger1.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
 
 ## GUI
 ### [gui1.py](examples/gui1.py) (ANSL)
 this example shows the usage of Pvi.py in tkinter
 
 ## IO
 ### [linknode1.py](examples/linknode1.py) (ANSL)
```

### Comparing `pvipy-0.3.0/pyproject.toml` & `pvipy-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pvipy"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Christoph Hilchenbach" },
 ]
 description = "Python connector for B&R Pvi (process visualization interface)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pvipy-0.3.0/PKG-INFO` & `pvipy-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvipy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python connector for B&R Pvi (process visualization interface)
 Project-URL: Homepage, https://github.com/hilch/Pvi.py
 Project-URL: Bug Tracker, https://github.com/hilch/Pvi.py/issues
 Author: Christoph Hilchenbach
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -51,29 +51,51 @@
 ## Start here
 ### [simple1.py](examples/simple1.py) (ANSL)
 this simple example just registers a variable, reads its value and then exit after a few seconds
 
 ### [simple2.py](examples/simple2.py) (ANSL)
 this simple example just registers a variable for reading and another for writing. In fact we switch on the 'coffee machine' and watch its temperature ...
 
+### [simple3.py](examples/simple3.py) (INA2000)
+this simple example just registers a variable for reading and another for writing. In fact we switch on the 'coffee machine' and watch its temperature ...
+This is similar to simple2.py but we use a control running AR 3.x. ANSL is not available here and we change to good old INA2000
+
+
 ## Basics
 ### [basics1.py](examples/basics1.py) (ANSL)
 shows reading and writing of basic data types
 
 ## Create Lists of objects
 ### [list_objects1.py](examples/list_objects1.py) (ANSL)
 this example lists objects with 'global scope' (modules, task and global variables)
-from 'coffe machine' cpu and returns status information about them
+from 'coffee machine' cpu and returns status information about them
 
 ### [list_objects2.py](examples/list_objects2.py) (ANSL)
 this example lists global and local variables and their content
 
 ### [list_objects3.py](examples/list_objects3.py) (ANSL)
 this example lists all local variables of a specific task and their content
 
+### [list_objects4.py](examples/list_objects4.py) (INA2000)
+this example lists objects with 'global scope' (modules, task and global variables)
+from 'coffee machine' cpu and returns status information about them
+
+This is similar to list_objects1.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+### [list_objects5.py](examples/list_objects5.py) (INA2000)
+this example lists global and local variables and their content
+
+This is similar to list_objects2.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+### [list_objects6.py](examples/list_objects6.py) (INA2000)
+this example lists all local variables of a specific task and their content
+
+This is similar to list_objects3.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
+
 ## Handling modules
 ### [modules1.py](examples/modules1.py) (ANSL)
 this simple example creates a module on CPU by downloading a bytestream and checks if it exists
 
 ### [modules2.py](examples/modules2.py) (ANSL)
 this simple example creates a module on CPU by downloading a bytestream and afterwards uploads it again
 
@@ -84,14 +106,19 @@
 
 ### [logger1.py](examples/logger1.py) (ANSL)
 this example uploads some loggers from CPU
 
 ### [logger2.py](examples/logger2.py) 
 extract all logger from a systemdump container and save them as csv
 
+### [logger3.py](examples/logger3.py) (INA2000)
+this example uploads some loggers from CPU
+
+This is similar to logger1.py but since we use a control running < AR 4.x ANSL is not available here and we change to good old INA2000
+
 
 ## GUI
 ### [gui1.py](examples/gui1.py) (ANSL)
 this example shows the usage of Pvi.py in tkinter
 
 ## IO
 ### [linknode1.py](examples/linknode1.py) (ANSL)
```

