# Comparing `tmp/inflatox-0.1.1-cp37-abi3-win_amd64.whl.zip` & `tmp/inflatox-0.2.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 345714 bytes, number of entries: 11
--rw-r--r--  4.6 unx     5235 b- defN 23-Jul-01 17:09 inflatox-0.1.1.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jul-01 17:09 inflatox-0.1.1.dist-info/WHEEL
--rw-r--r--  4.6 unx    14114 b- defN 23-Jul-01 17:09 inflatox-0.1.1.dist-info/license_files/LICENSE-EN.txt
--rw-r--r--  4.6 unx   377429 b- defN 23-Jul-01 17:09 inflatox-0.1.1.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx    12946 b- defN 23-Jul-01 17:09 inflatox/compiler.py
--rw-r--r--  4.6 unx     8656 b- defN 23-Jul-01 17:09 inflatox/consistency_conditions.py
--rw-r--r--  4.6 unx    20784 b- defN 23-Jul-01 17:09 inflatox/symbolic.py
--rw-r--r--  4.6 unx      908 b- defN 23-Jul-01 17:09 inflatox/version.py
--rw-r--r--  4.6 unx     1189 b- defN 23-Jul-01 17:09 inflatox/__init__.py
--rwxr-xr-x  4.6 unx   502784 b- defN 23-Jul-01 17:09 inflatox/libinflx_rs.pyd
--rw-r--r--  4.6 unx      910 b- defN 23-Jul-01 17:09 inflatox-0.1.1.dist-info/RECORD
-11 files, 945049 bytes uncompressed, 344190 bytes compressed:  63.6%
+Zip file size: 344796 bytes, number of entries: 11
+-rw-r--r--  4.6 unx     5170 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx    14114 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/license_files/LICENSE-EN.txt
+-rw-r--r--  4.6 unx   377429 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx    11416 b- defN 23-Jul-21 17:38 inflatox/compiler.py
+-rw-r--r--  4.6 unx     8656 b- defN 23-Jul-21 17:38 inflatox/consistency_conditions.py
+-rw-r--r--  4.6 unx    20784 b- defN 23-Jul-21 17:38 inflatox/symbolic.py
+-rw-r--r--  4.6 unx      908 b- defN 23-Jul-21 17:38 inflatox/version.py
+-rw-r--r--  4.6 unx     1189 b- defN 23-Jul-21 17:38 inflatox/__init__.py
+-rwxr-xr-x  4.6 unx   495616 b- defN 23-Jul-21 17:38 inflatox/libinflx_rs.pyd
+-rw-r--r--  4.6 unx      910 b- defN 23-Jul-21 17:38 inflatox-0.2.0.dist-info/RECORD
+11 files, 936286 bytes uncompressed, 343272 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,17 +1,17 @@
-Filename: inflatox-0.1.1.dist-info/METADATA
+Filename: inflatox-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: inflatox-0.1.1.dist-info/WHEEL
+Filename: inflatox-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: inflatox-0.1.1.dist-info/license_files/LICENSE-EN.txt
+Filename: inflatox-0.2.0.dist-info/license_files/LICENSE-EN.txt
 Comment: 
 
-Filename: inflatox-0.1.1.dist-info/license_files/LICENSE.md
+Filename: inflatox-0.2.0.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: inflatox/compiler.py
 Comment: 
 
 Filename: inflatox/consistency_conditions.py
 Comment: 
@@ -24,11 +24,11 @@
 
 Filename: inflatox/__init__.py
 Comment: 
 
 Filename: inflatox/libinflx_rs.pyd
 Comment: 
 
-Filename: inflatox-0.1.1.dist-info/RECORD
+Filename: inflatox-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inflatox/compiler.py

```diff
@@ -17,16 +17,17 @@
 #  (1) Resident of the Kingdom of the Netherlands; agreement between licensor and
 #  licensee subject to Dutch law as per article 15 of the EUPL.
 
 #System imports
 import os
 import tempfile
 import textwrap
-import distutils.ccompiler as ccomp
+import subprocess
 from datetime import datetime
+import sys
 from sys import version as sys_version
 
 #Sympy imports
 import sympy
 from sympy.printing.c import C99CodePrinter
 
 #Internal imports
@@ -142,42 +143,16 @@
   """This class wraps the native platform C compiler. It can be used to generate,
   compile and link C code from a `HesseMatrix` instance to produce a `CompilationArtifact`
   which can be used to calculate consistency conditions. This process involves
   creating a symbol dictionary that maps all symbols used in the `HesseMatrix` to
   C-friendly symbols.
   """
   
-  @classmethod
-  def _set_compiler(cls, compiler_path: str|None = None, linker_path: str|None = None):
-    """Configures the compiler to be the default compiler for the current platform,
-    unless an explicit compiler and linker path have been specified.
-
-    ### Args
-      compiler_path (str, optional): path to the compiler executable. Defaults to None.
-      linker_path (str, optional): path to the linker executable. Defaults to None.
-    """
-    default_compiler = ccomp.new_compiler()
-    if compiler_path is not None:
-      default_compiler.set_executables(compiler=compiler_path)
-    if linker_path is not None:
-      default_compiler.set_executables(linker_exe=linker_path)
-    default_compiler
-    cls.compiler = default_compiler
-    
-  @classmethod
-  def _compiler_options(cls):
-    """Sets the appropriate compiler flags based on the current platform"""
-    compiler_type = cls.compiler.compiler_type
-    if compiler_type == 'unix':
-      return ['-O3','-Wall','-Werror','-fpic', '-lm', '-march=native'], ['-O3', '-fpic', '-lm', '-march=native']
-    else:
-      raise NotImplementedError(f'Inflatox currently does not support {compiler_type}.')
-    #TODO: add Windows support
-        
-  compiler = None
+  c_prefix = "inflx_auto_"
+  lib_prefix = "libinflx_auto_"
   
   def __init__(self,
     hesse_matrix: HesseMatrix,
     output_path: str|None = None,
     cleanup: bool = True
   ):
     """Constructor for a C Compiler (provided by the platform), which can be used
@@ -202,21 +177,21 @@
     - `cleanup` (bool, optional): if `True`, generated artifacts will be deleted
       when they are no longer necessary. Defaults to True.
     """
     self.output_file = open(output_path) if output_path is not None else tempfile.NamedTemporaryFile(
       mode='wt',
       delete=False,
       suffix='.c',
-      prefix='inflx_autoc_'
+      prefix=Compiler.c_prefix
     )
-    if Compiler.compiler is None: Compiler._set_compiler()
     self.hesse = hesse_matrix
     self._set_preamble(hesse_matrix.model_name)
     self.cleanup = cleanup
-  
+    self.zigcc_opts = ['-O3','-Wall','-Werror','-fpic', '-lm', '-march=native','-shared']
+   
   def _set_preamble(self, model_name: str):
     """prints preamble in generated c code"""
     self.c_code_preamble = f"""//This source file was automatically generated by Inflatox v0.1
 // Model: {model_name}, timestamp: {datetime.now().strftime("%Y-%m-%d, %H:%M:%S")}
 // Inflatox version: v{__version__}
 // System info: {sys_version}
 
@@ -269,41 +244,32 @@
 //Number of parameters
 const uint32_t N_PARAMTERS = {len(ccode_writer.param_dict)};
 """)
       
     #(6) Update symbol dictionary
     self.symbol_dict = ccode_writer.coord_dict
     self.symbol_dict.update(ccode_writer.param_dict)
-    
-  def _c_compile_and_link_inner(self):
-    """Compiles and links the generated C source as a platform-specific shared lib"""
+  
+  def _zigcc_compile_and_link(self):
     source_path = f'{self.output_file.name}'
-    libname = os.path.basename(source_path)[:-2]
-    shared_obj_path = self.compiler.library_filename(
-      libname, 'shared', output_dir=tempfile.tempdir
-    )
-    
-    #(2) Compile the generated source file
-    compiler_args, linker_args = self._compiler_options()
-    obj_path = self.compiler.compile(
-      [source_path],
-      output_dir='/',
-      extra_preargs=compiler_args
-    )
-    
-    #(3) Link the generated source filewill
-    self.compiler.link_shared_lib(
-      obj_path,
-      libname,
-      output_dir=tempfile.tempdir,
-      extra_preargs=linker_args
-    )
+    source_name = os.path.basename(source_path)[:-2].removeprefix(Compiler.c_prefix)
+    lib_name = f'{Compiler.lib_prefix}{source_name}.bin'
+    lib_path = f'{tempfile.tempdir}/{lib_name}'
+    
+    # Compile source with zig
+    subprocess.call([
+      sys.executable,
+      "-m", "ziglang",
+      "cc", "-o",
+      lib_path, #out
+      source_path, #in
+      *self.zigcc_opts #compiler options
+    ])
     
-    #(R) Path to all generated artifacts
-    return (source_path, obj_path[0], shared_obj_path)
+    return (source_path, lib_path)
     
   def compile(self) -> CompilationArtifact:
     """Compiles the Hesse matrix specified in the constructor of this class into
     a shared library that can be used in further calculations. This process involves
     creating a symbol dictionary that maps all symbols used in the `HesseMatrix`
     to C-friendly symbols. The output of this function contains this dictionary,
     see the docs of `CompilationArtifact` for more info.
@@ -322,20 +288,19 @@
       It contains info about the model and inflatox version used to create the
       artifact.
     """
     #(1) generate the actual C-source
     self._generate_c_file()
     
     #(2) run compiler and linker
-    source_path, obj_path, dylib_path = self._c_compile_and_link_inner()
+    source_path, dylib_path = self._zigcc_compile_and_link()
     
     #(3) cleanup unused artifacts
     if self.cleanup:
       os.remove(source_path)
-      os.remove(obj_path)
     
     #(R) return compilation artifact
     return CompilationArtifact(
       self.symbol_dict,
       dylib_path,
       self.hesse.dim,
       len(self.symbol_dict) - self.hesse.dim,
```

## inflatox/version.py

```diff
@@ -13,8 +13,8 @@
 #  You should have received a copy of the EUPL in an/all official language(s) of
 #  the European Union along with Inflatox.  If not, see 
 #  <https://ec.europa.eu/info/european-union-public-licence_en/>.
 #
 #  (1) Resident of the Kingdom of the Netherlands; agreement between licensor and
 #  licensee subject to Dutch law as per article 15 of the EUPL.
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
```

## Comparing `inflatox-0.1.1.dist-info/METADATA` & `inflatox-0.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: inflatox
-Version: 0.1.1
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: cffi
 Requires-Dist: numpy >1
 Requires-Dist: sympy >1
 Requires-Dist: joblib >1
 Requires-Dist: einsteinpy >=0.4
+Requires-Dist: ziglang >=0.10
 License-File: LICENSE-EN.txt
 License-File: LICENSE.md
 Summary: Framework for implementing high-performance numerical consistency conditions for multifield inflation models.
 Keywords: physics,cosmology,inflation
 Home-Page: https://github.com/smups/inflatox/
 Author: Raúl Wolters <rawolters11@gmail.com>
 Author-email: Raúl Wolters <rawolters11@gmail.com>
@@ -28,20 +29,19 @@
 [![PyPi](https://img.shields.io/pypi/v/inflatox)](https://pypi.org/project/inflatox)
 [![CI](https://github.com/smups/inflatox/actions/workflows/CI.yml/badge.svg)](https://github.com/smups/inflatox/actions/workflows/CI.yml)
 
 Inflatox provides a framework to implement high-performance numerical consistency conditions for multifield inflation models. As an example, an implementation of the potential consistency condition for slow-roll rapid-turn two-field inflation from Anguelova & Lazaroiu (2023)[^1] is built right into the package.
 
 ## Features
 - symbolic solver for components of the Hesse matrix of an inflationary model with non-canonical kinetic terms, powered by [`sympy`](https://www.sympy.org).
-- compiler (with bindings to the platform-native C compiler) to transform `sympy` expressions into executable compiled code
+- transpiler (with bindings to the platform-native C compiler) to transform `sympy` expressions into executable compiled code
 - built-in multithreaded `rust` module for high-performance calculations of consistency conditions that interfaces directly with `numpy` and python.
 - no need to read, write or compile any `rust` or `C` code manually (this is all done automatically behind the scenes)
 
 ## Installation and Dependencies
-> Make sure to have a C compiler (and linker) installed on your computer when using `inflatox`.
 
 If you want to use the `inflatox` package and do not want to add your own native code to it, installing the `inflatox` python package is sufficient.
 - The `inflatox` python package can be installed by running the `pip install inflatox` command.
 
 If you would like to extend `inflatox` with your own native rust code, this can be achieved by extending the `inflatox` rust crate:
 - The `inflatox` rust crate can added to your rust project by adding it to your `Cargo.toml` as a dependency like so:
 ```toml
```

## Comparing `inflatox-0.1.1.dist-info/license_files/LICENSE-EN.txt` & `inflatox-0.2.0.dist-info/license_files/LICENSE-EN.txt`

 * *Files identical despite different names*

## Comparing `inflatox-0.1.1.dist-info/license_files/LICENSE.md` & `inflatox-0.2.0.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

## Comparing `inflatox-0.1.1.dist-info/RECORD` & `inflatox-0.2.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-inflatox-0.1.1.dist-info/METADATA,sha256=o6b8rBkAOKa-8uo9vosblw7UVVQuKKT19W8EsuzUQFA,5235
-inflatox-0.1.1.dist-info/WHEEL,sha256=EOMNtrT_gKkmhndb21X5-Kx7YThUf3BfKaagKjbmQiw,94
-inflatox-0.1.1.dist-info/license_files/LICENSE-EN.txt,sha256=Aif1zk6wdAUTw1KYZpRUC_cXUeVECcTDwYncAOS1DFI,14114
-inflatox-0.1.1.dist-info/license_files/LICENSE.md,sha256=KmidoWBnFWjACK_7WlJKWKoQmwzCzFjn5L5V0wPtcyQ,377429
-inflatox/compiler.py,sha256=UKSoZ71iEV9uOSML4M78g6_d7ZTRsuLEmAkSAHi-YQA,12946
+inflatox-0.2.0.dist-info/METADATA,sha256=LmZLc9Hc7IBabNup4jGAOPBkMzt30I54SQN8So8bG7U,5170
+inflatox-0.2.0.dist-info/WHEEL,sha256=EOMNtrT_gKkmhndb21X5-Kx7YThUf3BfKaagKjbmQiw,94
+inflatox-0.2.0.dist-info/license_files/LICENSE-EN.txt,sha256=Aif1zk6wdAUTw1KYZpRUC_cXUeVECcTDwYncAOS1DFI,14114
+inflatox-0.2.0.dist-info/license_files/LICENSE.md,sha256=KmidoWBnFWjACK_7WlJKWKoQmwzCzFjn5L5V0wPtcyQ,377429
+inflatox/compiler.py,sha256=D2gXrIYCIwh85h6R1q9S6gY-1APb1EQugateyB7Uo6Y,11416
 inflatox/consistency_conditions.py,sha256=oIvGdB37Inf0TUVv5jKp5aUQIxOdT4vrSG2CEL88Ofg,8656
 inflatox/symbolic.py,sha256=iLv2oTsGvfxy53qURfRx2cSu8thsIxSXB6ks0vekJDw,20784
-inflatox/version.py,sha256=2UGp86V-nPEeeCCqEZpOfxRiLcch0caP-tyN0yySn98,908
+inflatox/version.py,sha256=bgjvalwat8dCu27o6K_wuVg7hnihc6tjA5N-QgMwsek,908
 inflatox/__init__.py,sha256=pKHxt6-PAv5teetfVStAAFPkY1CY1H8cqcsR0sIl-5U,1189
-inflatox/libinflx_rs.pyd,sha256=P6rQUG2vVe6hPFmcuMa5yhoHQZhvVpwvJNy6QkrzoVk,502784
-inflatox-0.1.1.dist-info/RECORD,,
+inflatox/libinflx_rs.pyd,sha256=y3Lv8zVC0jqwOsc1qMoK_uZwxGEdSHPyNXJxOtVO42M,495616
+inflatox-0.2.0.dist-info/RECORD,,
```

