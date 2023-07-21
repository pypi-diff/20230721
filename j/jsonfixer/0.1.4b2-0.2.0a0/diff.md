# Comparing `tmp/jsonfixer-0.1.4b2.tar.gz` & `tmp/jsonfixer-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsonfixer-0.1.4b2.tar", last modified: Tue Jun  4 14:56:35 2019, max compression
+gzip compressed data, was "jsonfixer-0.2.0a0.tar", last modified: Fri Jul 21 16:08:12 2023, max compression
```

## Comparing `jsonfixer-0.1.4b2.tar` & `jsonfixer-0.2.0a0.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxr-xr-x   0 tink       (501) staff       (20)        0 2019-06-04 14:56:35.000000 jsonfixer-0.1.4b2/
--rw-r--r--   0 tink       (501) staff       (20)     2984 2019-06-04 14:56:35.000000 jsonfixer-0.1.4b2/PKG-INFO
-drwxr-xr-x   0 tink       (501) staff       (20)        0 2019-06-04 14:56:35.000000 jsonfixer-0.1.4b2/half_json/
--rw-r--r--   0 tink       (501) staff       (20)        0 2019-05-29 15:56:09.000000 jsonfixer-0.1.4b2/half_json/__init__.py
--rw-r--r--   0 tink       (501) staff       (20)     6680 2019-06-04 14:51:01.000000 jsonfixer-0.1.4b2/half_json/core.py
--rw-r--r--   0 tink       (501) staff       (20)     4724 2019-06-03 15:38:07.000000 jsonfixer-0.1.4b2/half_json/json_util.py
--rw-r--r--   0 tink       (501) staff       (20)      792 2019-06-03 14:28:21.000000 jsonfixer-0.1.4b2/half_json/main.py
-drwxr-xr-x   0 tink       (501) staff       (20)        0 2019-06-04 14:56:35.000000 jsonfixer-0.1.4b2/jsonfixer.egg-info/
--rw-r--r--   0 tink       (501) staff       (20)     2984 2019-06-04 14:56:34.000000 jsonfixer-0.1.4b2/jsonfixer.egg-info/PKG-INFO
--rw-r--r--   0 tink       (501) staff       (20)      278 2019-06-04 14:56:34.000000 jsonfixer-0.1.4b2/jsonfixer.egg-info/SOURCES.txt
--rw-r--r--   0 tink       (501) staff       (20)       54 2019-06-04 14:56:34.000000 jsonfixer-0.1.4b2/jsonfixer.egg-info/entry_points.txt
--rw-r--r--   0 tink       (501) staff       (20)       10 2019-06-04 14:56:34.000000 jsonfixer-0.1.4b2/jsonfixer.egg-info/top_level.txt
--rw-r--r--   0 tink       (501) staff       (20)        1 2019-06-04 14:56:34.000000 jsonfixer-0.1.4b2/jsonfixer.egg-info/dependency_links.txt
--rw-r--r--   0 tink       (501) staff       (20)     1802 2019-06-04 14:54:50.000000 jsonfixer-0.1.4b2/README.md
--rw-r--r--   0 tink       (501) staff       (20)      863 2019-06-04 14:56:30.000000 jsonfixer-0.1.4b2/setup.py
--rw-r--r--   0 tink       (501) staff       (20)       38 2019-06-04 14:56:35.000000 jsonfixer-0.1.4b2/setup.cfg
--rw-r--r--   0 tink       (501) staff       (20)     1893 2019-06-04 14:55:53.000000 jsonfixer-0.1.4b2/README.rst
+-rw-r--r--   0        0        0     1065 2023-07-11 16:12:34.649467 jsonfixer-0.2.0a0/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-11 16:12:34.649755 jsonfixer-0.2.0a0/README.md
+-rw-r--r--   0        0        0        0 2023-07-11 16:12:34.652360 jsonfixer-0.2.0a0/half_json/__init__.py
+-rw-r--r--   0        0        0     7043 2023-07-21 15:03:46.258286 jsonfixer-0.2.0a0/half_json/core.py
+-rw-r--r--   0        0        0     4569 2023-07-21 14:52:19.559846 jsonfixer-0.2.0a0/half_json/json_util.py
+-rw-r--r--   0        0        0      792 2023-07-11 16:12:34.653092 jsonfixer-0.2.0a0/half_json/main.py
+-rw-r--r--   0        0        0      693 2023-07-21 16:08:12.778862 jsonfixer-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 16:12:34.653671 jsonfixer-0.2.0a0/tests/__init__.py
+-rw-r--r--   0        0        0     3055 2023-07-11 16:12:34.653890 jsonfixer-0.2.0a0/tests/test_cases.py
+-rw-r--r--   0        0        0      868 2023-07-11 16:12:34.654177 jsonfixer-0.2.0a0/tests/test_js.py
+-rw-r--r--   0        0        0    10078 2023-07-11 16:12:34.654576 jsonfixer-0.2.0a0/tests/test_miss.py
+-rw-r--r--   0        0        0     2146 2023-07-11 16:53:02.922306 jsonfixer-0.2.0a0/tests/test_stop.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 jsonfixer-0.2.0a0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jsonfixer-0.1.4b2/half_json/core.py` & `jsonfixer-0.2.0a0/half_json/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,41 +7,48 @@
 
 
 FixResult = namedtuple('FixResult', ['success', 'line', 'origin'])
 
 
 class JSONFixer(object):
 
-    def __init__(self, max_try=20, max_stack=3):
+    def __init__(self, max_try=20, max_stack=3, js_style=False):
         self._max_try = max_try
         self._max_stack = max_stack
+        self._js_style = js_style
 
     def fix(self, line):
         try:
             json.loads(line)
             return FixResult(success=True, line=line, origin=True)
-        except Exception:
+        except Exception as e:
             pass
 
         ok, new_line = self.fixwithtry(line)
         return FixResult(success=ok, line=new_line, origin=False)
 
     def fixwithtry(self, line):
         if self._max_try <= 0:
             return False, line
 
-        # record
         self.fix_stack = []
+        self.last_fix = None
+
         for i in range(self._max_try):
-            self.fix_stack.append(line)
 
-            ok, line = self.patch_line(line)
+            ok, new_line = self.patch_line(line)
             if ok:
-                break
+                return ok, new_line
+
+            self.last_fix = line != new_line
+            if self.last_fix:
+                self.fix_stack.insert(0, new_line)
+                self.fix_stack = self.fix_stack[:self._max_stack]
 
+            line = new_line
         return ok, line
 
     def patch_line(self, line):
         result = decode_line(line)
         if result.success:
             return True, line
 
@@ -60,125 +67,115 @@
         if err_info["error"] is None:
             return False, line
 
         error = err_info["error"]
         pos = err_info["pos"]
         nextchar = line[pos: pos + 1]
         lastchar = line[pos - 1: pos]
-        # TODO
-        # nextline = line[pos:]
-        # lastline = line[:pos]
+        nextline = line[pos:]
+        lastline = line[:pos]
 
-        # 02
         if error == errors.StringUnterminatedString:
-            # TODO resolve "abc --> "abc"
-            return False, insert_line(line, "\"", len(line))
-        # 06
+            return False, insert_line(line, '"', len(line))
         if error == errors.ObjectExceptKey:
-            # quick
             if nextchar == "":
-                return False, insert_line(line, "}", pos)
-            # miss key
+                return False, insert_line(line, '}', pos)
             if nextchar == ":":
-                return False, insert_line(line, "\"\"", pos)
-            # miss a pair
-            if nextchar == "," and lastchar in "{,":
+                return False, insert_line(line, '""', pos)
+            if lastchar in "{," and nextchar == ",":
                 return False, remove_line(line, pos, pos + 1)
-            # fix-error
             if lastchar == "," and nextchar == "}":
                 return False, remove_line(line, pos - 1, pos)
-            # {[ or {"a":1,[ --> "":[
             if nextchar in "[{":
-                return False, insert_line(line, "\"\":", pos)
-            # dosomething
-            # if lastchar == "{":
-            return False, insert_line(line, "\"", pos)
-        # 07
+                return False, insert_line(line, '"":', pos)
+            if self._js_style:
+                # find 'abc'
+                if nextchar == "'":
+                    nextline = remove_line(nextline, 0, 1)
+                    idx = nextline.find(':')
+                    if idx != -1 and idx != 0 and nextline[idx - 1] == "'":
+                        nextline = remove_line(nextline, idx - 1, idx)
+
+                    return False, lastline + nextline
+                # abc:1 --> "aabc":1
+                idx = nextline.find(':')
+                if idx != -1:
+                    line = lastline + insert_line(nextline, '"', idx)
+                    return False, insert_line(line, '"', pos)
+            # TODO process more case "
+            return False, insert_line(line, '"', pos)
         if error == errors.ObjectExceptColon:
-            return False, insert_line(line, ":", pos)
-        # 08
+            return False, insert_line(line, ':', pos)
         if error == errors.ObjectExceptObject:
-            # 08.1
             if nextchar == "":
-                # quick
                 if lastchar == "{":
                     return False, insert_line(line, "}", pos)
                 return False, insert_line(line, "null}", pos)
-            # 08.2
-            return False, insert_line(line, "\"", pos)
-        # 09
+            if nextchar == "}":
+                return False, insert_line(line, "null", pos)
+            # TODO guess more
+            return False, insert_line(line, '"', pos)
         if error == errors.ObjectExceptComma:
             if nextchar == "":
                 return False, insert_line(line, "}", pos)
             return False, insert_line(line, ",", pos)
-        # 11
         if error == errors.ArrayExceptObject:
-            # fix-error
-            if lastchar == "[" and nextchar == ",":
+            if nextchar == "," and lastchar == "[":
                 return False, remove_line(line, pos, pos + 1)
             if nextchar == ",":
                 return False, insert_line(line, "null", pos)
-            # 11.1
+            if nextchar == "]":
+                return False, remove_line(line, pos - 1, pos)
             if nextchar == "":
-                # quick
                 if lastchar == "[":
                     return False, insert_line(line, "]", pos)
                 return False, insert_line(line, "null]", pos)
-            # 11.2
+            # TODO guess more?
             return False, insert_line(line, "{", pos)
-            # 也许可以删掉前面的 , 补一个]
-        # 12
         if error == errors.ArrayExceptComma:
-            """
-            code:
-            end += 1
-            if nextchar == ']':
-                break
-            elif nextchar != ',':
-                raise ValueError(errmsg("Expecting ',' delimiter", s, end))
-            """
-            pos = pos - 1
-            nextchar = line[pos: pos + 1]
-            # 11.1
-            if nextchar == "":
+            if len(line) == pos:
                 return False, insert_line(line, "]", pos)
-            # 11.2
             return False, insert_line(line, ",", pos)
-        # unknonwn
+        # TODO unknonwn
         return False, line
 
-    def patch_stop_iteration(self, line):
+    def patch_stop_iteration(self, line: str):
+        # TODO clean
         # TODO fix
         # 1. }]
         # 2. ]}
         # 3. constans
+        # 4. -
         # 先 patch 完 {[]}
+        # TODO: process number
+        if line.startswith('-.'):
+            new_line = '-0.' + line[2:]
+            return False, new_line
+        # patch
         left = patch_lastest_left_object_and_array(line)
         if left == "":
-            last_notfix = (len(self.fix_stack) >= 2 and self.fix_stack[-2] == line)
-            if last_notfix:
+            if not self.last_fix:
                 left = patch_guess_left(line)
 
         new_line = left + line
         return False, new_line
 
     def patch_half_parse(self, line, err_info):
         obj, end = err_info
         nextline = line[end:].strip()
         nextchar = nextline[:1]
         left = patch_lastest_left_object_and_array(nextline)
         # ??
         if left == "":
             if nextchar == ",":
                 left = "["
-            elif nextchar == ":" and isinstance(obj, basestring):
+            elif nextchar == ":" and isinstance(obj, str):
                 left = "{"
             else:
-                last_notfix = (len(self.fix_stack) >= 2 and self.fix_stack[-2] == line)
-                if last_notfix:
+                if not self.last_fix:
                     left = patch_guess_left(nextline)
 
         new_line = left + line[:end] + nextline
         return False, new_line
 
 
 # TODO better name
@@ -192,16 +189,17 @@
             break
         if char in pairs:
             left = pairs[char] + left
 
     return left
 
 
+# TODO better name
 # TODO 改成 lastest
-# {}}]]]] --> { not [
+# TODO {}}]]]] --> { not [
 def patch_guess_left(line):
     miss_object = line.count('}') - line.count('{')
     miss_array = line.count(']') - line.count('[')
     if miss_object == miss_array == 0:
         if line[-1:] == '"' and line.count('"') == 1:
             return '"'
     elif miss_object >= miss_array:
```

### Comparing `jsonfixer-0.1.4b2/half_json/json_util.py` & `jsonfixer-0.2.0a0/half_json/json_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf8
 
-import re
 import json.decoder
 from collections import namedtuple
 from json.decoder import JSONDecoder
 from json.scanner import py_make_scanner
 from json.decoder import py_scanstring
+from json.decoder import JSONDecodeError as PyJSONDecodeError
 
 
 class JSONDecodeError(object):
 
     def __init__(self, parser, message):
         self.message = message
         self.parser = parser
@@ -22,19 +22,19 @@
 
     StringInvalidUXXXXEscape = JSONDecodeError("py_scanstring", "Invalid \\uXXXX escape")
     # 2 different case
     StringUnterminatedString = JSONDecodeError("py_scanstring", "Unterminated string starting at")
     StringInvalidControlCharacter = JSONDecodeError("py_scanstring", "Invalid control character")
     StringInvalidEscape = JSONDecodeError("py_scanstring", "Invalid \\escape")
     ObjectExceptColon = JSONDecodeError("JSONObject", "Expecting ':' delimiter")
-    ObjectExceptObject = JSONDecodeError("JSONObject", "Expecting object")
+    ObjectExceptObject = JSONDecodeError("JSONObject", "Expecting value")
     # 2 different case
     ObjectExceptKey = JSONDecodeError("JSONObject", "Expecting property name enclosed in double quotes")
     ObjectExceptComma = JSONDecodeError("JSONObject", "Expecting ',' delimiter")
-    ArrayExceptObject = JSONDecodeError("JSONArray", "Expecting object")
+    ArrayExceptObject = JSONDecodeError("JSONArray", "Expecting value")
     ArrayExceptComma = JSONDecodeError("JSONArray", "Expecting ',' delimiter")
 
     @classmethod
     def get_decode_error(cls, parser, message):
         err = JSONDecodeError(parser, message)
         for _, value in cls.__dict__.items():
             if isinstance(value, JSONDecodeError):
@@ -64,47 +64,38 @@
     11.2 同 08.2,无脑补一个{ 看看
     12 array 解析完前一个 object, 需要一个 ,
         这里 nextchar 既不是 ] 也不是, 代表这个 nextchar 的 end 也已经+1 了，所以减 2
     """
 
 
 def errmsg_inv(e):
-    assert isinstance(e, ValueError)
-
-    message = e.message
-    idx = message.rindex(':')
-    errmsg, left = message[:idx], message[idx + 1:]
-    numbers = re.compile(r'\d+').findall(left)
+    assert isinstance(e, PyJSONDecodeError)
     parser = e.__dict__.get("parser", "")
-
+    errmsg = e.msg
+    localerr = errors.get_decode_error(parser, errmsg)
     result = {
-        "error": errors.get_decode_error(parser, errmsg),
-        "lineno": int(numbers[0]),
-        "colno": int(numbers[1]),
+        "parsers": e.__dict__.get("parsers", []),
+        "error": localerr,
+        "lineno": e.lineno,
+        "colno": e.colno,
+        "pos": e.pos,
     }
-
-    if len(numbers) == 3:
-        result["pos"] = int(numbers[2])
-
-    if len(numbers) > 3:
-        result["endlineno"] = int(numbers[2])
-        result["endcolno"] = int(numbers[3])
-        result["pos"] = int(numbers[4])
-        result["end"] = int(numbers[5])
     return result
 
 
 def record_parser_name(parser):
-
     def new_parser(*args, **kwargs):
         try:
             return parser(*args, **kwargs)
         except Exception as e:
             if "parser" not in e.__dict__:
                 e.__dict__["parser"] = parser.__name__
+            if "parsers" not in e.__dict__:
+                e.__dict__["parsers"] = []
+            e.__dict__["parsers"].append(parser.__name__)
             raise e
     return new_parser
 
 
 def make_decoder():
     json.decoder.scanstring = record_parser_name(py_scanstring)
 
@@ -121,15 +112,14 @@
 decoder = make_decoder()
 
 
 DecodeResult = namedtuple('DecodeResult', ['success', 'exception', 'err_info'])
 
 
 def decode_line(line):
-    # 暂时只考虑 1 行的情况
     try:
         obj, end = decoder.scan_once(line, 0)
         ok = end == len(line)
         return DecodeResult(success=ok, exception=None, err_info=(obj, end))
     except StopIteration as e:
         return DecodeResult(success=False, exception=e, err_info=None)
     except ValueError as e:
```

### Comparing `jsonfixer-0.1.4b2/half_json/main.py` & `jsonfixer-0.2.0a0/half_json/main.py`

 * *Files identical despite different names*

### Comparing `jsonfixer-0.1.4b2/README.md` & `jsonfixer-0.2.0a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,102 @@
-## Usage
+Metadata-Version: 2.1
+Name: jsonfixer
+Version: 0.2.0a0
+Summary: jsonfixer: fix invalid json: broken-json / truncated-json.
+Author-Email: alingse <alingse@foxmail.com>
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Project-URL: Homepage, https://github.com/half-pie/half-json
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
+# Usage
 
 ```python
 In [1]: from half_json.core import JSONFixer
 
 In [2]: f = JSONFixer()
 
 In [3]: f.fix('[{')
 Out[3]: FixResult(success=True, line='[{}]', origin=False)
 
 In [4]: f.fix('{"a')
 Out[4]: FixResult(success=True, line='{"a":null}', origin=False)
+
+In [5]: f.fix('{"a":}')
+Out[5]: FixResult(success=True, line='{"a":null}', origin=False)
 ```
 
 ## 目标
 
-修复残破的 json
+fix invalid/broken/truncated json
 
-## 修复原理
+# 修复原理
 
-1. 根据异常提示来做一些操作, json 预期啥给啥
-2. 根据文本前后,删除一些 BadCase
+1. JSONDecoderError
+2. line context
 
 ## HitRatio
 
+根据 checks 里面的工具来衡量修改效果
+
+ABC : autogen --> broken --> check
+TSR : run test.sh show.sh ratio.sh
+
+### FixRatio
+
+仅判断 result.success == True
+
 ```bash
-./runtest.sh
-# 查看准确率
-seq 1 10|xargs -I {} ./runtest.sh|grep ratio: |awk '{t += $3; h+= $6}{print h/t}'|tail -1
-```
-1. 0.4269, 0.4287, 0.4303   # 实现完 12 条规则
-2. 0.5037, 0.5084, 0.5077   # string 的 " 补充在末尾
-3. 0.5259, 0.5224, 0.5187   # Array 需要 pos - 2
-4. 0.5433, 0.5311, 0.5381   # Array 细化一下 [, 的情况
-5. 0.7192, 0.7216, 0.7265   # 大改进, FIX 之前的 Bug( parser 被冲掉了)
-6. 0.7732, 0.7686, 0.7701   # case: {"a":1 --> 补充 }
-7. 0.60  , 0.58             # 去掉了空行
-8. 0.6971, 0.6969, 0.6984   # 增加处理 StopIteration
-9. 0.7428, 0.7383, 0.7427   # 增加处理 half parse
-10. 0.7617,0.7631, 0.7558   # 细化处理 half parse
-11. 0.7608,0.7612, 0.7650   # 添加从左处理
-12. 0.9817,0.9827, 0.9819   # 增加对字符串的处理
-13. 0.8314,0.8302, 0.8312   # 去掉对字符串的额外处理
+./runratio.sh fix
+```
+```
+1.  0.4269, 0.4287, 0.4303   # 实现完 12 条规则
+2.  0.5037, 0.5084, 0.5077   # string 的 " 补充在末尾
+3.  0.5259, 0.5224, 0.5187   # Array 需要 pos - 2
+4.  0.5433, 0.5311, 0.5381   # Array 细化一下 [, 的情况
+5.  0.7192, 0.7216, 0.7265   # 大改进, FIX 之前的 Bug( parser 被冲掉了)
+6.  0.7732, 0.7686, 0.7701   # case: {"a":1 --> 补充 }
+7.  0.60  , 0.58             # 去掉了空行
+8.  0.6971, 0.6969, 0.6984   # 增加处理 StopIteration
+9.  0.7428, 0.7383, 0.7427   # 增加处理 half parse
+10. 0.7617, 0.7631, 0.7558   # 细化处理 half parse
+11. 0.7608, 0.7612, 0.7650   # 添加从左处理
+12. 0.9817, 0.9827, 0.9819   # 增加对字符串的处理
+13. 0.8314, 0.8302, 0.8312   # 去掉对字符串的额外处理
+14. 0.95X                    # 已不可参考
+```
+
+### Real HitRatio
+
+判断 result.success == True
+
+并且解析后的 json 大体和原来一致(equal && dictdiffer)
+
+```bash
+./runratio.sh hit
+```
+```
+1. 0.5610, 0.5563, 0.5529   # origin
+2. 0.5593, 0.5532, 0.5587   # fix :} --> :null}
+```
+
+# TODO
 
 ## 目前的缺点 && 发现
 
 3. 数字的支持比较弱 --> -02 / 0. / .0
 4. 还不支持分支回溯 --> [{]
 7. 突然想到, 应该反思一下, 这个是一个fixer, 而不是一个将任何字符串都转为 json 的东西
    应该明确 JSONFixer 的能力范围, 对 runratio.sh 也应该比较前后两个的 json 相似程度。
    (听起来像无能者的辩白?)
-
-## TODO
+8. 也需要吧 parser 也做成 stack 这样可以解决 ["a] --> ["a"] 这样的 case
 
 1. 考虑分支回溯的方式来试探
 2. 解析缺失的 JSON 常量
+9.
 
 ## BadCase
 1. 1- --> {"1-": null}
```

