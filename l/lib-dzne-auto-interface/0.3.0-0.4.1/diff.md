# Comparing `tmp/lib-dzne-auto-interface-0.3.0.tar.gz` & `tmp/lib-dzne-auto-interface-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-auto-interface-0.3.0.tar", last modified: Sun Jun 18 15:26:25 2023, max compression
+gzip compressed data, was "lib-dzne-auto-interface-0.4.1.tar", last modified: Fri Jul 21 19:26:10 2023, max compression
```

## Comparing `lib-dzne-auto-interface-0.3.0.tar` & `lib-dzne-auto-interface-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.3.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       26 2023-05-29 09:37:30.000000 lib-dzne-auto-interface-0.3.0/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      553 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/
--rw-r--r--   0 base      (1001) base      (1001)     2297 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/Information.py
--rw-rw-r--   0 base      (1001) base      (1001)    15234 2023-06-18 10:18:44.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/
--rw-r--r--   0 base      (1001) base      (1001)      886 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/HelpButton.py
--rw-r--r--   0 base      (1001) base      (1001)      654 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/Stack.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/inputs/
--rw-r--r--   0 base      (1001) base      (1001)     7764 2023-06-18 15:26:20.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/inputs/__init__.py
--rw-r--r--   0 base      (1001) base      (1001)     2265 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/inputs/_parsing_nargs.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-06-18 15:26:25.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      524 2023-06-18 15:26:25.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-18 15:26:25.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       24 2023-06-18 15:26:25.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-07-21 19:26:10.607008 lib-dzne-auto-interface-0.4.1/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.4.1/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-07-21 19:26:10.607008 lib-dzne-auto-interface-0.4.1/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       26 2023-05-29 09:37:30.000000 lib-dzne-auto-interface-0.4.1/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      553 2023-07-21 19:22:59.000000 lib-dzne-auto-interface-0.4.1/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-07-21 19:26:10.607008 lib-dzne-auto-interface-0.4.1/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-07-21 19:26:10.607008 lib-dzne-auto-interface-0.4.1/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-07-21 19:26:10.607008 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/
+-rw-r--r--   0 base      (1001) base      (1001)     2297 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/Information.py
+-rw-rw-r--   0 base      (1001) base      (1001)    17831 2023-06-25 12:46:44.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-07-21 19:26:10.607008 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/
+-rw-r--r--   0 base      (1001) base      (1001)      886 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/HelpButton.py
+-rw-r--r--   0 base      (1001) base      (1001)      654 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/Stack.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-07-21 19:26:10.607008 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/inputs/
+-rw-r--r--   0 base      (1001) base      (1001)     8026 2023-06-22 18:38:42.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/inputs/__init__.py
+-rw-r--r--   0 base      (1001) base      (1001)     2265 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/inputs/_parsing_nargs.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-07-21 19:26:10.607008 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-07-21 19:26:10.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      524 2023-07-21 19:26:10.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-07-21 19:26:10.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       24 2023-07-21 19:26:10.000000 lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface.egg-info/top_level.txt
```

### Comparing `lib-dzne-auto-interface-0.3.0/LICENSE` & `lib-dzne-auto-interface-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-auto-interface-0.3.0/PKG-INFO` & `lib-dzne-auto-interface-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.3.0
+Version: 0.4.1
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-auto-interface-0.3.0/pyproject.toml` & `lib-dzne-auto-interface-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-auto-interface"
-version = "0.3.0"
+version = "0.4.1"
 description = "Libary for automatically created interfaces. "
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/Information.py` & `lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/Information.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/__init__.py` & `lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-
 import argparse as _ap
+import contextlib as _ctx
 import inspect as _ins
+import os as _os
+import tempfile as _tmp
 import tkinter as _tk
+import tkinter.messagebox as _msg
 import tkinter.ttk as _ttk
 
+import lib_dzne_filedata as _fd
+
 import lib_dzne_auto_interface.gui.HelpButton as _HB
 import lib_dzne_auto_interface.gui.inputs as _inputs
 import lib_dzne_auto_interface.gui.Stack as _Stack
 import lib_dzne_auto_interface.Information as _Info
 
 
 class _KnotFrame(_tk.Frame):
@@ -32,15 +37,20 @@
     def parser(self, *, add_help):
         return _ap.ArgumentParser(
             add_help=add_help,
             parents=[self._parser],
             description=self._parser.description,
         )
     def parse(self, args, *, add_help=False):
-        return vars(self.parser(add_help=add_help).parse_args(args))
+        parser = self.parser(
+            add_help=add_help, 
+        )
+        namespace = parser.parse_args(args)
+        ans = vars(namespace)
+        return ans
     def frame(self, master):
         return type(self)._Frame(master=master, knot=self)
     @staticmethod
     def _details_from_annotation(annotation):
         if annotation is _ins.Parameter.empty:
             return {}
         if callable(annotation):
@@ -50,14 +60,19 @@
         return dict(annotation)      
     @property
     def subknots(self):
         return list(self._subknots)
 
 class _Argument(_Knot):
     class _Frame(_KnotFrame):
+        @property
+        def changed_argument(self):
+            ans = self.knot
+            ans = ans.change(help=None)
+            return ans
         def _init(self):
             self._labelFrame = self._add_labelFrame()
             self._helpButton = self._add_helpButton()
             self._argumentInput = self._add_argumentInput()
         def parse(self):
             args = self._argumentInput.get_args()
             kwargs = self.knot.parse(args)
@@ -83,91 +98,141 @@
                 padx=10,
                 pady=10,
             )
             return ans
         def _add_argumentInput(self):
             ans = _inputs.ArgumentInput(
                 self._labelFrame, 
-                argument=self.knot,
+                argument=self.changed_argument,
             )
             ans.pack(
                 padx=10,
                 pady=10,
                 side='left',
                 fill='both',
                 expand=True,
             )
             return ans
     def __init__(self, *args, **kwargs):
         self._subknots = list() # an argument cannot have subknots
-        self._dictionary = dict(*args, **kwargs)
-        info = _Info.Information(kwargs=self._dictionary)
+        dictionary = dict(*args, **kwargs)
+        for key in dictionary.keys():
+            if key not in self.keys():
+                raise KeyError(key)
+        info = _Info.Information(kwargs=dictionary)
+
+        # option_strings
         info.args = info.pop('option_strings', [])
+
+        # of_return
         of_return = info.pop('of_return', False)
         self._of_return = bool(of_return)
 
+        # required
+        if bool(info.pop('required', False)):
+            info['required'] = True
+
+        # help
+        Help = type(info.get('help', None))
+        if Help not in (type(None), str):
+            raise TypeError(f"{Help.__name__} is not a valid type for the parameter 'help'. ")
+
+        # nargs
+        Nargs = type(info.get('nargs', None))
+        if Nargs not in (type(None), str, int):
+            raise TypeError(f"{Nargs.__name__} is not a valid type for the parameter 'nargs'. ")
+
         # action
         info['action'] = info.get('action', 'store')
         self._action_string = info['action']
         if self._action_string not in (
             'store', 
-            #'store_const',
             'store_true', 
             'store_false', 
+            #'store_const',
             #'append',
             #'append_const',
         ):
             raise ValueError()
 
         self._parser = self._make_parser()
         self._action = info.exec(self._parser.add_argument)
+    def __getitem__(self, key):
+        if key not in self.keys():
+            raise KeyError(key)
+        if key == 'action':
+            return self._action_string
+        if key == 'of_return':
+            return self._of_return
+        if key == 'option_strings':
+            return tuple(self._action.option_strings)
+        return getattr(self._action, key)
+    @classmethod
+    def keys(cls):
+        return [
+            'option_strings',
+            'action',
+            'dest',
+            'nargs',
+            'const',
+            'default',
+            'type',
+            'choices',
+            'required',
+            'help',
+            'of_return',
+        ]
+    def items(self):
+        for key in self.keys():
+            yield key, self[key]
     def to_dict(self):
-        return dict(self._dictionary)
-    def configure(self, key, value):
+        return dict(self.items())
+    def change(self, **kwargs):
         dictionary = self.to_dict()
-        dictionary[key] = value
+        for key, value in kwargs.items():
+            dictionary[key] = value
         cls = type(self)
-        ans = cls(**dictionary)
+        ans = cls(dictionary)
         return ans
     @property
     def positional(self):
         return not bool(len(self.option_strings))
     @property
     def action(self):
-        return self._action_string
+        return self['action']
     @property
     def option_strings(self):
-        return tuple(self._action.option_strings)
+        return self['option_strings']
     @property
     def dest(self):
-        return self._action.dest
+        return self['dest']
     @property
     def nargs(self):
-        return self._action.nargs
+        return self['nargs']
     @property
     def const(self):
-        return self._action.const
+        return self['const']
     @property
     def default(self):
-        return self._action.default
+        return self['default']
     @property
     def type(self):
-        return self._action.type
+        return self['type']
     @property
     def choices(self):
-        return self._action.choices
+        return self['choices']
     @property
     def required(self):
-        return self._action.required
+        return self['required']
     @property
     def help(self):
-        return self._action.help
+        return self['help']
     @property
     def of_return(self):
-        return self._of_return
+        return self['of_return']
     @classmethod
     def argument_of_return(cls, annotation, *, details={}):
         if annotation is _ins.Parameter.empty:
             return None
         ann = cls._details_from_annotation(annotation)
         return _Argument(**ann, of_return=True, **details)
 
@@ -253,14 +318,15 @@
 
 class _Main(_Knot):
     def run_cli(self, args):
         dictionary = self.parse(args, add_help=True)
         self._run_dictionary(dictionary)
     def run_gui(self):
         root = _tk.Tk()
+        root.title("")
         frame = self.frame(root)
         frame.pack(fill='both', expand=True)
         root.mainloop()
     def run_dictionary(self, dictionary, /):
         dictionary = dict(dictionary)
         self._run_dictionary(dictionary)
     def _run_dictionary(self, dictionary):
@@ -280,16 +346,36 @@
         def parse(self):
             ans = dict()
             for level in self.stack.levels:
                 kwargs = level.parse()
                 ans = dict(**ans, **kwargs)
             return ans
         def go(self):
-            kwargs = self.parse()
-            self.knot.run_dictionary(kwargs)
+            with _tmp.TemporaryDirectory() as directory:
+                filename = "a" + _fd.TXTData.ext()
+                errlog = _os.path.join(directory, filename)
+                with open(errlog, "w") as s, _ctx.redirect_stderr(s):
+                    self._go_except()
+                txtData = _fd.TXTData.load(errlog)
+            text = str(txtData)
+            text = text.strip('\n')
+            if len(text):
+                _msg.showwarning(
+                    title="Error Log",
+                    message=text,
+                )
+        def _go_except(self):
+            try:
+                kwargs = self.parse()
+                self.knot.run_dictionary(kwargs)
+            except BaseException as exc:
+                _msg.showerror(
+                    title=type(exc).__name__,
+                    message=str(exc),
+                )
         def _add_buttonFrame(self):
             ans = _tk.Frame(self)
             ans.pack(
                 side='bottom',
                 fill='x',
                 padx=0,
                 pady=0,
@@ -423,15 +509,15 @@
                 pady=10,
             )
     def __init__(self, value, return_details):
         self._dest = value._dest
         self._description = value.__doc__
         self._mains = dict()
         parser = self._make_parser()
-        subparsers = parser.add_subparsers(dest=value._dest)
+        subparsers = parser.add_subparsers(dest=value._dest, required=True)
         for n, m in _ins.getmembers(value):
             if n.startswith("_"):
                 continue
             name = n.replace('_', '-')
             self._mains[name] = make(m, return_details=return_details)
             parent = self._mains[name].parser(add_help=False)
             subparser = subparsers.add_parser(
```

### Comparing `lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/HelpButton.py` & `lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/HelpButton.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/Stack.py` & `lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/Stack.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/inputs/__init__.py` & `lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/inputs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,30 +151,36 @@
         return [self.string]
 
 
 class CheckableInput(_Input):
     @property
     def checked(self):
         return bool(self._intVar.get())
-    def _init(self, factory, required):
+    def _init(self, *, factory, required, default=True, option_strings=[]):
+        default = int(bool(default))
         self._intVar = _tk.IntVar()
-        self._intVar.set(1)
+        self._intVar.set(default)
         self._checkbutton = self._add_checkbutton(required)
         self._subinput = self._add_subinput(factory)
+        self._option_strings = list(option_strings)
     def _config_active(self, value):
         self._subinput.active = value
         if self._checkbutton is not None:
             state = 'normal' if value else 'disabled'
             self._checkbutton.config(state=state)
     def get_args(self):
-        if self.checked is False:
-            return list()
+        ans = list()
+        if not self.checked:
+            return ans
+        if len(self._option_strings):
+            ans.append(self._option_strings[0])
         if self._subinput is None:
-            return list()
-        return self._subinput.get_args()
+            return ans
+        ans += self._subinput.get_args()
+        return ans
     def _check_change(self):
         if self._subinput is not None:
             self._subinput.active = self.checked
     def _add_checkbutton(self, required):
         if required:
             return None
         ans = _ttk.Checkbutton(
@@ -203,24 +209,22 @@
         return ans
 
 
 class QuestionInput(CheckableInput):
     def _init(self, argument):
         if argument.nargs != '?':
             raise ValueError
-        self._argument = argument
-        super()._init(factory=self._factory, required=False)
+        self._factory_argument = argument.change(nargs=None)
+        super()._init(
+            factory=self._factory, 
+            required=False,
+            option_strings=argument.option_strings,
+        )
     def _factory(self, master):
-        return _get_dim_0(master, argument=self._argument)
-    def get_args(self):
-        ans = list()
-        if self.checked and len(self._argument.option_strings):
-            ans.append(self._argument.option_strings[0])
-        ans += super().get_args()
-        return ans
+        return get(master, argument=self._factory_argument)
 
 
 class NargsIntInput(_Input):
     def _init(self, argument):
         if type(argument.nargs) is not int:
             raise TypeError
         if argument.nargs < 0:
@@ -251,16 +255,20 @@
         ans = self._scrolledText.get("1.0", "end-1c")
         ans = _parsing.parse(ans)
         return ans
 
 
 class ArgumentInput(CheckableInput):
     def _init(self, argument):
-        self._argument = argument
-        super()._init(factory=self._factory, required=argument.required)
+        self._factory_argument = argument.change(required=False)
+        super()._init(
+            factory=self._factory, 
+            required=argument.required,
+            option_strings=argument.option_strings,
+        )
     def _factory(self, master):
         return get(master, argument=self._argument)
```

### Comparing `lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/inputs/_parsing_nargs.py` & `lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface/gui/inputs/_parsing_nargs.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/PKG-INFO` & `lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.3.0
+Version: 0.4.1
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/SOURCES.txt` & `lib-dzne-auto-interface-0.4.1/src/lib_dzne_auto_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

