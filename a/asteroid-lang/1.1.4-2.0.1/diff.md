# Comparing `tmp/asteroid-lang-1.1.4.tar.gz` & `tmp/asteroid-lang-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asteroid-lang-1.1.4.tar", last modified: Thu Jan  5 18:35:37 2023, max compression
+gzip compressed data, was "asteroid-lang-2.0.1.tar", last modified: Fri Jul 21 11:18:19 2023, max compression
```

## Comparing `asteroid-lang-1.1.4.tar` & `asteroid-lang-2.0.1.tar`

### file list

```diff
@@ -1,48 +1,43 @@
-drwxr-xr-x   0 lutz       (501) staff       (20)        0 2023-01-05 18:35:37.154690 asteroid-lang-1.1.4/
--rw-r--r--   0 lutz       (501) staff       (20)     1084 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/LICENSE
--rw-r--r--   0 lutz       (501) staff       (20)     2694 2023-01-05 18:35:37.154574 asteroid-lang-1.1.4/PKG-INFO
--rw-r--r--   0 lutz       (501) staff       (20)     2105 2023-01-05 18:31:18.000000 asteroid-lang-1.1.4/README.md
-drwxr-xr-x   0 lutz       (501) staff       (20)        0 2023-01-05 18:35:37.149744 asteroid-lang-1.1.4/asteroid/
--rwxr-xr-x   0 lutz       (501) staff       (20)     5109 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/__init__.py
-drwxr-xr-x   0 lutz       (501) staff       (20)        0 2023-01-05 18:35:37.151134 asteroid-lang-1.1.4/asteroid/adb/
--rw-r--r--   0 lutz       (501) staff       (20)        0 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/adb/__init__.py
--rw-r--r--   0 lutz       (501) staff       (20)    32985 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/adb/adb.py
--rw-r--r--   0 lutz       (501) staff       (20)     7821 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/adb/command.py
--rw-r--r--   0 lutz       (501) staff       (20)     2425 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/adb/help.py
--rw-r--r--   0 lutz       (501) staff       (20)       15 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/adb/version.py
--rw-r--r--   0 lutz       (501) staff       (20)    36610 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/frontend.py
--rw-r--r--   0 lutz       (501) staff       (20)     5764 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/globals.py
--rw-r--r--   0 lutz       (501) staff       (20)     5562 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/interp.py
--rw-r--r--   0 lutz       (501) staff       (20)    10636 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/lex.py
-drwxr-xr-x   0 lutz       (501) staff       (20)        0 2023-01-05 18:35:37.153753 asteroid-lang-1.1.4/asteroid/modules/
--rw-r--r--   0 lutz       (501) staff       (20)     4960 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/bitwise.ast
--rw-r--r--   0 lutz       (501) staff       (20)     4813 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/modules/dataframe.ast
--rw-r--r--   0 lutz       (501) staff       (20)     3835 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/hash.ast
--rw-r--r--   0 lutz       (501) staff       (20)     7623 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/modules/io.ast
--rw-r--r--   0 lutz       (501) staff       (20)    11096 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/math.ast
--rw-r--r--   0 lutz       (501) staff       (20)    14265 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/os.ast
--rw-r--r--   0 lutz       (501) staff       (20)     1391 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/pick.ast
--rw-r--r--   0 lutz       (501) staff       (20)    22162 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/prologue.ast
--rw-r--r--   0 lutz       (501) staff       (20)     2179 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/random.ast
--rw-r--r--   0 lutz       (501) staff       (20)     2399 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/set.ast
--rw-r--r--   0 lutz       (501) staff       (20)     1189 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/modules/sort.ast
--rw-r--r--   0 lutz       (501) staff       (20)     2206 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/stream.ast
--rw-r--r--   0 lutz       (501) staff       (20)     7557 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/type.ast
--rw-r--r--   0 lutz       (501) staff       (20)     4123 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/util.ast
--rw-r--r--   0 lutz       (501) staff       (20)     2229 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/modules/vector.ast
--rw-r--r--   0 lutz       (501) staff       (20)     3636 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/repl.py
--rw-r--r--   0 lutz       (501) staff       (20)     1649 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/state.py
--rw-r--r--   0 lutz       (501) staff       (20)    14377 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/support.py
--rw-r--r--   0 lutz       (501) staff       (20)     4017 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/asteroid/symtab.py
--rw-r--r--   0 lutz       (501) staff       (20)      257 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/version.py
--rw-r--r--   0 lutz       (501) staff       (20)    84374 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/asteroid/walk.py
-drwxr-xr-x   0 lutz       (501) staff       (20)        0 2023-01-05 18:35:37.154430 asteroid-lang-1.1.4/asteroid_lang.egg-info/
--rw-r--r--   0 lutz       (501) staff       (20)     2694 2023-01-05 18:35:37.000000 asteroid-lang-1.1.4/asteroid_lang.egg-info/PKG-INFO
--rw-r--r--   0 lutz       (501) staff       (20)      990 2023-01-05 18:35:37.000000 asteroid-lang-1.1.4/asteroid_lang.egg-info/SOURCES.txt
--rw-r--r--   0 lutz       (501) staff       (20)        1 2023-01-05 18:35:37.000000 asteroid-lang-1.1.4/asteroid_lang.egg-info/dependency_links.txt
--rw-r--r--   0 lutz       (501) staff       (20)       43 2023-01-05 18:35:37.000000 asteroid-lang-1.1.4/asteroid_lang.egg-info/entry_points.txt
--rw-r--r--   0 lutz       (501) staff       (20)       24 2023-01-05 18:35:37.000000 asteroid-lang-1.1.4/asteroid_lang.egg-info/requires.txt
--rw-r--r--   0 lutz       (501) staff       (20)        9 2023-01-05 18:35:37.000000 asteroid-lang-1.1.4/asteroid_lang.egg-info/top_level.txt
--rw-r--r--   0 lutz       (501) staff       (20)      104 2022-12-19 19:53:15.000000 asteroid-lang-1.1.4/pyproject.toml
--rw-r--r--   0 lutz       (501) staff       (20)       38 2023-01-05 18:35:37.154723 asteroid-lang-1.1.4/setup.cfg
--rw-r--r--   0 lutz       (501) staff       (20)     1075 2023-01-05 18:11:02.000000 asteroid-lang-1.1.4/setup.py
+drwxr-xr-x   0 lutz       (501) staff       (20)        0 2023-07-21 11:18:19.072361 asteroid-lang-2.0.1/
+-rw-r--r--   0 lutz       (501) staff       (20)     1084 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/LICENSE
+-rw-r--r--   0 lutz       (501) staff       (20)     3860 2023-07-21 11:18:19.072239 asteroid-lang-2.0.1/PKG-INFO
+-rw-r--r--   0 lutz       (501) staff       (20)     3270 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/README.md
+drwxr-xr-x   0 lutz       (501) staff       (20)        0 2023-07-21 11:18:19.068108 asteroid-lang-2.0.1/asteroid/
+-rwxr-xr-x   0 lutz       (501) staff       (20)     4804 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/__init__.py
+-rw-r--r--   0 lutz       (501) staff       (20)    37051 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/frontend.py
+-rw-r--r--   0 lutz       (501) staff       (20)     5950 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/globals.py
+-rw-r--r--   0 lutz       (501) staff       (20)     5922 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/interp.py
+-rw-r--r--   0 lutz       (501) staff       (20)    10533 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/lex.py
+-rw-r--r--   0 lutz       (501) staff       (20)    16057 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/mad.py
+drwxr-xr-x   0 lutz       (501) staff       (20)        0 2023-07-21 11:18:19.071243 asteroid-lang-2.0.1/asteroid/modules/
+-rw-r--r--   0 lutz       (501) staff       (20)     4590 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/bitwise.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     4701 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/dataframe.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     3779 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/hash.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     7344 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/io.ast
+-rw-r--r--   0 lutz       (501) staff       (20)    23493 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/math.ast
+-rw-r--r--   0 lutz       (501) staff       (20)    13336 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/os.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     5103 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/patterns.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     1227 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/pick.ast
+-rw-r--r--   0 lutz       (501) staff       (20)    29554 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/prologue.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     1884 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/random.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     2116 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/set.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     1021 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/sort.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     2080 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/stream.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     3809 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/util.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     1983 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/modules/vector.ast
+-rw-r--r--   0 lutz       (501) staff       (20)     4204 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/repl.py
+-rw-r--r--   0 lutz       (501) staff       (20)     1540 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/state.py
+-rw-r--r--   0 lutz       (501) staff       (20)     8987 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/support.py
+-rw-r--r--   0 lutz       (501) staff       (20)     4614 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/symtab.py
+-rw-r--r--   0 lutz       (501) staff       (20)      280 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/version.py
+-rw-r--r--   0 lutz       (501) staff       (20)    76765 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/asteroid/walk.py
+drwxr-xr-x   0 lutz       (501) staff       (20)        0 2023-07-21 11:18:19.072068 asteroid-lang-2.0.1/asteroid_lang.egg-info/
+-rw-r--r--   0 lutz       (501) staff       (20)     3860 2023-07-21 11:18:19.000000 asteroid-lang-2.0.1/asteroid_lang.egg-info/PKG-INFO
+-rw-r--r--   0 lutz       (501) staff       (20)      896 2023-07-21 11:18:19.000000 asteroid-lang-2.0.1/asteroid_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 lutz       (501) staff       (20)        1 2023-07-21 11:18:19.000000 asteroid-lang-2.0.1/asteroid_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 lutz       (501) staff       (20)       43 2023-07-21 11:18:19.000000 asteroid-lang-2.0.1/asteroid_lang.egg-info/entry_points.txt
+-rw-r--r--   0 lutz       (501) staff       (20)       24 2023-07-21 11:18:19.000000 asteroid-lang-2.0.1/asteroid_lang.egg-info/requires.txt
+-rw-r--r--   0 lutz       (501) staff       (20)        9 2023-07-21 11:18:19.000000 asteroid-lang-2.0.1/asteroid_lang.egg-info/top_level.txt
+-rw-r--r--   0 lutz       (501) staff       (20)      104 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/pyproject.toml
+-rw-r--r--   0 lutz       (501) staff       (20)       38 2023-07-21 11:18:19.072404 asteroid-lang-2.0.1/setup.cfg
+-rw-r--r--   0 lutz       (501) staff       (20)     1214 2023-07-21 11:17:35.000000 asteroid-lang-2.0.1/setup.py
```

### Comparing `asteroid-lang-1.1.4/LICENSE` & `asteroid-lang-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asteroid-lang-1.1.4/PKG-INFO` & `asteroid-lang-2.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,54 @@
 Metadata-Version: 2.1
 Name: asteroid-lang
-Version: 1.1.4
+Version: 2.0.1
 Summary: A modern, multi-paradigm programming language.
 Home-page: https://asteroid-lang.org
 Author: University of Rhode Island
 Author-email: lutzhamel@uri.edu
 Project-URL: Documentation, https://asteroid-lang.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/asteroid-lang/asteroid/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Asteroid
 Asteroid is a modern, multi-paradigm programming language that supports first-class patterns.  More details can
 be found at the website [asteroid-lang.org](https://asteroid-lang.org).
 Documentation on Asteroid can be found at
 [asteroid-lang.readthedocs.io](https://asteroid-lang.readthedocs.io).
 
+## New in Release 2.0.1
+
+* We now support the ASTEROIDPATH environment variable which is expected to have a colon seperated list of directories to search for user defined modules.
+
+* The logical operators 'and' and 'or' are now evaluated in short-circuit fashion.
+
+* Files loaded with the 'load' statement are now considered modules and work similarly to Python modules.
+
+* Added the 'toplevel' function which returns true if control is in the module originally loaded by the interpreter.
+
+* Added the match statement similar to the match statement in Python.
+
+* No longer supports type hierarchies for the primitive types.  The functions in the 'type' module are now considered builtins. The 'type' module itself has been eliminated.
+
+* The Minimal Asteroid Debugger (MAD) replaces ADB in this release.
+
+* The shorthand conditional pattern can now be applied to arbitrary patterns. E.g. The pattern 
+  ```
+  (a,b,c):(%integer,%integer,%integer)
+  ```
+  constrains the triple `(a,b,c)` to be a triple of integers.  The above shorthand conditional pattern is equivalent to the conditional pattern,
+  ```
+  (a,b,c) if (a,b,c) is (%integer,%integer,%integer)
+  ```
+  
 ## New in Release 1.1.4
 
 * Allows pattern constraint operator to map certain variables that a pattern 
   matched to be bound into the current scope.
 
 * Supports a new OS module.
```

### Comparing `asteroid-lang-1.1.4/asteroid/__init__.py` & `asteroid-lang-2.0.1/asteroid/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,52 +8,53 @@
 import cProfile
 import sys
 import os
 import os.path
 from asteroid.interp import interp
 from asteroid.repl import repl
 from asteroid.version import VERSION
-from asteroid.adb import adb
+from asteroid.mad import MAD
 
 def display_help():
-    print("** Asteroid Version {} **".format(VERSION))
+    print("Asteroid {}".format(VERSION))
     print("(c) University of Rhode Island")
-    print("usage: asteroid [-<switch>] <input file>")
+    print("usage: asteroid [<switch>] <input file>")
     print("")
-    print("command line flags:")
+    print("command line switches:")
+    print(" -d             run program through debugger")
+    print(" -e             show Python exceptions")
+    print(" -F             functional mode")
+    print(" -h, --help     display help")
+    print(" -p             disable prologue")
+    print(" -r             disable redundant pattern detector")
     print(" -s             enable symbol table dump")
     print(" -t             AST dump")
     print(" -v, --version  version")
     print(" -w             disable tree walk")
+    print(" -W             disable warnings")
     print(" -z             generate pstats")
-    print(" -p             disable prologue")
-    print(" -h, --help     display help")
-    print(" -r             disable redundant pattern detector")
-    print(" -e             show Python exceptions")
-    print(" -F             functional mode")
-    print(" -g, --adb      run program through debugger")
 
 def main():
-    # defaults for the flags - when the flag is set on the command line
+    # defaults for the switches or flags - when the flag is set on the command line
     # it simply toggles the default value in this table.
     flags = {
+        '-d' : False,    # Short debugger flag
+        '-e' : False,  # show full exceptions
+        '-F' : False,  # functional mode
+        '--help' : False,  # display help flag
+        '-h' : False,  # display help flag
+        '-p' : True,   # prologue flag
+        '-r' : True,   # redundant pattern dectector
         '-s' : False,  # symbol table dump flag
         '-t' : False,  # AST dump flag
         '--version' : False,  # version flag
         '-v' : False,  # version flag
         '-w' : True,   # tree walk flag
+        '-W' : True,   # warnings
         '-z' : False,  # generate pstats flag
-        '-p' : True,   # prologue flag
-        '--help' : False,  # display help flag
-        '-h' : False,  # display help flag
-        '-r' : True,   # redundant pattern dectector
-        '-e' : False,  # show full exceptions
-        '-F' : False,  # functional mode
-        '--adb': False, # debugger flag
-        '-g': False    # Short debugger flag
     }
 
     flag_names = list(flags.keys())
     argv_ix = 1
     asteroid_ext = '.ast'
 
     # logic of command line parameters
@@ -76,18 +77,18 @@
 
     # determine if we need to respond to special flags and exit
     if flags['--help'] or flags['-h']:
         display_help()
         sys.exit(0)
 
     if flags['--version'] or flags['-v']:
-        print("** Asteroid Version {} **".format(VERSION))
+        print("Asteroid {}".format(VERSION))
         sys.exit(0)
 
-    debug_flag = flags['--adb'] or flags['-g']
+    debug_flag = flags['-d']
 
     # determine if we are starting in interactive mode or not
     # Note: first non-switch argument has to be an Asteroid source file
     if len(sys.argv) == argv_ix:
         input_file = ''
     else:
         input_file = sys.argv[argv_ix]
@@ -104,51 +105,43 @@
         sys.exit(0)
 
     # we have an input file, check if it exists
     if input_file and not os.path.isfile(input_file):
         print("error: unknown file '{}'".format(input_file))
         sys.exit(1)
 
-    # run the debugger
     if debug_flag:
-        if input_ext == '':
-            print("error: please provide a file to debug")
-            sys.exit(1)
         # Create a new debugger
-        db = adb.ADB()
-        # Set the debugger's internal interpretation options
-        db.interp_options = {
-            'redundancy': flags['-r'],
-            'prologue': flags['-p'],
-            'functional_mode': flags['-F'],
-            'exceptions': flags['-e'],
-        }
-        db.run(input_file)
-        sys.exit(0)
+        db = MAD()
+    else:
+        db = None
 
     # execute the interpreter
     f = open(input_file, 'r')
     input_stream = f.read()
     f.close()
 
     # execute interpreter
     interp_object = \
     '''interp(program=input_stream,
            program_name = input_file,
-           tree_dump=flags['-t'],
-           do_walk=flags['-w'],
-           symtab_dump=flags['-s'],
            exceptions=flags['-e'],
-           redundancy=flags['-r'],
+           functional_mode=flags['-F'],
            prologue=flags['-p'],
-           functional_mode=flags['-F'])'''
+           redundancy=flags['-r'],
+           symtab_dump=flags['-s'],
+           tree_dump=flags['-t'],
+           do_walk=flags['-w'],
+           warnings=flags['-W'],
+           debugger=db
+           )'''
 
     if flags['-z']:
         # generates pstats into the file 'pstats'
         # see https://docs.python.org/3/library/profile.html
-        cProfile.run(interp_object, 'pstats')
+        cProfile.runctx(interp_object, globals(), locals(), filename='pstats')
     else:
         exec(interp_object)
 
 # for manual testing purposes
 if __name__ == "__main__":
     main()
```

### Comparing `asteroid-lang-1.1.4/asteroid/frontend.py` & `asteroid-lang-2.0.1/asteroid/frontend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 ###########################################################################################
 # front end for Asteroid
 #
-# (c) Lutz Hamel, University of Rhode Island
+# (c) University of Rhode Island
 ###########################################################################################
 
 import os
 import sys
 from pathlib import Path, PurePath
 
 from asteroid.globals import asteroid_file_suffix, ExpectationError
 from asteroid.lex import Lexer, token_lookup
 from asteroid.state import state, warning
+from asteroid.support import gettemp
 
 ###########################################################################################
 def dbg_print(string):
     #print(string)
     pass
 
 ###########################################################################################
@@ -41,15 +42,15 @@
     'LBRACKET',
     'LPAREN',
     'TYPEMATCH',
     } | ops
 
 exp_lookahead = {
     'PATTERN',
-    'LCONSTRAINT',} | primary_lookahead
+    'LSCOPE',} | primary_lookahead
 
 exp_lookahead_no_ops = exp_lookahead - ops
 
 primary_lookahead_no_ops = exp_lookahead_no_ops
 
 stmt_lookahead = {
     'DOT',
@@ -58,14 +59,16 @@
     'FOR',
     'FUNCTION',
     'GLOBAL',
     'IF',
     'LET',
     'LOAD',
     'LOOP',
+    'MATCH',
+    'MODULE',
     'REPEAT',
     'RETURN',
     'STRUCTURE',
     'THROW',
     'TRY',
     'WHILE',
     #'WITH',
@@ -98,71 +101,53 @@
         return self.prog()
 
     ###########################################################################################
     # prog:
     #   stmt_list
     def prog(self):
         dbg_print("parsing PROG")
-        sl = self.stmt_list()
+        sl = ('stmt-list', self.stmt_list())
         if not self.lexer.EOF():
             raise SyntaxError("expected 'EOF' found {}." \
                               .format(token_lookup(self.lexer.peek().type)))
         else:
             dbg_print("parsing EOF")
         return sl
 
     ###########################################################################################
     # stmt_list
     #   : stmt*
     def stmt_list(self):
         dbg_print("parsing STMT_LIST")
 
         sl = []
-        while self.stmt_coming_up():
+        while self.lexer.peek().type in stmt_lookahead:
             sl += [('lineinfo', state.lineinfo)]
-
-            # Get the statment
-            stmt = self.stmt()
-
-            # This set of conditionals gives us the behavior we want
-            # wrt implicit return values. There's only one situation
-            # in which we want to set the return value. That is when
-            # a top level expression is the last in a stmt_list
-
-            # If there's a statement coming up or the current statement
-            # is not a top level expression, just append the statement
-            if self.stmt_coming_up() or stmt[0] != 'top-level-exp':
-                sl += [stmt]
-
-            # Otherwhise, if there's no statement coming up and the
-            # last statement was a top level expression, set the
-            # ret val
-            else:
-                sl += [('clear-ret-val',)]
-                sl += [('set-ret-val', stmt)]             
-
+            sl += [('clear-ret-val',)]
+            sl += [self.stmt()]
         return ('list', sl)
 
     ###########################################################################################
     # NOTE: periods are optional at end of sentences but leaving them out can
     #       lead to ambiguities
     # NOTE: the dot is also short hand for the 'noop' command
     #
     # stmt
     #    : '.' // NOOP
-    #    | LOAD SYSTEM? (STRING | ID) '.'?
+    #    | LOAD SYSTEM? (STRING | ID) (AS ID)? '.'?
     #    | GLOBAL id_list '.'?
     #    | ASSERT exp '.'?
     #    | STRUCTURE ID WITH struct_stmts END
     #    | LET pattern '=' exp '.'?
     #    | LOOP DO? stmt_list END
     #    | FOR pattern IN exp DO stmt_list END
     #    | WHILE exp DO stmt_list END
     #    | REPEAT (DO?) stmt_list UNTIL exp '.'?
     #    | BREAK
+    #    | MATCH exp (WITH pattern DO stmt_list)* END
     #    | IF exp DO stmt_list (ELIF exp DO stmt_list)* (ELSE (DO?) stmt_list)? END
     #    | RETURN exp? '.'?
     #    | TRY stmt_list (CATCH pattern DO stmt_list)+ END
     #    | THROW exp '.'?
     #    | function_def
     #    | exp '.'?
     def stmt(self):
@@ -177,47 +162,56 @@
             # expand the AST from the file into our current AST
             # using a nested parser object
             self.lexer.match('LOAD')
             sys_flag = bool(self.lexer.match_optional('SYSTEM'))
             # allow module names without quotes
             if self.lexer.peek().type in ['STRING', 'ID']:
                 str_tok = self.lexer.match(self.lexer.peek().type)
+                name_tok = None
             elif self.lexer.peek().type == 'EOF':
                 raise ExpectationError(expected="valid module name", found='EOF' )
             else:
                 raise SyntaxError("invalid module name '{}'"
                                   .format(self.lexer.peek().value))
+            # look for the 'as' modifier
+            if self.lexer.peek().type == 'AS':
+                self.lexer.match('AS')
+                name_tok = self.lexer.match('ID')
             self.lexer.match_optional('DOT')
 
             raw_pp = PurePath(str_tok.value)
-            module_name = raw_pp.stem
-
-            # if module is on the list of modules then we have loaded
-            # it already -- ignore -- continue parsing the program file
-            if module_name in state.modules:
-                # lhh
-                # print("Ignoring module {}".format(module_name))
-                return self.stmt_list()
+            base_name = raw_pp.stem
+            if name_tok:
+                module_name = name_tok.value
+            else:
+                module_name = base_name
 
             # search for module file:
             # 0. raw module name - could be an absolute path
             # 1. search in current working directory
             # 2. search in directory where Asteroid is installed
             # TODO: does this work on all OS's?
             # TODO: should have an env variable to set search path
             search_list = []
             if not sys_flag:
                 search_list.append(str_tok.value)
                 search_list.append(str_tok.value + asteroid_file_suffix)
-                search_list.append(os.path.join(os.getcwd(), module_name))
-                search_list.append(os.path.join(os.getcwd(), module_name + asteroid_file_suffix))
-                search_list.append(os.path.join(os.getcwd(), 'modules', module_name))
-                search_list.append(os.path.join(os.getcwd(), 'modules', module_name + asteroid_file_suffix))
-            search_list.append(os.path.join(os.path.split(os.path.abspath(__file__))[0], 'modules', module_name))
-            search_list.append(os.path.join(os.path.split(os.path.abspath(__file__))[0], 'modules', module_name + asteroid_file_suffix))
+                search_list.append(os.path.join(os.getcwd(), base_name))
+                search_list.append(os.path.join(os.getcwd(), base_name + asteroid_file_suffix))
+                search_list.append(os.path.join(os.getcwd(), 'modules', base_name))
+                search_list.append(os.path.join(os.getcwd(), 'modules', base_name + asteroid_file_suffix))
+                # check the ASTEROIDPATH variable
+                env_val = os.getenv('ASTEROIDPATH')
+                if env_val:
+                    path_list = env_val.split(':')
+                    for p in path_list:
+                        search_list.append(p+'/'+base_name+asteroid_file_suffix)
+
+            search_list.append(os.path.join(os.path.split(os.path.abspath(__file__))[0], 'modules', base_name))
+            search_list.append(os.path.join(os.path.split(os.path.abspath(__file__))[0], 'modules', base_name + asteroid_file_suffix))
 
             file_found = False
 
             for ix in range(len(search_list)):
                 ast_module_file = search_list[ix]
                 #lhh
                 #print("AST module: {}".format(ast_module_file))
@@ -232,39 +226,31 @@
                                  .format(str_tok.value))
 
             #lhh
             #print("opening module {}".format(ast_module_file))
 
             old_lineinfo = state.lineinfo
             with open(ast_module_file) as f:
-                #state.modules.append(module_name)
-                state.modules.append(ast_module_file)
                 data = f.read()
-
                 # Give the absolute path to the parser
                 fparser = Parser(str(ast_module_path))
-                (STMT_LIST, fstmts) = fparser.parse(data)
+                fstmts = fparser.parse(data)
             
             state.lineinfo = old_lineinfo
-            return ('import_stmt', fstmts)
+            return ('load-stmt', 
+                    ('module-def',
+                     ('id', module_name), fstmts))
 
         elif tt == 'GLOBAL':
             dbg_print("parsing GLOBAL")
             self.lexer.match('GLOBAL')
             id_list = self.id_list()
             self.lexer.match_optional('DOT')
             return ('global', id_list)
 
-        elif tt == 'ASSERT':
-            dbg_print("parsing ASSERT")
-            self.lexer.match('ASSERT')
-            exp = self.exp()
-            self.lexer.match_optional('DOT')
-            return ('assert', exp)
-
         elif tt == 'FUNCTION':
             return self.function_def()
 
         elif tt == 'STRUCTURE':
             dbg_print("parsing STRUCTURE")
             self.lexer.match('STRUCTURE')
             id_tok = self.lexer.match('ID')
@@ -344,14 +330,40 @@
         elif tt == 'BREAK':
             if self.functional_mode and not self.is_system_module():
                 raise SyntaxError("break statement is not supported in functional mode")
             dbg_print("parsing BREAK")
             self.lexer.match('BREAK')
             return ('break',)
 
+        elif tt == 'MATCH':
+            if self.functional_mode and not self.is_system_module():
+                raise SyntaxError("match statement is not supported in functional mode")
+            # we implement the match statement as a cascade of if-clauses
+            if_list = []
+            dbg_print("parsing MATCH")
+            self.lexer.match('MATCH')
+            temp = ('id', gettemp())
+            exp = self.exp()
+            while self.lexer.peek().type == 'WITH':
+                dbg_print("parsing WITH")
+                old_lineinfo = state.lineinfo
+                self.lexer.match('WITH')
+                pattern = self.pattern()
+                self.lexer.match('DO')
+                stmts = self.stmt_list()
+                if_list.append(('lineinfo',old_lineinfo))
+                if_list.append(
+                    ('if-clause', 
+                      ('cond', ('is', temp, pattern)), 
+                      ('stmt-list', stmts)))
+            self.lexer.match('END')
+            return ('match',
+                     ('unify', temp, exp), 
+                     ('if', ('list', if_list)))
+
         elif tt == 'IF':
             if self.functional_mode and not self.is_system_module():
                 raise SyntaxError("if statement is not supported in functional mode")
 
             # if statements are coded as a list of ('if-clause', condition, stmts)
             if_list = []
 
@@ -408,23 +420,23 @@
             self.lexer.match('TRY')
             try_stmts = self.stmt_list()
             self.lexer.match('CATCH')
             dbg_print("parsing CATCH")
             pattern = self.pattern()
             self.lexer.match('DO')
             stmts = self.stmt_list()
-            catch_list.append(('catch', ('pattern', pattern), ('stmt-list', stmts)))
+            catch_list.append(('catch', ('catch-pattern', pattern), ('stmt-list', stmts)))
 
             while self.lexer.peek().type == 'CATCH':
                 dbg_print("parsing CATCH")
                 self.lexer.match('CATCH')
                 pattern = self.pattern()
                 self.lexer.match('DO')
                 stmts = self.stmt_list()
-                catch_list.append(('catch',('pattern', pattern), ('stmt-list', stmts)))
+                catch_list.append(('catch',('catch-pattern', pattern), ('stmt-list', stmts)))
 
             self.lexer.match('END')
             #self.lexer.match_optional('TRY')
 
             return ('try',
                     ('stmt-list', try_stmts),
                     ('catch-list', ('list', catch_list)))
@@ -435,15 +447,15 @@
             e = self.exp()
             self.lexer.match_optional('DOT')
             return ('throw', e)
 
         elif tt in exp_lookahead:
             v = self.exp()
             self.lexer.match_optional('DOT')
-            return ('top-level-exp', v)
+            return ('exp-stmt', ('set-ret-val', v))
 
         else:
             raise SyntaxError("syntax error at '{}'"
                         .format(self.lexer.peek().value))
 
     ###########################################################################################
     # function_def
@@ -453,15 +465,16 @@
         self.lexer.match('FUNCTION')
         id_tok = self.lexer.match('ID')
         body_list = self.body_defs()
         self.lexer.match('END')
         #self.lexer.match('FUNCTION')
 
         # check if any useless patterns exist within the function
-        #lhh check_redundancy( body_list, id_tok )
+        #from asteroid.walk import check_redundancy
+        #check_redundancy( body_list, id_tok )
 
         # functions are function expressions bound to names
         return ('unify',
                 ('id',id_tok.value),
                 ('function-exp', body_list))
 
     ###########################################################################################
@@ -527,40 +540,39 @@
             self.lexer.match('COMMA')
             id_tok = self.lexer.match('ID')
             id_list.append(('id', id_tok.value))
         return ('list', id_list)
 
     ###########################################################################################
     # body_defs
-    #   : WITH pattern DO stmt_list (ORWITH pattern DO stmt_list)*
+    #   : WITH pattern DO stmt_list (WITH pattern DO stmt_list)*
     def body_defs(self):
         dbg_print("parsing BODY_DEFS")
 
         # a list of ('body', pattern, stmts) pairs
         body_list = []
 
         cur_lineinfo = state.lineinfo
         self.lexer.match('WITH')
         p = self.pattern()
         self.lexer.match('DO')
         sl = self.stmt_list()
         body_list.append( ('lineinfo', cur_lineinfo) )
-        body_list.append(('body', ('pattern', p), ('stmt-list', sl)))
+        body_list.append(('body', ('body-pattern', p), ('stmt-list', sl)))
 
         while self.lexer.peek().type in ['ORWITH','WITH']:
             cur_lineinfo = state.lineinfo
-
             if self.lexer.peek().type == 'ORWITH':
                 warning("'orwith' has been deprecated, please replace with 'with'")
             self.lexer.match(self.lexer.peek().type)
             p = self.pattern()
             self.lexer.match('DO')
             sl = self.stmt_list()
             body_list.append( ('lineinfo', cur_lineinfo) )
-            body_list.append(('body', ('pattern', p), ('stmt-list', sl)))
+            body_list.append(('body', ('body-pattern', p), ('stmt-list', sl)))
 
         return ('body-list', ('list', body_list))
 
     ###########################################################################################
     # exp
     #    : pattern
     def exp(self):
@@ -577,23 +589,23 @@
         dbg_print("parsing PATTERN")
 
         if self.lexer.peek().type == 'PATTERN':
             self.lexer.match('PATTERN')
             self.lexer.match_optional('WITH')
             v = self.exp()
             return ('pattern', v)
-        elif self.lexer.peek().type == 'LCONSTRAINT': #constraint-only pattern match
-            self.lexer.match('LCONSTRAINT')
+        elif self.lexer.peek().type == 'LSCOPE': # scoped pattern
+            self.lexer.match('LSCOPE')
             v = self.exp()
-            self.lexer.match('RCONSTRAINT')
+            self.lexer.match('RSCOPE')
             if self.lexer.peek().type == 'BIND':
                 bl = self.binding_list()            
-                return ('constraint', v, bl)
+                return ('scope', v, bl)
             else:
-                return ('constraint', v, ('nil',))
+                return ('scope', v, ('nil',))
         else:
             v = self.head_tail()
             return v
 
     ###########################################################################################
     # head_tail
     #    : conditional ('|' exp)?
@@ -687,15 +699,15 @@
                         ('step', ('integer', '1')))
 
         else:
             return v
 
     ###########################################################################################
     # NOTE: Builtin operators are mapped to 'apply' so that they don't have to be
-    #       special cased during pattern matching.  See operator_symbols above.
+    #       special cased during pattern matching.  See builtin in globals.
     ###########################################################################################
     # logic/relational/arithmetic operators with their precedence
     # logic_exp0
     #   : logic_exp1 (OR logic_exp1)*
     #
     # logic_exp1
     #   : rel_exp1 (AND rel_exp1)*
@@ -788,18 +800,28 @@
                 v2 = self.primary()
                 v = ('apply', v, v2)
             elif self.lexer.peek().type == 'AT':
                 self.lexer.match('AT')
                 ix = self.primary()
                 v = ('index', v, ix)
 
-        if self.lexer.peek().type == 'COLON': # if ':' exists - named pattern
+        # if ':' exists - constraint pattern
+        # 'p1:p2' is equivalent to 't if (t is p1) and (t is p2)'
+        # therefore we map the constraint pattern into
+        # a conditional pattern with a generated temp variable
+        if self.lexer.peek().type == 'COLON': 
             self.lexer.match('COLON')
             e = self.exp()
-            v = ('named-pattern', v, e)
+            t = gettemp()
+            v = ('if-exp',
+                    ('apply',
+                        ('id', '__and__'),
+                        ('tuple', [('is', ('id', t), v), ('is', ('id', t), e)])),
+                    ('id', t),
+                    ('null',))
 
         return v
 
     ###########################################################################################
     # primary
     #    : INTEGER
     #    | REAL
@@ -808,16 +830,14 @@
     #    | FALSE
     #    | NONE
     #    | ID
     #    | '*' call_or_index binding_list? /* pattern dereferencing */
     #    | NOT call_or_index
     #    | MINUS call_or_index
     #    | PLUS call_or_index
-    #    | ESCAPE STRING
-    #    | EVAL exp
     #    | '(' tuple_stuff ')' /* tuple/parenthesized expr */
     #    | '[' list_stuff ']'  /* list or list access */
     #    | function_const
     #    | TYPEMATCH // TYPEMATCH == '%'<typename>
     def primary(self):
         dbg_print("parsing PRIMARY")
 
@@ -879,24 +899,14 @@
             v = self.call_or_index()
             # if v is a real or integer constant we apply __uplus__
             if v[0] in ['integer', 'real']:
                 return (v[0], + v[1])
             else:
                 return ('apply', ('id', '__uplus__'), v)
 
-        elif tt == 'ESCAPE':
-            self.lexer.match('ESCAPE')
-            str_tok = self.lexer.match('STRING')
-            return ('escape', str_tok.value)
-
-        elif tt == 'EVAL':
-            self.lexer.match('EVAL')
-            exp = self.primary()
-            return ('eval', exp)
-
         elif tt == 'LPAREN':
             # Parenthesized expressions have the following meaning:
             #       (A)    means a parenthesized value A
             #       (A,)   means a tuple with a single value A
             #       (A, B) means a tuple with values A and B
             #       ()     shorthand for 'none'
             self.lexer.match('LPAREN')
@@ -1024,12 +1034,7 @@
     #    : LAMBDA body_defs
     def function_const(self):
         dbg_print("parsing FUNCTION_CONST")
         self.lexer.match('LAMBDA')
         body_list = self.body_defs()
 
         return ('function-exp', body_list)
-
-    ###########################################################################################
-    # Minor helper function
-    def stmt_coming_up(self):
-        return self.lexer.peek().type in stmt_lookahead
```

### Comparing `asteroid-lang-1.1.4/asteroid/globals.py` & `asteroid-lang-2.0.1/asteroid/globals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 ###########################################################################################
 # globals for Asteroid
 #
-# (c) Lutz Hamel, University of Rhode Island
+# (c) University of Rhode Island
 ###########################################################################################
 
 from asteroid.support import term2string #Used by redundantPatternFound exception
 
 ###########################################################################################
 # this is used to compute the filename extensions of the modules
 asteroid_file_suffix = ".ast"
 
 ###########################################################################################
-# symbols for builtin operators.
+# symbols for builtin operators and functions. these operators and functions do not 
+# need/are not allowed to have a function local scope.  therefore they are implemented
+# here as builtins as part of the interpreter proper.  for other builtins that do 
+# not have this restriction see the prologue.
 # NOTE: if you add new builtins make sure to keep this table in sync.
 
 binary_operators = {
     '__plus__',
     '__minus__',
     '__times__',
     '__divide__',
@@ -23,23 +26,30 @@
     '__and__',
     '__eq__',
     '__ne__',
     '__le__',
     '__lt__',
     '__ge__',
     '__gt__',
-    }
+}
 
 unary_operators = {
     '__uminus__',
     '__uplus__',
     '__not__',
+    'assert',
+    'escape',
+    'eval',
     }
 
-operator_symbols = binary_operators | unary_operators
+nullary_operators = {
+    'toplevel',
+}
+
+builtins = binary_operators | unary_operators | nullary_operators
 
 #########################################################################
 # Use the exception mechanism to return values from function calls
 
 class ReturnValue(Exception):
 
     def __init__(self, value):
@@ -117,19 +127,17 @@
                                             # 1 line(minus 1)
         self.pattern2 = pattern2
         if (location2 != None):
             self.line2 = str(location2[1] - 1)
         if (location1 != None):
             self.file = location1[0]
         self.function = function_name
-        self.message = "Redundant Pattern Detected\n"
-        self.message += "\tFunction: " + self.function + " from file " + self.file
-        self.message += "\n\tPattern: " + term2string(self.pattern1) + " on line " + self.line1
-        self.message += "\n\twill consume all matches for"
-        self.message += "\n\tPattern: " + term2string(self.pattern2) + " on line " + self.line2
+        self.message = "redundant pattern detected in '{}': ".format(self.function)
+        self.message += "the pattern on line {} will consume all matches for pattern on line {}"\
+                            .format(self.line1,self.line2)
         super().__init__(self.message)
 
     def __str__(self):
         return(self.message)
 
 ###########################################################################################
 # expression nodes not allowed in terms or patterns for unification. these are all nodes
@@ -137,15 +145,14 @@
 
 unify_not_allowed = {
     'function-val',
     'to-list',
     'where-list',
     'raw-to-list',
     'raw-where-list',
-    'if-exp',
     'foreign',
     'escape',
     'is',
     'in',
 }
 
 ###########################################################################################
@@ -165,8 +172,9 @@
     'struct',
     'typematch',
 }
 
 ###########################################################################################
 # list of structures that a pattern type-pattern will subsume/overlap
 
-pattern_subsumes = patterns - {'id'}
+pattern_subsumes = patterns - {'id'}
+
```

### Comparing `asteroid-lang-1.1.4/asteroid/interp.py` & `asteroid-lang-2.0.1/asteroid/interp.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,57 +7,55 @@
 import os
 import sys
 
 from asteroid.globals import *
 from asteroid.support import *
 from asteroid.frontend import Parser
 from asteroid.state import state, dump_trace
-from asteroid.walk import walk_program, debug_walk
+from asteroid.walk import walk
 
 # the prologue file is expected to be in the 'modules' folder
 prologue_name = 'prologue.ast'
 def load_prologue():
     """
     Load the prolog files and run them.
     """
     prologue_file = ''
     prologue_file_base = os.path.join('modules', prologue_name)
     module_path = os.path.join(os.path.split(os.path.abspath(__file__))[0], prologue_file_base)
     working_path = os.path.join(os.getcwd(), prologue_file_base)
 
     if os.path.isfile(module_path):
         prologue_file = module_path
-    
     elif os.path.isfile(working_path):
         prologue_file = working_path
-    
     else:
         raise ValueError("Asteroid prologue '{}' not found"
                         .format(prologue_file_base))
     
     with open(prologue_file) as f:
-        state.modules.append(prologue_name)
         data = f.read()
         pparser = Parser(prologue_file)
-        (LIST, pstmts) = pparser.parse(data)
+        pstmts = pparser.parse(data)
 
-    state.AST = ('list', pstmts)
-    walk_program(state.AST)
+    state.AST = pstmts
+    walk(state.AST)
     state.AST = None
 
 def interp(program,
            program_name = "<input>",
            tree_dump=False,
            do_walk=True,
            symtab_dump=False,
            exceptions=False,
            redundancy=True,
            prologue=True,
            debugger=None,
            functional_mode=False,
+           warnings=True,
            initialize_state = True
            ):
     '''
     The function 'interp' is the top-level entry point to the
     Asteroid interpreter with the following arguments:
       * program: a string representing an Asteroid program
       * program_name: the of the program to be interpreted
@@ -67,40 +65,50 @@
                      table should be printed out
       * exceptions: when true Python style exceptions are shown, otherwise
                     Asteroid style exceptions are shown
       * redundancy: a flag indicating whether the function pattern checker should be run
       * prologue: a flag indicating whether the Asteroid prologue file should be loaded
       * functional_mode: if set then the Asteroid interpreter behaves like an interpreter
                          functional programming language.
+      * warnings: if set will display warnings
       * initialize_state: if set then the interpreter will (re)initialize its state.  
     '''
     try:
         # initialize state
         if initialize_state:
             state.initialize(program_name)
 
         if prologue:
             load_prologue()
 
-        # initialize "check for useless clauses" flag
+        # initialize state flags
         state.eval_redundancy = redundancy
+        state.warning = warnings
 
         # build the AST
         parser = Parser(program_name, functional_mode)
-        (LIST, istmts) = parser.parse(program)
-        state.AST = ('list', istmts)
+        stmts = parser.parse(program)
+        state.AST = stmts
+        state.mainmodule = state.lineinfo[0]
 
         # walk the AST
         if tree_dump:
             dump_AST(state.AST)
+        if debugger:
+            state.debugger = debugger
+            (module,line) = state.lineinfo
+            state.lineinfo = (module,1)
+            debugger.start(state)
         if do_walk:
-            if debugger:
-                debug_walk(state.AST, debugger)
-            else:
-                walk_program(state.AST)
+            try:
+                walk(state.AST)
+                if debugger: debugger.stop()
+            except Exception as e:
+                if debugger: debugger.error(e)
+                raise e
         if symtab_dump:
             state.symbol_table.dump()
 
     # Note: all exceptions generated by Asteroid should go through the handler
     #       for 'Exception' unless the exception needs special handling like
     #       'ThrowValue' or 'ReturnValue' etc.
     except ThrowValue as throw_val:
@@ -123,25 +131,25 @@
         print("error: {}: {}: return statement used outside a function environment"
               .format(module, lineno))
         # needed for REPL
         if not exceptions:
             sys.exit(1)
 
     except  KeyboardInterrupt as e:
-        if debugger:
-            raise e
-
         dump_trace()
         print("error: keyboard interrupt")
         # needed for REPL
         if not exceptions:
             sys.exit(1)
 
-    except SystemExit:
-        exit(0)
+    except SystemExit as e:
+        # we simply pass along the exception
+        # this is just here in case in the future we need to 
+        # perform special handling
+        raise e
 
     except Exception as e:
         if exceptions: # rethrow the exception so that you can see the full backtrace
             if symtab_dump:
                 state.symbol_table.dump()
             raise e
         else:
```

### Comparing `asteroid-lang-1.1.4/asteroid/lex.py` & `asteroid-lang-2.0.1/asteroid/lex.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,43 +10,40 @@
 from asteroid.globals import ExpectationError
 
 # table that specifies the token value and type for keywords
 keywords = {
 #   value:          type:
     'and'           : 'AND',
     'as'            : 'AS',
-    'assert'        : 'ASSERT',
     'bind'          : 'BIND',
     'break'         : 'BREAK',
     'catch'         : 'CATCH',
     'data'          : 'DATA',
     'do'            : 'DO',
     'elif'          : 'ELIF',
     'else'          : 'ELSE',
     'end'           : 'END',
-    'escape'        : 'ESCAPE',
-    'eval'          : 'EVAL',
     'for'           : 'FOR',
     'from'          : 'FROM',
     'function'      : 'FUNCTION',
     'global'        : 'GLOBAL',
     'if'            : 'IF',
     'in'            : 'IN',
     'is'            : 'IS',
     'lambda'        : 'LAMBDA',
     'let'           : 'LET',
     'load'          : 'LOAD',
     'loop'          : 'LOOP',
+    'match'         : 'MATCH',
     'not'           : 'NOT',
     'or'            : 'OR',
-    'orwith'        : 'ORWITH',
     'pattern'       : 'PATTERN',
     'repeat'        : 'REPEAT',
     'return'        : 'RETURN',
-    'step'        : 'STEP',
+    'step'          : 'STEP',
     'structure'     : 'STRUCTURE',
     'system'        : 'SYSTEM',
     'throw'         : 'THROW',
     'to'            : 'TO',
     'try'           : 'TRY',
     'until'         : 'UNTIL',
     'while'         : 'WHILE',
@@ -80,16 +77,16 @@
     (r'==',                                       "'=='",       'EQ'),
     (r'=/=',                                      "'=/='",      'NE'),
     (r'<=',                                       "'<='",       'LE'),
     (r'<',                                        "'<'",        'LT'),
     (r'>=',                                       "'>='",       'GE'),
     (r'>',                                        "'>'",        'GT'),
     (r'@',                                        "'@'",        'AT'),
-    (r'\%\[',                                     "'%['",       'LCONSTRAINT'),
-    (r'\]\%',                                     "']%'",       'RCONSTRAINT'),
+    (r'\%\[',                                     "'%['",       'LSCOPE'),
+    (r'\]\%',                                     "']%'",       'RSCOPE'),
     (r'\(',                                       "'('",        'LPAREN'),
     (r'\)',                                       "')'",        'RPAREN'),
     (r'\[',                                       "'['",        'LBRACKET'),
     (r'\]',                                       "']'",        'RBRACKET'),
     (r':',                                        "':'",        'COLON'),
     (r'\|',                                       "'|'",        'BAR'),
     (r'\.',                                       "'.'",        'DOT'),
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/bitwise.ast` & `asteroid-lang-2.0.1/asteroid/modules/bitwise.ast`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,14 @@
 -- bitwise.ast
 --
 -- Defines bitwise operations
 --
 -- (c) University of Rhode Island
 ------------------------------------------------------------------
 
--- define the bitwise module object
-
-------------------------------------------------------------------
-structure __BITWISE_MODULE__
-------------------------------------------------------------------
-with
-
 ------------------------------------------------------------------
 function band
 ------------------------------------------------------------------
  -- Bitwise AND
 with(x:%integer, y:%integer) do return escape
 "
 global __retval__
@@ -176,12 +169,7 @@
 global __retval__
 x_val = state.symbol_table.lookup_sym('x')[1]
 
 __retval__ = ('integer', x_val.bit_length())
 "
 end
 
-end -- __BITWISE__
-
-------------------------------------------------------------------
--- instantiate the bitwise module object
-let bitwise = __BITWISE_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/dataframe.ast` & `asteroid-lang-2.0.1/asteroid/modules/dataframe.ast`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 --
 -- TODO: this is more of a proof of concept implementation
 -- demonstrating that we can have objects with escaped
 -- implementations.  DataFrames needs lots more functionality.
 ------------------------------------------------------------------
 
 ------------------------------------------------------------------
-structure __DATAFRAME__
+structure DataFrame with
 ------------------------------------------------------------------
-with
 
 ------------------------------------------------------------------
 data df.
 ------------------------------------------------------------------
 
 ------------------------------------------------------------------
 function read_csv
@@ -26,14 +25,15 @@
 this_val = state.symbol_table.lookup_sym('this')
 file_val = state.symbol_table.lookup_sym('file')
 header_row_val = state.symbol_table.lookup_sym('header_row')
 
 # destructure object
 (OBJECT,
  (CLASS_ID, (ID, class_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 # read as Pandas dataframe
 df = pandas.read_csv(file_val[1], header=0 if header_row_val[1] else None)
 
 # the dataframe is in the first slot in the object memory
 # store the Pandas dataframe as a foreign object in this slot
@@ -52,14 +52,15 @@
 
 this_val = state.symbol_table.lookup_sym('this')
 ix_val = state.symbol_table.lookup_sym('ix')
 
 # destructure object
 (OBJECT,
  (CLASS_ID, (ID, class_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
  # the dataframe is in the first slot in the object memory
 (FOREIGN, df_val) = memory[0]
 
 row = df_val.iloc[ix_val[1],:]
 lst = []
@@ -91,14 +92,15 @@
 import numpy
 this_val = state.symbol_table.lookup_sym('this')
 ix_val = state.symbol_table.lookup_sym('ix')
 
 # destructure object
 (OBJECT,
  (CLASS_ID, (ID, class_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
  # the dataframe is in the first slot in the object memory
 (FOREIGN, df_val) = memory[0]
 
 col = df_val.iloc[:,ix_val[1]]
 lst = []
@@ -128,14 +130,15 @@
 global __retval__
 from asteroid.state import state
 this_val = state.symbol_table.lookup_sym('this')
 
 # destructure object
 (OBJECT,
  (CLASS_ID, (ID, class_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
  # the dataframe is in the first slot in the object memory
 (FOREIGN, df_val) = memory[0]
 __retval__ = ('integer', df_val.shape[0])
 "
 end
@@ -148,29 +151,23 @@
 global __retval__
 from asteroid.state import state
 this_val = state.symbol_table.lookup_sym('this')
 
 # destructure object
 (OBJECT,
  (CLASS_ID, (ID, class_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
  # the dataframe is in the first slot in the object memory
 (FOREIGN, df_val) = memory[0]
 __retval__ = ('integer', df_val.shape[1])
 "
 end
-end -- __DATAFRAME__
+end -- DataFrame structure
 
-------------------------------------------------------------------
-structure __DATAFRAME_MODULE__
-------------------------------------------------------------------
-with
 
 function dataframe with none do
-  return __DATAFRAME__().
+  return DataFrame().
 end
 
-end -- __DATAFRAME_MODULE__
 
-------------------------------------------------------------------
-let dataframe = __DATAFRAME_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/hash.ast` & `asteroid-lang-2.0.1/asteroid/modules/hash.ast`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ------------------------------------------------------------------
 -- hash.ast
 --
 -- this module implements the HashTable structure
 --
 -- (c) Lutz Hamel, University of Rhode Island
 ------------------------------------------------------------------
-load system type.
+
 
 ------------------------------------------------------------------
-structure __HASH__ with
+structure Hash with
 ------------------------------------------------------------------
 -- Asteroid hash table implementation using Python dictionaries
 
 ------------------------------------------------------------------
 data table.
 
 ------------------------------------------------------------------
@@ -22,45 +22,52 @@
 with none do escape
 "
 this_val = state.symbol_table.lookup_sym('this')
 
 # destructure object
 (OBJECT,
  (STRUCT_ID, (ID, struct_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 # the table is in the first slot in the object memory
 # store the dictionary as a foreign object in this slot
 memory[0] = ('foreign', dict())
 "
 end -- __init__
 
 ------------------------------------------------------------------
 function insert
 ------------------------------------------------------------------
-with (name,value) do escape
+with (name,value) do 
+return escape
 "
+global __retval__
 this_val = state.symbol_table.lookup_sym('this')
 name_val = state.symbol_table.lookup_sym('name')
 value_val = state.symbol_table.lookup_sym('value')
 
 # destructure object
 (OBJECT,
  (STRUCT_ID, (ID, struct_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 # the table is in the first slot in the object memory
 # insert name-value pair
 (FOREIGN, dictionary) = memory[0]
 dictionary[name_val] = value_val
+
+__retval__ = this_val
 "
 with item_list:%list do
   for (k,v) in item_list do
     this @insert (k,v).
   end
+  return this
 end -- insert
 
 ------------------------------------------------------------------
 function get
 ------------------------------------------------------------------
 with name do return escape
 "
@@ -68,14 +75,15 @@
 
 this_val = state.symbol_table.lookup_sym('this')
 name_val = state.symbol_table.lookup_sym('name')
 
 # destructure object
 (OBJECT,
  (STRUCT_ID, (ID, struct_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 # the table is in the first slot in the object memory
 # get the value_val associated with name_val
 (FOREIGN, dictionary) = memory[0]
 if name_val not in dictionary.keys():
     __retval__ = ('none', None)
@@ -92,14 +100,15 @@
 global __retval__
 
 this_val = state.symbol_table.lookup_sym('this')
 
 # destructure object
 (OBJECT,
  (STRUCT_ID, (ID, struct_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 # the table is in the first slot in the object memory
 # get the value_val associated with name_val
 (FOREIGN, dictionary) = memory[0]
 
 # zip the keys and the values
@@ -117,25 +126,18 @@
 "
 end -- aslist
 
 ------------------------------------------------------------------
 function __str__
 ------------------------------------------------------------------
 with none do
-  return type @tostring (this @aslist ()).
+  return tostring (this @aslist ()).
 end -- __str__
 
-end -- __HASH__
-
-------------------------------------------------------------------
-structure __HASH_MODULE__
-------------------------------------------------------------------
-with
+end -- Hash structure
 
+-- here for backwards compatibility
 function hash with none do
-   return __HASH__().
+   return Hash().
 end
 
-end -- __HASH_MODULE__
 
-------------------------------------------------------------------
-let hash = __HASH_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/io.ast` & `asteroid-lang-2.0.1/asteroid/modules/io.ast`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ------------------------------------------------------------------
 -- io.ast
 --
 -- this module implements the I/O system for Asteroid
 --
 -- (c) University of Rhode Island
 
-
-load system type.
+-- define the io module.
 
 ------------------------------------------------------------------
--- Basic file i/o
+
 ------------------------------------------------------------------
 structure __FILE__ with
 ------------------------------------------------------------------
+-- Basic file i/o
 
 data fd.
 
 ------------------------------------------------------------------
 function __init__
 ------------------------------------------------------------------
 with (name:%string, mode:%string) do escape
@@ -28,14 +28,15 @@
 this_val = state.symbol_table.lookup_sym('this')
 name_val = state.symbol_table.lookup_sym('name')
 mode_val = state.symbol_table.lookup_sym('mode')
 
 # destructure object
 (OBJECT,
 (CLASS_ID, (ID, class_id)),
+(MEMBER_NAMES, (LIST, member_names)),
 (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 # Open file
 f = open(name_val[1], mode_val[1])
 memory[0] = ('foreign', f)
 
 __retval__ = this_val
@@ -58,14 +59,15 @@
     stream = sys.stderr
 else:
     raise Exception('Unknown standard stream' + std_val)
 
 # destructure object
 (OBJECT,
 (CLASS_ID, (ID, class_id)),
+(MEMBER_NAMES, (LIST, member_names)),
 (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 memory[0] = ('foreign', stream)
 "
 
 end
 ------------------------------------------------------------------
@@ -76,14 +78,15 @@
 with none do escape
 "
 from asteroid.state import state
 this_val = state.symbol_table.lookup_sym('this')
 
 (OBJECT,
  (CLASS_ID, (ID, class_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 (FOREIGN, f_val) = memory[0]
 f_val.close()
 "
 end
 ------------------------------------------------------------------
@@ -95,14 +98,15 @@
 "
 global __retval__
 from asteroid.state import state
 this_val = state.symbol_table.lookup_sym('this')
 
 (OBJECT,
  (CLASS_ID, (ID, class_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 (FOREIGN, f_val) = memory[0]
 
 __retval__ = ('string', f_val.read())
 "
 end
@@ -114,14 +118,15 @@
 "
 global __retval__
 from asteroid.state import state
 this_val = state.symbol_table.lookup_sym('this')
 
 (OBJECT,
  (CLASS_ID, (ID, class_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 (FOREIGN, f_val) = memory[0]
 
 __retval__ = ('string', f_val.readline())
 "
 end
@@ -133,43 +138,34 @@
 "
 from asteroid.state import state
 this_val = state.symbol_table.lookup_sym('this')
 what_val = state.symbol_table.lookup_sym('what')
 
 (OBJECT,
  (CLASS_ID, (ID, class_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 (FOREIGN, f_val) = memory[0]
 
-f_val.write(what_val[1])
+f_val.write(term2string(what_val))
 "
 end
 
 ------------------------------------------------------------------
 end -- __FILE__
 ------------------------------------------------------------------
 
 
 
--- define the io module object.
-------------------------------------------------------------------
-structure __IO_MODULE__ with
-------------------------------------------------------------------
 
 -- Predefined standard stream constants
-data __STDIN__.
-data __STDOUT__.
-data __STDERR__.
-
-function __init__ with none do
-   let this @__STDIN__ = __FILE__("__STDIN__").
-   let this @__STDOUT__ = __FILE__("__STDOUT__").
-   let this @__STDERR__ = __FILE__("__STDERR__").
-end
+let __STDIN__ = __FILE__("__STDIN__").
+let __STDOUT__ = __FILE__("__STDOUT__").
+let __STDERR__ = __FILE__("__STDERR__").
 
 -- File I/O library functions
 ------------------------------------------------------------------
 function open
 -- Open a file given a filename and mode
 ------------------------------------------------------------------
 with (name:%string, mode:%string) do
@@ -186,17 +182,16 @@
 
 ------------------------------------------------------------------
 function read
 -- Return the contents of a given file
 ------------------------------------------------------------------
 with(file:%__FILE__) do
     return file @read().
-
 with none do
-    return this @__STDIN__ @ read().
+    return __STDIN__ @ read().
 end
 
 ------------------------------------------------------------------
 function readln
 -- Return the next line of a given file
 -- Note: readln reads a single line from the stream; a newline
 -- character (\n) is left at the end of the string, and is only
@@ -205,70 +200,65 @@
 -- if readln returns an empty string, the end of the file has
 -- been reached, while a blank line is represented by '\n',
 -- a string containing only a single newline.
 ------------------------------------------------------------------
 with(file:%__FILE__) do
     return file @readln().
 with none do
-    return this @__STDIN__ @readln().
+    return __STDIN__ @readln().
 end
 
 ------------------------------------------------------------------
 function write
 -- Write to a given file
 ------------------------------------------------------------------
 with what:%string do
-this @__STDOUT__ @write(what).
-
-escape "
-import sys
-sys.stdout.flush()
-"
-
+    __STDOUT__ @write(what).
+    escape "import sys;sys.stdout.flush()".
 with(file:%__FILE__, what:%string) do
     file @write(what).
 end
 
 ------------------------------------------------------------------
 function writeln
 -- Write a complete line to a given file
 ------------------------------------------------------------------
 with what:%string do
-    this @__STDOUT__ @write(what + "\n").
+    __STDOUT__ @write(what + "\n").
 
 with(file:%__FILE__, what:%string) do
     file @write(what + "\n").
 end
 ------------------------------------------------------------------
 
 -- Basic console I/O functions
 
 ------------------------------------------------------------------
 function println
 ------------------------------------------------------------------
 with item do
-    this @writeln(type @tostring item).
+    writeln(tostring item).
 end
 
 ------------------------------------------------------------------
 function print
 ------------------------------------------------------------------
 with item do
-    this @write(type @tostring item).
+    write(tostring item).
 end
 
 ------------------------------------------------------------------
 function input
 ------------------------------------------------------------------
 -- input drops the trailing newline char
 with none do
-    return this @readln() @replace("\n","").
+    return readln() @replace("\n","").
 with prompt do
-    this @write (type @tostring prompt).
-    return this @readln() @replace("\n","").
+    write (tostring prompt).
+    return readln() @replace("\n","").
 end
 
 ------------------------------------------------------------------
 function __raw_print__
 ------------------------------------------------------------------
 -- dumps the AST to screen
 with item do escape
@@ -276,13 +266,7 @@
 from pprint import pprint
 item_val = state.symbol_table.lookup_sym('item')
 pprint(item_val)
 "
 return none
 end
 
-end -- __IO_MODULE__
-
-
-------------------------------------------------------------------
--- instantiate the io module object
-let io = __IO_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/os.ast` & `asteroid-lang-2.0.1/asteroid/modules/os.ast`

 * *Files 2% similar despite different names*

```diff
@@ -5,52 +5,15 @@
 --
 -- (c) University of Rhode Island
 ------------------------------------------------------------------
 -- modeled after the Python os, os.path, and sys modules
 ------------------------------------------------------------------
 load system hash.
 
-structure __OS_MODULE__ with
-
-------------------------------------------------------------------
--- The list of command line arguments passed to an Asteroid script. 
--- argv[0] is the name of the Asteroid script (it is operating 
--- system dependent whether this is a full pathname or not).
--- In interactive mode argv[0] will be the empty string.
-data argv.
-
-------------------------------------------------------------------
--- A hash table where keys and values are strings that represent 
--- the process environment. For example, 
---    os @env @get "HOME"
---  is the pathname of your home directory (on some platforms), 
--- and is equivalent to getenv("HOME") in C.
-data env.
-
-------------------------------------------------------------------
--- This string contains a platform identifier.
-data platform.
-
-------------------------------------------------------------------
-function __init__ 
-------------------------------------------------------------------
--- constructor for the __OS_MODULE__
-with none do
-   let this @argv = this @__getargv().
-   let this @platform = this @__getplatform().
-   -- construct the env hashtable
-   let l = this @__getenv(). -- list of key/value pairs
-   let this @env = hash @hash ().
-   this @env @insert l.
-end
-
-------------------------------------------------------------------
-function __getargv 
-------------------------------------------------------------------
-with none do return escape
+function __getargv  with none do return escape
 "
 global __retval__
 import sys
 import copy
 import os
 import os.path
 argv = copy.copy(sys.argv)
@@ -71,41 +34,54 @@
 out = []
 for e in argv:
    out.append(('string',e))
 __retval__ = ('list', out)
 "
 end -- __getargv
 
-------------------------------------------------------------------
-function __getenv
-------------------------------------------------------------------
-with none do return escape
+function __getenv with none do return escape
 "
 global __retval__
 from os import environ
 # turn dictionary into an Asteroid list
 outlist_val = []
 for (k,v) in environ.items():
    outlist_val.append(('tuple',[('string',k),('string',v)]))
 __retval__ = ('list', outlist_val)
 "
 end -- __getplatform
 
-------------------------------------------------------------------
-function __getplatform
-------------------------------------------------------------------
-with none do return escape
+function __getplatform with none do return escape
 "
 global __retval__
 from sys import platform
 __retval__ = ('string', platform)
 "
 end -- __getplatform
 
 ------------------------------------------------------------------
+-- The list of command line arguments passed to an Asteroid script. 
+-- argv[0] is the name of the Asteroid script (it is operating 
+-- system dependent whether this is a full pathname or not).
+-- In interactive mode argv[0] will be the empty string.
+let argv = __getargv().
+
+------------------------------------------------------------------
+-- A hash table where keys and values are strings that represent 
+-- the process environment. For example, 
+--    os @env @get "HOME"
+--  is the pathname of your home directory (on some platforms), 
+-- and is equivalent to getenv("HOME") in C.
+let env = hash @hash () @insert (__getenv ()).
+
+------------------------------------------------------------------
+-- This string contains a platform identifier.
+let platform = __getplatform().
+
+------------------------------------------------------------------
 function basename
 ------------------------------------------------------------------
 -- Return the base name of pathname path. This is the second element of the pair
 -- returned by passing path to the function split(). Note that the result of this
 -- function is different from the Unix basename program; where basename for '/foo/bar/'
 -- returns 'bar', the basename() function returns an empty string ('').
 with path:%string do return escape
@@ -161,17 +137,17 @@
 
 ------------------------------------------------------------------
 function exit
 ------------------------------------------------------------------
 -- Signaling an intention to exit the interpreter.
 -- When an argument value other than none is provided
 -- it is considered a status value. If it is 
--- an integer, zero is considered “successful termination” and any 
--- nonzero value is considered “abnormal termination” by shells and 
--- the like. Most systems require it to be in the range 0–127, and 
+-- an integer, zero is considered "successful termination" and any 
+-- nonzero value is considered "abnormal termination" by shells and 
+-- the like. Most systems require it to be in the range 0 to 127, and 
 -- produce undefined results otherwise. Some systems have a 
 -- convention for assigning specific meanings to specific exit codes, 
 -- but these are generally underdeveloped; Unix programs generally 
 -- use 2 for command line syntax errors and 1 for all other kind 
 -- of errors. If none is given as an argument value then is it
 -- is considered to be a successful exit equivalent to passing a zero. 
 -- If a string is passed then it is printed printed to 
@@ -394,11 +370,7 @@
 from os import system
 (STRING, cmd_val) = state.symbol_table.lookup_sym('cmd')
 status = sytem(cmd_val)
 __retval__ = ('integer', status)
 "
 end -- syscmd
 
-end -- __OS_MODULE__
-
-------------------------------------------------------------------
-let os = __OS_MODULE__().
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/pick.ast` & `asteroid-lang-2.0.1/asteroid/modules/pick.ast`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 --
 -- (c) Lutz Hamel, University of Rhode Island
 ------------------------------------------------------------------
 
 load system random.
 
 ------------------------------------------------------------------
-structure __PICK__
+structure Pick
 ------------------------------------------------------------------
 -- A pick object holds a list of items that
 -- we can randomly pick from with the 'pickitems'
 -- member function
 
   with
 
@@ -33,22 +33,16 @@
   end
 
   --make sure that we only pass lists into the constructor
   function __init__ with l:%list do
       let this @items = l.
   end
 
-end -- __PICK__
+end -- Pick
 
 ------------------------------------------------------------------
-structure __PICK_MODULE__
+function pick 
 ------------------------------------------------------------------
-with
-
-function pick with l:%list do
-   return __PICK__(l).
+with l:%list do
+   return Pick(l).
 end
 
-end -- __PICK_MODULE__
-
-------------------------------------------------------------------
-let pick = __PICK_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/prologue.ast` & `asteroid-lang-2.0.1/asteroid/modules/prologue.ast`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 ------------------------------------------------------------------
 -- prologue.ast
 --
 -- the standard Asteroid prologue defining global functions.
 --
 -- (c) University of Rhode Island
 ------------------------------------------------------------------
+-- Note: this is just a file with definitions that need to wind 
+-- up in the global scope of the interpreter.
+
 
 ------------------------------------------------------------------
 structure Error
 ------------------------------------------------------------------
 -- convenient user level exceptions
 with
   data err_val.
@@ -44,14 +47,15 @@
 item_val = state.symbol_table.lookup_sym('item')
 
 if item_val[0] in ['list','tuple','string']:
     __retval__ = ('integer', len(item_val[1]))
 elif item_val[0] == 'object':
     (OBJECT,
         (STRUCT_ID, (ID, name)),
+        (MEMBER_NAMES, (LIST, member_names)),
         (OBJECT_MEMORY, (LIST, object_memory))) = item_val
     l = len(data_only(object_memory))
     __retval__ = ('integer', l)
 elif item_val[0] == 'struct':
     (STRUCT,
         (MEMBER_NAMES, (LIST, member_names)),
         (STRUCT_MEMORY, (LIST, struct_memory))) = item_val
@@ -144,14 +148,242 @@
       with startval:%integer do
          let this @startix = startval.
          let this @endix = none.
       end
 end
 
 ------------------------------------------------------------------
+let __TP__ = pattern
+------------------------------------------------------------------
+-- pattern for selecting proper formatting body in 'tostring'
+with x if (x is %boolean) or
+         (x is %integer) or
+         (x is %string).
+
+------------------------------------------------------------------
+structure __STRINGFORMAT__
+------------------------------------------------------------------
+-- formatting object for 'tostring'
+with
+  data length.
+  data precision.
+  data scientific.
+  function __init__
+    with (l:%integer,p:%integer,s:%boolean) do
+      let this @length = l.
+      let this @precision = p.
+      let this @scientific = s.
+    with (l:%integer,p:%integer) do
+      let this @length = l.
+      let this @precision = p.
+      let this @scientific = none.
+    with l:%integer do
+      let this @length = l.
+      let this @precision = none.
+      let this @scientific = none.
+    end
+end
+
+------------------------------------------------------------------
+-- TYPE CONVERSION FUNCTIONS --
+------------------------------------------------------------------
+
+------------------------------------------------------------------
+function tobase
+------------------------------------------------------------------
+-- represent the given integer x as a numeral in different bases
+with (x:%integer,base:%integer) do return escape
+"
+global __retval__
+
+x_val = state.symbol_table.lookup_sym('x')
+base_val = state.symbol_table.lookup_sym('base')
+
+if base_val[1] == 2:
+  __retval__ = ('string', format(x_val[1],'b'))
+elif base_val[1] == 8:
+  __retval__ = ('string', format(x_val[1],'o'))
+elif base_val[1] == 16:
+  __retval__ = ('string', format(x_val[1],'X'))
+else:
+  raise ValueError('illegal base value {}'
+          .format(base_val[1]))
+"
+end
+
+-- Note: we no longer support this, it encourages lazy programming
+-- by relying on the fuzzy concept of "truthiness"
+------------------------------------------------------------------
+-- function toboolean
+------------------------------------------------------------------
+-- with item do return escape
+-- "
+-- global __retval__
+--
+-- item_val = state.symbol_table.lookup_sym('item')
+-- __retval__ = map2boolean(item_val)
+-- "
+-- end
+
+------------------------------------------------------------------
+function tointeger
+------------------------------------------------------------------
+with (item:%string,base:%integer) do return escape
+"
+global __retval__
+item_val = state.symbol_table.lookup_sym('item')
+base_val = state.symbol_table.lookup_sym('base')
+__retval__ = ('integer', int(item_val[1], base=base_val[1]))
+"
+with item do return escape
+"
+global __retval__
+
+item_val = state.symbol_table.lookup_sym('item')
+__retval__ = ('integer', int(item_val[1]))
+"
+end
+
+------------------------------------------------------------------
+function toreal
+------------------------------------------------------------------
+with item do return escape
+"
+global __retval__
+
+item_val = state.symbol_table.lookup_sym('item')
+__retval__ = ('real', float(item_val[1]))
+"
+end
+
+------------------------------------------------------------------
+function tostring
+------------------------------------------------------------------
+-- convert an asteroid object to string.
+-- if format values are given apply the
+-- formatting to the object.
+
+with (v:*__TP__,__STRINGFORMAT__(w:%integer,none,none)) do
+  -- booleans, integers, and strings (see TP pattern) with width spec are
+  -- right justified. if width spec is too narrow it is ignored.
+  let vs = tostring v.
+  let padl = w - vs @length().
+  if padl > 0 do
+    return [1 to padl] @map(lambda with _ do return " ") @join("") + vs.
+  else do
+    return vs.
+  end
+with (v:%real,__STRINGFORMAT__(w:%integer,none,none)) do return escape
+-- floating point values with only a width spec are left justified with
+-- zero padding on the right.
+"
+global __retval__
+(V_TYPE, v_val) = state.symbol_table.lookup_sym('v')
+(W_TYPE, w_val) = state.symbol_table.lookup_sym('w')
+
+fmtstr = '{:'+str(w_val)+'f}'
+__retval__ = ('string', fmtstr.format(v_val))
+"
+-- floating point values with a width and precision specs
+-- are formatted according to Python formatting rules
+with (v:%real,__STRINGFORMAT__(w:%integer,p:%integer,none)) do return escape
+"
+global __retval__
+(V_TYPE, v_val) = state.symbol_table.lookup_sym('v')
+(W_TYPE, w_val) = state.symbol_table.lookup_sym('w')
+(P_TYPE, p_val) = state.symbol_table.lookup_sym('p')
+
+fmtstr = '{:'+str(w_val)+'.'+str(p_val)+'f}'
+__retval__ = ('string', fmtstr.format(v_val))
+"
+-- floating point values with width, precision and scientific notation specs
+-- are formatted according to Python formatting rules
+with (v:%real,__STRINGFORMAT__(w:%integer,p:%integer,s:%boolean)) do return escape
+"
+global __retval__
+(V_TYPE, v_val) = state.symbol_table.lookup_sym('v')
+(W_TYPE, w_val) = state.symbol_table.lookup_sym('w')
+(P_TYPE, p_val) = state.symbol_table.lookup_sym('p')
+(S_TYPE, s_val) = state.symbol_table.lookup_sym('s')
+
+fmtstr = '{:'+str(w_val)+'.'+str(p_val)+('e}' if s_val else 'f}')
+__retval__ = ('string', fmtstr.format(v_val))
+"
+with item do return escape
+-- default clause
+"
+global __retval__
+from asteroid.support import term2string
+
+item_val = state.symbol_table.lookup_sym('item')
+__retval__ = ('string', term2string(item_val))
+"
+end
+
+------------------------------------------------------------------
+function stringformat
+------------------------------------------------------------------
+-- a wrapper around our __STRINGFORMAT__ object as a member
+-- of our module.
+with (l:%integer,p:%integer,s:%boolean) do
+  return __STRINGFORMAT__(l,p,s).
+with (l:%integer,p:%integer) do
+  return __STRINGFORMAT__(l,p).
+with l:%integer do
+  return __STRINGFORMAT__(l).
+end
+
+------------------------------------------------------------------
+-- TYPE QUERY FUNCTIONS --
+------------------------------------------------------------------
+
+------------------------------------------------------------------
+function islist
+------------------------------------------------------------------
+with item do
+  return item is %list
+end
+
+------------------------------------------------------------------
+function isnone
+------------------------------------------------------------------
+with x do
+  return x is %none.
+end
+
+------------------------------------------------------------------
+function isscalar
+------------------------------------------------------------------
+with item do
+  return (item is %integer) or (item is %real).
+end
+
+------------------------------------------------------------------
+function gettype
+------------------------------------------------------------------
+-- get the type of 'x' as an Asteroid string
+with x do return escape
+"
+global __retval__
+val = state.symbol_table.lookup_sym('x')
+if val[0] == 'object':
+  (OBJECT, (STRUCT_ID, (ID, x_type)), MEMBER_LIST, OBJECT_MEMORY) = val
+elif val[0] in ['function-val','member-function-val']:
+  # internally we store functions as function values
+  # but to the user these look like functions as the 
+  # type counter part to the %function type pattern
+  # will match both function-val and member-function-val
+  x_type = 'function'
+else:
+  x_type = val[0]
+__retval__ = ('string', x_type)
+"
+end
+
+------------------------------------------------------------------
 -- List member functions
 ------------------------------------------------------------------
 
 -- NOTE: these functions must appear the
 -- 'list_member_functions' dictionary
 
 -- for implementation details see python lists in
@@ -463,15 +695,19 @@
 ------------------------------------------------------------------
 -- Construct an output list from those elements of the list for which
 -- f returns true. If f is none, the identity function is assumed,
 -- that is, all elements of input list that are false are removed.
 with f:%function do
     let out = [].
     for e in this do
-        let out = out+([e] if f(e) else []).
+        let r = f e.
+        if gettype r =/= "boolean" do 
+          escape "raise ValueError('list filter function has to return a Boolean')"
+        end
+        let out = out+([e] if r else []).
     end
     return out.
 end
 
 ------------------------------------------------------------------
 function __list_member__
 ------------------------------------------------------------------
@@ -700,45 +936,36 @@
 
 this_val = state.symbol_table.lookup_sym('this')
 item_val = state.symbol_table.lookup_sym('item')
 startix_val = state.symbol_table.lookup_sym('startix')
 endix_val = state.symbol_table.lookup_sym('endix')
 
 val = this_val[1].find(item_val[1], startix_val[1], endix_val[1])
-if val == -1:
-    __retval__ = ('none', None)
-else:
-    __retval__ = ('integer', val)
+__retval__ = ('integer', val)
 "
 with (item:%string,loc(startix:%integer,none)) do return escape
 "
 global __retval__
 
 this_val = state.symbol_table.lookup_sym('this')
 item_val = state.symbol_table.lookup_sym('item')
 startix_val = state.symbol_table.lookup_sym('startix')
 
 val = this_val[1].find(item_val[1], startix_val[1])
-if val == -1:
-    __retval__ = ('none', None)
-else:
-    __retval__ = ('integer',val)
+__retval__ = ('integer',val)
 "
 with item:%string do return escape
 "
 global __retval__
 
 this_val = state.symbol_table.lookup_sym('this')
 item_val = state.symbol_table.lookup_sym('item')
 
 val = this_val[1].find(item_val[1])
-if val == -1:
-    __retval__ = ('none', None)
-else:
-    __retval__ = ('integer',val)
+__retval__ = ('integer',val)
 "
 end
 
 ------------------------------------------------------------------
 function __string_flip__
 ------------------------------------------------------------------
 with none do
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/random.ast` & `asteroid-lang-2.0.1/asteroid/modules/random.ast`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 --
 -- this module implements the random numbers
 --
 -- (c) University of Rhode Island
 ------------------------------------------------------------------
 
 ------------------------------------------------------------------
-structure __RANDOM_MODULE__
-------------------------------------------------------------------
-with
-
-------------------------------------------------------------------
 function random
 ------------------------------------------------------------------
 -- return a random floating point number in the range [0.0, 1.0).
 with none do return escape
 "
 import random
 global __retval__
@@ -66,11 +61,7 @@
 from asteroid.support import assert_match
 
 sd_val = state.symbol_table.lookup_sym('sd')
 random.seed(sd_val[1])
 "
 end
 
-end -- __RANDOM_MODULE__
-
-------------------------------------------------------------------
-let random = __RANDOM_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/set.ast` & `asteroid-lang-2.0.1/asteroid/modules/set.ast`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 -- between lists and sets is that sets do not have repeated
 -- members.
 --
 -- (c) Lutz Hamel, University of Rhode Island
 ------------------------------------------------------------------
 
 ------------------------------------------------------------------
-structure __SET_MODULE__
-------------------------------------------------------------------
-with
-
-------------------------------------------------------------------
 function diff
 ------------------------------------------------------------------
 with (a:%list,b:%list) do return escape
 "
 global __retval__
 a_val = state.symbol_table.lookup_sym('a')
 b_val = state.symbol_table.lookup_sym('b')
@@ -69,11 +64,7 @@
 global __retval__
 a_val = state.symbol_table.lookup_sym('a')
 b_val = state.symbol_table.lookup_sym('b')
 __retval__ = ('list', list(set(a_val[1]) ^ set(b_val[1])))
 "
 end
 
-end -- __SET_MODULE__
-
-------------------------------------------------------------------
-let set = __SET_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/sort.ast` & `asteroid-lang-2.0.1/asteroid/modules/sort.ast`

 * *Files 21% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 --  sort((lambda with (x,y) do return true if x<y else false),
 --       [10,5,110,50]).
 --
 -- (c) University of Rhode Island
 ------------------------------------------------------------------
 
 ------------------------------------------------------------------
-structure __SORT_MODULE__
-------------------------------------------------------------------
-with
-
 function sort
+------------------------------------------------------------------
     with (_,[]) do
         return [].
     with (_,[a]) do
         return [a].
     with (p,[pivot|rest]) do
         let less=[].
         let more=[].
@@ -31,13 +28,10 @@
             if p(e,pivot) do
                 let less = less + [e].
             else
                 let more = more + [e].
             end
         end
 
-        return this @sort(p,less) + [pivot] + this @sort(p,more).
-    end
-end -- __SORT_MODULE__
+        return sort(p,less) + [pivot] + sort(p,more).
+end
 
-------------------------------------------------------------------
-let sort = __SORT_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/stream.ast` & `asteroid-lang-2.0.1/asteroid/modules/stream.ast`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 --
 -- (c) University of Rhode Island
 ------------------------------------------------------------------
 
 load system util.
 
 ------------------------------------------------------------------
-structure __STREAM__
+structure Stream
 ------------------------------------------------------------------
 -- Asteroid stream implementation based on lists
 with
 
 data stream.
 data curr_ix.
 
@@ -67,41 +67,36 @@
   end
 
 function rewind
   with none do
     let this @curr_ix = 0.
   end
 
-function __string__
+function __str__
 with none do return
 escape
 "
 from asteroid.state import state
 global __retval__
 
 this_val = state.symbol_table.lookup_sym('this')
 
 # destructure object
 (OBJECT,
  (STRUCT_ID, (ID, struct_id)),
+ (MEMBER_NAMES, (LIST, member_names)),
  (OBJECT_MEMORY, (LIST, memory))) = this_val
 
 __retval__ = ('string', term2string(memory[0]))
 "
 end
 
-end -- __STREAM__
+end -- Stream structure
 
 
 ------------------------------------------------------------------
-structure __STREAM_MODULE__
+function stream 
 ------------------------------------------------------------------
-with
-
-function stream with l:%list do
-   return __STREAM__(l).
+with l:%list do
+   return Stream(l).
 end
 
-end -- __STREAM_MODULE__
-
-------------------------------------------------------------------
-let stream = __STREAM_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/util.ast` & `asteroid-lang-2.0.1/asteroid/modules/util.ast`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,14 @@
 -- util.ast
 --
 -- this module defines utility functions and structures
 --
 -- (c) University of Rhode Island
 ------------------------------------------------------------------
 
-load system type.
-
-------------------------------------------------------------------
-structure __UTIL_MODULE__ 
-------------------------------------------------------------------
-with
-
 ------------------------------------------------------------------
 function achar
 ------------------------------------------------------------------
 -- given a decimal ASCII code return the corresponding character symbol
 with item:%integer do return escape
 "
 global __retval__
@@ -81,15 +74,15 @@
 "
 end
 
 ------------------------------------------------------------------
 function sleep
 ------------------------------------------------------------------
 -- program sleep for secs seconds
-with secs if type @isscalar(secs) do escape
+with secs if isscalar secs do escape
 "
 from time import sleep
 secs_val = state.symbol_table.lookup_sym('secs')
 sleep(secs_val[1])
 "
 end
 
@@ -146,11 +139,7 @@
 for (i,t) in l:
   out_list.append(('tuple',[i,t]))
 
 __retval__ = ('list', out_list)
 "
 end
 
-end -- __UTIL_MODULE__
-
-------------------------------------------------------------------
-let util = __UTIL_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/modules/vector.ast` & `asteroid-lang-2.0.1/asteroid/modules/vector.ast`

 * *Files 12% similar despite different names*

```diff
@@ -3,68 +3,61 @@
 --
 -- this module defines functions useful for vector arithmetic
 --
 -- (c) University of Rhode Island
 ------------------------------------------------------------------
 
 load system util.
-load system type.
-
-------------------------------------------------------------------
-structure __VECTOR_MODULE__ with
 
 ------------------------------------------------------------------
 function add
 ------------------------------------------------------------------
 with (a,b) do
-  return this @op(lambda with (x,y) do return x+y,a,b).
+  return op(lambda with (x,y) do x+y,a,b).
 end
 
 ------------------------------------------------------------------
 function dot
 -- computes the dot product of two lists
 ------------------------------------------------------------------
 with (a:%list,b:%list) do
-  return this @mult(a,b) @reduce(lambda with (x,y) do return x+y).
+  return mult(a,b) @reduce(lambda with (x,y) do x+y).
 end
 
 ------------------------------------------------------------------
 function mult
 ------------------------------------------------------------------
 with (a,b) do
-  return this @op(lambda with (x,y) do return x*y,a,b).
+  return op(lambda with (x,y) do x*y,a,b).
 end
 
 ------------------------------------------------------------------
 function op
 ------------------------------------------------------------------
 -- worker function for actual vector arithmetic
 -- Note: it also implements vector/scalar arithmetic
 with (f:%function,a:%list,b:%list) do
   if a @length() =/= b @length() do
-      throw Error("vops only defined on lists of the same length").
+      throw Error("vector operations only defined on lists of the same length").
   end
   let v = util @zip(a,b).
   return v @map(f).
-with (f:%function,a:%list,b if type @isscalar(b)) do
+with (f:%function,a:%list,b if isscalar b) do
   -- promote b to a vector
-  let bv = [1 to a @length()] @map(lambda with _ do return b).
+  let bv = [1 to a @length()] @map(lambda with _ do b).
   let v = util @zip(a,bv).
   return v @map(f).
-with (f:%function,a if type @isscalar(a),b:%list) do
+with (f:%function,a if isscalar a,b:%list) do
   -- promote a to a vector
-  let av = [1 to b @length()] @map(lambda with _ do return a).
+  let av = [1 to b @length()] @map(lambda with _ do a).
   let v = util @zip(av,b).
   return v @map(f).
 end
 
 ------------------------------------------------------------------
 function sub
 ------------------------------------------------------------------
 with (a,b) do
-  return this @op(lambda with (x,y) do return x-y,a,b).
+  return op(lambda with (x,y) do x-y,a,b).
 end
 
 
-end -- __VECTOR_MODULE__
-
-let vector = __VECTOR_MODULE__().
```

### Comparing `asteroid-lang-1.1.4/asteroid/repl.py` & `asteroid-lang-2.0.1/asteroid/repl.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,103 +7,110 @@
 from asteroid.interp import interp, load_prologue
 from asteroid.version import VERSION
 from asteroid.state import state
 from asteroid.globals import ExpectationError
 from asteroid.walk import function_return_value
 from asteroid.support import term2string
 
-from sys import stdin
+from sys import stdin,exit
 import platform
 
 if platform.system() == 'Windows':
     import pyreadline3
 else:
     import readline
 
 def repl(new=True, redundancy=False, prologue=False, functional_mode=False):
 
     if new:
         state.initialize()
-        load_prologue()
+        if prologue:
+            load_prologue()
         print_repl_menu()
     try:
-        run_repl(redundancy, prologue, functional_mode)
+        run_repl(redundancy, functional_mode)
     except EOFError:
         print()
         pass
 
 def print_repl_menu():
-    print("Asteroid Version", VERSION)
+    print("Asteroid", VERSION)
     print("(c) University of Rhode Island")
-    print("Type \"asteroid -h\" for help")
-    if platform.system() == 'Windows':
-        print("Press CTRL-Z + Return to exit")
-    else:
-        print("Press CTRL-D to exit")
+    print("Type \"help\" for additional information")
 
-def run_repl(redundancy, prologue, functional_mode):
+def run_repl(redundancy, functional_mode):
 
     # The two different prompt types either > for a new statement
     # or . for continuing one
     # lhh: changed the prompt since replit.com uses the > as their console prompt
     arrow_prompt, continue_prompt = ("ast> ", ".... ")
     current_prompt = arrow_prompt
 
     # Our line to be interpreted
     line = ""
     while True:
-        """
-        Line input, breaking, and exiting
-        """
+        ### Line input, breaking, and exiting
         try:
             # Get the new input and append it to the previous line (Possibly empty)
             # with a newline in between
 
             # If the line is empty, just set the line
             if line == "":
                 line = input(current_prompt)
 
             # Otherwhise append a new line
             else:
                 line += "\n" + input(current_prompt)
 
+            # see if we are looking at native repl commands
+            if line in ["help","quit"]:
+                match line:
+                    case "help":
+                        print()
+                        print("help          -- this message")
+                        print("quit          -- leave the Asteroid interpreter")
+                        print("load \"<file>\" --  load and run the program in <file>")
+                        print()
+                        print("or type any valid Asteroid statement at the prompt")
+                        print()
+                        line = ""
+                    case "quit":
+                        exit(0)
+                continue
+
         except KeyboardInterrupt:
             line = ""
             current_prompt = arrow_prompt
             print()
             continue
 
         except EOFError:
             print()
             break
 
-        """
-        Interpretation, multiline input, and exception handling
-        """
+        ### Interpretation, multiline input, and exception handling
         try:
             # Try to interpret the new statement
             interp(line,
                    initialize_state=False,
                    redundancy=redundancy,
-                   prologue=prologue,
+                   prologue=False, # prologue is managed by repl above
                    functional_mode=functional_mode,
                    exceptions=True)
 
             # Try to
             line = ""
 
             # Check for return value
             if function_return_value[-1]:
                 # Get the last return value (type, value)
                 retval = function_return_value[-1]
-
                 # If it isn't none, print out the value
                 if retval[1] != None:
                     print(term2string(function_return_value[-1]))
-
                     # Reset the return value
                     function_return_value[0] = None
 
         except ExpectationError as e:
             # If we expected something but found EOF, it's a continue
             if e.found_EOF:
                 current_prompt = continue_prompt
```

### Comparing `asteroid-lang-1.1.4/asteroid/state.py` & `asteroid-lang-2.0.1/asteroid/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,35 +7,35 @@
 from asteroid.symtab import SymTab
 
 class State:
     def __init__(self):
         self.initialize()
 
     def initialize(self,module="<input>"):
+        self.mainmodule = None
         self.symbol_table = SymTab()
-        self.modules = [] # loaded modules
         self.AST = None
-        self.ignore_pattern = 0 # used to evaluate pattern expressions
-        self.cond_warning = False # used to indicate if conditional subsumption
-                                  # warning has been displayed
         self.eval_redundancy = True
+        self.warning = True # switch for general warnings
         self.lineinfo = (module, 1) # tuple: module, lineno
         # stack of 3-tuples for stack trace of function
         # calls: (module,lineno,function name)
         self.trace_stack = [(module,1,"<toplevel>")]
         # if an exception occurs then error_trace will point to
         # it.  an exception handler is responsible for clearing
         # this.
         self.error_trace = None
+        self.debugger = None
 
 state = State()
 
 def warning(str):
-    module, lineno = state.lineinfo
-    print("Warning: {}: {}: {}".format(module, lineno, str))
+    if state.warning:
+        module, lineno = state.lineinfo
+        print("Warning: {}: {}: {}".format(module, lineno, str))
 
 def dump_trace():
     if state.error_trace:
         _dump_trace(state.error_trace)
         return        
     else:
         _dump_trace(state.trace_stack)
```

### Comparing `asteroid-lang-1.1.4/asteroid/symtab.py` & `asteroid-lang-2.0.1/asteroid/symtab.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,29 @@
         if len(self.scoped_symtab) == 1:
             raise ValueError("cannot pop the global scope")
         else:
             scope = self.scoped_symtab.pop(CURR_SCOPE)
             self.globals.pop(CURR_SCOPE)
             return scope
 
+    def get_curr_scope(self, scope=CURR_SCOPE, option="items"):
+        if option == "items":
+            return list(self.scoped_symtab[scope].items())
+        elif option == "unifiers":
+            unifiers = []
+            for (sym,val) in self.scoped_symtab[scope].items():
+                unifiers += [(('id',sym),val)]
+            return unifiers
+        elif option == "keys":
+            return list(self.scoped_symtab[scope].keys())
+        elif option == "values":
+            return list(self.scoped_symtab[scope].values())
+        else:
+            raise ValueError("unknown option")
+
     def enter_sym(self, sym, value):
         # enter the symbol in the appropriate scope
         if sym in self.globals[CURR_SCOPE]:
             scope_dict = self.global_scope
         else:
             scope_dict = self.scoped_symtab[CURR_SCOPE]
```

### Comparing `asteroid-lang-1.1.4/asteroid/walk.py` & `asteroid-lang-2.0.1/asteroid/walk.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,21 @@
 # A tree walker to interpret Asteroid programs
 #
 # (c) University of Rhode Island
 #########################################################################
 
 from copy import deepcopy,copy
 from re import match as re_match
+from math import isclose
 
 from asteroid.globals import *
 from asteroid.support import *
 from asteroid.state import state, warning
 
 #########################################################################
-# These two variables are used by the debugger. "Debugging" is a flag
-# to tell if we're currently in debugging mode and "Debugger" is a
-# debugger object. For more information on the debugger's helper
-# functions. See the function definitions in this file.
-#########################################################################
-debugging = False
-debugger = None
-
-#########################################################################
 # this dictionary maps list member function names to function
 # implementations given in the Asteroid prologue.
 # see 'prologue.ast' for details
 list_member_functions = dict()
 
 #########################################################################
 # this dictionary maps string member function names to function
@@ -38,553 +30,274 @@
 #########################################################################
 # return values for function computed by the last expression executed
 # in the context of a function.  note that we consider global code
 # to be part of the 'top-level' function
 function_return_value = [None]
 
 ###########################################################################################
-def __unify(term, pattern, unifying = True ):
+def unify(term, pattern, unifying = True ):
     '''
     unify term and pattern recursively and return the unifier.
-    this unification allows for the same variable to appear
-    multiple times in the unifier.  the user of this
-    function must take appropriate actions if this happens.
 
-    we assume that both the term and the pattern are made up of tuple
+    we assume that both the term and the pattern are made up of AST tuple
     nodes:
 
              (<type>, children*)
 
-    leaf nodes must be nullary constructors.
-
     NOTE: if the pattern looks like an lval then it is treated like an lval, e.g.
-            let a@[0] = 'a@[0].
-          stores the term 'a@[0] into lval a@[0].
+            let a@[0] = a@[0].
+          stores the value stored at a@[0] into lval a@[0].
     NOTE: Default argument unifying is set to be true. If we are unifying, then we are
-          evaluating unification between a pattern and a term. If we are not
+          evaluating unification/matching between a pattern and a term. If we are not
           unifying, then we are evaluating subsumption between two patterns for the
           purpose of detecting redundant/useless pattern clauses in functions.
+    NOTE: The tests (if/elif clauses) are ordered:
+            1. Python instance level matching
+            2. Special match cases for terms and patterns
+            3. AST structural matching
     '''
 
-    ### Python value level matching
+    ################################
+    ### 1. Python instance level matching
     # NOTE: in the first rules where we test instances we are comparing
     # Python level values, if they don't match exactly then we have
     # a pattern match fail.
-    if isinstance(term, str): # apply regular expression match
-        message_explicit("Regex match: {} and {}", [pattern, term], level="secondary")
-
+    if isinstance(term, str): 
+        # apply regular expression match
+        # Note: a pattern needs to match the whole term.
         if isinstance(pattern, str) and re_match("^"+pattern+"$", term):
-            # Note: a pattern needs to match the whole term.
-            message_explicit("Matched!", level="tertiary")
             return [] # return empty unifier
         else:
-            message_explicit("Failed!", level="tertiary")
             raise PatternMatchFailed(
                 "regular expression '{}' did not match '{}'"
                 .format(pattern, term))
-
+                
     elif isinstance(term, (int, float, bool)):
-        message_explicit("Literal match: {} and {}", [pattern, term], level="primary")
-
         if term == pattern:
-            message_explicit("Matched!", level="secondary")
             return [] # return an empty unifier
         else:
-            message_explicit("Failed! {} != {}", [pattern, term], level="secondary")
             raise PatternMatchFailed(
                 "'{}' is not the same as '{}'"
                 .format(term, pattern))
 
     elif isinstance(term, list) or isinstance(pattern, list):
         if not(isinstance(term, list)) or not(isinstance(pattern, list)):
             raise PatternMatchFailed(
                 "term and pattern do not agree on list/tuple constructor")
         elif len(term) != len(pattern):
             raise PatternMatchFailed(
                 "term and pattern lists/tuples are not the same length")
         else:
-            message_explicit("Matching lists: {} and {}",
-                [gen_t2s( ('list', pattern) ), gen_t2s( ('list', term) )],
-                increase=True, notify=True)
-
             # Make our unifier(s)
             unifier = []
             for i in range(len(term)):
                 unifier += unify(term[i], pattern[i], unifying)
-
-            message_explicit("Matched!", decrease=True)
-
             # Ensure we have no non-linear patterns
             check_repeated_symbols(unifier)
-
             return unifier
     
-    elif ((not unifying) and (term[0] == 'named-pattern')):
+    #################################
+    ### 2. Special match cases for terms and patterns
+    # Asteroid value level matching
+    elif (not unifying) and (pattern[0] == 'deref' or term[0] == 'deref'):
+        # since first-class patterns are almost always conditional
+        # patterns and conditional patterns are not supported by
+        # the redundancy test we punt here and save computation time.
+        raise PatternMatchFailed(
+            "first-class patterns not supported.")
 
-        # Unpack a term-side named-pattern if evaluating redundant clauses
-        message_explicit("Evaluating named pattern", notify=True)
-        return unify(term[2],pattern,unifying)
+    elif (not unifying) and (pattern[0] == 'typematch' or term[0] == 'typematch'):
+        raise PatternMatchFailed(
+                "typematch patterns not supported")
 
-    elif ((not unifying) and (term[0] == 'deref')):
+    elif (not unifying) and (pattern[0] == 'if-exp' or term[0] == 'if-exp'):
+        # conditional patterns are not supported in redundancy
+        # test because they can involved arbitraty computations
+        # which cannot be tested.
+        raise PatternMatchFailed(
+            "conditional patterns not supported.")
 
-        # Unpack a term-side first-class pattern if evaluating redundant clauses
-        term_pattern = walk(term[1])
-        return unify(term_pattern, pattern, unifying)
+    elif (not unifying) and (pattern[0] in ['head-tail', 'raw-head-tail'] or 
+             term[0] in ['head-tail', 'raw-head-tail']):
+        raise PatternMatchFailed(
+            "head-tail operator not supported")
 
-    ### Asteroid value level matching
-    elif pattern[0] == 'object' and term[0] == 'object':
-        # this can happen when we dereference a variable pointing
-        # to an object as a pattern, e.g.
-        #    let o = A(1,2). -- A is a structure with 2 data members
-        #    let *o = o.
-        (OBJECT, (STRUCT_ID, (ID, pid)), (OBJECT_MEMORY, (LIST, pl))) = pattern
-        (OBJECT, (STRUCT_ID, (ID, tid)), (OBJECT_MEMORY, (LIST, tl))) = term
-        if pid != tid:
+    elif (not unifying) and pattern[0] == 'apply' and term[0] == 'apply':
+        fp = pattern[1]
+        ft = term[1]
+        if fp[0] != 'id' or ft[0] != 'id':
+            raise ValueError("pattern subsumption not supported")
+        # unpack the apply structures
+        (APPLY, (ID, t_id), t_arg) = term
+        (APPLY, (ID, p_id), p_arg) = pattern
+        # only constructors are allowed in patterns
+        type = state.symbol_table.lookup_sym(t_id,strict=False)
+        if not type or type[0] != 'struct':
+            raise ValueError(
+                    "illegal pattern: function or operator '{}' not supported"
+                    .format(t_id))
+        type = state.symbol_table.lookup_sym(p_id,strict=False)
+        if not type or type[0] != 'struct':
+            raise ValueError(
+                    "illegal pattern: function or operator '{}' not supported"
+                    .format(p_id))
+        # make sure apply id's match
+        if t_id != p_id:
             raise PatternMatchFailed(
-                "pattern type '{}' and term type '{}' do not agree"
-                .format(pid,tid))
-
-        message_explicit("Matching objects {}{} and {}{}",
-            [pid, gen_t2s( ('tuple', pl) ), tid, gen_t2s( ('tuple', tl) )],
-            increase=True
-        )
-
-        unifiers = []
-
-        for i in range(len(pl)):
-            # OWM: We can't actually unify function-vals. If we know the type is
-            # the same, can we just assume the function-val is the same?
-            notify_explicit()
-
-            if tl[i][0] != 'function-val':
-                unifiers += unify(tl[i], pl[i])
-        
-        message_explicit("Objects matched", decrease=True)
-        return unifiers
+                "term '{}' does not match pattern '{}'"
+                .format(t_id, p_id))
+        # unify the args
+        return unify(t_arg, p_arg, unifying)
 
-    # no implicit type conversions during pattern matching
-    # removing this code, see the discussion in issue 95
-    # elif pattern[0] == 'string' and term[0] != 'string':
-        # regular expression applied to a non-string structure
-        # this is possible because all data types are subtypes of string
-    #    message_explicit("Matching string {} and non-string {}",
-    #        [gen_t2s(pattern), gen_t2s(term)],
-    #        notify=True
-    #    )
-    #
-    #    return unify(term2string(term), pattern[1])
+    elif term[0] in (unify_not_allowed - {'function-val', 'foreign'}):
+        # NOTE: functions/foreign are allowed in terms as long as they are matched
+        # by a variable in the pattern - anything else will fail
+        raise PatternMatchFailed(
+            "term of type '{}' not allowed in pattern matching"
+            .format(term[0]))
 
-    elif pattern[0] == 'if-exp':
+    elif pattern[0] in unify_not_allowed:
+        raise PatternMatchFailed(
+            "pattern of type '{}' not allowed in pattern matching"
+            .format(pattern[0]))
 
-        # If we are evaluating subsumtion
-        if not unifying:
+    elif pattern[0] == 'id': # variable in pattern add to unifier
+        if pattern[1] == '_': # anonymous variable - ignore unifier
+            return []
+        else:
+            id_val = state.symbol_table.lookup_sym(pattern[1],strict=False)
+            if id_val and id_val[0] == 'pattern':
+                warning("you are overwriting a pattern stored in '{}'".format(pattern[1]))
+            unifier = (pattern, term)
+            return [unifier]
 
-            # If we are evaluating subsumption between two different conditional patterns
-            # we want to 'punt' and print a warning message.
-            if term[0] == 'if-exp':
-
-                if not state.cond_warning:
-                    warning("Redundant pattern detection is not supported for conditional pattern expressions.")
-                    state.cond_warning = True
+    elif pattern[0] == 'index': # index act like a var
+        unifier = (pattern, term)
+        return [unifier]
 
-            # Otherwise if the term is not another cmatch the clauses are correctly ordered.
+    elif pattern[0] == 'none':
+        if term[0] == 'none':
+            return []
+        else:
             raise PatternMatchFailed(
-                "Subsumption relatioship broken, pattern will not be rendered redundant.")
-
-        (IF_EXP, cond_exp, pexp, else_exp) = pattern
+                    "expected 'none' got '{}'"
+                    .format(term[0]))
 
+    elif pattern[0] == 'if-exp':
+        (IF_EXP, cond_exp, patexp, else_exp) = pattern
         if else_exp[0] != 'null':
-            raise PatternMatchFailed("conditional patterns do not support 'else' clauses")
-
-        # Explicit messaging
-        message_explicit("Conditional match: if ({})",
-            [gen_t2s(cond_exp)],
-            notify=True, increase=True
-        )
-
-        unifiers = unify(term, pexp, unifying)
-
+            raise PatternMatchFailed(
+                    "conditional patterns do not support 'else' clauses")
         # evaluate the conditional expression in the
-        # context of the unifiers.
-        declare_unifiers(unifiers)
-        bool_val = map2boolean(walk(cond_exp))
-
+        # context of the unifiers of the pattern before the 
+        # if clause and only expose all
+        # unifiers if conditional was successful
+        state.symbol_table.push_scope({})
+        declare_unifiers(unify(term, patexp, unifying))
+        bool_val = walk(cond_exp)
+        if bool_val[0] != 'boolean':
+            raise ValueError("found '{}' expected 'boolean' in conditional pattern"
+                             .format(bool_val[0]))
+        # copy unifiers out of the temporary scope of the
+        # if expression.
+        unifiers = state.symbol_table.get_curr_scope(option="unifiers")
+        state.symbol_table.pop_scope()
         if bool_val[1]:
-            message_explicit("Condition met, {}",
-                [gen_t2s(cond_exp)], decrease=True
-            )
             return unifiers
         else:
-            message_explicit("Condition ({}) failed",
-                [gen_t2s(cond_exp)], decrease=True
-            )
             raise PatternMatchFailed(
-                "conditional pattern match failed")
-
-    elif term[0] == 'if-exp':
-        # We will only get here when evaluating subsumption
-
-        # If we get here, a conditional pattern clause is placed after a non-conditonal
-        # pattern clause. Therefore, we need to check if the subsume because if they do
-        # the conditonal clause is redundant.
-        (IF_EXP, cond_exp, pexp, else_exp) = term
-
-        if else_exp[0] != 'null':
-            raise PatternMatchFailed("conditional patterns do not support 'else' clauses")
-
-        #return unify(pexp,pattern,False)
-        # Otherwise if the term is not another cmatch the clauses are correctly ordered.
-        raise PatternMatchFailed(
-            "conditional patterns not supported.")
+                    "conditional pattern match failed")
 
     elif pattern[0] == 'typematch':
-        typematch = pattern[1]
-        nextIndex = 0 #indicates index of where we will 'look' next
-        
-        message_explicit("Typematch {} to type {}", [gen_t2s(term), typematch])
-
-        if typematch in ['string','real','integer','list','tuple','boolean','none']:
-
-            if (not unifying):
-
-                #walk a different path for this node
-                if (term[0] == 'typematch'):
-                    nextIndex = 1
-
-                #handle lists/head-tails subsuming each other
-                if (term[0] in ["list","head-tail"]):
-                    if ((typematch == 'list')):
-                        return []
-
-            if typematch == term[nextIndex]:
-                message_explicit("Success!", level="secondary")
+        typematch_kind = pattern[1]
+        if typematch_kind in ['string','real','integer','list','tuple','boolean','none']:
+            if typematch_kind == term[0]:
                 return []
             else:
-                message_explicit("Failure", level="secondary")
                 raise PatternMatchFailed(
-                    "expected type '{}' got a term of type '{}'"
-                    .format(typematch, term[nextIndex]))
-
-        elif typematch == 'function':
+                    "expected a value of type '{}' got a value of type '{}'"
+                    .format(typematch_kind, term[0]))
+        elif typematch_kind == 'function':
             # matching function and member function values
             if term[0] in ['function-val','member-function-val']:
-                message_explicit("Success!", level="secondary")
                 return []
             else:
-                message_explicit("Failure", level="secondary")
                 raise PatternMatchFailed(
-                    "expected type '{}' got a term of type '{}'"
-                    .format(typematch, term[0]))
-
-        elif typematch == 'pattern':
-            if unifying:
-
-                # any kind of structure can be a pattern, and variables
-                # see globals.py for a definition of 'patterns'
-                if term[nextIndex] in patterns:
-                    message_explicit("Success!", level="secondary")
-                    return []
-                else:
-                    message_explicit("Failure", level="secondary")
-                    raise PatternMatchFailed(
-                            "expected type '{}' got a term of type '{}'"
-                            .format(typematch, term[0]))
-
-            else: # Evaluating typematch-pattern subsumption
-                #walk a different path for this one node
-                if (term[0] == 'typematch'):
-                    nextIndex = 1
-
-                #handle lists/head-tails subsuming each other
-                if (term[0] in ["list","head-tail"]):
-                    if ((typematch == 'list')):
-                        message_explicit("Success!", level="secondary")
-                        return []
-
-                if term[nextIndex] in pattern_subsumes:
-                    message_explicit("Success!", level="secondary")
-                    return []
-                else:
-                    message_explicit("Failure", level="secondary")
-                    raise PatternMatchFailed(
-                        "expected type '{}' got a term of type '{}'"
-                        .format(typematch, term[nextIndex]))
-
-        elif term[0] == 'object':
-            if state.symbol_table.lookup_sym(typematch)[0] != 'struct':
-                raise PatternMatchFailed( "'{}' is not a type".format(typematch) )
-
+                    "expected a value of type '{}' got a value of type '{}'"
+                    .format(typematch_kind, term[0]))
+        elif typematch_kind == 'pattern':
+            # any kind of structure can be a pattern, and variables
+            # see globals.py for a definition of 'patterns'
+            if term[0] in patterns:
+                return []
+            else:
+                raise PatternMatchFailed(
+                        "expected a value of type '{}' got a value of type '{}'"
+                        .format(typematch_kind, term[0]))
+        elif term[0] == 'object': # then typematch_kind has to be a structure type
+            if state.symbol_table.lookup_sym(typematch_kind)[0] != 'struct':
+                raise PatternMatchFailed( 
+                        "'{}' is not a type"
+                        .format(typematch_kind) )
             (OBJECT,
                 (STRUCT_ID, (ID, struct_id)),
+                (MEMBER_NAMES, LIST),
                 (OBJECT_MEMORY, LIST)) = term
-            if struct_id == typematch:
-                message_explicit("Success!", level="secondary")
+            if struct_id == typematch_kind:
                 return []
             else:
-                message_explicit("Failure", level="secondary", increase=True)
                 raise PatternMatchFailed(
-                    "expected type '{}' got an object of type '{}'"
-                    .format(typematch, struct_id))
-
+                    "expected a value of type '{}' got a value of type '{}'"
+                    .format(typematch_kind, struct_id))
         else:
-            if state.symbol_table.lookup_sym(typematch)[0] != 'struct':
-                message_explicit("Failure", level="secondary", increase=True)
-
-                raise PatternMatchFailed( "'{}' is not a type".format(typematch) )
+            if state.symbol_table.lookup_sym(typematch_kind)[0] != 'struct':
+                raise PatternMatchFailed( "'{}' is not a type".format(typematch_kind) )
             else:
-                message_explicit("Failure", level="secondary", increase=True)
-
                 raise PatternMatchFailed(
-                    "expected type '{}' got an object of type '{}'"
-                    .format(typematch, term[0]))
-
-
-    elif pattern[0] == 'named-pattern':
-        # unpack pattern
-        (NAMED_PATTERN, name_exp, p) = pattern
-        message_explicit("Matching term {} and pattern {} to [{}]",
-            [gen_t2s(term), gen_t2s(p), gen_t2s(name_exp)],
-            notify=True, increase=True
-        )
-        # name_exp has to be an id or an index expression.
-        if name_exp[0] not in ['id','index']:
-            raise ValueError(
-                "expected a variable, list element, or data member in named pattern\
-                 instead of {}".format(term2string(name_exp)))
-
-        unifiers = unify(term, p, unifying) + [(name_exp, term)]
-        
-        message_explicit("Matched ({} and {})", 
-            [gen_t2s(unifiers[0][0]), gen_t2s(unifiers[0][1])],
-            decrease=True
-        )
-
-        return unifiers
-
-    elif pattern[0] == 'none':
-        if term[0] != 'none':
-            message_explicit("{} and none do not match",
-                [gen_t2s(term)]
-            )
-            raise PatternMatchFailed("expected 'none' got '{}'"
-                    .format(term[0]))
-        else:
-            message_explicit("None and None match", level="secondary")
-            return []
-
-    # NOTE: functions/foreign are allowed in terms as long as they are matched
-    # by a variable in the pattern - anything else will fail
-    elif term[0] in (unify_not_allowed - {'function-val', 'foreign'}):
-        raise PatternMatchFailed(
-            "term of type '{}' not allowed in pattern matching"
-            .format(term[0]))
-
-    elif pattern[0] in unify_not_allowed:
-        raise PatternMatchFailed(
-            "pattern of type '{}' not allowed in pattern matching"
-            .format(pattern[0]))
+                    "expected a value of type '{}' got a value of type '{}'"
+                    .format(typematch_kind, term[0]))
 
     elif pattern[0] == 'pattern':
-        # pattern operator on the pattern side can always be ignored
-        # --TODO double check - ttc
         if term[0] == 'pattern':
-            return unify(term[1], pattern[1], unifying)
+            # term is a first-class pattern, ie, a pattern value
+            # we are not allowed to match on that.
+            raise PatternMatchFailed(
+                "cannot pattern-match patterns")
         else:
+            # treat the pattern value as a pattern and continue matching.
             return unify(term, pattern[1], unifying)
 
-    elif term[0] == 'pattern' and pattern[0] not in ['id', 'index']:
-        # ignore pattern operator on the term if we are not trying to unify term with
-        # a variable or other kind of lval
-        return unify(term[1], pattern, unifying)
-
-    elif term[0] == 'object' and pattern[0] == 'apply':
-        # unpack term
-        (OBJECT,
-         (STRUCT_ID, (ID, struct_id)),
-         (OBJECT_MEMORY, (LIST, obj_memory))) = term
-        # unpack pattern
-        (APPLY,
-         (ID, apply_id),
-         arg) = pattern
-        type = state.symbol_table.lookup_sym(apply_id)
-        if type[0] != 'struct':
-            raise PatternMatchFailed("'{}' is not a type".format(apply_id))
-
-        if struct_id != apply_id:
-            raise PatternMatchFailed("expected type '{}' got type '{}'"
-                .format(apply_id, struct_id))
-        # we are comparing raw lists here
-        if arg[0] == 'tuple':
-            pattern_list = arg[1]
-        else:
-            pattern_list = [arg]
-
-        # only pattern match on object data members
-        message_explicit("Matching object {}{} and pattern {}{}",
-            [apply_id,  gen_t2s( ('tuple', data_only(obj_memory)) ),
-            struct_id, gen_t2s( ('tuple', pattern_list) )],
-            notify=True
-        )
-        # Running through the list elements indivuidually allows for
-        # better debugging information
-        unifiers = []
-        data = data_only(obj_memory)
-
-        for i in range(len(data)):
-            unifiers += unify(data[i], pattern_list[i], unifying)
-
-        return unifiers
-
-    elif pattern[0] == 'index': # list element lval access
-        unifier = (pattern, term)
-        return [unifier]
-
-# lhh: looking at patterns as values we are now allowed to match
-# against patterns as terms where the terms now include variables.
-#    elif term[0] == 'id' and unifying: # variable in term not allowed
-#        raise PatternMatchFailed(      # when unifying
-#            "variable '{}' in term not allowed"
-#            .format(term[1]))
-
-    elif pattern[0] == 'id': # variable in pattern add to unifier
-        sym = pattern[1]
-        if sym == '_': # anonymous variable - ignore unifier
-            return []
-        else:
-            unifier = (pattern, term)
-            return [unifier]
-
-    elif pattern[0] in ['head-tail', 'raw-head-tail']:
-        message_explicit("Matching {} to {}",
-            [gen_t2s(term), gen_t2s(pattern)],
-            notify=True
-        )
-        # if we are unifying or we are not evaluating subsumption
-        #  to another head-tail
-        if unifying or term[0] not in ['head-tail', 'raw-head-tail']:
-            (HEAD_TAIL, pattern_head, pattern_tail) = pattern
-            (LIST, list_val) = term
-
-            if LIST != 'list':
-                message_explicit("Failed", level="secondary")
-                raise PatternMatchFailed(
-                    "head-tail operator expected type 'list' got type '{}'"
-                    .format(LIST))
-
-            if not len(list_val):
-                message_explicit("Failed", level="secondary")
-
-                raise PatternMatchFailed(
-                    "head-tail operator expected a non-empty list")
-
-            list_head = list_val[0]
-            list_tail = ('list', list_val[1:])
-            unifier = []
-
-            unifier += unify(list_head, pattern_head, unifying)
-            unifier += unify(list_tail, pattern_tail, unifying)
-
-            check_repeated_symbols(unifier) #Ensure we have no non-linear patterns
-            message_explicit("Success!", level="secondary")
-
-            return unifier
-
-        else: #Else we are evaluating subsumption to another head-tail
-
-            lengthH = head_tail_length(pattern) #H->higher order of predcence pattern
-            lengthL = head_tail_length(term)    #L->lower order of predcence pattern
-
-            if lengthH == 2 and lengthL != 2:
-                return unify(pattern[1],term[1],unifying)
-
-            if (lengthH > lengthL): # If the length of the higher presedence pattern is greater
-                                    # then length of the lower precedence pattern, it is not redundant
-                message_explicit("Failed", level="secondary")
-                raise PatternMatchFailed(
-                    "Subsumption relatioship broken, pattern will not be rendered redundant.")
-
-            else: #Else we continue evaluating the different terms in the head-tail pattern
-                (HEAD_TAIL, patternH_head, patternH_tail) = pattern
-                (HEAD_TAIL, patternL_head, patternL_tail) = term
-
-                unifier = []
-                for i in range(lengthH):
-                    unifier += unify(patternL_head,patternH_head,unifying)
-                    try:
-                        (RAW_HEAD_TAIL, patternH_head, patternH_tail) = patternH_tail
-                        (RAW_HEAD_TAIL, patternL_head, patternL_tail) = patternL_tail
-                    except:
-                        break
-
-                check_repeated_symbols(unifier) #Ensure we have no non-linear patterns
-                message_explicit("Success!", level="secondary")
-                return unifier
-
     elif pattern[0] == 'deref':  # ('deref', v, bl)
         # v can be an AST representing any computation
         # that produces a pattern.
-
-        message_explicit("Dereferencing {}", [gen_t2s(pattern[1])])
-
         p = walk(pattern[1])
-
         if pattern[2][0] != 'nil': # we have a binding term list
-            if p[1][0] != 'constraint':
+            if p[1][0] != 'scope':
                 raise ValueError(
                     "binding term lists only supported for constraint patterns")
             else: 
                 # construct a new constraint pattern with the binding term list in place
                 p = ('pattern',
-                        ('constraint',
+                        ('scope',
                             p[1][1],
                             pattern[2]))
-
-
-        message_explicit("{} -> {}", [gen_t2s(pattern), gen_t2s(p)], 
-            level="secondary")
-
-        notify_explicit()
-
         return unify(term,p,unifying)
 
-    # builtin operators look like apply lists with operator names
-    elif pattern[0] == 'apply':
-        if term[0] != pattern[0]: # make sure both are applys
-            raise PatternMatchFailed(
-                "term and pattern disagree on structure")
-
-        # unpack the apply structures
-        (APPLY, (ID, t_id), t_arg) = term
-        (APPLY, (ID, p_id), p_arg) = pattern
-
-        # make sure apply id's match
-        if t_id != p_id:
-            raise PatternMatchFailed(
-                "term '{}' does not match pattern '{}'"
-                .format(t_id, p_id))
-
-        # unify the args
-        return unify(t_arg, p_arg, unifying)
-
-    elif pattern[0] == 'constraint':
-        message_explicit("[Begin] constraint pattern: {}",
-            [gen_t2s(pattern[1])],
-            notify=True, increase=True
-        )
-
+    elif pattern[0] == 'scope':
         p = pattern[1]
         bl = pattern[2] # binding term list
-
         # constraint patterns are evaluated in their own scope
-        state.symbol_table.push_scope({})
-        unifier = unify(term,p)
-        state.symbol_table.pop_scope()
-
-        message_explicit("[End] constraint pattern", decrease=True)
-
+        try:
+            state.symbol_table.push_scope({})
+            unifier = unify(term,p)
+            state.symbol_table.pop_scope()
+        except PatternMatchFailed as e:
+            state.symbol_table.pop_scope()
+            # rethrow exception so that pattern match failure is properly propagated
+            raise e 
         # process binding list
         if bl[0] == 'nil':
             return [] #Return an empty unifier
         else:
             # binding list is non-empty, map variables
             # that appear in the binding list into
             # the returned unifier
@@ -593,41 +306,113 @@
                 ((ID,x),exp) = u
                 for bt in bl[1]:
                     (BINDING_TERM, (ID,y), new_id) = bt
                     if x == y:
                         new_unifier += [(new_id,exp)]
             return new_unifier
 
-    elif term[0] != pattern[0]:  # nodes are not the same
-        message_explicit("Fail: {} and {} are not the same",
-            [term[0], pattern[0]], level="secondary")
-        
+    elif pattern[0] == 'object' and term[0] == 'object':
+        # this can happen when we dereference a variable pointing
+        # to an object as a pattern, e.g.
+        #    let o = A(1,2). -- A is a structure with 2 data members
+        #    let *o = o.
+        (OBJECT, (STRUCT_ID, (ID, pid)), pml, (OBJECT_MEMORY, (LIST, pl))) = pattern
+        (OBJECT, (STRUCT_ID, (ID, tid)), tml, (OBJECT_MEMORY, (LIST, tl))) = term
+        if pid != tid:
+            raise PatternMatchFailed(
+                "pattern type '{}' and term type '{}' do not agree"
+                .format(pid,tid))
+        unifiers = []
+        # we only pattern match on data members
+        tl_data_members = data_only(tl)
+        pl_data_members = data_only(pl)
+        if len(tl_data_members) != len(pl_data_members):
+            raise ValueError("internal error: not the same number of data members for objects")
+        for i in range(len(pl_data_members)):
+            unifiers += unify(tl_data_members[i], pl_data_members[i])
+        return unifiers
+
+    elif pattern[0] == 'apply' and term[0] == 'object':
+        # in patterns constructor functions match objects, e.g.
+        #   let A(x,y) = A(1,2)
+        # only constructors are allowed in patterns
+        f = pattern[1]
+        if f[0] == 'index':
+            # scope qualified pattern name
+            (APPLY,
+              (INDEX,
+                (ID, modname),
+                (ID, apply_id)),
+              arg) = pattern
+        else:
+            modname = None
+            (APPLY,
+              (ID, apply_id),
+              arg) = pattern
+        # unpack term
+        (OBJECT,
+         (STRUCT_ID, (ID, struct_id)),
+         (MEMBER_NAMES, (LIST, member_names)),
+         (OBJECT_MEMORY, (LIST, obj_memory))) = term
+        if modname:
+            orig_config = set_module_env(modname)        
+        type = state.symbol_table.lookup_sym(apply_id,strict=False)
+        if modname:
+            set_config(orig_config)
+        if not type or type[0] != 'struct':
+            raise ValueError("illegal pattern, '{}' is not a type".format(apply_id))
+        if struct_id != apply_id:
+            raise PatternMatchFailed("expected type '{}' got type '{}'"
+                .format(apply_id, struct_id))
+        # retrieve argument list to constructor
+        # Note: we want it to be a list so we can compare it to the object memory
+        if arg[0] == 'tuple':
+            arg_list = arg[1]
+        else:
+            arg_list = [arg]
+        # only pattern match on object data members
+        data_list = data_only(obj_memory)
+        return unify(data_list, arg_list, unifying)
+
+    elif pattern[0] in ['head-tail', 'raw-head-tail']:
+        (HEAD_TAIL, pattern_head, pattern_tail) = pattern
+        if term[0] != 'list':
+            raise PatternMatchFailed(
+                "head-tail operator expected a list got a value of type '{}'"
+                .format(term[0]))
+        (LIST, list_val) = term
+        if not len(list_val):
+            raise PatternMatchFailed(
+                "head-tail operator expected a non-empty list")
+        list_head = list_val[0]
+        list_tail = ('list', list_val[1:])
+        unifier = []
+        unifier += unify(list_head, pattern_head, unifying)
+        unifier += unify(list_tail, pattern_tail, unifying)
+        check_repeated_symbols(unifier) #Ensure we have no non-linear patterns
+        return unifier
+ 
+    #################################
+    ### 3. AST structural matching
+    elif pattern[0] != term[0]:  # node types are not the same
         raise PatternMatchFailed(
             "nodes '{}' and '{}' are not the same"
             .format(term[0], pattern[0]))
 
-    elif len(term) != len(pattern): # nodes are not of same the arity
-        message_explicit("Fail: {} and {} are not the same arity",
-            [term[0], pattern[0]], level="secondary")
-
+    elif len(pattern) != len(term): # nodes are not of same the arity
         raise PatternMatchFailed(
             "nodes '{}' and '{}'' are not of the same arity"
             .format(term[0], pattern[0]))
 
-    else:
-        #lhh
-        #print("unifying {}".format(pattern[0]))
+    else: # unify AST children nodes
         unifier = []
         for i in range(1,len(term)):
             unifier += unify(term[i], pattern[i], unifying)
-        #lhh
-        #print("returning unifier: {}".format(unifier))
         return unifier
 
-
 #########################################################################
 def eval_actual_args(args):
 
     return walk(args)
 
 #########################################################################
 def declare_formal_args(unifiers):
@@ -720,27 +505,30 @@
             # compute the index
             ix_val = walk(ix)
 
     # for objects we access the object memory
     elif structure_val[0] == 'object':
         (OBJECT,
          (STRUCT_ID, (ID, struct_id)),
-         (OBJECT_MEMORY, (LIST, memory))) = structure_val
-        # compute the index -- for objects this has to be done
-        # in the context of the struct scope
-        struct_val = state.symbol_table.lookup_sym(struct_id)
-        # unpack the struct value
-        (STRUCT,
          (MEMBER_NAMES, (LIST, member_names)),
-         (STRUCT_MEMORY, (LIST, struct_memory))) = struct_val
-
+         (OBJECT_MEMORY, (LIST, memory))) = structure_val
         if ix[0] == 'id' and ix[1] in member_names:
             ix_val = ('integer', member_names.index(ix[1]))
         else:
-            ix_val = walk(ix)
+            raise ValueError("{} is not a member of type {}"
+                .format(term2string(ix),struct_id))
+            #ix_val = walk(ix)
+
+    elif structure_val[0] == 'module':
+        (MODULE, id, (CLOSURE, closure)) = structure_val
+        config = state.symbol_table.get_config()
+        state.symbol_table.set_config(closure)
+        val = walk(ix)
+        state.symbol_table.set_config(config)
+        return val
 
     elif structure_val[0] == 'pattern':
         # simple patterns are just structures - skip the pattern operator
         return read_at_ix(structure_val[1], ix)
 
     else:
         raise ValueError("term '{}' is not indexable"
@@ -791,31 +579,34 @@
         # compute the index
         ix_val = walk(ix)
 
     # for objects we access the object memory
     elif structure_val[0] == 'object':
         (OBJECT,
          (STRUCT_ID, (ID, struct_id)),
-         (OBJECT_MEMORY, (LIST, memory))) = structure_val
-        # compute the index -- for objects this has to be done
-        # in the context of the struct scope
-        struct_val = state.symbol_table.lookup_sym(struct_id)
-        # unpack the struct value
-        (STRUCT,
          (MEMBER_NAMES, (LIST, member_names)),
-         (STRUCT_MEMORY, (LIST, struct_memory))) = struct_val
-
+         (OBJECT_MEMORY, (LIST, memory))) = structure_val
         if ix[0] == 'id' and ix[1] in member_names:
             ix_val = ('integer', member_names.index(ix[1]))
         else:
             ix_val = walk(ix)
 
+    elif structure_val[0] == 'module':
+        (MODULE, id, (CLOSURE, closure)) = structure_val
+        config = state.symbol_table.get_config()
+        state.symbol_table.set_config(closure)
+        # execute an assignment in the context of the module
+        walk(('unify', ix, value))
+        state.symbol_table.set_config(config)
+        return
+
     elif structure_val[0] == 'pattern':
         # simple patterns are just structures - skip the pattern operator
-        return store_at_ix(structure_val[1], ix, value)
+        store_at_ix(structure_val[1], ix, value)
+        return
 
     else:
         raise ValueError("term '{}' is not a mutable structure"
                          .format(term2string(structure_val)))
 
     # Next, we do the actual memory storage operation
 
@@ -840,156 +631,388 @@
 
         # For each index
         for i in range(len(lval)):
             # Get the memory location of the lval and set it to the
             # corresponding rval value
             (INTEGER, location) = lval[i]
             memory[location] = rval[i]
-
         return
 
     else:
         raise ValueError("index op '{}' in patterns not supported"
                          .format(ix_val[0]))
 
 #########################################################################
+# set module environment
+def set_module_env(modname):
+    module_val = state.symbol_table.lookup_sym(modname)
+    if module_val[0] != 'module':
+        raise ValueError("{} is not a module".format(modname))
+    (MODULE, id, (CLOSURE, closure)) = module_val
+    config = state.symbol_table.get_config()
+    state.symbol_table.set_config(closure)
+    return config
+
+#########################################################################
+def set_config(config):
+    state.symbol_table.set_config(config)
+
+#########################################################################
+# implementations for builtin operators and functions. these operators 
+# and functions do not need/are not allowed to have a function 
+# local scope.  therefore they are implemented here as builtins as 
+# part of the interpreter proper.  for other builtins that do 
+# not have this restriction see the prologue.
+
 def handle_builtins(node):
     (APPLY, (ID, opname), args) = node
     assert_match(APPLY, 'apply')
     assert_match(ID, 'id')
 
+    # deal with binary operators
     if opname in binary_operators:
-        (TUPLE, bin_args)= args
-        val_a = walk(bin_args[0])
-        val_b = walk(bin_args[1])
+        (TUPLE, [a,b])= args
 
         if opname == '__plus__':
-            type = promote(val_a[0], val_b[0])
-            if type in ['integer', 'real', 'list', 'boolean']:
-                return (type, val_a[1] + val_b[1])
-            elif type == 'string':
-                return (type, term2string(val_a) + term2string(val_b))
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real', 'list', 'string']:
+                if val_b[0] in ['integer', 'real', 'list', 'string']:
+                    if val_a[0]==val_b[0]:
+                        return (val_a[0], val_a[1] + val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} + {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} + {}' expected '{} + {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '+'".format(val_b[0]))
             else:
-                raise ValueError("unsupported type '{}' in +".format(type))
+                raise ValueError("unsupported type '{}' in '+'".format(val_a[0]))
         elif opname == '__minus__':
-            type = promote(val_a[0], val_b[0])
-            if type in ['integer', 'real']:
-                return (type, val_a[1] - val_b[1])
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real']:
+                if val_b[0] in ['integer', 'real']:
+                    if val_a[0]==val_b[0]:
+                        return (val_a[0], val_a[1] - val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} - {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} - {}' expected '{} - {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '-'".format(val_b[0]))
             else:
-                raise ValueError("unsupported type '{}' in -".format(type))
+                raise ValueError("unsupported type '{}' in '-'".format(val_a[0]))
         elif opname == '__times__':
-            type = promote(val_a[0], val_b[0])
-            if type in ['integer', 'real']:
-                return (type, val_a[1] * val_b[1])
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real']:
+                if val_b[0] in ['integer', 'real']:
+                    if val_a[0]==val_b[0]:
+                        return (val_a[0], val_a[1] * val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} * {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} * {}' expected '{} * {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '*'".format(val_b[0]))
             else:
-                raise ValueError('unsupported type in *')
+                raise ValueError("unsupported type '{}' in '*'".format(val_a[0]))
         elif opname == '__divide__':
-            type = promote(val_a[0], val_b[0])
-            if type == 'integer':
-                return (type, int(val_a[1]) // int(val_b[1]))
-            elif type == 'real':
-                return ('real', float(val_a[1]) / float(val_b[1]))
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real']:
+                if val_b[0] in ['integer', 'real']:
+                    if val_a[0]==val_b[0]:
+                        if val_a[0] == 'integer':
+                            return ('integer', val_a[1] // val_b[1])
+                        elif val_a[0] == 'real':
+                            return ('real', val_a[1] / val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} / {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} / {}' expected '{} / {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '/'".format(val_b[0]))
             else:
-                raise ValueError('unsupported type in /')
+                raise ValueError("unsupported type '{}' in '/'".format(val_a[0]))
         elif opname == '__or__':
-            # NOTE: do we need to typecheck here?
-            if map2boolean(val_a)[1] == True or map2boolean(val_b)[1] == True:
-               return ('boolean', True)
+            # short circuit evaluation
+            val_a = walk(a)
+            if val_a[0] == 'boolean':
+                if val_a[1] == True:
+                    return ('boolean', True)
+            else:
+                raise ValueError(
+                    "found '{} expected 'boolean and boolean'"
+                    .format(val_a[0]))
+            val_b = walk(b)
+            if val_b[0] == 'boolean':
+                return ('boolean', val_a[1] or val_b[1])
             else:
-               return ('boolean', False)
+                raise ValueError(
+                    "found '{} and {}' expected 'boolean and boolean'"
+                    .format(val_a[0],val_b[0]))
         elif opname == '__and__':
-            # NOTE: do we need to typecheck here?
-            if map2boolean(val_a)[1] == True and map2boolean(val_b)[1] == True:
-               return ('boolean', True)
+            # short circuit evaluation
+            val_a = walk(a)
+            if val_a[0] == 'boolean':
+                if val_a[1] == False:
+                    return ('boolean', False)
+            else:
+                raise ValueError(
+                    "found '{} expected 'boolean and boolean'"
+                    .format(val_a[0]))
+            val_b = walk(b)
+            if val_b[0] == 'boolean':
+                return ('boolean', val_a[1] and val_b[1])
             else:
-               return ('boolean', False)
+                raise ValueError(
+                    "found '{} and {}' expected 'boolean and boolean'"
+                    .format(val_a[0],val_b[0]))
         elif opname == '__eq__':
-            type = promote(val_a[0], val_b[0])
-            if type in ['integer', 'real', 'list', 'tuple', 'boolean', 'none']:
-                return ('boolean', val_a[1] == val_b[1])
-            elif type == 'string':
-                return ('boolean', term2string(val_a) == term2string(val_b))
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real', 'list', 'tuple', 'boolean', 'string', 'none']:
+                if val_b[0] in ['integer', 'real', 'list', 'tuple', 'boolean', 'string', 'none']:
+                    if val_a[0]==val_b[0]:
+                        if val_a[0] == 'real' and val_a[1] != val_b[1] and isclose(val_a[1],val_b[1]):
+                            warning("possible rounding error issue")
+                        return ('boolean', val_a[1] == val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} == {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} == {}' expected '{} == {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '=='".format(val_b[0]))
             else:
-                raise ValueError('unsupported type in ==')
+                raise ValueError("unsupported type '{}' in '=='".format(val_a[0]))
         elif opname  == '__ne__':
-            type = promote(val_a[0], val_b[0])
-            if type in ['integer', 'real', 'list', 'tuple', 'boolean', 'none']:
-                return ('boolean', val_a[1] != val_b[1])
-            elif type == 'string':
-                return ('boolean', term2string(val_a) != term2string(val_b))
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real', 'list', 'tuple', 'boolean', 'string', 'none']:
+                if val_b[0] in ['integer', 'real', 'list', 'tuple', 'boolean', 'string', 'none']:
+                    if val_a[0]==val_b[0]:
+                        if val_a[0] == 'real' and val_a[1] != val_b[1] and isclose(val_a[1],val_b[1]):
+                            warning("possible rounding error issue")
+                        return ('boolean', val_a[1] != val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} =/= {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} =/= {}' expected '{} =/= {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '=/='".format(val_b[0]))
             else:
-                raise ValueError('unsupported type in =/=')
+                raise ValueError("unsupported type '{}' in '=/='".format(val_a[0]))
         elif opname == '__le__':
-            type = promote(val_a[0], val_b[0])
-            if type in ['integer', 'real']:
-                return ('boolean', val_a[1] <= val_b[1])
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real', 'string']:
+                if val_b[0] in ['integer', 'real', 'string']:
+                    if val_a[0]==val_b[0]:
+                        if val_a[0] == 'real' and val_a[1] != val_b[1] and isclose(val_a[1],val_b[1]):
+                            warning("possible rounding error issue")
+                        return ('boolean', val_a[1] <= val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} <= {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} <= {}' expected '{} <= {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '<='".format(val_b[0]))
             else:
-                raise ValueError('unsupported type in <=')
+                raise ValueError("unsupported type '{}' in '<='".format(val_a[0]))
         elif opname == '__lt__':
-            type = promote(val_a[0], val_b[0])
-            if type in ['integer', 'real']:
-                return ('boolean', val_a[1] < val_b[1])
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real', 'string']:
+                if val_b[0] in ['integer', 'real', 'string']:
+                    if val_a[0]==val_b[0]:
+                        if val_a[0] == 'real' and val_a[1] != val_b[1] and isclose(val_a[1],val_b[1]):
+                            warning("possible rounding error issue")
+                        return ('boolean', val_a[1] < val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} < {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} < {}' expected '{} < {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '<'".format(val_b[0]))
             else:
-                raise ValueError('unsupported type in <')
+                raise ValueError("unsupported type '{}' in '<'".format(val_a[0]))
         elif opname == '__ge__':
-            type = promote(val_a[0], val_b[0])
-            if type in ['integer', 'real']:
-                return ('boolean', val_a[1] >= val_b[1])
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real', 'string']:
+                if val_b[0] in ['integer', 'real', 'string']:
+                    if val_a[0]==val_b[0]:
+                        if val_a[0] == 'real' and val_a[1] != val_b[1] and isclose(val_a[1],val_b[1]):
+                            warning("possible rounding error issue")
+                        return ('boolean', val_a[1] >= val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} >= {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} >= {}' expected '{} >= {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '>='".format(val_b[0]))
             else:
-                raise ValueError('unsupported type in >=')
+                raise ValueError("unsupported type '{}' in '>='".format(val_a[0])) 
         elif opname == '__gt__':
-            type = promote(val_a[0], val_b[0])
-            if type in ['integer', 'real']:
-                return ('boolean', val_a[1] > val_b[1])
+            val_a = walk(a)
+            val_b = walk(b)
+            if val_a[0] in ['integer', 'real', 'string']:
+                if val_b[0] in ['integer', 'real', 'string']:
+                    if val_a[0]==val_b[0]:
+                        if val_a[0] == 'real' and val_a[1] != val_b[1] and isclose(val_a[1],val_b[1]):
+                            warning("possible rounding error issue")
+                        return ('boolean', val_a[1] > val_b[1])
+                    else:
+                        type = promote(val_a[0], val_b[0])
+                        if type == None:
+                            raise ValueError(
+                                "operation '{} > {}' not supported"
+                                .format(val_a[0],val_b[0]))
+                        else:
+                            raise ValueError(
+                                "found '{} > {}' expected '{} > {}'"
+                                .format(val_a[0],val_b[0],type,type))
+                else:
+                    raise ValueError("unsupported type '{}' in '>'".format(val_b[0]))
             else:
-                raise ValueError('unsupported type in >')
+                raise ValueError("unsupported type '{}' in '>'".format(val_a[0])) 
         else:
-            raise ValueError("unknown builtin binary operation '{}'".format(opname))
+            raise ValueError("unknown builtin binary operator '{}'".format(opname))
 
+    # deal with unary operators
     elif opname in unary_operators:
-        arg_val = walk(args)
-
+        arg_val = walk(args)             
         if opname == '__not__':
-            val = map2boolean(arg_val)
-            if val[1] == False:
-                return ('boolean', True)
-            elif val[1] == True:
-                return ('boolean', False)
+            if arg_val[0] == 'boolean':
+                if arg_val[1] == False:
+                    return ('boolean', True)
+                else:
+                    return ('boolean', False)
             else:
-                raise ValueError("not a boolean value in 'not'")
+                raise ValueError("found 'not {}' expected 'not boolean'"
+                                 .format(arg_val[0]))
         elif opname == '__uminus__':
             if arg_val[0] in ['integer', 'real']:
                 return (arg_val[0], - arg_val[1])
             else:
                 raise ValueError(
                     "unsupported type '{}' in unary minus"
                     .format(arg_val[0]))
         elif opname == '__uplus__':
             if arg_val[0] in ['integer', 'real']:
                 return (arg_val[0], + arg_val[1])
             else:
                 raise ValueError(
                     "unsupported type '{}' in unary plus"
                     .format(arg_val[0]))
+        elif opname == 'assert':
+            if arg_val[0] != 'boolean':
+                raise ValueError('the assert operator expected a Boolean value')
+            if not arg_val[1]:
+                raise ValueError('assert failed')
+            else:
+                return ('none', None)
+        elif opname == 'escape':
+            global __retval__
+            __retval__ = ('none', None)
+            if arg_val[0] != 'string':
+                raise ValueError('expected a string as argument to the escape operator')
+            exec(arg_val[1])
+            return __retval__
+        elif opname == 'eval':
+            if arg_val[0] == 'string':
+                import frontend
+                parser = frontend.Parser(filename="<eval>")
+                eval_ast = parser.parse(arg_val[1])
+                walk(eval_ast)
+                return function_return_value[-1]
+            else:
+                raise ValueError('expected a string as argument to the eval operator')
+
+        else:
+            raise ValueError("unknown builtin unary operator '{}'".format(opname))
+
+    # deal with nullary operators
+    elif opname in nullary_operators:
+        (type, _) = walk(args)
+        if type != 'none':
+            raise ValueError("{} is a nullary operator".format(opname))
+        if opname == 'toplevel':
+            return ('boolean', state.mainmodule == state.lineinfo[0])
         else:
-            raise ValueError("unknown builtin unary operation '{}'".format(opname))
+            raise ValueError("unknown builtin nullary operator '{}'".format(opname))
+        
 
 #########################################################################
 def pop_stackframe(error_trace=False): 
     # pop frame off the stack
     state.symbol_table.pop_scope()
     state.symbol_table.set_config(state.symbol_table.saved_configs.pop())
     if error_trace:
         state.error_trace = copy(state.trace_stack)
     state.trace_stack.pop()
 
 #########################################################################
 def handle_call(obj_ref, fval, actual_val_args, fname):
-    # Needed for later
-    global debugging
 
     # function calls transfer control - save our caller's lineinfo
     # we save the debug information here to preserve lineinfo between
     # function calls between files.
     old_lineinfo = state.lineinfo
 
     (FUNCTION_VAL, body_list, closure) = fval
@@ -999,125 +1022,83 @@
                               state.lineinfo[1],
                               fname))
 
     # static scoping for functions
     # Note: we have to do this here because unifying
     # over the body patterns can introduce variable declarations,
     # think conditional pattern matching.
+    # Note: we are keeping a stack of configs so that
+    # the debugger can look at contents of 
+    # Asteroid stack frames
     state.symbol_table.saved_configs.append(
         state.symbol_table.get_config()
     )
-
     state.symbol_table.set_config(closure)
     state.symbol_table.push_scope({})
 
-    # Explicit message
-    message_explicit("Call: {}({})",
-        [fname, gen_t2s(actual_val_args)],
-        increase=True
-    )
-
-    # We want to return back to whatever tab level the function
-    # call started at, so, we grab this here to reset to at
-    # the return. This allows recursive functions to have
-    # the proper formatting
-    if debugging: cur_tab_level = debugger.tab_level
+    # if we have an obj reference bind it to the
+    # variable 'this'
+    if obj_ref:
+        state.symbol_table.enter_sym('this', obj_ref)
 
     # iterate over the bodies to find one that unifies with the actual parameters
     (BODY_LIST, (LIST, body_list_val)) = body_list
     unified = False
 
     for i in range(0, len(body_list_val), 2):
         # Process lineinfo
         lineinfo = body_list_val[ i ]
         process_lineinfo(lineinfo)
 
         # Deconstruct function body
         (BODY,
-        (PATTERN, p),
-        (STMT_LIST, stmts)) = body_list_val[ i + 1]
+          (PATTERN, p),
+          stmts) = body_list_val[ i + 1]
 
-        message_explicit("Attempting to match {} with pattern {}",
-            [gen_t2s(actual_val_args), gen_t2s(p)], level="primary",
-            notify=True, increase=True
-        )
-        
         try:
             # Attempt to unify the actual args and the pattern
             unifiers = unify(actual_val_args, p)
             unified = True
-
-            # Do our explicit message
-            message_explicit("Success! Matched function body", level="primary", decrease=True)
-
         except PatternMatchFailed:
-            # Reset the tab level
-            if explicit_enabled():
-                debugger.tab_level = cur_tab_level + 1
-
-            # Print the explicit messaging
-            message_explicit("Failed to match function body", level="tertiary", decrease=True)
-
             unifiers = []
             unified = False
 
         if unified:
             break
 
-    # Reset the tab level back to the function call's level
-    if debugging: debugger.tab_level = cur_tab_level
-
     if not unified:
         raise ValueError("actual argument '{}' not recognized by function '{}'"
                          .format(term2string(actual_val_args),fname))
     declare_formal_args(unifiers)
 
-    # if we have an obj reference bind it to the
-    # variable 'this'
-    if obj_ref:
-        state.symbol_table.enter_sym('this', obj_ref)
-
     # OWM: The following segment is a repeat of the bottom of this function.
     # We need to do this because redundant patterns can break scope and
     # some debugger and state features as they exit computation.
 
     # Check for useless patterns
     try:
         if state.eval_redundancy:
-            old_debugging = debugging
-            debugging = False
             check_redundancy(body_list, fname)
-            debugging = old_debugging
 
     # Reset settings
     except RedundantPatternFound as r:
-        debugging = old_debugging
         # restore caller's env
         state.lineinfo = old_lineinfo
-        # Keep debugger up to date
-        if debugging: debugger.set_lineinfo(state.lineinfo)
         pop_stackframe()
         raise r
 
     # execute the function
+    if state.debugger: state.debugger.enter_function(fname)
     global function_return_value
-
     try:
         function_return_value.append(None)
-
-        walk_stmt_list(stmts)
-
-        # Pop the return value
+        walk(stmts)
         val = function_return_value.pop()
-
-        # If we have one, set it as the retval
         if val:
             return_value = val
-
-        # Otherwhise default the return value to none
         else:
             return_value = ('none', None)
 
     except ReturnValue as val:
         # we got here because a return statement threw a return object
         function_return_value.pop()
         return_value = val.value
@@ -1128,24 +1109,17 @@
         # Note: do not reset lineinfo, this way the state points at the source 
         # of the exception
         pop_stackframe(error_trace=True)
         raise e
 
     # all done with function call -- clean up and exit
     # restore caller's env
+    if state.debugger: state.debugger.exit_function(fname)
     state.lineinfo = old_lineinfo
-    # Keep debugger up to date
-    if debugging: debugger.set_lineinfo(state.lineinfo)
     pop_stackframe()
-    message_explicit("Return: {} from {}",
-            [("None" if (not return_value[1]) else gen_t2s(return_value)), 
-            fname],
-            decrease=True
-    )
-
     return return_value
 
 #########################################################################
 def declare_unifiers(unifiers):
     # walk the unifiers and bind name-value pairs into the symtab
 
     # TODO: check for repeated names in the unfiers
@@ -1171,124 +1145,105 @@
             # indexing/slicing
             # update the memory of the object.
             store_at_ix(structure_val, ix, value)
 
         else:
             raise ValueError("unknown unifier type '{}'".format(lval[0]))
     
-    # Explicit messaging for unifiers
-    if explicit_enabled():
-        # if we've unified anything
-        if unifiers:
-            # Create our format string and list of terms
-            fstring = ""
-            terms = []
-
-            # For each unifier except the last one
-            for (lval, value) in unifiers[:-1]:
-                # Add to our format string and our terms
-                fstring += "{} = {}, "
-                terms += [gen_t2s(lval), gen_t2s(value)]
-
-            # Get the last unifier and add it to the terms and fstring
-            (lval, value) = unifiers[-1]
-            fstring += "{} = {}"
-            terms += [gen_t2s(lval), gen_t2s(value)]
+#########################################################################
+# node functions
+#########################################################################
+def stmt_list(node):
 
-            # Print our message
-            message_explicit(fstring, terms)
+    (STMT_LIST, stmts) = node
+    assert_match(STMT_LIST, 'stmt-list')
+    
+    walk(stmts)
 
 #########################################################################
-# node functions
+def exp_stmt(node):
+    if state.debugger: state.debugger.step()
+
+    (EXP_STMT, exp) = node
+    assert_match(EXP_STMT,'exp-stmt')
+
+    walk(exp)
+    # statements don't return values
+    return
+
 #########################################################################
 def global_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
     (GLOBAL, (LIST, id_list)) = node
     assert_match(GLOBAL, 'global')
     assert_match(LIST, 'list')
 
     global_str = ""
 
     for id_tuple in id_list:
         (ID, id_val) = id_tuple
         if state.symbol_table.is_symbol_local(id_val):
             raise ValueError("'{}' is already local, cannot be declared global"
                              .format(id_val))
         state.symbol_table.enter_global(id_val)
         global_str += "{}, ".format(id_val)
-    
-    message_explicit("Global defs: {}", [global_str[:-1]] )
-
-#########################################################################
-def assert_stmt(node):
-    notify_debugger()
-
-    (ASSERT, exp) = node
-    assert_match(ASSERT, 'assert')
-
-    exp_val = walk(exp)
-
-    # mapping asteroid assert into python assert
-    assert exp_val[1], 'assert failed'
+ 
 #########################################################################
 def unify_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
     (UNIFY, pattern, exp) = node
     assert_match(UNIFY, 'unify')
 
     term = walk(exp)
-
     unifiers = unify(term, pattern)
-
     declare_unifiers(unifiers)
 
 #########################################################################
 def return_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
     (RETURN, e) = node
     assert_match(RETURN, 'return')
     
     retval = walk(e)
 
     raise ReturnValue(retval)
 
 #########################################################################
 def break_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
     (BREAK,) = node
     assert_match(BREAK, 'break')
 
     raise Break()
 
 #########################################################################
 def throw_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
     (THROW, object) = node
     assert_match(THROW, 'throw')
     
     throw_object = walk(object)
 
     raise ThrowValue(throw_object)
 
 #########################################################################
 def try_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
     (TRY,
-     (STMT_LIST, try_stmts),
+     try_stmts,
      (CATCH_LIST, (LIST, catch_list))) = node
 
-    stepping = debugger_has_stepped()
     try:
-        walk_stmt_list(try_stmts)
+        walk(try_stmts)
 
     # NOTE: in Python the 'as inst' variable is only local to the catch block???
     # NOTE: we map user visible Python exceptions into standard Asteroid exceptions
     #       by constructing Exception objects - see prologue.ast
     except ThrowValue as inst:
         except_val = inst.value
         inst_val = inst
@@ -1296,60 +1251,66 @@
     except ReturnValue as inst:
         # return values should never be captured by user level try stmts - rethrow
         raise inst
 
     except PatternMatchFailed as inst:
         except_val = ('object',
                          ('struct-id', ('id', 'Exception')),
+                         ('member-names', ('list',["kind","val","__init__"])),
                          ('object-memory',
                           ('list',
                            [('string', 'PatternMatchFailed'),
                             ('string', inst.value)])))
         inst_val = inst
 
     except RedundantPatternFound as inst:
         except_val = ('object',
                          ('struct-id', ('id', 'Exception')),
+                         ('member-names', ('list',["kind","val","__init__"])),
                          ('object-memory',
                           ('list',
                            [('string', 'RedundantPatternFound'),
                             ('string', str(inst))])))
         inst_val = inst
 
     except NonLinearPatternError as inst:
         except_val = ('object',
                          ('struct-id', ('id', 'Exception')),
+                         ('member-names', ('list',["kind","val","__init__"])),
                          ('object-memory',
                           ('list',
                            [('string', 'NonLinearPatternError'),
                             ('string', str(inst))])))
         inst_val = inst
 
     except ArithmeticError as inst:
         except_val = ('object',
                          ('struct-id', ('id', 'Exception')),
+                         ('member-names', ('list',["kind","val","__init__"])),
                          ('object-memory',
                           ('list',
                            [('string', 'ArithmeticError'),
                             ('string', str(inst))])))
         inst_val = inst
 
     except FileNotFoundError as inst:
         except_val = ('object',
                          ('struct-id', ('id', 'Exception')),
+                         ('member-names', ('list',["kind","val","__init__"])),
                          ('object-memory',
                           ('list',
                            [('string', 'FileNotFound'),
                             ('string', str(inst))])))
         inst_val = inst
 
     except Exception as inst:
         # mapping general Python exceptions into Asteroid's SystemError
         except_val = ('object',
                          ('struct-id', ('id', 'Exception')),
+                         ('member-names', ('list',["kind","val","__init__"])),
                          ('object-memory',
                           ('list',
                            [('string', 'SystemError'),
                             ('string', str(inst))])))
         inst_val = inst
 
     else:
@@ -1357,91 +1318,88 @@
         return
 
     # we had an exception - walk the catch list and find an appropriate set of
     # catch statements.
     for catch_val in catch_list:
         (CATCH,
          (CATCH_PATTERN, catch_pattern),
-         (CATCH_STMTS, catch_stmts)) = catch_val
+         catch_stmts) = catch_val
         try:
             unifiers = unify(except_val, catch_pattern)
         except PatternMatchFailed:
             pass
         else:
             # handler found - null out error_trace
             state.error_trace = None
             declare_unifiers(unifiers)
-            walk_stmt_list(catch_stmts, step_state=stepping)
+            walk(catch_stmts)
             return
 
     # no exception handler found - rethrow the exception
     raise inst_val
 
 #########################################################################
 def loop_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
     (LOOP, body_stmts) = node
     assert_match(LOOP, 'loop')
 
-    (STMT_LIST, body) = body_stmts
-
     try:
-        stepping = debugger_has_stepped()
         while True:
-            walk_stmt_list(body, step_state=stepping)
+            walk(body_stmts)
     except Break:
         pass
 
 #########################################################################
 def while_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
-    (WHILE, cond_exp, body_stmts) = node
+    (WHILE, (COND_EXP, cond), body_stmts) = node
     assert_match(WHILE, 'while')
 
-    (COND_EXP, cond) = cond_exp
-    (STMT_LIST, body) = body_stmts
-
     try:
-        stepping = debugger_has_stepped()
-
-        (COND_TYPE, cond_val) = map2boolean(walk(cond))
+        (cond_type, cond_val) = walk(cond)
+        if cond_type != 'boolean':
+            raise ValueError("found '{}' expected 'boolean' in while loop"
+                             .format(cond_type))
         while cond_val:
-            walk_stmt_list(body, step_state=stepping)
-            (COND_TYPE, cond_val) = map2boolean(walk(cond))
+            walk(body_stmts)
+            (cond_type, cond_val) = walk(cond)
+            if cond_type != 'boolean':
+                raise ValueError("found '{}' expected 'boolean' in while loop"
+                                .format(cond_type))
     except Break:
         pass
 
 #########################################################################
 def repeat_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
-    (REPEAT, body_stmts, cond_exp) = node
+    (REPEAT, body_stmts, (COND_EXP, cond)) = node
     assert_match(REPEAT, 'repeat')
 
-    (COND_EXP, cond) = cond_exp
-    (STMT_LIST, body) = body_stmts
-
     try:
-        stepping = debugger_has_stepped()
         while True:
-            walk_stmt_list(body, step_state=stepping)
-            (COND_TYPE, cond_val) = map2boolean(walk(cond))
+            walk(body_stmts)
+            (cond_type, cond_val) = walk(cond)
+            if cond_type != 'boolean':
+                raise ValueError("found '{}' expected 'boolean' in repeat loop"
+                                .format(cond_type))
             if cond_val:
                 break
 
     except Break:
         pass
 
 #########################################################################
 def for_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
-    (FOR, (IN_EXP, in_exp), (STMT_LIST, stmt_list)) = node
+    (FOR, (IN_EXP, in_exp), stmt_list) = node
     assert_match(FOR, 'for')
 
     (IN, pattern, list_term) = in_exp
 
     # expand the list_term
     (LIST_TYPE, list_val) = walk(list_term)
     if LIST_TYPE not in ['list','string','tuple']:
@@ -1459,52 +1417,65 @@
     # NOTE: just like Python, loop bodies do not create a new scope!
     # NOTE: we can use unification as a filter of elements:
     #
     #      for (2,y) in [(1,11), (1,12), (1,13), (2,21), (2,22), (2,23)]  do
     #             print y.
     #      end for
     try:
-        stepping = debugger_has_stepped()
         for term in list_val:
             try:
                 unifiers = unify(term,pattern)
             except PatternMatchFailed:
                 pass
             else:
                 declare_unifiers(unifiers)
-                walk_stmt_list(stmt_list, step_state=stepping)
+                walk(stmt_list)
                 
     except Break:
         pass
 
 #########################################################################
+def match_stmt(node):
+    if state.debugger: state.debugger.step()
+
+    (MATCH, val, if_clauses) = node
+    assert_match(MATCH, 'match')
+
+    walk(val)
+    walk(if_clauses)
+    
+#########################################################################
 def if_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
     (IF, (LIST, if_list)) = node
     assert_match(IF, 'if')
     assert_match(LIST, 'list')
 
     for i in range(0,len(if_list),2):
 
         lineinfo = if_list[ i ]
         process_lineinfo(lineinfo)
 
         (IF_CLAUSE,
          (COND, cond),
-         (STMT_LIST, stmts)) = if_list[ i + 1 ]
+         stmts) = if_list[ i + 1 ]
 
-        (BOOLEAN, cond_val) = map2boolean(walk(cond))
+        (cond_type, cond_val) = walk(cond)
+        if cond_type != 'boolean':
+            raise ValueError("found '{}' expected 'boolean' in if clause"
+                            .format(cond_type))
 
         if cond_val:
-            walk_stmt_list(stmts)
+            walk(stmts)
             break
+
 #########################################################################
 def struct_def_stmt(node):
-    notify_debugger()
+    if state.debugger: state.debugger.step()
 
     (STRUCT_DEF, (ID, struct_id), (MEMBER_LIST, (LIST, member_list))) = node
     assert_match(STRUCT_DEF, 'struct-def')
     assert_match(ID, 'id')
     assert_match(MEMBER_LIST, 'member-list')
     assert_match(LIST, 'list')
 
@@ -1536,100 +1507,63 @@
     struct_type = ('struct',
                   ('member-names', ('list', member_names)),
                   ('struct-memory', ('list', struct_memory)))
 
     state.symbol_table.enter_sym(struct_id, struct_type)
 
 #########################################################################
-def import_stmt(node):
-    notify_debugger()
-
-    global debugging
-    old_debugging = debugging
-    debugging = False
+def module_def_stmt(node):
 
-    (LIST, inlist) = node
-    assert_match(LIST, 'import_stmt')
-
-    for e in inlist:
-        walk(e)
-
-    debugging = old_debugging
+    (MODULE_DEF, (ID, modname), stmts) = node
+    assert_match(MODULE_DEF, 'module-def')
 
-    return
-
-#########################################################################
-def top_level_exp_stmt(node):
 
-    (TOP_LEVEL_EXP, exp) = node
-    assert_match(TOP_LEVEL_EXP, 'top-level-exp')
-
-    notify_debugger()
+    state.symbol_table.push_scope({})
+    if state.debugger: state.debugger.enter_module(modname)
+    walk(stmts)
+    closure = state.symbol_table.get_closure()
+    if state.debugger: state.debugger.exit_module(modname)
+    state.symbol_table.pop_scope()
 
-    return walk(exp)
+    module_type = ('module', ('id', modname), ('scope', closure))
+    state.symbol_table.enter_sym(modname, module_type)
 
 #########################################################################
-def eval_exp(node):
-
-    (EVAL, exp) = node
-    assert_match(EVAL, 'eval')
- 
-    # Note: eval is essentially a macro call - that is a function
-    # call without pushing a symbol table record.  That means
-    # we have to first evaluate the argument to 'eval' before
-    # walking the term.  This is safe because if the arg is already
-    # the actual term it will be quoted and nothing happens if it is
-    # a variable it will be expanded to the actual term.
-
-    state.trace_stack.append((state.lineinfo[0],
-                              state.lineinfo[1],
-                              "eval"))
+def load_stmt(node):
+    if state.debugger: state.debugger.step()
 
+    (LOAD_STMT, inlist) = node
+    assert_match(LOAD_STMT, 'load-stmt')
 
-    # evaluate actual parameter
-    exp_val_expand = walk(exp)
-
-    # now walk the actual term
-    if exp_val_expand[0] == 'string':
-        import frontend
-        parser = frontend.Parser(filename="<eval>")
-        eval_ast = parser.parse(exp_val_expand[1])
-        walk(eval_ast)
-        exp_val = function_return_value[-1]
-    else:
-        state.ignore_pattern += 1
-        exp_val = walk(exp_val_expand)
-        state.ignore_pattern -= 1
+    walk(inlist)
 
-    state.trace_stack.pop()
-    return exp_val
+    return
 
 #########################################################################
 def apply_exp(node):
     (APPLY, f, arg) = node
     assert_match(APPLY, 'apply')
 
     # handle builtin operators that look like apply lists.
-    if f[0] == 'id' and f[1] in operator_symbols:
+    if f[0] == 'id' and f[1] in builtins:
         return handle_builtins(node)
 
     # handle function application
     # retrieve the function name from the AST
     if f[0] in ['function-exp','apply']:
         # cannot use the function expression as a name,
         # could be a very complex computation. the apply
         # node means that the lambda function has to still be
         # computed.
         f_name = 'lambda'
     elif f[0] == 'index':
-        # object member function
+        # member/module function
         (INDEX, ix, (ID, f_name)) = f
-        # 'str' is necessary in case we use an index value
-        # instead of a function name -- see regression test test085.ast
-        f_name = "member function " + str(f_name)
+        if not isinstance(f_name, str):
+            raise ValueError("function names have to be strings")
     else:
         # just a regular function call
         (ID, f_name) = f
 
     # evaluate the function expression and the arguments
     f_val = walk(f)
     arg_val = walk(arg)
@@ -1647,37 +1581,48 @@
 
     # regular function call
     elif f_val[0] == 'function-val':
         result = handle_call(None, f_val, arg_val, f_name)
 
     # object constructor call
     elif f_val[0] == 'struct':
-        (ID, struct_id) = f
+        if f[0] == 'index':
+            # constructor name qualified with a module name
+            (INDEX, (ID, modname), (ID, struct_id)) = f
+        else: 
+            # inscope constructor call
+            modname = None
+            (ID, struct_id) = f
         (STRUCT,
          (MEMBER_NAMES, (LIST, member_names)),
          (STRUCT_MEMORY, (LIST, struct_memory))) = f_val
 
         # create our object memory - memory cells now have initial values
         # we use structure memory as an init template
         object_memory = struct_memory.copy()
         # create our object
         obj_ref = ('object',
                    ('struct-id', ('id', struct_id)),
+                   ('member-names', ('list', member_names)),
                    ('object-memory', ('list', object_memory)))
         # if the struct has an __init__ function call it on the object
         # NOTE: constructor functions do not have return values.
 
         if '__init__' in member_names:
             slot_ix = member_names.index('__init__')
             init_fval = struct_memory[slot_ix]
-            # calling a member function - push struct scope
+            # calling a member function
+            if modname:
+                orig_config = set_module_env(modname)
             handle_call(obj_ref,
                         init_fval,
                         arg_val,
                         f_name)
+            if modname:
+                set_config(orig_config)
         # the struct does not have an __init__ function but
         # we have a constructor call with args, e.g. Foo(1,2)
         # try to apply a default constructor by copying the
         # values from the arg list to the data slots of the object
         elif arg_val[0] != 'none':
             if arg_val[0] != 'tuple':
                 arg_array = [arg_val]
@@ -1744,27 +1689,14 @@
 
     for e in intuple:
         outtuple.append(walk(e))
 
     return ('tuple', outtuple)
 
 #########################################################################
-def escape_exp(node):
-
-    (ESCAPE, s) = node
-    assert_match(ESCAPE, 'escape')
-
-    global __retval__
-    __retval__ = ('none', None)
-
-    exec(s)
-
-    return __retval__
-
-#########################################################################
 def is_exp(node):
 
     (IS, term, pattern) = node
     assert_match(IS, 'is')
 
     term_val = walk(term)
 
@@ -1801,16 +1733,18 @@
     assert_match(IF_EXP, 'if-exp')
 
     # if expressions without an else clause are only allowed in
     # conditional patterns.
     if else_exp[0] == 'null':
         raise ValueError("if expressions need an 'else' clause")
 
-    (BOOLEAN, cond_val) = map2boolean(walk(cond_exp))
-
+    (cond_type, cond_val) = walk(cond_exp)
+    if cond_type != 'boolean':
+        raise ValueError("found '{}' expected 'boolean' in if expression"
+                        .format(cond_type))
     if cond_val:
         return walk(then_exp)
     else:
         return walk(else_exp)
 
 #########################################################################
 # NOTE: 'to-list' is not a semantic value and should never appear in
@@ -1883,238 +1817,118 @@
     assert_match(FUNCTION_EXP,'function-exp')
 
     return ('function-val',
             body_list,
             state.symbol_table.get_closure())
 
 #########################################################################
-# Named patterns - when walking a named pattern we are interpreting a
-# a pattern as a constructor - ignore the name
-def named_pattern_exp(node):
-
-    (NAMED_PATTERN, name, pattern) = node
-    assert_match(NAMED_PATTERN,'named-pattern')
-
-    return walk(pattern)
-
-#########################################################################
 def process_lineinfo(node):
 
     (LINEINFO, lineinfo_val) = node
     assert_match(LINEINFO, 'lineinfo')
 
-    if debugging:
-        debugger.set_lineinfo(lineinfo_val)
-
-    #lhh
-    #print("lineinfo: {}".format(lineinfo_val))
-
     state.lineinfo = lineinfo_val
 
 #########################################################################
-def deref_exp(node):
-
-    # deref operators are only meaningful during pattern matching
-    # it is an error to have the deref operator appear in an expression
-    raise ValueError("dereferencing patterns is not valid in expressions.")
-
-#########################################################################
-def constraint_exp(node):
-
-    # Constraint-only pattern matches should not exist where only an
-    # expression is expected. If we get here, we have come across this
-    # situation.
-    # A constraint-only pattern match AST cannot be walked and therefore
-    # we raise an error.
-    raise ValueError("a constraint pattern cannot be used as an expression.")
+def illegal_exp(_):
+    # we got here because we tried to use a non-trivial pattern as 
+    # constructors.
+    raise ValueError("not a valid expression")
 
 #########################################################################
 def set_ret_val(node):
     (SET_RET_VAL, exp) = node
     assert_match(SET_RET_VAL,'set-ret-val')
 
     global function_return_value
     val = walk(exp)
     function_return_value.pop()
     function_return_value.append(val)
 
-    # Debugger keeps track of the most recent
-    # return value
-    if debugging and val:
-        debugger.retval = term2string(val)
-
     return
 
 #########################################################################
-def walk_stmt_list(stmts, step_state=None):
-    # step_stae is a flag to tell us if we actually
-    # want to step through to the next line of the stmt
-    # list while debugging
-    
-    # We only want to do this if we're debugging
-    # and we've stepped through to this point or
-    # have continued to this point. Basically, this
-    # flag tells us if we've stepped or continued 
-    # into this function call, effectively telling
-    # the debugger to treat it as the top level
-
-    # This also allows us to keep loop execution
-    # control working with the debugger. Meaning
-    # we can do a "next" on the last line in a 
-    # loop and go back to the top as opposed to the
-    # next line after the loop
-    if step_state:
-        stepping = step_state
-    else:
-        stepping = debugger_has_stepped()
-
-    for s in stmts[1]:
-
-        if debugging:
-            # Set the debugger's info reflect new "top level"
-            if stepping: debugger.set_top_level(True)
-
-            # If we've hit a return and we're in continue-until-return
-            # mode, notify the debugger
-
-            # TODO: (OWM) get this working for implicit returns as well.
-            # This currently doesn't work because you can have an implicit
-            # return before a return statement. In this case, the return
-            # statement consumes the return behavior because it is the
-            # final statement in the stmt_list
-
-            # OWM -- This is still true but I'm not sure the fix for it
-            # nor if it should even be fixed
-
-            # The statement is a return the debugger is executing until return
-            # then notify the debugger
-            if debugging and \
-                debugger.exc['RETURN'] and s[0] == 'return':
-                
-                notify_debugger(at_return=True)
-            
-        walk(s)
+def clear_ret_val(node):
+    (CLEAR_RET_VAL,) = node
+    assert_match(CLEAR_RET_VAL, 'clear-ret-val')
+
+    global function_return_value    
+    # If we have no function return value, then append None    
+    if function_return_value != []:
+        function_return_value.pop()       
+    function_return_value.append(None)
+    return
 
 #########################################################################
 # walk
 #########################################################################
 def walk(node):
     # node format: (TYPE, [child1[, child2[, ...]]])
     type = node[0]
 
-    if type == 'clear-ret-val':
-        # implemented here instead of dictionary for efficiency reasons
-        global function_return_value    
-
-        # If we have no function return value, then append None    
-        if function_return_value != []:
-            function_return_value.pop()
-        
-        function_return_value.append(None)
-        return
-    elif type in dispatch_dict:
+    if type in dispatch_dict:
         node_function = dispatch_dict[type]
         return node_function(node)
     else:
         raise ValueError("feature '{}' not yet implemented".format(type))
 
 #########################################################################
-# walk_program
-#########################################################################
-def walk_program(node):
-    """
-    This function exists mostly as a performance
-    boost to unify. Running the program through
-    this function overrides the debugger wrapping
-    on unify.
-    """
-    global unify
-    unify = __unify
-
-    walk(node)
-
-#########################################################################
-# debug_walk
-#########################################################################
-def debug_walk(node, dbg):
-    """
-    This function allows us to keep the top-level distinction
-    at the program level.
-    """
-    global debugging, debugger, unify
-    debugging, debugger = (True, dbg)
-
-    unify = debug_unify
-
-    (LIST, inlist) = node
-
-    for e in inlist:
-        # We want to differentiate between top level and nested
-        # statements. So, we run the list of statements outright
-        # so we can control when we know we are at the top level
-        debugger.set_top_level(True)
-        walk(e)
-
 # a dictionary to associate tree nodes with node functions
 dispatch_dict = {
-    # Note: statement lists are now handled by separate functions outside
-    #       the walk function
     # statements - statements do not produce return values
+    'load-stmt'     : load_stmt,
+    'stmt-list'     : stmt_list,
     'lineinfo'      : process_lineinfo,
     'set-ret-val'   : set_ret_val,
+    'clear-ret-val' : clear_ret_val,
+    'exp-stmt'      : exp_stmt,
     'noop'          : lambda node : None,
-    'assert'        : assert_stmt,
     'unify'         : unify_stmt,
     'while'         : while_stmt,
     'loop'          : loop_stmt,
     'repeat'        : repeat_stmt,
     'for'           : for_stmt,
     'global'        : global_stmt,
     'return'        : return_stmt,
     'break'         : break_stmt,
+    'match'         : match_stmt,
     'if'            : if_stmt,
     'throw'         : throw_stmt,
     'try'           : try_stmt,
     'struct-def'    : struct_def_stmt,
-    'top-level-exp' : top_level_exp_stmt,
+    'module-def'    : module_def_stmt,  # this is part of the load statement
     # expressions - expressions do produce return values
     'list'          : list_exp,
-    'import_stmt'   : import_stmt,
     'tuple'         : tuple_exp,
     'to-list'       : to_list_exp,
     'head-tail'     : head_tail_exp,
     'raw-to-list'   : lambda node : walk(('to-list', node[1], node[2], node[3])),
     'raw-head-tail' : lambda node : walk(('head-tail', node[1], node[2])),
     'none'          : lambda node : node,
     'nil'           : lambda node : node,
     'function-exp'  : function_exp,
     'string'        : lambda node : node,
     'integer'       : lambda node : node,
     'real'          : lambda node : node,
     'boolean'       : lambda node : node,
     'object'        : lambda node : node,
-    'eval'          : eval_exp,
-    # pattern code should be treated like a constant if not ignore_pattern
-    'pattern'         : lambda node : walk(node[1]) if state.ignore_pattern else node,
-    # constraint patterns
-    'constraint'    : constraint_exp,
-    'typematch'     : constraint_exp,
+    'pattern'       : lambda node : node,
+    'scope'         : illegal_exp,
+    'typematch'     : illegal_exp,
     # type tag used in conjunction with escaped code in order to store
     # foreign objects in Asteroid data structures
     'foreign'       : lambda node : node,
     'id'            : lambda node : state.symbol_table.lookup_sym(node[1]),
     'apply'         : apply_exp,
     'index'         : index_exp,
-    'escape'        : escape_exp,
     'is'            : is_exp,
     'in'            : in_exp,
     'if-exp'        : if_exp,
-    'named-pattern' : named_pattern_exp,
     'member-function-val' : lambda node : node,
-    'deref'         : deref_exp,
+    'deref'         : illegal_exp,
 }
 
 ##############################################################################################
 # *** The Redundant Pattern Detector ***
 #
 # Evaluates the presence of redundant, or 'useless', pattern clauses in an Asteroid function:
 #
@@ -2154,24 +1968,24 @@
         # Process lineinfo
         lineinfo = bodies[ i ]
         process_lineinfo(lineinfo)
 
         #get the pattern with the higher level of precedence
         (BODY_H,(PTRN,ptrn_h),stmts_h) = bodies[i + 1]
         assert_match(BODY_H,'body')
-        assert_match(PTRN,'pattern')
+        assert_match(PTRN,'body-pattern')
 
         for j in range(i + 2, len(bodies), 2):
             lineinfo = bodies[ j ]
             process_lineinfo(lineinfo)
 
             #get the pattern with the lower level of precedence
             (BODY_L,(PTRN,ptrn_l),stmts_l) = bodies[j + 1]
             assert_match(BODY_L,'body')
-            assert_match(PTRN,'pattern')
+            assert_match(PTRN,'body-pattern')
 
             #Here we get line numbers in case we throw an error
             # we have to do a little 'tree walking' to get to the
             # line #, hence all the unpacking.
             (STMT_LIST,(LIST,LINE_LIST)) = stmts_l
             first_line_l = LINE_LIST[0]
             (LINE_INFO,location_l) = first_line_l
@@ -2188,186 +2002,7 @@
             try:                                #CHECK FOR CONFLICTION
                 unify( ptrn_l, ptrn_h , False )
             except PatternMatchFailed:          #NO CONFLICTION
                 pass
             else:                               #CONFLICTION
                 raise RedundantPatternFound( ptrn_h , ptrn_l , f_name, location_h, location_l )
 
-#######################################################################################
-# *** Asteroid Debugger (ADB) helper functions ***
-# 
-# message_explicit:
-#   The main messaging function for explicit mode. Operates in a similar way the
-#   string.format function does. Read the function's internal docstring for more
-#   information.
-# 
-# notify_debugger:
-#   Notifies the debugger of the current program position. If the debugger is
-#   accepting notifications at the time of call, the debugger will pause and
-#   run the interactive prompt.
-# 
-# notify_explicit:
-#   Similar to notify_debugger but only runs in explicit mode.
-# 
-# explicit_enabled:
-#   A simple helper function. Equivalent to `debugging and debugger.explicit_enabled`
-# 
-# decrease_tab_level:
-#   A simple helper function to manage debugger tab level decrementing.
-#
-# debugger_has_stepped::
-#   Helper function that returns if the debugger has stepped into a function
-#   body or other compound statement
-#
-# gen_t2s:
-#   A generator function used in place of term2string in message_explicit calls.
-#   This allows the computation to be deferred or completely ignored. Much like
-#   a function returning a lambda function
-#
-# debug_unify:
-#   A wrapper for the normal unify function that automatically decreases
-#   the tab level of failed pattern matches.
-#
-#######################################################################################
-def message_explicit(fmt_message, terms=None, level="primary", 
-    increase=False, decrease=False, notify=False):
-
-    """
-    Message explicit expects 1-3 main arguments
-
-    1. A string, which can be a format string or a normal string.
-    2. (Optional) A list of terms to express for a given format string
-    3. The message level (Defaults to primary)
-
-    Format terms can be either plain strings or generators. If a gener-
-    ator is supplied, this function will express it
-
-    fmt_message is a list of terms to be applied in the same
-    way as .format
-
-    --------------------------------------------------------------
-    This function also supports three other options that shorten
-    common development patterns.
-
-    increase: Increases the tab level after the message is written
-    decrease: Decreases the tab level before the message is written
-    notify: Makes a notify_explicit call to stop the debugger within
-            a pattern
-    """
-    from types import GeneratorType
-
-    if explicit_enabled():
-        if decrease: decrease_tab_level()
-
-        if not terms:
-            debugger.message_explicit(fmt_message, level)
-        else:
-            expressed_terms = []
-            for t in terms:
-                if isinstance(t, GeneratorType):
-                    expressed_terms.append(next(t))
-                else:
-                    expressed_terms.append(t)
-            
-            expressed_string = fmt_message.format(*expressed_terms)
-            debugger.message_explicit(expressed_string, level)
-        
-        if increase:    debugger.tab_level += 1
-        if notify:      notify_explicit()
-
-#########################################################################
-def notify_debugger(at_return=False):
-    """
-    If the debugger is accepting notifications at the time of call,
-    the debugger will pause and run the interactive prompt.
-    """
-    if debugging:
-        # We need to save the old lineinfo in case we go into a REPL
-        old_lineinfo = state.lineinfo
-
-        debugger.notify(at_return)
-
-        # Reset our lineinfo
-        state.lineinfo = old_lineinfo
-        debugger.set_lineinfo(state.lineinfo)
-
-#########################################################################
-def notify_explicit():
-    """
-    If the debugger is accepting notifications at the time of call and
-    the debugger is in explicit mode, the debugger will pause and run
-    the interactive prompt.
-    """
-    if debugging and explicit_enabled:
-        old_lineinfo = state.lineinfo
-        
-        debugger.notify_explicit()
-
-        # Reset our lineinfo
-        state.lineinfo = old_lineinfo
-        debugger.set_lineinfo(state.lineinfo)
-
-#########################################################################
-def explicit_enabled():
-    """
-    Helper function that returns the state
-    of explicit mode if debugging is enableds
-    """
-    return debugging and debugger.explicit_enabled
-
-#########################################################################
-def gen_t2s(node):
-    """
-    Generator function for term2string. This cuts down on
-    runtime as it defers term2string computations to when
-    they're actually needed.
-    """
-    yield term2string(node)
-
-#########################################################################
-def debugger_has_stepped():
-    """
-    Returns the step/continue state of the debugger
-    """
-    return debugging and \
-            (debugger.exc['STEP'] or debugger.exc['CONTINUE'])
-
-#########################################################################
-def decrease_tab_level():
-    """
-    Decreases/handles the debugger's tab level
-    """
-    if debugging:
-        debugger.tab_level = debugger.tab_level - 1
-
-        if debugger.tab_level < 0:
-            debugger.tab_level = 0
-
-#########################################################################
-def debug_unify(term, pattern, unifying = True):
-    '''
-    Proxy function for unify to make the debugger's formatting
-    work properly
-
-    OWM - This proxy function allows us to wrap unification
-    in an except block and catch when PatternMatchFailed exceptions
-    occur. In this situation, we need to decrease the tab level
-    and then re-raise the exception. Being able to "unravel"
-    tab levels is essential to making things look good.
-
-    In normal, non-debugging execution, this function is overridden
-    and not used.
-    '''
-
-    # Try to call the actual unify function
-    try:
-        return __unify(term, pattern, unifying)
-
-    # If there's a pattern match failed, decrease
-    # the tab level and reraise the exception
-    except PatternMatchFailed as r:
-        decrease_tab_level()
-        raise r
-
-    # If there's a normal exception, reraise it
-    except Exception as e:
-        raise e
```

### Comparing `asteroid-lang-1.1.4/asteroid_lang.egg-info/PKG-INFO` & `asteroid-lang-2.0.1/asteroid_lang.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,54 @@
 Metadata-Version: 2.1
 Name: asteroid-lang
-Version: 1.1.4
+Version: 2.0.1
 Summary: A modern, multi-paradigm programming language.
 Home-page: https://asteroid-lang.org
 Author: University of Rhode Island
 Author-email: lutzhamel@uri.edu
 Project-URL: Documentation, https://asteroid-lang.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/asteroid-lang/asteroid/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Asteroid
 Asteroid is a modern, multi-paradigm programming language that supports first-class patterns.  More details can
 be found at the website [asteroid-lang.org](https://asteroid-lang.org).
 Documentation on Asteroid can be found at
 [asteroid-lang.readthedocs.io](https://asteroid-lang.readthedocs.io).
 
+## New in Release 2.0.1
+
+* We now support the ASTEROIDPATH environment variable which is expected to have a colon seperated list of directories to search for user defined modules.
+
+* The logical operators 'and' and 'or' are now evaluated in short-circuit fashion.
+
+* Files loaded with the 'load' statement are now considered modules and work similarly to Python modules.
+
+* Added the 'toplevel' function which returns true if control is in the module originally loaded by the interpreter.
+
+* Added the match statement similar to the match statement in Python.
+
+* No longer supports type hierarchies for the primitive types.  The functions in the 'type' module are now considered builtins. The 'type' module itself has been eliminated.
+
+* The Minimal Asteroid Debugger (MAD) replaces ADB in this release.
+
+* The shorthand conditional pattern can now be applied to arbitrary patterns. E.g. The pattern 
+  ```
+  (a,b,c):(%integer,%integer,%integer)
+  ```
+  constrains the triple `(a,b,c)` to be a triple of integers.  The above shorthand conditional pattern is equivalent to the conditional pattern,
+  ```
+  (a,b,c) if (a,b,c) is (%integer,%integer,%integer)
+  ```
+  
 ## New in Release 1.1.4
 
 * Allows pattern constraint operator to map certain variables that a pattern 
   matched to be bound into the current scope.
 
 * Supports a new OS module.
```

### Comparing `asteroid-lang-1.1.4/asteroid_lang.egg-info/SOURCES.txt` & `asteroid-lang-2.0.1/asteroid_lang.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,38 +3,34 @@
 pyproject.toml
 setup.py
 asteroid/__init__.py
 asteroid/frontend.py
 asteroid/globals.py
 asteroid/interp.py
 asteroid/lex.py
+asteroid/mad.py
 asteroid/repl.py
 asteroid/state.py
 asteroid/support.py
 asteroid/symtab.py
 asteroid/version.py
 asteroid/walk.py
-asteroid/adb/__init__.py
-asteroid/adb/adb.py
-asteroid/adb/command.py
-asteroid/adb/help.py
-asteroid/adb/version.py
 asteroid/modules/bitwise.ast
 asteroid/modules/dataframe.ast
 asteroid/modules/hash.ast
 asteroid/modules/io.ast
 asteroid/modules/math.ast
 asteroid/modules/os.ast
+asteroid/modules/patterns.ast
 asteroid/modules/pick.ast
 asteroid/modules/prologue.ast
 asteroid/modules/random.ast
 asteroid/modules/set.ast
 asteroid/modules/sort.ast
 asteroid/modules/stream.ast
-asteroid/modules/type.ast
 asteroid/modules/util.ast
 asteroid/modules/vector.ast
 asteroid_lang.egg-info/PKG-INFO
 asteroid_lang.egg-info/SOURCES.txt
 asteroid_lang.egg-info/dependency_links.txt
 asteroid_lang.egg-info/entry_points.txt
 asteroid_lang.egg-info/requires.txt
```

### Comparing `asteroid-lang-1.1.4/setup.py` & `asteroid-lang-2.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+# when cutting releases make sure that PYTHONPATH points
+# to the root directory of the github repo
+
 from setuptools import setup, find_packages
+from asteroid.version import VERSION
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="asteroid-lang",
-    version="1.1.4",
+    version=VERSION,
     author="University of Rhode Island",
     author_email="lutzhamel@uri.edu",
     description="A modern, multi-paradigm programming language.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://asteroid-lang.org",
     project_urls={
@@ -24,14 +28,14 @@
         "matplotlib"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.10",
     entry_points={
         "console_scripts": [
             "asteroid = asteroid:main",
         ],
     },
 )
```

