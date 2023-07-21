# Comparing `tmp/mypy-gpt-1.0.3.tar.gz` & `tmp/mypy-gpt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-gpt-1.0.3.tar", last modified: Fri Jul 21 19:20:09 2023, max compression
+gzip compressed data, was "mypy-gpt-1.0.4.tar", last modified: Fri Jul 21 20:02:09 2023, max compression
```

## Comparing `mypy-gpt-1.0.3.tar` & `mypy-gpt-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 19:20:09.369508 mypy-gpt-1.0.3/
--rw-rw-rw-   0        0        0    35184 2023-07-21 03:02:01.000000 mypy-gpt-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       24 2023-07-21 19:08:18.000000 mypy-gpt-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      498 2023-07-21 19:20:09.369508 mypy-gpt-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2181 2023-07-21 18:29:39.000000 mypy-gpt-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 19:20:09.356508 mypy-gpt-1.0.3/mypy_gpt/
--rw-rw-rw-   0        0        0        0 2023-07-21 18:55:16.000000 mypy-gpt-1.0.3/mypy_gpt/__init__.py
--rw-rw-rw-   0        0        0       33 2023-07-21 18:55:16.000000 mypy-gpt-1.0.3/mypy_gpt/__main__.py
--rw-rw-rw-   0        0        0     9926 2023-07-21 18:55:16.000000 mypy-gpt-1.0.3/mypy_gpt/mypygpt.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:20:09.368508 mypy-gpt-1.0.3/mypy_gpt.egg-info/
--rw-rw-rw-   0        0        0      498 2023-07-21 19:20:09.000000 mypy-gpt-1.0.3/mypy_gpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-21 19:20:09.000000 mypy-gpt-1.0.3/mypy_gpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 19:20:09.000000 mypy-gpt-1.0.3/mypy_gpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-21 19:20:09.000000 mypy-gpt-1.0.3/mypy_gpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 19:20:09.000000 mypy-gpt-1.0.3/mypy_gpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       36 2023-07-21 18:56:44.000000 mypy-gpt-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 19:20:09.369508 mypy-gpt-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-07-21 19:19:23.000000 mypy-gpt-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:02:09.334572 mypy-gpt-1.0.4/
+-rw-rw-rw-   0        0        0    35184 2023-07-21 03:02:01.000000 mypy-gpt-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-07-21 19:08:18.000000 mypy-gpt-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      498 2023-07-21 20:02:09.334572 mypy-gpt-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1234 2023-07-21 20:00:17.000000 mypy-gpt-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 20:02:09.325572 mypy-gpt-1.0.4/mypy_gpt/
+-rw-rw-rw-   0        0        0        0 2023-07-21 18:55:16.000000 mypy-gpt-1.0.4/mypy_gpt/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-07-21 18:55:16.000000 mypy-gpt-1.0.4/mypy_gpt/__main__.py
+-rw-rw-rw-   0        0        0    10086 2023-07-21 20:00:17.000000 mypy-gpt-1.0.4/mypy_gpt/mypygpt.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:02:09.333571 mypy-gpt-1.0.4/mypy_gpt.egg-info/
+-rw-rw-rw-   0        0        0      498 2023-07-21 20:02:09.000000 mypy-gpt-1.0.4/mypy_gpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-21 20:02:09.000000 mypy-gpt-1.0.4/mypy_gpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:02:09.000000 mypy-gpt-1.0.4/mypy_gpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-21 20:02:09.000000 mypy-gpt-1.0.4/mypy_gpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 20:02:09.000000 mypy-gpt-1.0.4/mypy_gpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       36 2023-07-21 18:56:44.000000 mypy-gpt-1.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 20:02:09.334572 mypy-gpt-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-07-21 20:01:20.000000 mypy-gpt-1.0.4/setup.py
```

### Comparing `mypy-gpt-1.0.3/LICENSE` & `mypy-gpt-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-gpt-1.0.3/mypy_gpt/mypygpt.py` & `mypy-gpt-1.0.4/mypy_gpt/mypygpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 # Press Shift+F10 to execute it or replace it with your code.
 # Press Double Shift to search everywhere for classes, files, tool windows, actions, and settings.
 import pandas
 import guidance
 import re
 import difflib
 import logging
-
+DEFAULTS_DIFF_FILE="suggestion.diff"
 logger=logging.getLogger('mypygpt')
 
 DEFAULT_MODEL = "gpt-3.5-turbo-16k"
 
 MYPYARGS = '--disallow-untyped-defs'
 
 older_path = r"c:\gitproj\Auto-GPT"
 DEFAULT_TOKENS =3600
 DEFAULT_TOKENS_PER_FIX =400
 import subprocess
-
 import argparse
 def run_mypy(file, mypy_args, mypy_path,proj_path):
     # Construct the mypy command
     command = [mypy_path] +mypy_args.split() + [file]
     # Run mypy command and capture the output
     result = subprocess.run(command, capture_output=True, text=True,cwd=os.path.abspath(proj_path))
     # Print the output
@@ -129,18 +128,20 @@
             elif line.startswith('^'):
                 yield Fore.BLUE + line + Fore.RESET
             elif line.startswith('@@'):
                 yield Fore.BLUE + line[:line.rindex('@@')+2] + Fore.RESET
             else:
                 yield line
 
-    diffres =list(difflib.unified_diff(original_content.split('\n'), new_content.split('\n'), fromfile=path, tofile=path+"b"))
-    return '\n'.join(color_diff(diffres)),'\n'.join(diffres)
+    diffres =list(difflib.unified_diff(original_content.split('\n'), new_content.split('\n'), fromfile=path, tofile=path+"b",lineterm=''))
+    return os.linesep.join(color_diff(diffres)),os.linesep.join(diffres)
 
 def main_internal(args):
+    if args.diff_file != DEFAULTS_DIFF_FILE:
+        args.store_diff = True
     logger.setLevel(logging.DEBUG if args.debug else logging.INFO)
     if 'OPEN_AI_KEY' not in os.environ:
         logger.error('OPEN_AI_KEY not set')
         return
     logger.info("mypy output:")
 
     errors = get_errors_from_mypy(args)
@@ -173,15 +174,15 @@
             logger.error('cant continue')
             return
     colored_diff,diff= generate_diff(original_content, new_content,args.file.replace("\\",'/'))
 
     if args.store_file:
         open(args.new_file_path, 'wt').write(new_content)
     if args.store_diff:
-        open(args.diff_file_path, 'wt').write(diff)
+        open(args.diff_file, 'wt').write(diff)
 
 
     with NamedTemporaryFile(mode='w', delete=False) as f:
         f.write(new_content)
         logger.info('output from mypy after applying the fixes:')
         errors=get_errors_from_mypy(args,override_file=f.name)
     print(colored_diff)
@@ -226,18 +227,18 @@
     # Add the arguments
     parser.add_argument('file', help='Python file to run mypy on')
     parser.add_argument('mypy_args', nargs='?', default=MYPYARGS, help='Additional options for mypy')
     parser.add_argument('--mypy_path', default='mypy', help='Path to mypy executable (default: "mypy")')
     parser.add_argument('--error_categories', action='store', help='Type of errors to process')
     parser.add_argument('--max_errors', action='store', type=int, default=10, help='Max number of errors to process')
     parser.add_argument('--proj-path', default='.', help='Path to project')
-    parser.add_argument('--diff_file', action='store', default='suggestion.diff', help='Store diff in file')
+    parser.add_argument('--diff_file', action='store', default=DEFAULTS_DIFF_FILE, help='Store diff in file')
     parser.add_argument('--new_file_path', action='store', default='suggestion.py', help='Store new content in file')
     parser.add_argument('--store_file', action='store_true', default=False, help='Store new content in file')
-    parser.add_argument('--store_diff', action='store_true', default=False, help='Store diff in a file')
+    parser.add_argument('--store-diff', action='store_true', default=False, help='Store diff in a file. by default suggestion.diff')
 
     parser.add_argument('--dont-ask', action='store_true', default=False,
                         help='Dont ask if to apply to changes. Useful for generting diff')
     parser.add_argument('--model', default=DEFAULT_MODEL, help='Openai model to use')
     parser.add_argument('--max_tokens_per_fix', default=DEFAULT_TOKENS_PER_FIX, help='tokens to use for fixes')
     parser.add_argument('--max_tokens_for_file', default=DEFAULT_TOKENS, help='tokens to use for file')
     parser.add_argument('--dont_recheck', action='store_true', default=False,
```

### Comparing `mypy-gpt-1.0.3/setup.py` & `mypy-gpt-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         str(requirement)
         for requirement
         in pkg_resources.parse_requirements(requirements_txt)
     ]
 
 setup(
     name='mypy-gpt',
-    version='1.0.3',
+    version='1.0.4',
     packages=['mypy_gpt'],
     url='https://github.com/eyalk11/mypy-gpt',
     license=' AGPL-3.0 license',
     author='ekarni',
     author_email='',
     description=desc,
     long_description=long_desc,
```

