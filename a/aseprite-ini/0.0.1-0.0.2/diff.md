# Comparing `tmp/aseprite-ini-0.0.1.tar.gz` & `tmp/aseprite-ini-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aseprite-ini-0.0.1.tar", last modified: Sat Jul 15 20:37:03 2023, max compression
+gzip compressed data, was "aseprite-ini-0.0.2.tar", last modified: Fri Jul 21 05:10:20 2023, max compression
```

## Comparing `aseprite-ini-0.0.1.tar` & `aseprite-ini-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/src/aseprite_ini/
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/src/aseprite_ini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:10:20.941077 aseprite-ini-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 05:10:06.000000 aseprite-ini-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-21 05:10:20.941077 aseprite-ini-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-21 05:10:06.000000 aseprite-ini-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-21 05:10:06.000000 aseprite-ini-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:10:20.941077 aseprite-ini-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:10:20.941077 aseprite-ini-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:10:20.941077 aseprite-ini-0.0.2/src/aseprite_ini/
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-21 05:10:06.000000 aseprite-ini-0.0.2/src/aseprite_ini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:10:20.941077 aseprite-ini-0.0.2/src/aseprite_ini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-21 05:10:20.000000 aseprite-ini-0.0.2/src/aseprite_ini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-21 05:10:20.000000 aseprite-ini-0.0.2/src/aseprite_ini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:10:20.000000 aseprite-ini-0.0.2/src/aseprite_ini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-21 05:10:20.000000 aseprite-ini-0.0.2/src/aseprite_ini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 05:10:20.000000 aseprite-ini-0.0.2/src/aseprite_ini.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:10:20.941077 aseprite-ini-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-21 05:10:06.000000 aseprite-ini-0.0.2/tests/test_.py
```

### Comparing `aseprite-ini-0.0.1/LICENSE` & `aseprite-ini-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aseprite-ini-0.0.1/PKG-INFO` & `aseprite-ini-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aseprite-ini
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to parse Aseprite '.ini' format file.
 Author: Aseprite Quest
 Maintainer: Aseprite Quest
 License: MIT License
 Project-URL: homepage, https://github.com/aseprite-quest/aseprite-ini
 Project-URL: source, https://github.com/aseprite-quest/aseprite-ini
 Project-URL: issues, https://github.com/aseprite-quest/aseprite-ini/issues
```

### Comparing `aseprite-ini-0.0.1/README.md` & `aseprite-ini-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aseprite-ini-0.0.1/pyproject.toml` & `aseprite-ini-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aseprite-ini"
-version = "0.0.1"
+version = "0.0.2"
 description = "A tool to parse Aseprite '.ini' format file."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "Aseprite Quest" },
 ]
```

### Comparing `aseprite-ini-0.0.1/src/aseprite_ini/__init__.py` & `aseprite-ini-0.0.2/src/aseprite_ini/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,26 +63,39 @@
 
     @staticmethod
     def load(file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes]) -> 'Aseini':
         with open(file_path, 'r', encoding='utf-8') as file:
             return Aseini.decode_str(file.read())
 
     @staticmethod
-    def pull_strings(tag_name: str = 'main', lang: str = 'en') -> 'Aseini':
-        url = f'https://raw.githubusercontent.com/aseprite/aseprite/{tag_name}/data/strings/{lang}.ini'
+    def pull_strings_by_url(url: str) -> 'Aseini':
         response = requests.get(url)
         assert response.ok, url
         return Aseini.decode_str(response.text)
 
+    @staticmethod
+    def pull_strings(tag_name: str = 'main', lang: str = 'en') -> 'Aseini':
+        url = f'https://raw.githubusercontent.com/aseprite/aseprite/{tag_name}/data/strings/{lang}.ini'
+        return Aseini.pull_strings_by_url(url)
+
     def __init__(self, headers: list[str] = None):
         super().__init__()
         if headers is None:
             headers = list[str]()
         self.headers = headers
 
+    def patch(self, other: 'Aseini'):
+        for section_name, other_section in other.items():
+            if section_name in self:
+                section = self[section_name]
+            else:
+                section = dict[str, str]()
+                self[section_name] = section
+            section.update(other_section)
+
     def fallback(self, other: 'Aseini'):
         for section_name, other_section in other.items():
             if section_name in self:
                 section = self[section_name]
             else:
                 section = dict[str, str]()
                 self[section_name] = section
@@ -105,14 +118,16 @@
             source = self
 
         lines = list[str]()
         for header in self.headers:
             lines.append(f'# {header}')
         lines.append('')
         for section_name, source_section in source.items():
+            if len(source_section) <= 0:
+                continue
             lines.append(f'[{section_name}]')
             for key, source_value in source_section.items():
                 value = None
                 if section_name in self and key in self[section_name]:
                     value = self[section_name][key]
                 if source_value.startswith('<<<'):
                     if value is None:
```

### Comparing `aseprite-ini-0.0.1/src/aseprite_ini.egg-info/PKG-INFO` & `aseprite-ini-0.0.2/src/aseprite_ini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aseprite-ini
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to parse Aseprite '.ini' format file.
 Author: Aseprite Quest
 Maintainer: Aseprite Quest
 License: MIT License
 Project-URL: homepage, https://github.com/aseprite-quest/aseprite-ini
 Project-URL: source, https://github.com/aseprite-quest/aseprite-ini
 Project-URL: issues, https://github.com/aseprite-quest/aseprite-ini/issues
```

### Comparing `aseprite-ini-0.0.1/tests/test_.py` & `aseprite-ini-0.0.2/tests/test_.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,25 @@
     assert strings_en.headers[0] == 'Header 1'
     assert strings_en.headers[1] == 'Header 2'
     assert strings_en.headers[2] == 'Header 3'
     assert strings_en['game_mode']['title'] == 'Game Mode'
     assert strings_en['game_mode']['message'] == '<<<END\nThis is Game Mode.\nEND'
 
 
+def test_patch():
+    strings_en = Aseini.load(os.path.join(assets_dir, 'en.ini'))
+    strings_en.patch(Aseini.load(os.path.join(assets_dir, 'en-old.ini')))
+    assert len(strings_en.headers) == 3
+    assert strings_en.headers[0] == 'Header 1'
+    assert strings_en.headers[1] == 'Header 2'
+    assert strings_en.headers[2] == 'Header 3'
+    assert strings_en['game_mode']['title'] == 'Game Mode - Old'
+    assert strings_en['legacy_mode']['title'] == 'Legacy Mode - Old'
+
+
 def test_fallback():
     strings_en = Aseini.load(os.path.join(assets_dir, 'en.ini'))
     strings_en.fallback(Aseini.load(os.path.join(assets_dir, 'en-old.ini')))
     assert len(strings_en.headers) == 3
     assert strings_en.headers[0] == 'Header 1'
     assert strings_en.headers[1] == 'Header 2'
     assert strings_en.headers[2] == 'Header 3'
@@ -36,14 +47,15 @@
     translated, total = strings_zh.coverage(strings_en)
     assert total == 6
     assert translated == 4
 
 
 def test_encode_1():
     strings_en = Aseini.load(os.path.join(assets_dir, 'en.ini'))
+    strings_en['blank_section'] = {}
     text = strings_en.encode_str()
     text2 = read_str(os.path.join(assets_dir, 'en-clean.ini'))
     assert text == text2
 
 
 def test_encode_2():
     strings_en = Aseini.load(os.path.join(assets_dir, 'en.ini'))
```

