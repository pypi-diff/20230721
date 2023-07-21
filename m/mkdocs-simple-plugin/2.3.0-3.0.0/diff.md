# Comparing `tmp/mkdocs_simple_plugin-2.3.0.tar.gz` & `tmp/mkdocs_simple_plugin-3.0.0.tar.gz`

## Comparing `mkdocs_simple_plugin-2.3.0.tar` & `mkdocs_simple_plugin-3.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/.pages
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/README.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/__init__.py
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/generator.py
--rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/plugin.py
--rw-r--r--   0        0        0    16281 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/semiliterate.py
--rw-r--r--   0        0        0     8717 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/simple.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/LICENSE
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/README.md
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/.pages
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/README.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/__init__.py
+-rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/generator.py
+-rw-r--r--   0        0        0    13548 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/plugin.py
+-rw-r--r--   0        0        0    16520 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/semiliterate.py
+-rw-r--r--   0        0        0     9429 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/simple.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/README.md
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 mkdocs_simple_plugin-3.0.0/PKG-INFO
```

### Comparing `mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/README.md` & `mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-# Developing
+# Package Guide
 
 ## Prerequisites
 
 {% include "setup.snippet" %}
 
 
 ## Building
 
 {% include "build.snippet" %}
 
 ## Testing
  
-{% include "tests/test.snippet" %}
+{% include "tests/linters.snippet" %}
+
+{% include "tests/unit_tests.snippet" %}
+
+{% include "tests/integration_tests.snippet" %}
+
+{% include "tests/local_tests.snippet" %}
 
 ## VSCode
 
 Included in this package is a VSCode workspace and development container.  See [how I develop with VSCode and Docker](https://allisonthackston.com/articles/docker-development.html) and [how I use VSCode tasks](https://allisonthackston.com/articles/vscode-tasks.html).
 
 ## Packaging
```

### Comparing `mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/generator.py` & `mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     :command: main
     :prog_name: mkdocs_simple_gen
     :depth: 2
 
 """
 import os
 import tempfile
+import sys
 
 import click
 import yaml
 
 
 def default_config():
     """Get default configuration for mkdocs.yml file."""
@@ -116,15 +117,16 @@
                 #  Ensure docs directory exists.
                 print("making docs_dir %s", config["docs_dir"])
                 os.makedirs(config["docs_dir"], exist_ok=True)
 
         except yaml.YAMLError as exc:
             print(exc)
             raise
-    write_config(config_file, config)
+    if config != local_config:
+        write_config(config_file, config)
     return config
 
 
 @click.command()
 @click.option("--config-file", default="mkdocs.yml",
               help="Set the configuration file.")
 @click.option('--build/--no-build', default=False,
@@ -142,8 +144,8 @@
         os.system("mkdocs serve " + " ".join(args))
 
 
 if __name__ == "__main__":
     # pylint doesn't know how to parse the click decorators,
     # so disable no-value-for-parameter on main
     # pylint: disable=no-value-for-parameter
-    main(['--help'])
+    main(sys.argv)
```

### Comparing `mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/plugin.py` & `mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,20 +84,20 @@
 
 ```bash
 mkdocs serve
 ```
 
 """
 import os
-import shutil
 import tempfile
 import time
 import yaml
 
 
+from mkdocs.structure.files import Files, File
 from mkdocs.plugins import BasePlugin
 from mkdocs.config import config_options
 from mkdocs import config as mkdocs_config
 from mkdocs import utils
 
 from mkdocs_simple_plugin.simple import Simple
 
@@ -281,64 +281,87 @@
             allow_unicode=True,
             encoding=None)
 
         # Read previous config first so updates don't get overwritten
         config_site_dir = get_config_site_dir(config.config_file_path)
 
         # Set the build docs dir to tmp location if not set by user
-        if not self.config['build_docs_dir']:
+        if not self.config['build_docs_dir'] and self.config['merge_docs_dir']:
+            self.config['build_docs_dir'] = config['docs_dir']
+        else:
             self.config['build_docs_dir'] = self.tmp_build_docs_dir
 
         utils.log.info(
             "mkdocs-simple-plugin: build_docs_dir: %s",
             self.config['build_docs_dir'])
 
-        # Clean out build folder on config
-        if not self.dirty:
-            shutil.rmtree(self.config['build_docs_dir'], ignore_errors=True)
+        # Create build directory
         os.makedirs(self.config['build_docs_dir'], exist_ok=True)
         # Save original docs directory location
         self.orig_docs_dir = config['docs_dir']
-        # Update the docs_dir with our temporary one
-        config['docs_dir'] = self.config['build_docs_dir']
+        # Update the docs_dir with our temporary one if not merging
+        if not self.config['merge_docs_dir']:
+            config['docs_dir'] = self.config['build_docs_dir']
         # Add all markdown extensions to include list
         self.config['include_extensions'] = list(utils.markdown_extensions) + \
             self.config['include_extensions']
 
         # Always ignore the output paths
         self.config["ignore_paths"] = [
-            config_site_dir,
-            config['site_dir'],
-            self.config['build_docs_dir']]
+            os.path.abspath(config_site_dir),
+            os.path.abspath(config['site_dir']),
+            os.path.abspath(self.config['build_docs_dir'])]
+        if self.config['merge_docs_dir']:
+            self.config["ignore_paths"].append(
+                os.path.abspath(config['docs_dir']))
         return config
 
-    def on_pre_build(self, *, config):
-        """Build documentation directory with files according to settings."""
+    def on_files(self, files: Files, *, config):
+        """Update files based on plugin settings."""
         # Configure simple
         simple = Simple(**self.config)
 
-        # Merge docs
-        if self.config["merge_docs_dir"]:
-            simple.merge_docs(self.orig_docs_dir, self.dirty)
-        # Copy all of the valid doc files into build_docs_dir
         # Save paths to add to watch if serving
         self.paths = simple.build_docs(self.dirty, self.last_build_time)
         self.last_build_time = time.time()
 
+        if not self.config["merge_docs_dir"]:
+            # If not merging, remove files that are from the docs dir
+            # pylint: disable=protected-access
+            for file in files._files[:]:
+                if file.abs_src_path.startswith(
+                        os.path.abspath(config['docs_dir'])):
+                    files.remove(file)
+
+        dedupe_files = {}
+        for file in files:
+            dedupe_files[file.abs_dest_path] = file
+
+        for path in self.paths:
+            file = File(
+                src_dir=os.path.abspath(path.output_root),
+                path=path.output_relpath,
+                dest_dir=config.site_dir,
+                use_directory_urls=config["use_directory_urls"]
+            )
+            if file.abs_dest_path in dedupe_files:
+                files.remove(dedupe_files[file.abs_dest_path])
+            files.append(file)
+        return files
+
     def on_serve(self, server, *, config, builder):
         """Add files to watch server."""
-        # watch the original docs/ directory
-        if os.path.exists(self.orig_docs_dir):
-            server.watch(self.orig_docs_dir)
         # don't watch the build directory
-        server.unwatch(self.config["build_docs_dir"])
+        # pylint: disable=protected-access
+        if self.config["build_docs_dir"] in server._watched_paths:
+            server.unwatch(self.config["build_docs_dir"])
 
         # watch all the doc files
         for path in self.paths:
-            server.watch(path)
+            server.watch(path.input_path)
 
         return server
 
 
 def get_config_site_dir(config_file_path: str) -> str:
     """Get configuration directory from mkdocs.yml file.
```

### Comparing `mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/semiliterate.py` & `mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/semiliterate.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         #
         # ```
         # stop=<regex>
         # ```
         self._stop_pattern = re.compile(r"stop=[\"']?([^\"']*)[\"']?")
         # /md
 
-    def setup(self, line: str):
+    def setup(self, line: str) -> None:
         """Process input parameters."""
         self._filename = None
         file_match = get_match(self._filename_pattern, line)
         if file_match and file_match.lastindex:
             self._filename = file_match[file_match.lastindex]
 
         self._trim = 0
@@ -200,43 +200,42 @@
 
     def __init__(self, directory: str, name: str):
         """Initialize with a directory and file name."""
         self.file_directory = directory
         self.file_name = name
         self.file_object = None
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         """Check equality if directory and names are the same."""
         return self.file_directory == other.file_directory \
             and self.file_name == other.file_name
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Return the full file path as a string."""
         return os.path.join(self.file_directory, self.file_name)
 
-    def write(self, arg: str):
+    def write(self, arg: str) -> None:
         """Create and write the file, only if not empty."""
         if not arg:
             return
         if self.file_object is None:
             filename = os.path.join(self.file_directory, self.file_name)
             os.makedirs(self.file_directory, exist_ok=True)
             self.file_object = open(filename, 'w+')
         self.file_object.write(arg)
 
-    def close(self):
+    def close(self) -> str:
         """Finish the file."""
         if self.file_object is not None:
-            utils.log.info(
-                "        ... extracted %s",
-                os.path.join(
-                    self.file_directory,
-                    self.file_name))
+            file = os.path.join(self.file_directory, self.file_name)
+            utils.log.debug("        ... extracted %s", file)
             self.file_object.close()
             self.file_object = None
+            return file
+        return None
 
 
 class StreamExtract:
     """Extract documentation portions of files to an output stream."""
 
     def __init__(
             self,
@@ -248,19 +247,20 @@
         """Initialize StreamExtract with input and output streams."""
         self.input_stream = input_stream
         self.default_stream = output_stream
         self.output_stream = output_stream
         self.terminate = terminate
         self.patterns = patterns
         self.wrote_something = False
+        self.output_files = []
         self.streams = {
             output_stream.file_name: output_stream
         }
 
-    def transcribe(self, text: str):
+    def transcribe(self, text: str) -> None:
         """Write some text and record if something was written."""
         self.output_stream.write(text)
         if text:
             self.wrote_something = True
 
     def try_extract_match(
             self,
@@ -273,39 +273,41 @@
         """
         if not match_object:
             return False
         if match_object.lastindex and emit_last:
             self.transcribe(get_line(match_object[match_object.lastindex]))
         return True
 
-    def close(self) -> bool:
+    def close(self) -> list:
         """Returns true if something was written"""
-        self.output_stream.close()
-        return self.wrote_something
+        file = self.output_stream.close()
+        if file and self.wrote_something:
+            self.output_files.append(file)
+        return self.output_files
 
-    def set_output_file(self, filename: str):
+    def set_output_file(self, filename: str) -> None:
         """Set output stream from filename."""
         output_stream = self.output_stream
         if filename:
             # If we've opened this file before, re-use its stream.
             if filename in self.streams:
                 return self.set_output_stream(self.streams[filename])
             # Otherwise, make a new one and save it to the list.
             output_stream = LazyFile(
                 self.output_stream.file_directory, filename)
             self.streams[filename] = output_stream
         self.set_output_stream(output_stream)
 
-    def set_output_stream(self, stream: LazyFile):
+    def set_output_stream(self, stream: LazyFile) -> None:
         """Set the output stream."""
         if self.output_stream != stream:
             self.close()
             self.output_stream = stream
 
-    def extract(self, **kwargs) -> bool:
+    def extract(self, **kwargs) -> list:
         """Extract from file with semiliterate configuration.
 
         Invoke this method to perform the extraction. Returns true if
         any text is actually extracted, false otherwise.
         """
         active_pattern = None if self.patterns else ExtractionPattern()
         for pattern in self.patterns:
@@ -333,15 +335,15 @@
                 active_pattern = None
                 self.set_output_stream(self.default_stream)
                 continue
             # Extract all other lines in the normal way:
             self.extract_line(line, active_pattern)
         return self.close()
 
-    def extract_line(self, line: str, extraction_pattern: re.Pattern):
+    def extract_line(self, line: str, extraction_pattern: re.Pattern) -> None:
         """Copy line to the output stream, applying specified replacements."""
         line = get_line(extraction_pattern.replace_line(line))
         self.transcribe(line)
 
 
 class Semiliterate:
     """Extract documentation from source files using regex settings."""
@@ -416,34 +418,35 @@
         return None
 
     def try_extraction(
             self,
             from_directory: str,
             from_file: str,
             destination_directory: str,
-            **kwargs) -> bool:
+            **kwargs) -> list:
         """Try to extract documentation from file with name.
 
         Returns True if extraction was successful.
         """
         to_file = self.filename_match(from_file)
         if not to_file:
-            return False
+            return []
         from_file_path = os.path.join(from_directory, from_file)
         try:
             with open(from_file_path) as original_file:
                 utils.log.debug(
-                    "mkdocs-simple-plugin: Scanning %s...", from_file)
+                    "mkdocs-simple-plugin: Scanning %s...", from_file_path)
                 extraction = StreamExtract(
                     input_stream=original_file,
                     output_stream=LazyFile(destination_directory, to_file),
                     terminate=self.terminate,
                     patterns=self.patterns,
                     **kwargs)
                 return extraction.extract()
         except (UnicodeDecodeError) as error:
-            utils.log.info("mkdocs-simple-plugin: skipping  %s\n %s",
-                           from_file_path, str(error))
+            utils.log.info("mkdocs-simple-plugin: Skipped  %s", from_file_path)
+            utils.log.debug(
+                "mkdocs-simple-plugin: Error details: %s", str(error))
         except (OSError, IOError) as error:
             utils.log.error("mkdocs-simple-plugin: could not build %s\n %s",
                             from_file_path, str(error))
-        return False
+        return []
```

### Comparing `mkdocs_simple_plugin-2.3.0/mkdocs_simple_plugin/simple.py` & `mkdocs_simple_plugin-3.0.0/mkdocs_simple_plugin/simple.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 """Simple module handles document extraction from source files."""
 import os
 import fnmatch
 import stat
 import pathlib
 
 from shutil import copy2 as copy
+from dataclasses import dataclass
 
 from mkdocs import utils
 from mkdocs_simple_plugin.semiliterate import Semiliterate
 
 
+@dataclass
+class SimplePath:
+    """Paths processed by Simple."""
+    output_root: str
+    output_relpath: str
+    input_path: str
+
+
 class Simple():
     """Mkdocs Simple Plugin"""
 
     # pylint: disable=too-many-arguments
     # pylint: disable=too-many-instance-attributes
     def __init__(
             self,
@@ -81,15 +90,15 @@
     def is_path_ignored(self, path: str = None) -> bool:
         """Check if path should be ignored."""
         path = os.path.normpath(path)
         base_path = os.path.dirname(path)
 
         # Check if its an internally required ignore path
         for ignored in self.ignore_paths:
-            if ignored in os.path.abspath(path):
+            if os.path.abspath(path).startswith(ignored):
                 return True
 
         # Update ignore patterns from .mkdocsignore file
         mkdocsignore = os.path.join(base_path, ".mkdocsignore")
         if os.path.exists(mkdocsignore):
             ignore_list = []
             with open(mkdocsignore, "r") as txt_file:
@@ -175,48 +184,64 @@
                     os.path.getmtime(file) <= last_build_time):
                 continue
             from_dir = os.path.dirname(file)
             name = os.path.basename(file)
             build_prefix = os.path.normpath(
                 os.path.join(self.build_dir, from_dir))
 
-            if (self.try_copy_file(from_dir, name, build_prefix) or
-                    self.try_extract(from_dir, name, build_prefix)):
-                paths.append(file)
+            copy_paths = self.try_copy_file(from_dir, name, build_prefix)
+            if copy_paths:
+                paths.append(
+                    SimplePath(
+                        output_root=".",
+                        output_relpath=os.path.relpath(path=file, start="."),
+                        input_path=file)
+                )
+                utils.log.info("mkdocs-simple-plugin: Added %s", file)
+                continue
+
+            extracted_paths = self.try_extract(from_dir, name, build_prefix)
+            for path in extracted_paths:
+                paths.append(
+                    SimplePath(
+                        output_root=self.build_dir,
+                        output_relpath=os.path.relpath(
+                            path=path,
+                            start=self.build_dir),
+                        input_path=file))
+                utils.log.info(
+                    "mkdocs-simple-plugin: Added %s->%s", file, path)
+            if extracted_paths:
+                continue
+
         return paths
 
-    def try_extract(self, from_dir: str, name: str, to_dir: str) -> bool:
+    def try_extract(self, from_dir: str, name: str, to_dir: str) -> list:
         """Extract content from file into destination.
 
         Returns the name of the file extracted if extractable.
         """
         # Check if it's hidden
         path = os.path.join(from_dir, name)
         if not self.should_extract_file(path):
-            return False
+            return []
         for item in self.semiliterate:
-            if item.try_extraction(from_dir, name, to_dir):
-                return True
+            paths = item.try_extraction(from_dir, name, to_dir)
+            if paths:
+                return paths
 
-        return False
+        return []
 
-    def try_copy_file(self, from_dir: str, name: str, to_dir: str) -> bool:
+    def try_copy_file(self, from_dir: str, name: str, to_dir: str) -> list:
         """Copy file with the same name to a new directory.
 
         Returns true if file copied.
         """
         original = os.path.join(from_dir, name)
-        new_file = os.path.join(to_dir, name)
+        destination = os.path.join(to_dir, name)
 
         if not self.should_copy_file(os.path.join(from_dir, name)):
-            return False
-        try:
-            os.makedirs(to_dir, exist_ok=True)
-            copy(original, new_file)
-            utils.log.info("mkdocs-simple-plugin: %s --> %s",
-                           original, new_file)
-            return True
-        except (OSError, IOError, UnicodeDecodeError) as error:
-            utils.log.warning(
-                "mkdocs-simple-plugin: %s.. skipping %s",
-                error, original)
-        return False
+            return []
+
+        os.makedirs(to_dir, exist_ok=True)
+        copy(original, destination)
+        return [original]
```

### Comparing `mkdocs_simple_plugin-2.3.0/LICENSE` & `mkdocs_simple_plugin-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_simple_plugin-2.3.0/README.md` & `mkdocs_simple_plugin-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_simple_plugin-2.3.0/pyproject.toml` & `mkdocs_simple_plugin-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs_simple_plugin-2.3.0/PKG-INFO` & `mkdocs_simple_plugin-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-simple-plugin
-Version: 2.3.0
+Version: 3.0.0
 Summary: Plugin for adding simple wiki site creation from markdown files interspersed within your code with MkDocs.
 Project-URL: Documentation, http://www.althack.dev/mkdocs-simple-plugin
 Project-URL: Homepage, http://www.althack.dev/mkdocs-simple-plugin
 Project-URL: Issues, https://github.com/athackst/mkdocs-simple-plugin/issues
 Project-URL: Source Code, https://github.com/athackst/mkdocs-simple-plugin
 Author-email: Allison Thackston <allison@allisonthackston.com>
 License-Expression: Apache-2.0
```

