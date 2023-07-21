# Comparing `tmp/pyees-1.4.4.tar.gz` & `tmp/pyees-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.4.4.tar", last modified: Wed Jul 19 11:54:56 2023, max compression
+gzip compressed data, was "pyees-1.4.5.tar", last modified: Fri Jul 21 11:21:45 2023, max compression
```

## Comparing `pyees-1.4.4.tar` & `pyees-1.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 11:54:56.576949 pyees-1.4.4/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-07-19 11:54:56.592575 pyees-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 11:54:56.310010 pyees-1.4.4/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.4/pyees/__init__.py
--rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.4/pyees/fit.py
--rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.4/pyees/profileFit.py
--rw-rw-rw-   0        0        0      807 2023-07-19 11:53:33.000000 pyees-1.4.4/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.4/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.4/pyees/sheet.py
--rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.4.4/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.4/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.4/pyees/testFit.py
--rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.4.4/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-07-17 07:24:43.000000 pyees-1.4.4/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.4/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.4/pyees/testSolve.py
--rw-rw-rw-   0        0        0    10768 2023-07-19 11:49:07.000000 pyees-1.4.4/pyees/testUnit.py
--rw-rw-rw-   0        0        0    84450 2023-07-19 07:25:55.000000 pyees-1.4.4/pyees/testVariable.py
--rw-rw-rw-   0        0        0    36092 2023-07-19 11:50:47.000000 pyees-1.4.4/pyees/unit.py
--rw-rw-rw-   0        0        0    35993 2023-07-19 09:10:11.000000 pyees-1.4.4/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-07-19 11:54:56.529010 pyees-1.4.4/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-19 11:54:54.000000 pyees-1.4.4/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-19 11:54:54.000000 pyees-1.4.4/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 11:54:54.000000 pyees-1.4.4/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-19 11:54:54.000000 pyees-1.4.4/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-19 11:54:54.000000 pyees-1.4.4/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-19 11:54:56.623826 pyees-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-07-19 11:54:49.000000 pyees-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:21:45.316561 pyees-1.4.5/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-21 11:21:45.322544 pyees-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 11:21:45.125074 pyees-1.4.5/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.5/pyees/__init__.py
+-rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.5/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.5/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      812 2023-07-21 11:13:10.000000 pyees-1.4.5/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.5/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.5/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10180 2023-07-21 06:44:16.000000 pyees-1.4.5/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.5/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.5/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13364 2023-07-21 06:43:40.000000 pyees-1.4.5/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-07-21 10:48:22.000000 pyees-1.4.5/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.5/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.5/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10768 2023-07-21 11:19:40.000000 pyees-1.4.5/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    84469 2023-07-21 08:40:30.000000 pyees-1.4.5/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    37325 2023-07-21 11:18:44.000000 pyees-1.4.5/pyees/unit.py
+-rw-rw-rw-   0        0        0    36151 2023-07-21 09:10:18.000000 pyees-1.4.5/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:21:45.294620 pyees-1.4.5/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 11:21:45.350469 pyees-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-21 11:21:38.000000 pyees-1.4.5/setup.py
```

### Comparing `pyees-1.4.4/LICENSE.txt` & `pyees-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/PKG-INFO` & `pyees-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.4
+Version: 1.4.5
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.4/README.md` & `pyees-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/fit.py` & `pyees-1.4.5/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/profileFit.py` & `pyees-1.4.5/pyees/profileFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/profilePyees.py` & `pyees-1.4.5/pyees/profilePyees.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     from variable import variable
 except ImportError:
     from pyees.variable import variable
     
 pr = cProfile.Profile()
 pr.enable()
 
-for _ in range(1):
+for _ in range(50_000):
 
     c = variable(4.182, 'J/kg-K', 0.130)
     rho = variable(1000, 'kg/m3', 0.01)
     t_in = variable(50, 'C', 1.2)
     t_out = variable([10, 15, 20, 25, 30, 35, 40], 'C', [0.9, 1.1, 1.0, 0.8, 0.9, 1.3, 1.1])
     v_dot = variable(300, 'L/min', 3)
     air_speed = variable([6.5, 6, 5.5, 5, 4.5, 4, 3.5], 'm/s', [0.1, 0.15, 0.12, 0.13, 0.9, 1.1, 1.0])
```

### Comparing `pyees-1.4.4/pyees/prop.py` & `pyees-1.4.5/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/sheet.py` & `pyees-1.4.5/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/solve.py` & `pyees-1.4.5/pyees/solve.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
     for i, res in enumerate(residuals):
         ## loop over the variables
         currentIndex = 0
         for xj in x:
             for xjj in xj:
                 if xjj in res.dependsOn:               
                     ## add the gradient d(residual)/d(xj) to the jacobian matrix
-                    J[i, currentIndex] += res.dependsOn[xjj][1]
+                    J[i, currentIndex] += res.dependsOn[xjj]
                 currentIndex += 1
            
     # inverse the jacobian
     Jinv = np.linalg.inv(J)
 
     ## add the dependency from the residual to the variables
     for i, res in enumerate(residuals):
```

### Comparing `pyees-1.4.4/pyees/stackOverflowODR.py` & `pyees-1.4.5/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/testFit.py` & `pyees-1.4.5/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/testProp.py` & `pyees-1.4.5/pyees/testProp.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         massFlow = flow * rho
         
         dMassFlow_dFlow = [998.206543497641114, 997.05155024142658, 995.644405820880468]
         dMassFlow_dP = [7.32946279081818364e-10, 7.21788150328467529e-10, 7.13326743322344253e-10]
         dMassFlow_dT = [-0.000330293371618005199, -0.000410463892510075697, -0.000483157770611803349]
         
         for i, elem in enumerate(massFlow):
-            self.assertAlmostEqual(elem.dependsOn[flow][1], dMassFlow_dFlow[i], 6)
-            self.assertAlmostEqual(elem.dependsOn[T[i]][1], dMassFlow_dT[i], 6)
-            self.assertAlmostEqual(elem.dependsOn[P[i]][1], dMassFlow_dP[i], 6)
+            self.assertAlmostEqual(elem.dependsOn[flow], dMassFlow_dFlow[i], 6)
+            self.assertAlmostEqual(elem.dependsOn[T[i]], dMassFlow_dT[i], 6)
+            self.assertAlmostEqual(elem.dependsOn[P[i]], dMassFlow_dP[i], 6)
         
       
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyees-1.4.4/pyees/testPyees.py` & `pyees-1.4.5/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/testSheet.py` & `pyees-1.4.5/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/testSolve.py` & `pyees-1.4.5/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/testUnit.py` & `pyees-1.4.5/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.4/pyees/testVariable.py` & `pyees-1.4.5/pyees/testVariable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1265,15 +1265,15 @@
         a = variable(123, 'L/min', 9.7)
         b = variable(93, 'Pa', 1.2)
         a.addCovariance(b, 23, 'L-Pa/min')
         a.convert('m3/s')
         c = a * b
         self.assertEqual(c.value, 123 * 93 / 1000 / 60)
         self.assertTrue(c._unitObject ==unit('m3-Pa/s'))
-        self.assertEqual(c.uncert, np.sqrt((123 / 1000 / 60 * 1.2)**2 + (93 * 9.7 / 1000 / 60)**2 + 2 * 93 * 123 / 1000 / 60 * 23 / 1000 / 60))
+        self.assertAlmostEqual(c.uncert, np.sqrt((123 / 1000 / 60 * 1.2)**2 + (93 * 9.7 / 1000 / 60)**2 + 2 * 93 * 123 / 1000 / 60 * 23 / 1000 / 60))
         
         a = variable(123, 'L/min', 9.7)
         b = variable(93, 'Pa', 1.2)
         a.addCovariance(b, 23, 'm3-Pa/s')
         a.convert('m3/s')
         c = a * b
         self.assertEqual(c.value, 123 * 93 / 1000 / 60)
@@ -1289,15 +1289,15 @@
         dcda = np.array([93, 97, 102], dtype = float)
         dcdb = np.array([1, 2, 3], dtype = float)
         ua = np.array([0.1, 0.2, 0.3], dtype = float)
         ub = np.array([1.2, 2.4, 4.7], dtype = float)
         uab = np.array([2, 3, 4], dtype = float)
 
         uc = np.sqrt((dcda * ua)**2 + (dcdb * ub)**2 + 2 * dcda * dcdb * uab)
-        np.testing.assert_equal(c.uncert, uc)
+        np.testing.assert_array_almost_equal(c.uncert, uc)
 
     def testConvert(self):
         a = variable(1, 'km', 0.1)
         b = variable(1, 'm', 0.1)
         c = a * b
         c.convert('mm2')
         self.assertEqual(c.value, 1e9)
```

### Comparing `pyees-1.4.4/pyees/unit.py` & `pyees-1.4.5/pyees/unit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import numpy as np
 from fractions import Fraction
-from copy import copy
+
 
 class _unitConversion():
     def __init__(self, scale, offset=0) -> None:
         self.scale, self.offset = scale, offset
      
     @staticmethod
     def staticMul(selfScale, selfOffset, otherScale, otherOffset = 0):
         scale = selfScale * otherScale
         offset = selfScale * otherOffset + selfOffset
         return scale, offset
     
     @staticmethod
     def staticPow(scale, offset, pow):
         if pow == 1: return scale, offset
+                
+        pos = pow > 0
+        scale, offset = (scale, offset) * pos + _unitConversion.staticTruediv(1,0,scale, offset) * (not pos)
+        pow = pow * pos - pow * (not pos)
+        
         scale = scale ** pow
         offset = offset * sum([scale ** (pow - i) for i in range(pow)])
         return scale, offset
        
     @staticmethod
     def staticTruediv(selfScale, selfOffset, otherScale, otherOffset = 0):
         return _unitConversion.staticMul(1 / otherScale, - otherOffset / otherScale, selfScale, selfOffset)
@@ -27,43 +32,49 @@
         return self.scale * value + useOffset * self.offset
 
 class neperConversion():
             
     @staticmethod
     def convertToSignal(var):
         var._uncert = 2*np.exp(2*var.value) * var.uncert
+        var._uncertSI = 2*np.exp(2*var.value) * var._uncertSI
         var._value = np.exp(2*var.value)
         
     @staticmethod
     def convertFromSignal(var):
         var._uncert = 1 / (2*var.value) * var.uncert
+        var._uncertSI = 1 / (2*var.value) * var._uncertSI
         var._value = 1/2 * np.log(var.value)
 
 class bellConversion():
         
     @staticmethod
     def convertToSignal(var):
         var._uncert = 10**var.value * np.log(10) * var.uncert
+        var._uncertSI = 10**var.value * np.log(10) * var._uncertSI
         var._value = 10**var.value
         
     @staticmethod
     def convertFromSignal(var):
         var._uncert = 1 / (var.value * np.log(10)) * var.uncert
+        var._uncertSI = 1 / (var.value * np.log(10)) * var._uncertSI
         var._value = np.log10(var.value)
 
 class octaveConversion():
         
     @staticmethod
     def convertToSignal(var):
         var._uncert = 2**var.value * np.log(2) * var.uncert
+        var._uncertSI = 2**var.value * np.log(2) * var._uncertSI
         var._value = 2**var.value
         
     @staticmethod
     def convertFromSignal(var):
         var._uncert = 1 / (var.value * np.log(2)) * var.uncert
+        var._uncertSI = 1 / (var.value * np.log(2)) * var._uncertSI
         var._value = np.log2(var.value)
 
     
     
 baseUnit = {
     '1': (1,0),
     '': (1,0),
@@ -277,17 +288,19 @@
     def existingUnitDictSIMethod(): return existingUnitDictSI
 
     
     for u, item in existingUnitDict.items():
         for pre, exp in item.items():
             convScale, convOffset = knownUnits[u][1]
             convScale = convScale * knownPrefixes[pre]
+            if convScale == 1 and convOffset == 0: continue
             isUpper = exp > 0
             if not isUpper: exp = -exp 
             convScale, convOffset = _unitConversion.staticPow(convScale, convOffset, exp)
+            ## i have no idea why the order of the inputs has to be swapped when comparing _unitConversion.staticMul and _unitConversion.staticTruediv
             if isUpper:
                 scale, offset = _unitConversion.staticMul(convScale, convOffset, scale, offset)
             else:
                 scale, offset = _unitConversion.staticTruediv(scale, offset, convScale, convOffset)      
     
     knownUnits[newUnit] = [existingUnitDictSIMethod, (scale, offset)]
         
@@ -299,57 +312,59 @@
 hyphen = '-'
 slash = '/'
 integers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
 
 
 class unit():
 
-    def __init__(self, unitStr = None, unitDict = None, unitDictSI = None):
+    def __init__(self, unitStr = None, unitDict = None, unitDictSI = None, selfUnitStr = None, selfUnitStrSI = None, converterToSI = None):
         if unitStr is None:
             unitStr = ''
         
         if unitDict is None:
             self.unitDict = self._getUnitDict(self._formatUnitStr(unitStr))
         else:
             self.unitDict = unitDict
         
         if unitDictSI is None:
             self.unitDictSI = self._getUnitDictSI(self.unitDict)
         else:
             self.unitDictSI = unitDictSI    
-            
-        self.unitStr = self._getUnitStrFromDict(self.unitDict)
-        self.unitStrSI = self._getUnitStrFromDict(self.unitDictSI)
-        self.getConverterToSI()
+        
+        if selfUnitStr is None:
+            self.unitStr = self._getUnitStrFromDict(self.unitDict)
+        else:
+            self.unitStr = selfUnitStr
+        
+        if selfUnitStrSI is None:
+            self.unitStrSI = self._getUnitStrFromDict(self.unitDictSI)
+        else:
+            self.unitStrSI = selfUnitStrSI
+        
+        if converterToSI is None:
+            self.getConverterToSI()
+        else:
+            self._converterToSI = converterToSI
 
     @staticmethod
     def _getUnitStrFromDict(unitDict):
         upper, lower = [], []
+        
         for u, item in unitDict.items():    
             for p, exp in item.items():
-                up = exp > 0
-                
-                if not up:
-                    exp *= -1
-                
-                if exp == 1:
-                    exp = ''
-                
-                s = f'{p}{u}{exp}'
-                if up:
-                    upper.append(s)
-                else:
-                    lower.append(s)
-                                
-        upper = '-'.join(upper)
-        
-        if lower:
-            upper += '/' + '-'.join(lower)
-                
-        return upper
+                isUpper = exp > 0
+                if not isUpper: exp = -exp
+                if exp == 1: s = p+u
+                else: s = p+u+str(exp)
+                if isUpper: upper.append(s)
+                else: lower.append(s)
+                            
+        out = '-'.join(upper)
+        if lower: out = out + '/' + '-'.join(lower)
+        return out
       
     def getUnitWithoutPrefix(self):
         
         upper, lower = [],[]
         
         for key, item in self.unitDict.items():
             exp = sum(item.values())
@@ -395,44 +410,44 @@
     def _reduceDict(unitDict):
         
         ## loop over all units, and remove any prefixes, which has an exponenet of 0
         for key, item in unitDict.items():
             prefixesToRemove = []
             for pre, exp in item.items():
                 if exp == 0:  prefixesToRemove.append(pre)
-            for pre in prefixesToRemove: unitDict[key].pop(pre)
+            for pre in prefixesToRemove: item.pop(pre)
     
         ## remove the units, which has no items in their dictionary
         keysToRemove = []
         for key, item in unitDict.items():
             if not item: keysToRemove.append(key)
         for key in keysToRemove: unitDict.pop(key)
         
         ## remove the unit '1' above the fraction line, if there are any other units above the fraction line
         if len(unitDict) > 1 and '1' in unitDict:
             otherUpper = False
             for key, item in unitDict.items():
                 if key == '1':
                     continue
-                for pre, exp in item.items():
+                for exp in item.values():
                     if exp > 0:
                         otherUpper = True
                         break
                 if otherUpper:
                     break
             if otherUpper:
                 unitDict.pop('1')
                 
+        ## return '1' if there are not other units
+        if not unitDict:
+            return {'1': {'': 1}}
+                
         ## set the exponent of the unit '1' to 1
         if '1' in unitDict:
-            unitDict['1'] = {'':1}
-            
-        ## add the units '1' if there are not other units
-        if not unitDict:
-            unitDict = {'1': {'': 1}}
+            unitDict['1'][''] = 1
         
         ## make temperature units in to temperature differences, if there are any other units in the dict
         if len(unitDict) > 1:
             keysToChange = []
             for key in unitDict.keys():
                 if key in temperature: keysToChange.append(key)
             for key in keysToChange: 
@@ -718,45 +733,46 @@
             selfUnitDictWithoutPrefixes[key] = {}
             selfUnitDictWithoutPrefixes[key][''] = 0
             for exp in item.values():
                 selfUnitDictWithoutPrefixes[key][''] += exp
         
         ## determine if self is the same as other - then no conversions are necessary
         if self.unitDict == other.unitDict:
-            return unit(unitDict=self.unitDict, unitDictSI=self.unitDictSI)  
-        
+            return self
+            
         ## determine the units of other without any prefixes and convert this to a string
         otherUnitDictWithoutPrefixes = {}
         for key, item in other.unitDict.items():
             otherUnitDictWithoutPrefixes[key] = {}
             otherUnitDictWithoutPrefixes[key][''] = 0
             for exp in item.values():
                 otherUnitDictWithoutPrefixes[key][''] += exp
         
         ## determine if the self and other are identical once any prefixes has been removed
         if selfUnitDictWithoutPrefixes == otherUnitDictWithoutPrefixes:
-            return unit(unitDict=selfUnitDictWithoutPrefixes, unitDictSI=self.unitDictSI)
+            return unit(unitDict=selfUnitDictWithoutPrefixes, unitDictSI=self.unitDictSI, selfUnitStrSI=self.unitStrSI)
         
         # determine if the SI base units of self and other are equal
         if self.unitDictSI == other.unitDictSI:
-            return unit(unitDict=self.unitDictSI, unitDictSI=self.unitDictSI)
+            return unit(unitDict=self.unitDictSI, unitDictSI=self.unitDictSI, selfUnitStr=self.unitStrSI, selfUnitStrSI = self.unitStrSI, converterToSI=_unitConversion(1,0))
         
         ## determine if "DELTAK" and "K" are the SI Baseunits of self and other
         SIBaseUnits = [self.unitDictSI, other.unitDictSI]        
         if {'DELTAK':{'':1}} in SIBaseUnits and {'K':{'':1}} in SIBaseUnits:
             
             indexTemp = SIBaseUnits.index({'K':{'':1}})
             indexDiff = 0 if indexTemp == 1 else 1
             
-            units = [list(selfUnitDictWithoutPrefixes.keys())[0], list(otherUnitDictWithoutPrefixes.keys())[0]]
+            units = [self.unitStr, other.unitStr]
 
-            if units[indexTemp] == units[indexDiff][-1]:        
-                return unit(unitDict=[selfUnitDictWithoutPrefixes, otherUnitDictWithoutPrefixes][indexTemp], unitDictSI = SIBaseUnits[indexTemp])
-            
-            return unit(unitDict={'K':{'':1}}, unitDictSI={'K':{'':1}})
+            ## check to see if the temperature differnce has the same unit as the temperature
+            if units[indexTemp] == units[indexDiff][-1]:
+                return [self, other][indexTemp]        
+                
+            return unit(unitDict={'K':{'':1}}, unitDictSI={'K':{'':1}}, selfUnitStr = 'K', selfUnitStrSI = 'K', converterToSI=_unitConversion(1,0))
 
         raise ValueError(f'You tried to add a variable in [{self}] to a variable in [{other}], but the units do not have the same SI base unit')
 
     def __sub__(self, other):
         
         ## determine the units of self without any prefixes
         selfUnitDictWithoutPrefixes = {}
@@ -776,88 +792,95 @@
                 otherUnitDictWithoutPrefixes[key][''] += exp
         
         
         ## determine if "DELTAK" and "K" are the SI Baseunits of self and other
         SIBaseUnits = [self.unitDictSI, other.unitDictSI]        
         if SIBaseUnits[0] == {'K':{'':1}} and SIBaseUnits[1] == {'K':{'':1}}:
             if self.unitDict == other.unitDict:
-                return unit(unitDict = self.unitDict, unitDictSI=self.unitDictSI)
-            return unit(unitDict={'K':{'':1}}, unitDictSI={'K':{'':1}})
+                return self
+            return unit(unitDict={'K':{'':1}}, unitDictSI={'K':{'':1}}, selfUnitStr='K', selfUnitStrSI = 'K', converterToSI=_unitConversion(1,0))
 
         if {'DELTAK':{'':1}} in SIBaseUnits and {'K':{'':1}} in SIBaseUnits:
             indexTemp = SIBaseUnits.index({'K':{'':1}})
             if indexTemp != 0:
                 raise ValueError('You tried to subtract a temperature from a temperature differnce. This is not possible.')      
-            return unit(unitDict=[selfUnitDictWithoutPrefixes, otherUnitDictWithoutPrefixes][indexTemp], unitDictSI=SIBaseUnits[indexTemp])
-        
+            return [self, other][indexTemp]
                 
         ## determine if self is the same as other - then no conversions are necessary
         if self.unitDict == other.unitDict:
-            return unit(unitDict=self.unitDict, unitDictSI = self.unitDictSI)
+            return self
         
         ## determine if the self and other are identical once any prefixes has been removed
         if selfUnitDictWithoutPrefixes == otherUnitDictWithoutPrefixes:
-            return unit(unitDict=selfUnitDictWithoutPrefixes, unitDictSI=self.unitDictSI)
+            return unit(unitDict=selfUnitDictWithoutPrefixes, unitDictSI=self.unitDictSI, selfUnitStrSI=self.unitStrSI)
         
         # determine if the SI base units of self and other are equal
         if self.unitDictSI == other.unitDictSI:
-            return unit(unitDict=self.unitDictSI, unitDictSI = self.unitDictSI)
+            return unit(unitDict=self.unitDictSI, unitDictSI = self.unitDictSI, selfUnitStr = self.unitStrSI, selfUnitStrSI=self.unitStrSI, converterToSI=_unitConversion(1,0))
         
         
         raise ValueError(f'You tried to subtract a variable in [{other}] from a variable in [{self}], but the units do not have the same SI base unit')
 
     def __mul__(self, other):
-        out = {}
-        
+        unitDict = {}
         for key, item in self.unitDict.items():
-            out[key]= {}
+            unitDict[key]= {}
             for pre, exp in item.items():
-                out[key][pre] = exp
-        
+                unitDict[key][pre] = exp
+                
         for key, item in other.unitDict.items():
-            if not key in out:
-                out[key] = item
+            if not key in unitDict:
+                unitDict[key] = {}
+                for pre, exp in item.items():
+                    unitDict[key][pre] = exp
             else:
                 for pre, exp in item.items():
-                    if not pre in out[key]:
-                        out[key][pre] = exp
+                    if not pre in unitDict[key]:
+                        unitDict[key][pre] = exp
                     else:
-                        out[key][pre] += exp
+                        unitDict[key][pre] += exp
+                        
+        unitDict = unit._reduceDict(unitDict)
+                
+        converterToSI = _unitConversion(*_unitConversion.staticMul(self._converterToSI.scale, self._converterToSI.offset, other._converterToSI.scale, other._converterToSI.offset))
         
-        out = unit._reduceDict(out)
-        return unit(unitDict = out)
+        return unit(unitDict = unitDict, converterToSI = converterToSI)
     
     def __truediv__(self, other):
-        return unit(unitDict = unit.staticTruediv(self.unitDict, other.unitDict))
+        unitDict = unit.staticTruediv(self.unitDict, other.unitDict)
+        converterToSI = _unitConversion(*_unitConversion.staticTruediv(self._converterToSI.scale, self._converterToSI.offset, other._converterToSI.scale, other._converterToSI.offset))
+        return unit(unitDict = unitDict, converterToSI = converterToSI)
+   
     
     @staticmethod
     def staticTruediv(a, b):
-        out = {}
-        
+       
+        unitDict = {}
         for key, item in a.items():
-            out[key]= {}
+            unitDict[key]= {}
             for pre, exp in item.items():
-                out[key][pre] = exp
-        
+                unitDict[key][pre] = exp
+                
         for key, item in b.items():
-            if not key in out:
-                out[key] = {}
+            if not key in unitDict:
+                unitDict[key] = {}
                 for pre, exp in item.items():
-                    out[key][pre] = -1 * exp
+                    unitDict[key][pre] = -exp
             else:
                 for pre, exp in item.items():
-                    if not pre in out[key]:
-                        out[key][pre] = -exp
+                    if not pre in unitDict[key]:
+                        unitDict[key][pre] = -exp
                     else:
-                        out[key][pre] -= exp
-        
-        return unit._reduceDict(out)
+                        unitDict[key][pre] -= exp
+    
+        return unit._reduceDict(unitDict)
     
     def __pow__(self, power):
-        return unit(unitDict= unit.staticPow(self.unitDict, self.unitDictSI, self.unitStr, power))
+        unitDict = unit.staticPow(self.unitDict, self.unitDictSI, self.unitStr, power)
+        return unit(unitDict= unitDict)
     
     @staticmethod
     def staticPow(unitDict, unitDictSI, unitStr, power):
         
         if unitDict == {'1': {'': 1}}:
             return unitDict
         
@@ -908,21 +931,19 @@
         # initialize the scale and offset
         outScale, outOffset = 1,0
         
         ## loop over self.unitDict
         for u, item in self.unitDict.items():
             for pre, exp in item.items():
                 convScale, convOffset = knownUnits[u][1]
-                isUpper = exp > 0
-                if not isUpper: exp = -exp  
-                convScale, convOffset = _unitConversion.staticPow(convScale * knownPrefixes[pre], convOffset, exp)
-                if isUpper:
-                    outScale, outOffset = _unitConversion.staticMul(outScale, outOffset, convScale, convOffset)
-                else:
-                    outScale, outOffset = _unitConversion.staticTruediv(outScale, outOffset, convScale, convOffset)      
+                convScale = convScale * knownPrefixes[pre]
+                if convScale == 1 and convOffset == 0: continue
+                convScale, convOffset = _unitConversion.staticPow(convScale, convOffset, exp)
+                outScale, outOffset = _unitConversion.staticMul(outScale, outOffset, convScale, convOffset)
+     
         self._converterToSI = _unitConversion(outScale, outOffset)
 
     def getConverter(self, newUnitStr):  
         newUnitStr =  unit._formatUnitStr(newUnitStr)
         newUnitDict = unit._getUnitDict(newUnitStr)
         if newUnitDict == self.unitDictSI:
             return self._converterToSI
@@ -933,21 +954,18 @@
         
         outScale, outOffset = self._converterToSI.scale, self._converterToSI.offset
         
         ## loop over newUnitDict
         for u, item in newUnitDict.items():
             for pre, exp in item.items():
                 convScale, convOffset = knownUnits[u][1]
-                isUpper = exp > 0
-                if not isUpper: exp = -exp
-                convScale, convOffset = _unitConversion.staticPow(convScale * knownPrefixes[pre], convOffset, exp)
-                if not isUpper:
-                    outScale, outOffset = _unitConversion.staticMul(outScale, outOffset, convScale, convOffset)
-                else:
-                    outScale, outOffset = _unitConversion.staticTruediv(outScale, outOffset, convScale, convOffset)      
+                convScale = convScale * knownPrefixes[pre]
+                if convScale == 1 and convOffset == 0: continue
+                convScale, convOffset = _unitConversion.staticPow(convScale, convOffset, exp)
+                outScale, outOffset = _unitConversion.staticTruediv(outScale, outOffset, convScale, convOffset)      
             
         return _unitConversion(outScale, outOffset)
 
     def isCombinationUnit(self):
         return len(list(self.unitDict.keys())) > 1
 
     def getLogarithmicConverter(self):
@@ -957,15 +975,10 @@
             return bellConversion()
         if u == 'Np':
             return neperConversion()
         if u == 'oct':
             return octaveConversion()
         return bellConversion()
 
-if __name__ == '__main__':
 
-    addNewUnit('gnA', 9.81, 'm/s2')
-    a = unit('gnA')
-    converter = a.getConverter('m/s2')
-    print(converter.convert(1), 9.81)
-    # converter = unit('Rø').getConverter('C')
-    # print(converter.convert(100), 176.190476190476190476)
+    
+
```

### Comparing `pyees-1.4.4/pyees/variable.py` & `pyees-1.4.5/pyees/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     def __init__(self, value, unitObject : str | unit, uncert, nDigits) -> None:
         
         self._value = value
         self._uncert = uncert
 
         # create a unit object
         self._unitObject = unitObject if isinstance(unitObject, unit) else unit(unitObject)
+        self._uncertSI = self._unitObject._converterToSI.convert(self._uncert, useOffset=False)
 
         # number of digits to show
         self.nDigits = nDigits
 
         # uncertanty
         self.dependsOn = {}
         self.covariance = {}
@@ -209,28 +210,27 @@
             self.___addDependent(var, grad)    
             return
         
         # the variable depends on other variables
         # loop over the dependencies of the variables and add them to the dependencies of self.
         # this ensures that the product rule is used
         for vvar, dependency in var.dependsOn.items():
-            self.___addDependent(vvar, grad * dependency[1])
+            self.___addDependent(vvar, grad * dependency)
         
-    
     def ___addDependent(self, var, grad):
-        if not var in self.dependsOn:
-            ## the variable is not in the dependencies of self.
-            ## add it to the dictionary
-            unc = var._converterToSI.convert(var.uncert, useOffset = False)
-            self.dependsOn[var] = [unc, grad]
-        else:
+        if var in self.dependsOn:
             ## the variable is already in the dependencies of self
             ## increment the gradient
             ## this makes sure that the productrule of differentiation is followed
-            self.dependsOn[var][1] += grad
+            self.dependsOn[var] += grad
+            return 
+        
+        ## the variable is not in the dependencies of self.
+        ## add it to the dictionary
+        self.dependsOn[var] = grad
 
     def __iter__(self):
         self.n = 0
         return self
 
     def __next__(self):
         if self.n == 0:
@@ -252,33 +252,31 @@
         covariance = covUnit._converterToSI.convert(covariance, useOffset=False)
         
         self.covariance[var] = covariance        
         var.covariance[self] = covariance
         
     def _calculateUncertanty(self):
         
+        variance = 0
+        for var, grad in self.dependsOn.items():
+            ## variance from the measurements     
+            variance += (var._uncertSI * grad)**2
+           
+            # variance from the corralation between measurements
+            ## covariance = dict(var: covariance)
+            ## the gradients can be found in self.dependsOn
+            ## loop over all variables that are in var.covariance and also self.dependsOn
+            if not var.covariance: continue
+            for var2 in filter(lambda x: x in self.dependsOn, var.covariance):
+                variance += grad * self.dependsOn[var2] * var.covariance[var2]
+        
         ## all variances are determined in the SI unit system.
         ## these has to be converted back in the the unit of self
-        scale = 1 / self._converterToSI.convert(1, useOffset=False) ** 2
-        
-        # variance from each measurement
-        variance = sum([(unc * grad)**2 for unc, grad in self.dependsOn.values()]) * scale
-        
-        # variance from the corralation between measurements
-        ## covariance = list(vari, vari.currentValue, vari.currentUncert, varj, varj.currentValue, varj.currenctUncert, cov)
-        ## from the above the gradients can be found from self.dependsOn
-        for var1 in self.dependsOn.keys():
-            for var2 in var1.covariance.keys():
-                if var2 in self.dependsOn:
-                    grad1 = self.dependsOn[var1][1]
-                    grad2 = self.dependsOn[var2][1]
-                    cov = var1.covariance[var2]
-                    variance += scale * grad1 * grad2 * cov
-
-        self._uncert = np.sqrt(variance)
+        self._uncertSI = np.sqrt(variance)
+        self._uncert = self._uncertSI / self._converterToSI.convert(1, useOffset=False)
         
     def __add__(self, other):
         
         if not isinstance(other, scalarVariable):
             return self + variable(other, self.unit)
 
         # determine if the two variable can be added
@@ -1004,9 +1002,14 @@
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
     
 if __name__ == "__main__":
     a = variable(11,'dB', 0.1)
-    b = variable(19,'dB',1.2)
+    b = variable(19,'dB', 1.2)
+    print(a._uncertSI)
+    print(b._uncertSI)
     c = a + b
+    gradA = (10**(11/10)) / (10**(19/10) + 10**(11/10))
+    gradB = (10**(19/10)) / (10**(19/10) + 10**(11/10))
+    print(c.uncert, np.sqrt( (gradA * a.uncert)**2 + (gradB * b.uncert)**2))
```

### Comparing `pyees-1.4.4/pyees.egg-info/PKG-INFO` & `pyees-1.4.5/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.4
+Version: 1.4.5
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.4/setup.py` & `pyees-1.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.4.4',
+    version='1.4.5',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

