# Comparing `tmp/nonebot-plugin-sayoroll-0.4.0.tar.gz` & `tmp/nonebot-plugin-sayoroll-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sayoroll-0.4.0.tar", last modified: Thu Jul 20 07:47:45 2023, max compression
+gzip compressed data, was "nonebot-plugin-sayoroll-0.4.1.tar", last modified: Thu Jul 20 07:55:56 2023, max compression
```

## Comparing `nonebot-plugin-sayoroll-0.4.0.tar` & `nonebot-plugin-sayoroll-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 07:47:45.937476 nonebot-plugin-sayoroll-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-20 07:47:32.000000 nonebot-plugin-sayoroll-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-20 07:47:45.937476 nonebot-plugin-sayoroll-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-07-20 07:47:32.000000 nonebot-plugin-sayoroll-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 07:47:45.933476 nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll/
--rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-07-20 07:47:32.000000 nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 07:47:45.937476 nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-20 07:47:45.000000 nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-20 07:47:45.000000 nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 07:47:45.000000 nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-20 07:47:45.000000 nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-20 07:47:45.000000 nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 07:47:45.937476 nonebot-plugin-sayoroll-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-20 07:47:32.000000 nonebot-plugin-sayoroll-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 07:55:56.451268 nonebot-plugin-sayoroll-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-20 07:55:48.000000 nonebot-plugin-sayoroll-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-20 07:55:56.451268 nonebot-plugin-sayoroll-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-07-20 07:55:48.000000 nonebot-plugin-sayoroll-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 07:55:56.447268 nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll/
+-rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-07-20 07:55:48.000000 nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 07:55:56.451268 nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-20 07:55:56.000000 nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-20 07:55:56.000000 nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 07:55:56.000000 nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-20 07:55:56.000000 nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-20 07:55:56.000000 nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 07:55:56.451268 nonebot-plugin-sayoroll-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-20 07:55:48.000000 nonebot-plugin-sayoroll-0.4.1/setup.py
```

### Comparing `nonebot-plugin-sayoroll-0.4.0/LICENSE` & `nonebot-plugin-sayoroll-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-0.4.0/PKG-INFO` & `nonebot-plugin-sayoroll-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 0.4.0
+Version: 0.4.1
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.4.1 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                              [NoneBotPluginLogo]
```

### Comparing `nonebot-plugin-sayoroll-0.4.0/README.md` & `nonebot-plugin-sayoroll-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll/__init__.py` & `nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,19 +41,18 @@
 
     elif args.isdigit():
         msg = '你的数字是[{}]'.format(random.randint(0, int(args)))
         await roll.finish(
             message=MessageSegment.reply(event.message_id) + Message(msg)
         )
 
-    elif re.search('(.)(.)\\1(.*?)', args):
-        result = re.search('(.)(.)\\1(.*?)', args)
+    elif re.search(r'([\u4e00-\u9fff])([\u4e00-\u9fff])\1(.*?)', args):
+        result = re.search(r'([\u4e00-\u9fff])([\u4e00-\u9fff])\1(.*?)', args)
         options = [result.group()[:1], result.group()[1:]]
-        temp_str = args[:result.span()[0]].replace('我', 'temp').replace('你', '我').replace('temp', '你')
-        msg = '我觉得' + temp_str + random.choice(options) + args[result.span()[1]:]
+        msg = '我觉得' + args[:result.span()[0]].replace('我', 'temp').replace('你', '我').replace('temp', '你') + random.choice(options) + args[result.span()[1]:]
         await roll.finish(
             message=MessageSegment.reply(event.message_id) + Message(msg)
         )
 
     args = normalize_str(args)
     args_without_punctuation = args.translate(str.maketrans('', '', string.punctuation))
     if len(args_without_punctuation.split(' ')) == 1:
```

### Comparing `nonebot-plugin-sayoroll-0.4.0/nonebot_plugin_sayoroll.egg-info/PKG-INFO` & `nonebot-plugin-sayoroll-0.4.1/nonebot_plugin_sayoroll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 0.4.0
+Version: 0.4.1
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.4.1 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                              [NoneBotPluginLogo]
```

### Comparing `nonebot-plugin-sayoroll-0.4.0/setup.py` & `nonebot-plugin-sayoroll-0.4.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-sayoroll",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.4.0",  # 程序版本
+    version="0.4.1",  # 程序版本
     author="A M D",  # 项目作者
     author_email="mas_alone@qq.com",  # 作者邮件
     description="基于NoneBot的高仿以前小夜bot的roll功能",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/mas-alone/nonebot-plugin-sayoroll",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

