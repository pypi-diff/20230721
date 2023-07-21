# Comparing `tmp/pyLauda-1.0.5-py2.py3-none-any.whl.zip` & `tmp/pyLauda-1.0.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6615 bytes, number of entries: 8
--rw-rw-r--  2.0 unx       22 b- defN 23-Jul-21 13:27 pyLauda/__init__.py
+Zip file size: 6625 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx       22 b- defN 23-Jul-21 14:29 pyLauda/__init__.py
 -rw-rw-r--  2.0 unx     6349 b- defN 22-Mar-28 18:30 pyLauda/re206.py
--rw-rw-r--  2.0 unx     9174 b- defN 23-Jul-21 13:10 pyLauda/variocool.py
--rw-rw-r--  2.0 unx     1080 b- defN 23-Jul-21 13:27 pyLauda-1.0.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx      370 b- defN 23-Jul-21 13:27 pyLauda-1.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jul-21 13:27 pyLauda-1.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Jul-21 13:27 pyLauda-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      609 b- defN 23-Jul-21 13:27 pyLauda-1.0.5.dist-info/RECORD
-8 files, 17722 bytes uncompressed, 5557 bytes compressed:  68.6%
+-rw-rw-r--  2.0 unx     9216 b- defN 23-Jul-21 14:28 pyLauda/variocool.py
+-rw-rw-r--  2.0 unx     1080 b- defN 23-Jul-21 14:29 pyLauda-1.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      370 b- defN 23-Jul-21 14:29 pyLauda-1.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-21 14:29 pyLauda-1.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-21 14:29 pyLauda-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      609 b- defN 23-Jul-21 14:29 pyLauda-1.0.6.dist-info/RECORD
+8 files, 17764 bytes uncompressed, 5567 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pyLauda/re206.py
 Comment: 
 
 Filename: pyLauda/variocool.py
 Comment: 
 
-Filename: pyLauda-1.0.5.dist-info/LICENSE
+Filename: pyLauda-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: pyLauda-1.0.5.dist-info/METADATA
+Filename: pyLauda-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: pyLauda-1.0.5.dist-info/WHEEL
+Filename: pyLauda-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: pyLauda-1.0.5.dist-info/top_level.txt
+Filename: pyLauda-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: pyLauda-1.0.5.dist-info/RECORD
+Filename: pyLauda-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyLauda/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.0.5'
+__version__ = '1.0.6'
```

## pyLauda/variocool.py

```diff
@@ -224,27 +224,27 @@
     @timeout_decorator.timeout(4, timeout_exception=TimeoutError)
     def test(self):
         """
         Check if device is reponsive
         :return: device availability
         :type: boolean
         """
-        state = self.__txrx('STAT').decode('utf-8').strip('\r\n')
-        self._log.info(f"Device state: {state}")
-        if "ERR" in state:
+        status = self.__txrx('STATUS').decode('utf-8').strip('\r\n')
+        self._log.info(f"Device status: {status}")
+        if "-1" in status:
             return False
 
-        if int(state) == 0:
+        if "0" in status:
             return True
 
         return False
 
     def __write(self, cmd):
         try:
-            self.device.write(str.encode(cmd + "\r"))
+            self.device.write(str.encode(cmd)+b'\r')
         except SerialException:
             raise SerialException('Lauda ' +  self.__DEVICE_IDENTIFIER + ': Error while writing.')
 
     def __readline(self, n=0):
         out = bytearray()
         eol = b'\r'
         leneol = len(eol)
@@ -261,14 +261,15 @@
             c = self.device.read(1)
             if c:
                 out += c
                 if out[-leneol:] == eol:
                     break
             else:
                 break
+
         if not out and n<30:
             self._log.warning(f"Retry reading.")
             time.sleep(0.5)
             if self.device.isOpen():
                 self.device.close()
             self.device.open()
             self.read_buffer()
@@ -283,11 +284,13 @@
         for i in range(3):
             self.read_buffer()
             self.__write(cmd)
             time.sleep(0.1)
             answ = self.__readline()
             if answ is not None:
                 break
+        print(cmd)
+        print(answ)
         self._log.debug(f"CMD: {cmd}\t Return: {answ}")
 
         return answ
```

## Comparing `pyLauda-1.0.5.dist-info/LICENSE` & `pyLauda-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

