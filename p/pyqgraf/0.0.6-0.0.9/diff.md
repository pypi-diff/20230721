# Comparing `tmp/pyqgraf-0.0.6.tar.gz` & `tmp/pyqgraf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqgraf-0.0.6.tar", max compression
+gzip compressed data, was "pyqgraf-0.0.9.tar", max compression
```

## Comparing `pyqgraf-0.0.6.tar` & `pyqgraf-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2785 2023-01-03 01:26:44.183396 pyqgraf-0.0.6/README.md
--rw-r--r--   0        0        0     1128 2023-02-04 14:04:02.551192 pyqgraf-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    35149 2022-12-27 13:03:17.690042 pyqgraf-0.0.6/pyqgraf/LICENSE
--rw-r--r--   0        0        0        0 2022-12-27 10:20:42.543991 pyqgraf-0.0.6/pyqgraf/__init__.py
--rw-r--r--   0        0        0     3838 2022-12-27 10:35:26.531792 pyqgraf-0.0.6/pyqgraf/model.py
--rw-r--r--   0        0        0     4543 2023-02-04 14:02:50.309199 pyqgraf-0.0.6/pyqgraf/qgraf.py
--rw-r--r--   0        0        0     2783 2023-02-04 14:01:39.607247 pyqgraf-0.0.6/pyqgraf/wrap.py
--rw-r--r--   0        0        0     3568 1970-01-01 00:00:00.000000 pyqgraf-0.0.6/setup.py
--rw-r--r--   0        0        0     3497 1970-01-01 00:00:00.000000 pyqgraf-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2785 2023-04-16 12:16:51.905508 pyqgraf-0.0.9/README.md
+-rw-r--r--   0        0        0     1128 2023-04-16 12:16:53.361531 pyqgraf-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    35149 2023-04-16 12:16:51.905508 pyqgraf-0.0.9/pyqgraf/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-16 12:16:51.905508 pyqgraf-0.0.9/pyqgraf/__init__.py
+-rw-r--r--   0        0        0     3838 2023-04-16 12:16:51.909508 pyqgraf-0.0.9/pyqgraf/model.py
+-rw-r--r--   0        0        0     4805 2023-04-16 12:16:51.909508 pyqgraf-0.0.9/pyqgraf/qgraf.py
+-rw-r--r--   0        0        0     2879 2023-04-16 12:16:51.909508 pyqgraf-0.0.9/pyqgraf/wrap.py
+-rw-r--r--   0        0        0     3568 1970-01-01 00:00:00.000000 pyqgraf-0.0.9/setup.py
+-rw-r--r--   0        0        0     3497 1970-01-01 00:00:00.000000 pyqgraf-0.0.9/PKG-INFO
```

### Comparing `pyqgraf-0.0.6/README.md` & `pyqgraf-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyqgraf-0.0.6/pyproject.toml` & `pyqgraf-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqgraf"
-version = "0.0.6"
+version = "0.0.9"
 description = "PyQgraf is a Python wrapper for Qgraf, a Feynman diagram generator."
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyqgraf"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pyqgraf-0.0.6/pyqgraf/LICENSE` & `pyqgraf-0.0.9/pyqgraf/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqgraf-0.0.6/pyqgraf/model.py` & `pyqgraf-0.0.9/pyqgraf/model.py`

 * *Files identical despite different names*

### Comparing `pyqgraf-0.0.6/pyqgraf/qgraf.py` & `pyqgraf-0.0.9/pyqgraf/qgraf.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     if not reinstall and os.path.exists(qgraf_path):
         return
 
     import tempfile
     from skbuild import cmaker
 
     with tempfile.TemporaryDirectory() as tmpdirname:
-
         import tarfile
         import requests
 
         sub_ver = ".".join(version.split(".")[0:2])
 
         r = requests.get(
             f"http://anonymous:anonymous@qgraf.tecnico.ulisboa.pt/v{sub_ver}/qgraf-{version}.tgz",
@@ -84,19 +83,23 @@
 
       [3] Feynman graph generation and propagator mixing, I Comput. Phys. Commun. 269 (2021) 108103 https://doi.org/10.1016/j.cpc.2021.108103
 
 	"""
 )
 
 
-def call(dat="qgraf.dat"):
+def call(dat="qgraf.dat",silent=True):
     """Call qgraf with the given dat file."""
     global qgraf_path
-    print(f"{qgraf_path} {dat}")
-    subprocess.call(shlex.split(f"{qgraf_path} {dat}"))
+    # print(f"{qgraf_path} {dat}")
+    subprocess.call(
+        shlex.split(f"{qgraf_path} {dat}"),
+        stdout=subprocess.DEVNULL if silent else subprocess.STDOUT,
+        stderr=subprocess.STDOUT,
+    )
 
 
 def run(
     in_,
     out,
     loops,
     loop_momentum,
@@ -106,14 +109,15 @@
     output=None,
     fstyle="tmp.sty",
     fmodel="tmp.model",
     fdat="qgraf.dat",
     foutput="output.out",
     prefix_path=None,
     wrap=True,
+    silent=True,
     **kwargs,
 ):
     """
     Run qgraf with the given parameters.
 
     Args:
         in_ (str): list of incoming particles
@@ -124,28 +128,29 @@
         style (str): style file
         output (str): output file, unused
         options (str): options
         fstyle (str): style file
         fmodel (str): model file
         fdat (str): dat file
         foutput (str): output file
+        silent (bool): suppress qgraf output
 
 
     """
     if prefix_path is not None:
         fstyle = prefix_path + style
         fmodel = prefix_path + model
         fdat = prefix_path + fdat
         foutput = prefix_path + foutput
     if model is not None:
         if wrap:
-            model,wrapd = wrap_model(model)
-            for k,v in wrapd.items():
-                in_.replace(k,v)
-                out.replace(k,v)
+            model, wrapd = wrap_model(model)
+            for k, v in sorted(wrapd.items(), key=lambda x: len(x[0]), reverse=True):
+                in_ = in_.replace(k, v)
+                out = out.replace(k, v)
         io.write(fmodel, model, create_dir=False)
     if style is not None:
         io.write(fstyle, style, create_dir=False)
     args = ""
     for k, v in kwargs.items():
         args = args + f" {k} = {v};\n"
     io.write(
@@ -161,12 +166,12 @@
  options= {options};
      """
         + args,
         create_dir=False,
     )
     # remove output file if it exists
     io.remove(foutput)
-    call(fdat)
+    call(fdat,silent)
     ret = io.read(foutput)
     if wrap and model is not None:
         ret = dewrap_all(ret)
     return ret
```

### Comparing `pyqgraf-0.0.6/pyqgraf/wrap.py` & `pyqgraf-0.0.9/pyqgraf/wrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,33 +30,37 @@
         if "[" in line and "]" in line:
             content = line[line.index("[") + 1 : line.index("]")]
             contents = content.split(",")
             for i in range(len(contents)):
                 contents[i] = contents[i].strip()
             for i in range(len(contents)):
                 if contents[i] != "+" and contents[i] != "-":
-                    wrap_dict[contents[i]] = wrap(contents[i])
-                    contents[i] = begin + wrap_dict[contents[i]] + end
+                    wrap_dict[contents[i]] = begin +wrap(contents[i])+ end
+                    contents[i] =  wrap_dict[contents[i]] 
             rs += (
                 line[: line.index("[") + 1]
                 + ",".join(contents)
                 + line[line.index("]") :]
+                + "\n"
             )
         else:
             rs += line
+    # we need the wrap dict to be able to wrap the input for qgraf
     return rs, wrap_dict
 
 
-def dewrap_all(str, wrap_dict = None, begin=DEFAULT_BEGIN, end=DEFAULT_END):
+def dewrap_all(str, wrap_dict=None, begin=DEFAULT_BEGIN, end=DEFAULT_END):
     if wrap_dict is None:
-        for match in re.finditer(re.escape(begin) + r"([a-f0-9]+)" + re.escape(end), str):
+        for match in re.finditer(
+            re.escape(begin) + r"([a-f0-9]+)" + re.escape(end), str
+        ):
             str = str.replace(match.group(0), dewrap(match.group(1)))
     else:
         for key in wrap_dict:
-            str = str.replace(begin + wrap_dict[key] + end, key)
+            str = str.replace(wrap_dict[key], key)
     return str
 
 
 def dewrap_model(model, begin=DEFAULT_BEGIN, end=DEFAULT_END):
     """Dewrap a qgraf model with illegal characters in the name."""
     chars = "".join(str(n) for n in range(10)) + "abcdefg"
     rs = ""
```

### Comparing `pyqgraf-0.0.6/setup.py` & `pyqgraf-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests', 'scikit-build', 'smpl_io']
 
 setup_kwargs = {
     'name': 'pyqgraf',
-    'version': '0.0.6',
+    'version': '0.0.9',
     'description': 'PyQgraf is a Python wrapper for Qgraf, a Feynman diagram generator.',
     'long_description': '# pyqgraf\nSimplified plotting and fitting in python.\n\n[![PyPI version][pypi image]][pypi link] [![PyPI version][pypi versions]][pypi link] ![downloads](https://img.shields.io/pypi/dm/pyqgraf.svg)\n\n [![test][a t image]][a t link] [![Coverage Status][c t i]][c t l] [![Documentation][rtd t i]][rtd t l]\n\n## Documentation\n\n...\n\n## Versions\n\n### Stable\n\n```sh\npip install pyqgraf\n```\n\nOptional: --user or --upgrade\n\n### Dev\n\n```sh\npip install --index-url https://test.pypi.org/simple/ pyqgraf\n```\n\n[doc stable]: https://apn-pucky.github.io/pyqgraf/index.html\n[doc test]: https://apn-pucky.github.io/pyqgraf/test/index.html\n\n[pypi image]: https://badge.fury.io/py/pyqgraf.svg\n[pypi link]: https://pypi.org/project/pyqgraf/\n[pypi versions]: https://img.shields.io/pypi/pyversions/pyqgraf.svg\n\n[a s image]: https://github.com/APN-Pucky/pyqgraf/actions/workflows/stable.yml/badge.svg\n[a s link]: https://github.com/APN-Pucky/pyqgraf/actions/workflows/stable.yml\n[a t link]: https://github.com/APN-Pucky/pyqgraf/actions/workflows/test.yml\n[a t image]: https://github.com/APN-Pucky/pyqgraf/actions/workflows/test.yml/badge.svg\n\n[cc s q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s q l]: https://www.codacy.com/gh/APN-Pucky/pyqgraf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade?branch=stable\n[cc s c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2?branch=stable\n[cc s c l]: https://www.codacy.com/gh/APN-Pucky/pyqgraf/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage?branch=stable\n\n[cc q i]: https://app.codacy.com/project/badge/Grade/38630d0063814027bd4d0ffaa73790a2\n[cc q l]: https://www.codacy.com/gh/APN-Pucky/pyqgraf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=APN-Pucky/smpl&amp;utm_campaign=Badge_Grade\n[cc c i]: https://app.codacy.com/project/badge/Coverage/38630d0063814027bd4d0ffaa73790a2\n[cc c l]: https://www.codacy.com/gh/APN-Pucky/pyqgraf/dashboard?utm_source=github.com&utm_medium=referral&utm_content=APN-Pucky/smpl&utm_campaign=Badge_Coverage\n\n[c s i]: https://coveralls.io/repos/github/APN-Pucky/pyqgraf/badge.svg?branch=stable\n[c s l]: https://coveralls.io/github/APN-Pucky/pyqgraf?branch=stable\n[c t l]: https://coveralls.io/github/APN-Pucky/pyqgraf?branch=master\n[c t i]: https://coveralls.io/repos/github/APN-Pucky/pyqgraf/badge.svg?branch=master\n\n[rtd s i]: https://readthedocs.org/projects/pyqgraf/badge/?version=stable\n[rtd s l]: https://pyqgraf.readthedocs.io/en/stable/?badge=stable\n[rtd t i]: https://readthedocs.org/projects/pyqgraf/badge/?version=latest\n[rtd t l]: https://pyqgraf.readthedocs.io/en/latest/?badge=latest\n',
     'author': 'Alexander Puck Neuwirth',
     'author_email': 'alexander@neuwirth-informatik.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/APN-Pucky/pyqgraf',
```

### Comparing `pyqgraf-0.0.6/PKG-INFO` & `pyqgraf-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqgraf
-Version: 0.0.6
+Version: 0.0.9
 Summary: PyQgraf is a Python wrapper for Qgraf, a Feynman diagram generator.
 Home-page: https://github.com/APN-Pucky/pyqgraf
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

