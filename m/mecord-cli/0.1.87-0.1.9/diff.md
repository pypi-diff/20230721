# Comparing `tmp/mecord-cli-0.1.87.tar.gz` & `tmp/mecord-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecord-cli-0.1.87.tar", last modified: Fri Jul 21 03:58:56 2023, max compression
+gzip compressed data, was "mecord-cli-0.1.9.tar", last modified: Mon Mar 13 11:30:29 2023, max compression
```

## Comparing `mecord-cli-0.1.87.tar` & `mecord-cli-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 03:58:56.372189 mecord-cli-0.1.87/
--rw-rw-rw-   0        0        0     1078 2023-02-16 06:18:02.000000 mecord-cli-0.1.87/LICENSE
--rw-rw-rw-   0        0        0     2364 2023-07-21 03:58:56.371190 mecord-cli-0.1.87/PKG-INFO
--rw-rw-rw-   0        0        0     1942 2023-04-21 14:39:36.000000 mecord-cli-0.1.87/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 03:58:56.354188 mecord-cli-0.1.87/mecord/
--rw-rw-rw-   0        0        0        0 2023-02-27 08:17:36.000000 mecord-cli-0.1.87/mecord/__init__.py
--rw-rw-rw-   0        0        0    56500 2023-06-09 09:58:53.000000 mecord-cli-0.1.87/mecord/aigc_ext_pb2.py
--rw-rw-rw-   0        0        0    10618 2023-07-21 03:43:25.000000 mecord-cli-0.1.87/mecord/capability_provider.py
--rw-rw-rw-   0        0        0    40930 2023-06-09 09:58:18.000000 mecord-cli-0.1.87/mecord/common_ext_pb2.py
--rw-rw-rw-   0        0        0      173 2023-07-21 03:58:55.000000 mecord-cli-0.1.87/mecord/constant.py
--rw-rw-rw-   0        0        0     1934 2023-07-17 07:17:48.000000 mecord-cli-0.1.87/mecord/main.py
--rw-rw-rw-   0        0        0    10506 2023-07-21 03:29:55.000000 mecord-cli-0.1.87/mecord/mecord_service.py
--rw-rw-rw-   0        0        0    11578 2023-07-19 09:58:48.000000 mecord-cli-0.1.87/mecord/mecord_widget.py
--rw-rw-rw-   0        0        0    11164 2023-07-20 10:37:03.000000 mecord-cli-0.1.87/mecord/progress_monitor.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:58:56.356188 mecord-cli-0.1.87/mecord/public_tools/
--rw-rw-rw-   0        0        0        0 2023-04-21 14:39:36.000000 mecord-cli-0.1.87/mecord/public_tools/__init__.py
--rw-rw-rw-   0        0        0      302 2023-04-21 14:39:36.000000 mecord-cli-0.1.87/mecord/public_tools/decorator_tools.py
--rw-rw-rw-   0        0        0     3250 2023-06-09 09:58:18.000000 mecord-cli-0.1.87/mecord/rpcinput_pb2.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:58:56.360192 mecord-cli-0.1.87/mecord/script_template/
--rw-rw-rw-   0        0        0        0 2023-03-01 01:46:57.000000 mecord-cli-0.1.87/mecord/script_template/__init__.py
--rw-rw-rw-   0        0        0      312 2023-04-21 14:39:36.000000 mecord-cli-0.1.87/mecord/script_template/launch.py
--rw-rw-rw-   0        0        0      915 2023-04-10 11:57:12.000000 mecord-cli-0.1.87/mecord/script_template/main.py
--rw-rw-rw-   0        0        0      801 2023-03-15 02:24:04.000000 mecord-cli-0.1.87/mecord/script_template/run.py
--rw-rw-rw-   0        0        0     6214 2023-07-20 09:18:18.000000 mecord-cli-0.1.87/mecord/store.py
--rw-rw-rw-   0        0        0     8745 2023-06-09 09:58:18.000000 mecord-cli-0.1.87/mecord/uauth_common_pb2.py
--rw-rw-rw-   0        0        0   108609 2023-06-09 09:58:56.000000 mecord-cli-0.1.87/mecord/uauth_ext_pb2.py
--rw-rw-rw-   0        0        0     2375 2023-07-20 07:39:19.000000 mecord-cli-0.1.87/mecord/upload.py
--rw-rw-rw-   0        0        0    12849 2023-06-09 09:58:55.000000 mecord-cli-0.1.87/mecord/user_status_ext_pb2.py
--rw-rw-rw-   0        0        0    12538 2023-07-17 06:01:30.000000 mecord-cli-0.1.87/mecord/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:58:56.365190 mecord-cli-0.1.87/mecord/widget_template/
--rw-rw-rw-   0        0        0     1977 2023-03-14 11:34:25.000000 mecord-cli-0.1.87/mecord/widget_template/MekongJS.js.py
--rw-rw-rw-   0        0        0        0 2023-03-01 01:46:57.000000 mecord-cli-0.1.87/mecord/widget_template/__init__.py
--rw-rw-rw-   0        0        0      219 2023-04-21 14:39:36.000000 mecord-cli-0.1.87/mecord/widget_template/config.json.py
--rw-rw-rw-   0        0        0     1678 2023-03-14 11:34:25.000000 mecord-cli-0.1.87/mecord/widget_template/icon.png.py
--rw-rw-rw-   0        0        0      719 2023-03-14 11:34:25.000000 mecord-cli-0.1.87/mecord/widget_template/index.html.py
--rw-rw-rw-   0        0        0     9664 2023-07-21 03:58:44.000000 mecord-cli-0.1.87/mecord/xy_pb.py
--rw-rw-rw-   0        0        0     2216 2023-04-10 11:57:12.000000 mecord-cli-0.1.87/mecord/xy_user.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:58:56.370190 mecord-cli-0.1.87/mecord_cli.egg-info/
--rw-rw-rw-   0        0        0     2364 2023-07-21 03:58:56.000000 mecord-cli-0.1.87/mecord_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2023-07-21 03:58:56.000000 mecord-cli-0.1.87/mecord_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 03:58:56.000000 mecord-cli-0.1.87/mecord_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-21 03:58:56.000000 mecord-cli-0.1.87/mecord_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-07-21 03:58:56.000000 mecord-cli-0.1.87/mecord_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-21 03:58:56.000000 mecord-cli-0.1.87/mecord_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 03:58:56.372189 mecord-cli-0.1.87/setup.cfg
--rw-rw-rw-   0        0        0     2523 2023-07-21 03:58:54.000000 mecord-cli-0.1.87/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-13 11:30:29.835509 mecord-cli-0.1.9/
+-rw-rw-rw-   0        0        0     1078 2023-02-16 06:18:02.000000 mecord-cli-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1757 2023-03-13 11:30:29.835509 mecord-cli-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1336 2023-03-04 10:14:50.000000 mecord-cli-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-13 11:30:29.826539 mecord-cli-0.1.9/mecord/
+-rw-rw-rw-   0        0        0        0 2023-02-27 08:17:36.000000 mecord-cli-0.1.9/mecord/__init__.py
+-rw-rw-rw-   0        0        0    17672 2023-03-13 10:24:58.000000 mecord-cli-0.1.9/mecord/aigc_ext_pb2.py
+-rw-rw-rw-   0        0        0    39477 2023-03-13 10:24:23.000000 mecord-cli-0.1.9/mecord/common_ext_pb2.py
+-rw-rw-rw-   0        0        0       66 2023-03-13 11:25:22.000000 mecord-cli-0.1.9/mecord/constant.py
+-rw-rw-rw-   0        0        0     1119 2023-02-27 06:35:59.000000 mecord-cli-0.1.9/mecord/ftp_upload.py
+-rw-rw-rw-   0        0        0     5423 2023-03-10 09:35:28.000000 mecord-cli-0.1.9/mecord/main.py
+-rw-rw-rw-   0        0        0     6632 2023-03-13 11:28:39.000000 mecord-cli-0.1.9/mecord/mecord_service.py
+-rw-rw-rw-   0        0        0     6257 2023-03-13 11:20:07.000000 mecord-cli-0.1.9/mecord/mecord_widget.py
+-rw-rw-rw-   0        0        0     3250 2023-03-13 10:24:23.000000 mecord-cli-0.1.9/mecord/rpcinput_pb2.py
+drwxrwxrwx   0        0        0        0 2023-03-13 11:30:29.828533 mecord-cli-0.1.9/mecord/script_template/
+-rw-rw-rw-   0        0        0        0 2023-03-01 01:46:57.000000 mecord-cli-0.1.9/mecord/script_template/__init__.py
+-rw-rw-rw-   0        0        0      966 2023-03-13 08:44:35.000000 mecord-cli-0.1.9/mecord/script_template/main.py
+-rw-rw-rw-   0        0        0      801 2023-03-13 08:52:23.000000 mecord-cli-0.1.9/mecord/script_template/run.py
+-rw-rw-rw-   0        0        0     2354 2023-03-13 10:22:49.000000 mecord-cli-0.1.9/mecord/store.py
+-rw-rw-rw-   0        0        0     8745 2023-03-13 10:24:23.000000 mecord-cli-0.1.9/mecord/uauth_common_pb2.py
+-rw-rw-rw-   0        0        0   108609 2023-03-13 10:25:01.000000 mecord-cli-0.1.9/mecord/uauth_ext_pb2.py
+-rw-rw-rw-   0        0        0     1828 2023-03-13 10:54:19.000000 mecord-cli-0.1.9/mecord/upload.py
+-rw-rw-rw-   0        0        0    12849 2023-03-13 10:24:59.000000 mecord-cli-0.1.9/mecord/user_status_ext_pb2.py
+-rw-rw-rw-   0        0        0     4774 2023-03-13 10:42:05.000000 mecord-cli-0.1.9/mecord/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-13 11:30:29.831523 mecord-cli-0.1.9/mecord/widget_template/
+-rw-rw-rw-   0        0        0     1977 2023-03-13 09:18:19.000000 mecord-cli-0.1.9/mecord/widget_template/MekongJS.js.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 01:46:57.000000 mecord-cli-0.1.9/mecord/widget_template/__init__.py
+-rw-rw-rw-   0        0        0      147 2023-03-01 01:46:57.000000 mecord-cli-0.1.9/mecord/widget_template/config.json.py
+-rw-rw-rw-   0        0        0     1678 2023-03-13 02:53:47.000000 mecord-cli-0.1.9/mecord/widget_template/icon.png.py
+-rw-rw-rw-   0        0        0      719 2023-03-13 11:19:24.000000 mecord-cli-0.1.9/mecord/widget_template/index.html.py
+-rw-rw-rw-   0        0        0     7004 2023-03-13 11:26:14.000000 mecord-cli-0.1.9/mecord/xy_pb.py
+-rw-rw-rw-   0        0        0     2738 2023-02-20 13:11:01.000000 mecord-cli-0.1.9/mecord/xy_socket.py
+-rw-rw-rw-   0        0        0     2234 2023-03-02 08:06:21.000000 mecord-cli-0.1.9/mecord/xy_user.py
+drwxrwxrwx   0        0        0        0 2023-03-13 11:30:29.834513 mecord-cli-0.1.9/mecord_cli.egg-info/
+-rw-rw-rw-   0        0        0     1757 2023-03-13 11:30:29.000000 mecord-cli-0.1.9/mecord_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-03-13 11:30:29.000000 mecord-cli-0.1.9/mecord_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-13 11:30:29.000000 mecord-cli-0.1.9/mecord_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-03-13 11:30:29.000000 mecord-cli-0.1.9/mecord_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-03-13 11:30:29.000000 mecord-cli-0.1.9/mecord_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-03-13 11:30:29.000000 mecord-cli-0.1.9/mecord_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-13 11:30:29.835509 mecord-cli-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1446 2023-03-13 11:30:12.000000 mecord-cli-0.1.9/setup.py
```

### Comparing `mecord-cli-0.1.87/LICENSE` & `mecord-cli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.87/PKG-INFO` & `mecord-cli-0.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecord-cli
-Version: 0.1.87
+Version: 0.1.9
 Summary: mecord tools
 Home-page: https://github.com/mecordofficial
 Author: pengjun
 Author-email: mr_lonely@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,43 +36,20 @@
 ##### 2. Running
     $ mecord service start
 start a process to wait for the server to issue tasks. **Please do not close it**
 
 Module Developer
 ------------
     $ mecord widget init
-
 in empty folder, use above command craete a mecord module, structure is like 
     
     [widget folder]
         |-- h5
-            |-- config.json     //*required, do not change*
+            |-- config.json     //*required* widget config file
             |-- icon.png
             |-- index.html      //*required* index web page
-            |-- MekongJS.js      //*required, do not change*
         |-- script
-            |-- main.py         //*required, do not change* 
+            |-- main.py         //*required* entry file of receiving task
             |-- run.py
-
-if other person share widget code to you , you can add widget path in your computer to mecord environment
-
-    $ mecord widget add [path_with_widget_code]
-
 you can modify script and h5 file yourself, then publish to mecord sever 
     
     $ mecord widget publish
-
-#####other command
-set/get multi process task number
-
-    $ mecord set_multitask_num / get_multitask_num 1
-
-add this device joined to other group using token, or show current group token , you can share it to other person
-
-    $ mecord add_token /  show_token [token_string]
-
-unregister this device from mecord server
-
-    $ mecord unbind
-
-get mecord version
-    $ mecord version
```

### Comparing `mecord-cli-0.1.87/README.md` & `mecord-cli-0.1.9/mecord_cli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: mecord-cli
+Version: 0.1.9
+Summary: mecord tools
+Home-page: https://github.com/mecordofficial
+Author: pengjun
+Author-email: mr_lonely@foxmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Mecord Python Tool
 ===============================================
 The Mecord Python Tool is a official tool for mecodr, you can use it to **Register** device to mecord server, other person can use **Mecord Application** assign tasks to you for implementation
 
 Installation
 ------------
 
@@ -22,43 +36,20 @@
 ##### 2. Running
     $ mecord service start
 start a process to wait for the server to issue tasks. **Please do not close it**
 
 Module Developer
 ------------
     $ mecord widget init
-
 in empty folder, use above command craete a mecord module, structure is like 
     
     [widget folder]
         |-- h5
-            |-- config.json     //*required, do not change*
+            |-- config.json     //*required* widget config file
             |-- icon.png
             |-- index.html      //*required* index web page
-            |-- MekongJS.js      //*required, do not change*
         |-- script
-            |-- main.py         //*required, do not change* 
+            |-- main.py         //*required* entry file of receiving task
             |-- run.py
-
-if other person share widget code to you , you can add widget path in your computer to mecord environment
-
-    $ mecord widget add [path_with_widget_code]
-
 you can modify script and h5 file yourself, then publish to mecord sever 
     
     $ mecord widget publish
-
-#####other command
-set/get multi process task number
-
-    $ mecord set_multitask_num / get_multitask_num 1
-
-add this device joined to other group using token, or show current group token , you can share it to other person
-
-    $ mecord add_token /  show_token [token_string]
-
-unregister this device from mecord server
-
-    $ mecord unbind
-
-get mecord version
-    $ mecord version
```

### Comparing `mecord-cli-0.1.87/mecord/common_ext_pb2.py` & `mecord-cli-0.1.9/mecord/common_ext_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ommon_ext.proto\x12\x02pb\"\xf7\x02\n\x06Player\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12\x18\n\x03sex\x18\x03 \x01(\x0e\x32\x0b.pb.SexType\x12\x0b\n\x03id2\x18\x04 \x01(\x03\x12\x0c\n\x04icon\x18\x05 \x01(\t\x12\r\n\x05\x66lags\x18\x06 \x01(\x03\x12\r\n\x05\x63harm\x18\x08 \x01(\x03\x12\x13\n\x0b\x63harm_level\x18\t \x01(\x05\x12\x14\n\x0cwealth_level\x18\n \x01(\x05\x12\x0e\n\x06wealth\x18\x0b \x01(\x03\x12\x12\n\nonline_exp\x18\x0c \x01(\r\x12\x11\n\tcreate_at\x18\r \x01(\r\x12\x11\n\tis_delete\x18\x0e \x01(\x08\x12\r\n\x05point\x18\x0f \x01(\x03\x12\x13\n\x0bpoint_level\x18\x10 \x01(\x05\x12\x11\n\tsignature\x18\x11 \x01(\t\x12\x0c\n\x04\x63ity\x18\x12 \x01(\t\x12\x10\n\x08\x62irthday\x18\x13 \x01(\t\x12\x14\n\x0conline_state\x18\x14 \x01(\x05\x12\x1a\n\x12NicknameUpdateTime\x18\x15 \x01(\r\"\x81\x01\n\x08UserInfo\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04\x63ity\x18\x02 \x01(\t\x12\x11\n\tsignature\x18\x03 \x01(\t\x12\x0c\n\x04mind\x18\x04 \x01(\t\x12\x10\n\x08\x62irthday\x18\x05 \x01(\t\x12\x15\n\rintimate_slot\x18\x06 \x01(\x11\x12\x11\n\tnameplate\x18\x07 \x01(\t\"\xd7\x02\n\nPlayerInfo\x12\x1a\n\x06player\x18\x01 \x01(\x0b\x32\n.pb.Player\x12\x1a\n\x06\x65\x66\x66\x65\x63t\x18\x02 \x03(\x0b\x32\n.pb.Effect\x12\x1a\n\x04\x63lan\x18\x03 \x01(\x0b\x32\x0c.pb.ClanInfo\x12\x10\n\x08\x66\x61ns_num\x18\x04 \x01(\x05\x12\x15\n\rfollowing_num\x18\x05 \x01(\x05\x12\x14\n\x0c\x66riend_alias\x18\x06 \x01(\t\x12\x1f\n\x07\x65\x66\x66\x65\x63ts\x18\x07 \x03(\x0b\x32\x0e.pb.EffectInfo\x12\x18\n\x10\x61ttitude_yes_num\x18\x08 \x01(\x03\x12\x17\n\x0ftotal_visit_num\x18\t \x01(\x03\x12\x15\n\radd_visit_num\x18\n \x01(\x03\x12\x1c\n\x05label\x18\x0b \x03(\x0b\x32\r.pb.LabelInfo\x12-\n\x0c\x64\x65grees_info\x18\x0c \x01(\x0b\x32\x17.pb.AttitudeDegreesInfo\"=\n\x07\x42\x61gItem\x12\x0f\n\x07gift_id\x18\x01 \x01(\r\x12\x0e\n\x06\x61mount\x18\x02 \x01(\r\x12\x11\n\tcteate_at\x18\x03 \x01(\t\"\"\n\x08\x41godaKey\x12\x16\n\x0epermission_key\x18\x01 \x01(\t\":\n\x0bOnOffStatus\x12\x0e\n\x06status\x18\x01 \x01(\x11\x12\x1b\n\x04type\x18\x02 \x01(\x0e\x32\r.pb.OnOffType\"\xf8\x01\n\x11SearchPlayerEntry\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0b\n\x03id2\x18\x02 \x01(\x12\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x18\n\x03sex\x18\x04 \x01(\x0e\x32\x0b.pb.SexType\x12\x0c\n\x04icon\x18\x05 \x01(\t\x12\r\n\x05\x63harm\x18\x06 \x01(\x12\x12\x13\n\x0b\x63harm_level\x18\x07 \x01(\x11\x12\x0e\n\x06wealth\x18\x08 \x01(\x12\x12\x14\n\x0cwealth_level\x18\t \x01(\x11\x12\x0e\n\x06online\x18\n \x01(\x08\x12\x0f\n\x07room_id\x18\x0b \x01(\x12\x12\x12\n\nhas_passwd\x18\r \x01(\x08\x12\x11\n\tsignature\x18\x0e \x01(\t\"\x9f\x01\n\nEffectInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12%\n\ttime_type\x18\x02 \x01(\x0e\x32\x12.pb.EffectTimeType\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\x03\x12\'\n\nuse_status\x18\x04 \x01(\x0e\x32\x13.pb.EffectUseStatus\x12#\n\x0b\x65\x66\x66\x65\x63t_type\x18\x05 \x01(\x0e\x32\x0e.pb.EffectType\"\xaf\x01\n\x06\x45\x66\x66\x65\x63t\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04\x66lag\x18\x02 \x01(\x05\x12\x0b\n\x03str\x18\x03 \x01(\t\x12%\n\ttime_type\x18\x04 \x01(\x0e\x32\x12.pb.EffectTimeType\x12\x10\n\x08\x65nd_time\x18\x05 \x01(\x05\x12\'\n\nuse_status\x18\x06 \x01(\x0e\x32\x13.pb.EffectUseStatus\x12\x1c\n\x04type\x18\x07 \x01(\x0e\x32\x0e.pb.EffectType\"T\n\x0c\x45\x66\x66\x65\x63tConfig\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x1c\n\x04type\x18\x02 \x01(\x0e\x32\x0e.pb.EffectType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\"6\n\x15\x45\x66\x66\x65\x63tNicknamePendant\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x10\n\x08show_url\x18\x02 \x01(\t\"G\n\rEffectSerConf\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x1c\n\x04type\x18\x02 \x01(\x0e\x32\x0e.pb.EffectType\x12\x0c\n\x04name\x18\x03 \x01(\t\"0\n\rIndexTipRooms\x12\x0f\n\x07room_id\x18\x01 \x01(\x03\x12\x0e\n\x06tip_id\x18\x02 \x01(\x05\"=\n\x07RegisId\x12\x0b\n\x03ios\x18\x01 \x01(\t\x12\x0f\n\x07\x61ndroid\x18\x02 \x01(\t\x12\x14\n\x0cmanufacturer\x18\x03 \x01(\t\"P\n\nModelOnOff\x12\x1c\n\x05onOff\x18\x01 \x01(\x0e\x32\r.pb.OnOffType\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.pb.ModelOnOffStatus\"\xd0\x01\n\x04Rank\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x03sex\x18\x03 \x01(\x0e\x32\x0b.pb.SexType\x12\r\n\x05level\x18\x04 \x01(\r\x12\r\n\x05value\x18\x05 \x01(\x04\x12\x10\n\x08res_time\x18\x06 \x01(\r\x12\x0f\n\x07gap_val\x18\x07 \x01(\r\x12\x0c\n\x04icon\x18\x08 \x01(\t\x12\x0f\n\x07gift_id\x18\t \x01(\x04\x12\x10\n\x08gift_num\x18\n \x01(\r\x12\x0f\n\x07ranking\x18\x0b \x01(\r\x12\x11\n\tgift_name\x18\x0c \x01(\t\"5\n\x0fPlayerChairRoom\x12\x11\n\tplayer_id\x18\x01 \x01(\x03\x12\x0f\n\x07room_id\x18\x02 \x01(\x03\"l\n\x08\x43lanInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x11\n\ticon_word\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\x03\x12\x12\n\nlevel_name\x18\x05 \x01(\t\x12\x10\n\x08is_admin\x18\x06 \x01(\x08\"*\n\x06Period\x12\x10\n\x08\x62\x65gin_at\x18\x01 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x02 \x01(\x03\",\n\tLabelInfo\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63lassify_id\x18\x02 \x01(\x05\"Y\n\x13PlayerResourceShort\x12-\n\rresource_type\x18\x01 \x01(\x0e\x32\x16.pb.PlayerResourceType\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\"\x96\x01\n\x0ePlayerResource\x12-\n\rresource_type\x18\x01 \x01(\x0e\x32\x16.pb.PlayerResourceType\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x14\n\x0chead_img_url\x18\x04 \x01(\t\x12\x18\n\x03sex\x18\x05 \x01(\x0e\x32\x0b.pb.SexType\"c\n\x17PlayerResourceWithScore\x12+\n\x0fplayer_resource\x18\x01 \x01(\x0b\x32\x12.pb.PlayerResource\x12\r\n\x05score\x18\x02 \x01(\x03\x12\x0c\n\x04rank\x18\x03 \x01(\x05\"\xb4\x01\n\x13\x41ttitudeDegreesInfo\x12\x35\n\x0e\x64\x65grees_status\x18\x01 \x01(\x0e\x32\x1d.pb.AttitudeDegreesStatusType\x12\x36\n\rcategory_info\x18\x02 \x03(\x0b\x32\x1f.pb.AttitudeCategoryDegreesInfo\x12\x14\n\x0ctotal_degree\x18\x03 \x01(\x05\x12\x18\n\x10\x61nalysis_content\x18\x04 \x01(\t\"g\n\x1b\x41ttitudeCategoryDegreesInfo\x12\x13\n\x0b\x63\x61tegory_id\x18\x01 \x01(\x05\x12\x15\n\rcategory_name\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65gree\x18\x03 \x01(\x05\x12\x0c\n\x04icon\x18\x04 \x01(\t\"\x85\x01\n\x0e\x43MediaResource\x12\"\n\nmedia_type\x18\x01 \x01(\x0e\x32\x0e.pb.CMediaType\x12\x11\n\tmedia_url\x18\x02 \x01(\t\x12\x11\n\tcover_url\x18\x03 \x01(\t\x12\x13\n\x0bmedia_width\x18\x04 \x01(\x05\x12\x14\n\x0cmedia_height\x18\x05 \x01(\x05\"\x1b\n\x0bSayHelloReq\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1c\n\x0bSayHelloRes\x12\r\n\x05reply\x18\x01 \x01(\t\"b\n\x0cHeartbeatReq\x12\x0f\n\x07goim_id\x18\x01 \x01(\x03\x12\x11\n\tplayer_id\x18\x02 \x01(\x03\x12\n\n\x02ip\x18\x03 \x01(\t\x12\"\n\ndeviceType\x18\x04 \x01(\x0e\x32\x0e.pb.DeviceType\"!\n\x0cHeartbeatRes\x12\x11\n\ttimestamp\x18\x02 \x01(\x03*\xad\x01\n\tCommonErr\x12\x0f\n\x0b\x45rrCodeNone\x10\x00\x12\x11\n\x0c\x45rrCodeRedis\x10\x91N\x12\x11\n\x0c\x45rrCodeMysql\x10\x92N\x12\x15\n\x10\x45rrCodeFrequency\x10\x93N\x12\x11\n\x0c\x45rrCodeParam\x10\x94N\x12\x16\n\x11\x45rrCodeNoMatchObj\x10\x95N\x12\x10\n\x0b\x45rrCodeBusy\x10\x96N\x12\x15\n\x0f\x45rrCodeMaintain\x10\x9a\x82\x01*,\n\x07SexType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04MALE\x10\x01\x12\n\n\x06\x46\x45MALE\x10\x02*0\n\x0bOwnerInRoom\x12\x11\n\rNotInSelfRoom\x10\x00\x12\x0e\n\nInSelfRoom\x10\x01*%\n\tSceneType\x12\x0b\n\x07ST_ZERO\x10\x00\x12\x0b\n\x07ST_HOME\x10\x01*y\n\rRoomAdminType\x12\r\n\tRAT_GUEST\x10\x00\x12\x0e\n\nRAT_NORMAL\x10\n\x12\r\n\tRAT_ADMIN\x10\x14\x12\r\n\tRAT_OWNER\x10\x1e\x12\x13\n\x0fRAT_SUPER_ADMIN\x10(\x12\x16\n\tRAT_BLACK\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xfb\x01\n\nDeviceType\x12\x0e\n\nDT_UNKNOWN\x10\x00\x12\x12\n\x0e\x44T_FLASHPLAYER\x10\x01\x12\x14\n\x10\x44T_ANDROID_PHONE\x10\x14\x12\x10\n\x0c\x44T_IOS_PHONE\x10(\x12\x18\n\x14\x44T_WINDOWS_ASSISTANT\x10P\x12\x11\n\rDT_WINDOWS_PC\x10Z\x12\x0c\n\x08\x44T_ROBOT\x10\x64\x12\x1a\n\x16\x44T_WECHAT_SUBSCRIPTION\x10n\x12\x17\n\x13\x44T_QQ_SMALL_PROGRAM\x10x\x12\x17\n\x12\x44T_WX_MINI_PROGRAM\x10\x82\x01\x12\x0b\n\x06\x44T_WEB\x10\x8c\x01\x12\x0b\n\x06\x44T_MAC\x10\x96\x01*\x99\x01\n\x0bPlayerFlags\x12\x0b\n\x07PF_ZERO\x10\x00\x12\x14\n\x10PF_CERTIFICATION\x10\x01\x12\x10\n\x0cPF_BIND_BANK\x10\x04\x12\r\n\tPF_INVITE\x10\x05\x12\x13\n\x0fPF_CHARGE_FIRST\x10\x0c\x12\x18\n\x14PF_ATTITUDE_QUESTION\x10\r\x12\x17\n\x13PF_END_REGISTRATION\x10\x0e*2\n\x0c\x41\x63\x63ountFlags\x12\x0b\n\x07\x41\x46_ZERO\x10\x00\x12\x15\n\x11\x41\x46_PHONE_VERIFIED\x10\x01*\xfc\r\n\tOnOffType\x12\x0c\n\x08YEAR_BAG\x10\x00\x12\r\n\tCRACK_EGG\x10\x01\x12\x0e\n\nGOOGLE_PAY\x10\x05\x12\x0b\n\x07IAP_PAY\x10\x06\x12\n\n\x06INVITE\x10\x07\x12\x12\n\x0eINDEX_CATEGORY\x10\x08\x12\n\n\x06\x43\x45RTIF\x10\t\x12\t\n\x05GUARD\x10\n\x12\x10\n\x0cLOTTERY_DRAW\x10\x0c\x12\x0f\n\x0bMENTOR_SHIP\x10\r\x12\x0e\n\nCERTIF_IOS\x10\x0e\x12\x11\n\rREAL_IDENTITY\x10\x0f\x12\x0f\n\x0bNOVICE_GIFT\x10\x10\x12\x12\n\x0eROOM_SET_MODEL\x10\x12\x12\x11\n\rACTIVITY_TYPE\x10\x14\x12\x0c\n\x08\x41\x43TIVITY\x10\x15\x12\x0c\n\x08HOT_SONG\x10\x17\x12\x0e\n\nROOM_ENTER\x10\"\x12\x1d\n\x19ROOM_PATTERN_HIGH_QUALITY\x10#\x12\x11\n\rAUTH_LOGIN_UI\x10&\x12\x12\n\x0eUSER_DATA_EDIT\x10)\x12\x11\n\rCERTIFICATION\x10+\x12\x1b\n\x17\x43\x45RTIFICATION_ROOM_SHOW\x10,\x12%\n!CERTIFICATION_ROOM_WIN_OPEN_CLOSE\x10-\x12\x10\n\x0c\x43\x45RTIFY_WORD\x10.\x12\x11\n\rCERTIFY_CHAIR\x10/\x12\x1c\n\x18\x43\x45RTIFY_UPDATE_USER_INFO\x10\x30\x12\x1c\n\x18\x43\x45RTIFY_BROADCAST_FRIEND\x10\x31\x12\x15\n\x11\x43\x45RTIFY_HEAD_LINE\x10\x32\x12\x15\n\x11\x43\x45RTIFY_TIAO_TIAO\x10\x33\x12\x14\n\x10LOGIN_BIND_PHONE\x10\x34\x12\x1c\n\x18\x43\x45RTIFY_OWNER_ENTER_ROOM\x10\x35\x12\x0f\n\x0bYoung_Model\x10:\x12\x14\n\x10\x43USTOMER_SERVICE\x10;\x12\x15\n\x11OVERSEAS_IP_LIMIT\x10\x42\x12\x12\n\x0eOLD_NAME_LIMIT\x10\x43\x12\x12\n\x0e\x43RACK_SELF_MSG\x10\x44\x12\x12\n\x0eORDER_LOCATION\x10G\x12\x12\n\x0e\x44\x45LETE_ACCOUNT\x10I\x12\x0f\n\x0bYUNPIAN_SMS\x10J\x12\x11\n\rBIND_PHONE_V2\x10K\x12\x14\n\x10\x42IND_PHONE_LOGIN\x10L\x12\x0e\n\nCOUNT_DOWN\x10N\x12\x0e\n\nOXYGEN_BAR\x10^\x12\x13\n\x0fPRIVACY_SETTING\x10_\x12\x1f\n\x1bOXYGEN_BAR_CLAN_MEMBER_ONLY\x10`\x12\x18\n\x14OXYGEN_BAR_TREND_GIF\x10\x61\x12\x0e\n\nDATA_AUDIT\x10\x62\x12\r\n\tInner_Tec\x10\x64\x12\r\n\tInner_Ali\x10\x65\x12\x16\n\x12\x43\x45RTIFY_IM_PICTURE\x10g\x12\x0b\n\x07\x43MB_VIP\x10h\x12\x13\n\x0f\x43RACKEGG_FOREST\x10i\x12\x13\n\x0e\x41NTI_ADDICTION\x10\xc8\x01\x12&\n!TEXT_FILTER_ROOM_SCREEN_ENCRYPTED\x10\xc9\x01\x12(\n#TEXT_FILTER_ROOM_SCREEN_UNENCRYPTED\x10\xca\x01\x12!\n\x1cTEXT_FILTER_BROADCAST_FRIEND\x10\xcb\x01\x12\x1d\n\x18TEXT_FILTER_PRIVATE_CHAT\x10\xcc\x01\x12\x10\n\x0c\x42\x43_HEAD_LINE\x10n\x12\x13\n\x0fONE_CLICK_LOGIN\x10o\x12\x0e\n\nCERTIFY_PM\x10p\x12\x13\n\x0f\x43\x45RTIFY_PICTURE\x10q\x12\x19\n\x15\x43HANNEL_ADVERT_AUDITS\x10r\x12\x1a\n\x16\x43\x45RTIFY_CREATE_CHANNEL\x10t\x12\x18\n\x14\x43\x45RTIFY_JOIN_CHANNEL\x10u\x12\x10\n\x0c\x43\x45RTIFY_GIVE\x10v\x12\x17\n\x13\x43\x45RTIFY_ROOM_NOTICE\x10w\x12\x14\n\x10\x43\x45RTIFY_RECHARGE\x10x\x12\x19\n\x15\x43\x45RTIFY_PUBLISH_TREND\x10y\x12\x19\n\x15\x43\x45RTIFY_COMMENT_TREND\x10z\x12\x11\n\rHOME_NAV_TYPE\x10{\x12\x11\n\rLOGIN_CHECKED\x10|\x12\x0e\n\nHIGH_SOUND\x10}\x12\x16\n\x12HIGH_SOUND_CHANNEL\x10~\x12\x1a\n\x16\x43HANNEL_STAR_CHALLENGE\x10\x7f\x12\x11\n\x0c\x43HANNEL_STAT\x10\x80\x01\x12\x11\n\x0cREGISTER_SEX\x10\x82\x01\x12\x16\n\x11REGISTER_NICKNAME\x10\x83\x01\x12\x16\n\x11REGISTER_ATTITUDE\x10\x84\x01\x12\x13\n\x0e\x43REATE_CHANNEL\x10\x85\x01\x12\x1a\n\x15\x43OMMUNITY_TREND_AUDIO\x10\x86\x01\x12\x0c\n\x07IM_TIPS\x10\x87\x01\x12\x18\n\x13MULTI_CLIENT_ONLINE\x10\xfd\x01*)\n\nStatusCode\x12\x0b\n\x07SC_FAIL\x10\x00\x12\x0e\n\nSC_SUCCESS\x10\x01*?\n\nEffectType\x12\x12\n\x0e\x45\x66\x66\x65\x63tTypeNone\x10\x00\x12\x1d\n\x19\x45\x66\x66\x65\x63tTypeNicknamePendant\x10\x01*\x7f\n\x0e\x45\x66\x66\x65\x63tTimeType\x12\x18\n\x14\x45\x66\x66\x65\x63tTimeTypeAlways\x10\x00\x12\x16\n\x12\x45\x66\x66\x65\x63tTimeTypeMike\x10\x01\x12\x1e\n\x1a\x45\x66\x66\x65\x63tTimeTypeWearInPacket\x10\x02\x12\x1b\n\x17\x45\x66\x66\x65\x63tTimeTypePermanent\x10\x03*,\n\x0f\x45\x66\x66\x65\x63tUseStatus\x12\n\n\x06\x45S_Use\x10\x00\x12\r\n\tES_NotUse\x10\x01*I\n\x10\x45\x66\x66\x65\x63tNoticeType\x12\x18\n\x14\x45\x66\x66\x65\x63tNoticeTypeGain\x10\x00\x12\x1b\n\x17\x45\x66\x66\x65\x63tNoticeTypeTimeout\x10\x01*:\n\x10ModelOnOffStatus\x12\x0b\n\x07\x41LL_OFF\x10\x00\x12\n\n\x06\x41LL_ON\x10\x01\x12\r\n\tWHITELIST\x10\x02*A\n\x08RankType\x12\x0b\n\x07RT_ZERO\x10\x00\x12\x0c\n\x08RT_CHARM\x10\x01\x12\r\n\tRT_WEALTH\x10\x02\x12\x0b\n\x07RT_GIFT\x10\x03*N\n\rLoadClickType\x12\x0c\n\x08LCT_ZERO\x10\x00\x12\x17\n\x13LCT_INTIMATE_DETAIL\x10\x01\x12\x16\n\x12LCT_INTIMATE_STORE\x10\x02*F\n\x0b\x41uditStatus\x12\x11\n\rAS_Audit_Pass\x10\x00\x12\x0f\n\x0b\x41S_Auditing\x10\x01\x12\x13\n\x0f\x41S_Audit_Refuse\x10\x02*\xf3\x01\n\nUploadType\x12\x0c\n\x08TypeZero\x10\x00\x12\x10\n\x0cHeadAlbumImg\x10\x01\x12\x0f\n\x0bHeadIconImg\x10\x02\x12\x0f\n\x0b\x44ynamicsImg\x10\x03\x12\r\n\tClientLog\x10\x04\x12\x0e\n\nTipOffsImg\x10\x05\x12\x0c\n\x08Indetity\x10\x06\x12\x0b\n\x07PMMedia\x10\x07\x12\t\n\x05Voice\x10\x08\x12\x11\n\rBackgroundImg\x10\x17\x12\x0f\n\x0b\x43hannelIcon\x10\x18\x12\x11\n\rWXRobotQRcode\x10\x19\x12\x13\n\x0f\x43ommunityTagImg\x10\x1c\x12\x12\n\x0ePersonLabelImg\x10\x1d*\xe9\x01\n\x0ePayChannelType\x12\x0c\n\x08PCT_NULL\x10\x00\x12\x11\n\rPCT_ALIPAY_H5\x10\x02\x12\x12\n\x0ePCT_ALIPAY_APP\x10\x03\x12\x11\n\rPCT_WXPAY_APP\x10\x04\x12\x10\n\x0cPCT_WXPAY_H5\x10\x05\x12\x0b\n\x07PCT_IAP\x10\x06\x12\x0c\n\x08PCT_PLAY\x10\x08\x12\x0e\n\nPCT_PAYPAL\x10\n\x12\r\n\tPCT_BOING\x10\x0b\x12\x10\n\x0cPCT_UNIONPAY\x10\x0c\x12\x0e\n\tPCT_AGENT\x10\xfd\x01\x12\x0f\n\nPCT_MANUAL\x10\xfe\x01\x12\x10\n\x0bPCT_DEVTEST\x10\xff\x01*i\n\x04Role\x12\n\n\x06R_NONE\x10\x00\x12\x0f\n\x0bR_SUPERUSER\x10\x01\x12\x08\n\x04R_OW\x10\x02\x12\x08\n\x04R_VP\x10\x03\x12\x08\n\x04R_MA\x10\x04\x12\t\n\x05R_CA1\x10\x05\x12\t\n\x05R_CA2\x10\x06\x12\x07\n\x03R_R\x10\x07\x12\x07\n\x03R_U\x10\x08*]\n\x0eNameplateStyle\x12\x0b\n\x07NS_NONE\x10\x00\x12\x0e\n\nNS_STYLE_1\x10\x01\x12\x0e\n\nNS_STYLE_2\x10\x02\x12\x0e\n\nNS_STYLE_3\x10\x03\x12\x0e\n\nNS_STYLE_4\x10\x04*E\n\x12PlayerResourceType\x12\x0c\n\x08PRT_NONE\x10\x00\x12\x15\n\x11PRT_FIRST_ACCOUNT\x10\x01\x12\n\n\x06PRT_WX\x10\x02*f\n\x19\x41ttitudeDegreesStatusType\x12\x13\n\x0f\x41\x44ST_BOTH_EVERY\x10\x00\x12\x17\n\x13\x41\x44ST_OPPOSITE_EVERY\x10\x01\x12\x1b\n\x17\x41\x44ST_OPPOSITE_NOTENOUGH\x10\x02*u\n\nCMediaType\x12\x13\n\x0f\x43MediaType_None\x10\x00\x12\x12\n\x0e\x43MediaType_Png\x10\x01\x12\x12\n\x0e\x43MediaType_Gif\x10\x02\x12\x14\n\x10\x43MediaType_Video\x10\x03\x12\x14\n\x10\x43MediaType_Audio\x10\x04*w\n\x11\x44\x65viceConnectOper\x12\x0c\n\x08\x44\x43S_None\x10\x00\x12\x12\n\x0e\x44\x43S_Requesting\x10\x01\x12\x0f\n\x0b\x44\x43S_Receive\x10\x02\x12\x0e\n\nDCS_Refuse\x10\x03\x12\x0f\n\x0b\x44\x43S_Timeout\x10\x04\x12\x0e\n\nDCS_Cancel\x10\x05*\xa7\x01\n\x0b\x44\x65viceCmdId\x12\x11\n\rDC_DeviceZero\x10\x00\x12\x14\n\x0e\x44\x43_DeviceLogin\x10\x99\x98\x1f\x12\x1e\n\x18\x44\x43_MessageConnectOperate\x10\x9a\x98\x1f\x12\x1c\n\x16\x44\x43_MessageStatusUpdate\x10\x9b\x98\x1f\x12\x1a\n\x14\x44\x43_DeviceShareStatus\x10\x9c\x98\x1f\x12\x15\n\x0f\x44\x43_SingoConnect\x10\xb9\xa5%*L\n\nTaskStatus\x12\x0b\n\x07TS_None\x10\x00\x12\x11\n\rTS_Processing\x10\x01\x12\x0e\n\nTS_Success\x10\x02\x12\x0e\n\nTS_Failure\x10\x03*N\n\x08TaskType\x12\x0b\n\x07TT_None\x10\x00\x12\x0c\n\x08TT_Image\x10\x01\x12\x0c\n\x08TT_Video\x10\x02\x12\x0c\n\x08TT_Audio\x10\x03\x12\x0b\n\x07TT_Text\x10\x04*o\n\tLabelType\x12\x0b\n\x07LT_NONE\x10\x00\x12\x0b\n\x07LT_POST\x10\x01\x12\x0e\n\nLT_Gallery\x10\x02\x12\x0c\n\x08LT_Group\x10\x03\x12\x0e\n\nLT_Comment\x10\x04\x12\x0b\n\x07LT_Lora\x10\x05\x12\r\n\tLT_Client\x10\x06*N\n\x08\x41igcType\x12\x0b\n\x07\x41T_NONE\x10\x00\x12\x0c\n\x08\x41T_IMAGE\x10\x01\x12\x0c\n\x08\x41T_VIDEO\x10\x02\x12\x0c\n\x08\x41T_AUDIO\x10\x03\x12\x0b\n\x07\x41T_TEXT\x10\x04*%\n\x06Module\x12\n\n\x06M_None\x10\x00\x12\x0f\n\x0bM_Subscribe\x10\x01*A\n\nWidgetType\x12\x0b\n\x07WT_None\x10\x00\x12\x0e\n\nWT_General\x10\x01\x12\t\n\x05WT_SD\x10\x02\x12\x0b\n\x07WT_Lora\x10\x03*:\n\rCalculateMode\x12\x0b\n\x07\x43M_None\x10\x00\x12\r\n\tCM_Single\x10\x01\x12\r\n\tCM_Minute\x10\x02*1\n\x0e\x43hargeCateType\x12\x0e\n\nCCT_Normal\x10\x00\x12\x0f\n\x0b\x43\x43T_ActCard\x10\x01\x42\x06\xa2\x02\x03PB3b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ommon_ext.proto\x12\x02pb\"\xf7\x02\n\x06Player\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12\x18\n\x03sex\x18\x03 \x01(\x0e\x32\x0b.pb.SexType\x12\x0b\n\x03id2\x18\x04 \x01(\x03\x12\x0c\n\x04icon\x18\x05 \x01(\t\x12\r\n\x05\x66lags\x18\x06 \x01(\x03\x12\r\n\x05\x63harm\x18\x08 \x01(\x03\x12\x13\n\x0b\x63harm_level\x18\t \x01(\x05\x12\x14\n\x0cwealth_level\x18\n \x01(\x05\x12\x0e\n\x06wealth\x18\x0b \x01(\x03\x12\x12\n\nonline_exp\x18\x0c \x01(\r\x12\x11\n\tcreate_at\x18\r \x01(\r\x12\x11\n\tis_delete\x18\x0e \x01(\x08\x12\r\n\x05point\x18\x0f \x01(\x03\x12\x13\n\x0bpoint_level\x18\x10 \x01(\x05\x12\x11\n\tsignature\x18\x11 \x01(\t\x12\x0c\n\x04\x63ity\x18\x12 \x01(\t\x12\x10\n\x08\x62irthday\x18\x13 \x01(\t\x12\x14\n\x0conline_state\x18\x14 \x01(\x05\x12\x1a\n\x12NicknameUpdateTime\x18\x15 \x01(\r\"\x81\x01\n\x08UserInfo\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04\x63ity\x18\x02 \x01(\t\x12\x11\n\tsignature\x18\x03 \x01(\t\x12\x0c\n\x04mind\x18\x04 \x01(\t\x12\x10\n\x08\x62irthday\x18\x05 \x01(\t\x12\x15\n\rintimate_slot\x18\x06 \x01(\x11\x12\x11\n\tnameplate\x18\x07 \x01(\t\"\xd7\x02\n\nPlayerInfo\x12\x1a\n\x06player\x18\x01 \x01(\x0b\x32\n.pb.Player\x12\x1a\n\x06\x65\x66\x66\x65\x63t\x18\x02 \x03(\x0b\x32\n.pb.Effect\x12\x1a\n\x04\x63lan\x18\x03 \x01(\x0b\x32\x0c.pb.ClanInfo\x12\x10\n\x08\x66\x61ns_num\x18\x04 \x01(\x05\x12\x15\n\rfollowing_num\x18\x05 \x01(\x05\x12\x14\n\x0c\x66riend_alias\x18\x06 \x01(\t\x12\x1f\n\x07\x65\x66\x66\x65\x63ts\x18\x07 \x03(\x0b\x32\x0e.pb.EffectInfo\x12\x18\n\x10\x61ttitude_yes_num\x18\x08 \x01(\x03\x12\x17\n\x0ftotal_visit_num\x18\t \x01(\x03\x12\x15\n\radd_visit_num\x18\n \x01(\x03\x12\x1c\n\x05label\x18\x0b \x03(\x0b\x32\r.pb.LabelInfo\x12-\n\x0c\x64\x65grees_info\x18\x0c \x01(\x0b\x32\x17.pb.AttitudeDegreesInfo\"=\n\x07\x42\x61gItem\x12\x0f\n\x07gift_id\x18\x01 \x01(\r\x12\x0e\n\x06\x61mount\x18\x02 \x01(\r\x12\x11\n\tcteate_at\x18\x03 \x01(\t\"\"\n\x08\x41godaKey\x12\x16\n\x0epermission_key\x18\x01 \x01(\t\":\n\x0bOnOffStatus\x12\x0e\n\x06status\x18\x01 \x01(\x11\x12\x1b\n\x04type\x18\x02 \x01(\x0e\x32\r.pb.OnOffType\"\xf8\x01\n\x11SearchPlayerEntry\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0b\n\x03id2\x18\x02 \x01(\x12\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x18\n\x03sex\x18\x04 \x01(\x0e\x32\x0b.pb.SexType\x12\x0c\n\x04icon\x18\x05 \x01(\t\x12\r\n\x05\x63harm\x18\x06 \x01(\x12\x12\x13\n\x0b\x63harm_level\x18\x07 \x01(\x11\x12\x0e\n\x06wealth\x18\x08 \x01(\x12\x12\x14\n\x0cwealth_level\x18\t \x01(\x11\x12\x0e\n\x06online\x18\n \x01(\x08\x12\x0f\n\x07room_id\x18\x0b \x01(\x12\x12\x12\n\nhas_passwd\x18\r \x01(\x08\x12\x11\n\tsignature\x18\x0e \x01(\t\"\x9f\x01\n\nEffectInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12%\n\ttime_type\x18\x02 \x01(\x0e\x32\x12.pb.EffectTimeType\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\x03\x12\'\n\nuse_status\x18\x04 \x01(\x0e\x32\x13.pb.EffectUseStatus\x12#\n\x0b\x65\x66\x66\x65\x63t_type\x18\x05 \x01(\x0e\x32\x0e.pb.EffectType\"\xaf\x01\n\x06\x45\x66\x66\x65\x63t\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04\x66lag\x18\x02 \x01(\x05\x12\x0b\n\x03str\x18\x03 \x01(\t\x12%\n\ttime_type\x18\x04 \x01(\x0e\x32\x12.pb.EffectTimeType\x12\x10\n\x08\x65nd_time\x18\x05 \x01(\x05\x12\'\n\nuse_status\x18\x06 \x01(\x0e\x32\x13.pb.EffectUseStatus\x12\x1c\n\x04type\x18\x07 \x01(\x0e\x32\x0e.pb.EffectType\"T\n\x0c\x45\x66\x66\x65\x63tConfig\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x1c\n\x04type\x18\x02 \x01(\x0e\x32\x0e.pb.EffectType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\"6\n\x15\x45\x66\x66\x65\x63tNicknamePendant\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x10\n\x08show_url\x18\x02 \x01(\t\"G\n\rEffectSerConf\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x1c\n\x04type\x18\x02 \x01(\x0e\x32\x0e.pb.EffectType\x12\x0c\n\x04name\x18\x03 \x01(\t\"0\n\rIndexTipRooms\x12\x0f\n\x07room_id\x18\x01 \x01(\x03\x12\x0e\n\x06tip_id\x18\x02 \x01(\x05\"=\n\x07RegisId\x12\x0b\n\x03ios\x18\x01 \x01(\t\x12\x0f\n\x07\x61ndroid\x18\x02 \x01(\t\x12\x14\n\x0cmanufacturer\x18\x03 \x01(\t\"P\n\nModelOnOff\x12\x1c\n\x05onOff\x18\x01 \x01(\x0e\x32\r.pb.OnOffType\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.pb.ModelOnOffStatus\"\xd0\x01\n\x04Rank\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x03sex\x18\x03 \x01(\x0e\x32\x0b.pb.SexType\x12\r\n\x05level\x18\x04 \x01(\r\x12\r\n\x05value\x18\x05 \x01(\x04\x12\x10\n\x08res_time\x18\x06 \x01(\r\x12\x0f\n\x07gap_val\x18\x07 \x01(\r\x12\x0c\n\x04icon\x18\x08 \x01(\t\x12\x0f\n\x07gift_id\x18\t \x01(\x04\x12\x10\n\x08gift_num\x18\n \x01(\r\x12\x0f\n\x07ranking\x18\x0b \x01(\r\x12\x11\n\tgift_name\x18\x0c \x01(\t\"5\n\x0fPlayerChairRoom\x12\x11\n\tplayer_id\x18\x01 \x01(\x03\x12\x0f\n\x07room_id\x18\x02 \x01(\x03\"l\n\x08\x43lanInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x11\n\ticon_word\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\x03\x12\x12\n\nlevel_name\x18\x05 \x01(\t\x12\x10\n\x08is_admin\x18\x06 \x01(\x08\"*\n\x06Period\x12\x10\n\x08\x62\x65gin_at\x18\x01 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x02 \x01(\x03\",\n\tLabelInfo\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63lassify_id\x18\x02 \x01(\x05\"Y\n\x13PlayerResourceShort\x12-\n\rresource_type\x18\x01 \x01(\x0e\x32\x16.pb.PlayerResourceType\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\"\x96\x01\n\x0ePlayerResource\x12-\n\rresource_type\x18\x01 \x01(\x0e\x32\x16.pb.PlayerResourceType\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x14\n\x0chead_img_url\x18\x04 \x01(\t\x12\x18\n\x03sex\x18\x05 \x01(\x0e\x32\x0b.pb.SexType\"c\n\x17PlayerResourceWithScore\x12+\n\x0fplayer_resource\x18\x01 \x01(\x0b\x32\x12.pb.PlayerResource\x12\r\n\x05score\x18\x02 \x01(\x03\x12\x0c\n\x04rank\x18\x03 \x01(\x05\"\xb4\x01\n\x13\x41ttitudeDegreesInfo\x12\x35\n\x0e\x64\x65grees_status\x18\x01 \x01(\x0e\x32\x1d.pb.AttitudeDegreesStatusType\x12\x36\n\rcategory_info\x18\x02 \x03(\x0b\x32\x1f.pb.AttitudeCategoryDegreesInfo\x12\x14\n\x0ctotal_degree\x18\x03 \x01(\x05\x12\x18\n\x10\x61nalysis_content\x18\x04 \x01(\t\"g\n\x1b\x41ttitudeCategoryDegreesInfo\x12\x13\n\x0b\x63\x61tegory_id\x18\x01 \x01(\x05\x12\x15\n\rcategory_name\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65gree\x18\x03 \x01(\x05\x12\x0c\n\x04icon\x18\x04 \x01(\t\"\x85\x01\n\x0e\x43MediaResource\x12\"\n\nmedia_type\x18\x01 \x01(\x0e\x32\x0e.pb.CMediaType\x12\x11\n\tmedia_url\x18\x02 \x01(\t\x12\x11\n\tcover_url\x18\x03 \x01(\t\x12\x13\n\x0bmedia_width\x18\x04 \x01(\x05\x12\x14\n\x0cmedia_height\x18\x05 \x01(\x05\"\x1b\n\x0bSayHelloReq\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1c\n\x0bSayHelloRes\x12\r\n\x05reply\x18\x01 \x01(\t\"b\n\x0cHeartbeatReq\x12\x0f\n\x07goim_id\x18\x01 \x01(\x03\x12\x11\n\tplayer_id\x18\x02 \x01(\x03\x12\n\n\x02ip\x18\x03 \x01(\t\x12\"\n\ndeviceType\x18\x04 \x01(\x0e\x32\x0e.pb.DeviceType\"!\n\x0cHeartbeatRes\x12\x11\n\ttimestamp\x18\x02 \x01(\x03*\xad\x01\n\tCommonErr\x12\x0f\n\x0b\x45rrCodeNone\x10\x00\x12\x11\n\x0c\x45rrCodeRedis\x10\x91N\x12\x11\n\x0c\x45rrCodeMysql\x10\x92N\x12\x15\n\x10\x45rrCodeFrequency\x10\x93N\x12\x11\n\x0c\x45rrCodeParam\x10\x94N\x12\x16\n\x11\x45rrCodeNoMatchObj\x10\x95N\x12\x10\n\x0b\x45rrCodeBusy\x10\x96N\x12\x15\n\x0f\x45rrCodeMaintain\x10\x9a\x82\x01*,\n\x07SexType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04MALE\x10\x01\x12\n\n\x06\x46\x45MALE\x10\x02*0\n\x0bOwnerInRoom\x12\x11\n\rNotInSelfRoom\x10\x00\x12\x0e\n\nInSelfRoom\x10\x01*%\n\tSceneType\x12\x0b\n\x07ST_ZERO\x10\x00\x12\x0b\n\x07ST_HOME\x10\x01*y\n\rRoomAdminType\x12\r\n\tRAT_GUEST\x10\x00\x12\x0e\n\nRAT_NORMAL\x10\n\x12\r\n\tRAT_ADMIN\x10\x14\x12\r\n\tRAT_OWNER\x10\x1e\x12\x13\n\x0fRAT_SUPER_ADMIN\x10(\x12\x16\n\tRAT_BLACK\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xfb\x01\n\nDeviceType\x12\x0e\n\nDT_UNKNOWN\x10\x00\x12\x12\n\x0e\x44T_FLASHPLAYER\x10\x01\x12\x14\n\x10\x44T_ANDROID_PHONE\x10\x14\x12\x10\n\x0c\x44T_IOS_PHONE\x10(\x12\x18\n\x14\x44T_WINDOWS_ASSISTANT\x10P\x12\x11\n\rDT_WINDOWS_PC\x10Z\x12\x0c\n\x08\x44T_ROBOT\x10\x64\x12\x1a\n\x16\x44T_WECHAT_SUBSCRIPTION\x10n\x12\x17\n\x13\x44T_QQ_SMALL_PROGRAM\x10x\x12\x17\n\x12\x44T_WX_MINI_PROGRAM\x10\x82\x01\x12\x0b\n\x06\x44T_WEB\x10\x8c\x01\x12\x0b\n\x06\x44T_MAC\x10\x96\x01*\x99\x01\n\x0bPlayerFlags\x12\x0b\n\x07PF_ZERO\x10\x00\x12\x14\n\x10PF_CERTIFICATION\x10\x01\x12\x10\n\x0cPF_BIND_BANK\x10\x04\x12\r\n\tPF_INVITE\x10\x05\x12\x13\n\x0fPF_CHARGE_FIRST\x10\x0c\x12\x18\n\x14PF_ATTITUDE_QUESTION\x10\r\x12\x17\n\x13PF_END_REGISTRATION\x10\x0e*2\n\x0c\x41\x63\x63ountFlags\x12\x0b\n\x07\x41\x46_ZERO\x10\x00\x12\x15\n\x11\x41\x46_PHONE_VERIFIED\x10\x01*\xfc\r\n\tOnOffType\x12\x0c\n\x08YEAR_BAG\x10\x00\x12\r\n\tCRACK_EGG\x10\x01\x12\x0e\n\nGOOGLE_PAY\x10\x05\x12\x0b\n\x07IAP_PAY\x10\x06\x12\n\n\x06INVITE\x10\x07\x12\x12\n\x0eINDEX_CATEGORY\x10\x08\x12\n\n\x06\x43\x45RTIF\x10\t\x12\t\n\x05GUARD\x10\n\x12\x10\n\x0cLOTTERY_DRAW\x10\x0c\x12\x0f\n\x0bMENTOR_SHIP\x10\r\x12\x0e\n\nCERTIF_IOS\x10\x0e\x12\x11\n\rREAL_IDENTITY\x10\x0f\x12\x0f\n\x0bNOVICE_GIFT\x10\x10\x12\x12\n\x0eROOM_SET_MODEL\x10\x12\x12\x11\n\rACTIVITY_TYPE\x10\x14\x12\x0c\n\x08\x41\x43TIVITY\x10\x15\x12\x0c\n\x08HOT_SONG\x10\x17\x12\x0e\n\nROOM_ENTER\x10\"\x12\x1d\n\x19ROOM_PATTERN_HIGH_QUALITY\x10#\x12\x11\n\rAUTH_LOGIN_UI\x10&\x12\x12\n\x0eUSER_DATA_EDIT\x10)\x12\x11\n\rCERTIFICATION\x10+\x12\x1b\n\x17\x43\x45RTIFICATION_ROOM_SHOW\x10,\x12%\n!CERTIFICATION_ROOM_WIN_OPEN_CLOSE\x10-\x12\x10\n\x0c\x43\x45RTIFY_WORD\x10.\x12\x11\n\rCERTIFY_CHAIR\x10/\x12\x1c\n\x18\x43\x45RTIFY_UPDATE_USER_INFO\x10\x30\x12\x1c\n\x18\x43\x45RTIFY_BROADCAST_FRIEND\x10\x31\x12\x15\n\x11\x43\x45RTIFY_HEAD_LINE\x10\x32\x12\x15\n\x11\x43\x45RTIFY_TIAO_TIAO\x10\x33\x12\x14\n\x10LOGIN_BIND_PHONE\x10\x34\x12\x1c\n\x18\x43\x45RTIFY_OWNER_ENTER_ROOM\x10\x35\x12\x0f\n\x0bYoung_Model\x10:\x12\x14\n\x10\x43USTOMER_SERVICE\x10;\x12\x15\n\x11OVERSEAS_IP_LIMIT\x10\x42\x12\x12\n\x0eOLD_NAME_LIMIT\x10\x43\x12\x12\n\x0e\x43RACK_SELF_MSG\x10\x44\x12\x12\n\x0eORDER_LOCATION\x10G\x12\x12\n\x0e\x44\x45LETE_ACCOUNT\x10I\x12\x0f\n\x0bYUNPIAN_SMS\x10J\x12\x11\n\rBIND_PHONE_V2\x10K\x12\x14\n\x10\x42IND_PHONE_LOGIN\x10L\x12\x0e\n\nCOUNT_DOWN\x10N\x12\x0e\n\nOXYGEN_BAR\x10^\x12\x13\n\x0fPRIVACY_SETTING\x10_\x12\x1f\n\x1bOXYGEN_BAR_CLAN_MEMBER_ONLY\x10`\x12\x18\n\x14OXYGEN_BAR_TREND_GIF\x10\x61\x12\x0e\n\nDATA_AUDIT\x10\x62\x12\r\n\tInner_Tec\x10\x64\x12\r\n\tInner_Ali\x10\x65\x12\x16\n\x12\x43\x45RTIFY_IM_PICTURE\x10g\x12\x0b\n\x07\x43MB_VIP\x10h\x12\x13\n\x0f\x43RACKEGG_FOREST\x10i\x12\x13\n\x0e\x41NTI_ADDICTION\x10\xc8\x01\x12&\n!TEXT_FILTER_ROOM_SCREEN_ENCRYPTED\x10\xc9\x01\x12(\n#TEXT_FILTER_ROOM_SCREEN_UNENCRYPTED\x10\xca\x01\x12!\n\x1cTEXT_FILTER_BROADCAST_FRIEND\x10\xcb\x01\x12\x1d\n\x18TEXT_FILTER_PRIVATE_CHAT\x10\xcc\x01\x12\x10\n\x0c\x42\x43_HEAD_LINE\x10n\x12\x13\n\x0fONE_CLICK_LOGIN\x10o\x12\x0e\n\nCERTIFY_PM\x10p\x12\x13\n\x0f\x43\x45RTIFY_PICTURE\x10q\x12\x19\n\x15\x43HANNEL_ADVERT_AUDITS\x10r\x12\x1a\n\x16\x43\x45RTIFY_CREATE_CHANNEL\x10t\x12\x18\n\x14\x43\x45RTIFY_JOIN_CHANNEL\x10u\x12\x10\n\x0c\x43\x45RTIFY_GIVE\x10v\x12\x17\n\x13\x43\x45RTIFY_ROOM_NOTICE\x10w\x12\x14\n\x10\x43\x45RTIFY_RECHARGE\x10x\x12\x19\n\x15\x43\x45RTIFY_PUBLISH_TREND\x10y\x12\x19\n\x15\x43\x45RTIFY_COMMENT_TREND\x10z\x12\x11\n\rHOME_NAV_TYPE\x10{\x12\x11\n\rLOGIN_CHECKED\x10|\x12\x0e\n\nHIGH_SOUND\x10}\x12\x16\n\x12HIGH_SOUND_CHANNEL\x10~\x12\x1a\n\x16\x43HANNEL_STAR_CHALLENGE\x10\x7f\x12\x11\n\x0c\x43HANNEL_STAT\x10\x80\x01\x12\x11\n\x0cREGISTER_SEX\x10\x82\x01\x12\x16\n\x11REGISTER_NICKNAME\x10\x83\x01\x12\x16\n\x11REGISTER_ATTITUDE\x10\x84\x01\x12\x13\n\x0e\x43REATE_CHANNEL\x10\x85\x01\x12\x1a\n\x15\x43OMMUNITY_TREND_AUDIO\x10\x86\x01\x12\x0c\n\x07IM_TIPS\x10\x87\x01\x12\x18\n\x13MULTI_CLIENT_ONLINE\x10\xfd\x01*)\n\nStatusCode\x12\x0b\n\x07SC_FAIL\x10\x00\x12\x0e\n\nSC_SUCCESS\x10\x01*?\n\nEffectType\x12\x12\n\x0e\x45\x66\x66\x65\x63tTypeNone\x10\x00\x12\x1d\n\x19\x45\x66\x66\x65\x63tTypeNicknamePendant\x10\x01*\x7f\n\x0e\x45\x66\x66\x65\x63tTimeType\x12\x18\n\x14\x45\x66\x66\x65\x63tTimeTypeAlways\x10\x00\x12\x16\n\x12\x45\x66\x66\x65\x63tTimeTypeMike\x10\x01\x12\x1e\n\x1a\x45\x66\x66\x65\x63tTimeTypeWearInPacket\x10\x02\x12\x1b\n\x17\x45\x66\x66\x65\x63tTimeTypePermanent\x10\x03*,\n\x0f\x45\x66\x66\x65\x63tUseStatus\x12\n\n\x06\x45S_Use\x10\x00\x12\r\n\tES_NotUse\x10\x01*I\n\x10\x45\x66\x66\x65\x63tNoticeType\x12\x18\n\x14\x45\x66\x66\x65\x63tNoticeTypeGain\x10\x00\x12\x1b\n\x17\x45\x66\x66\x65\x63tNoticeTypeTimeout\x10\x01*:\n\x10ModelOnOffStatus\x12\x0b\n\x07\x41LL_OFF\x10\x00\x12\n\n\x06\x41LL_ON\x10\x01\x12\r\n\tWHITELIST\x10\x02*A\n\x08RankType\x12\x0b\n\x07RT_ZERO\x10\x00\x12\x0c\n\x08RT_CHARM\x10\x01\x12\r\n\tRT_WEALTH\x10\x02\x12\x0b\n\x07RT_GIFT\x10\x03*N\n\rLoadClickType\x12\x0c\n\x08LCT_ZERO\x10\x00\x12\x17\n\x13LCT_INTIMATE_DETAIL\x10\x01\x12\x16\n\x12LCT_INTIMATE_STORE\x10\x02*F\n\x0b\x41uditStatus\x12\x11\n\rAS_Audit_Pass\x10\x00\x12\x0f\n\x0b\x41S_Auditing\x10\x01\x12\x13\n\x0f\x41S_Audit_Refuse\x10\x02*\xf3\x01\n\nUploadType\x12\x0c\n\x08TypeZero\x10\x00\x12\x10\n\x0cHeadAlbumImg\x10\x01\x12\x0f\n\x0bHeadIconImg\x10\x02\x12\x0f\n\x0b\x44ynamicsImg\x10\x03\x12\r\n\tClientLog\x10\x04\x12\x0e\n\nTipOffsImg\x10\x05\x12\x0c\n\x08Indetity\x10\x06\x12\x0b\n\x07PMMedia\x10\x07\x12\t\n\x05Voice\x10\x08\x12\x11\n\rBackgroundImg\x10\x17\x12\x0f\n\x0b\x43hannelIcon\x10\x18\x12\x11\n\rWXRobotQRcode\x10\x19\x12\x13\n\x0f\x43ommunityTagImg\x10\x1c\x12\x12\n\x0ePersonLabelImg\x10\x1d*\xe9\x01\n\x0ePayChannelType\x12\x0c\n\x08PCT_NULL\x10\x00\x12\x11\n\rPCT_ALIPAY_H5\x10\x02\x12\x12\n\x0ePCT_ALIPAY_APP\x10\x03\x12\x11\n\rPCT_WXPAY_APP\x10\x04\x12\x10\n\x0cPCT_WXPAY_H5\x10\x05\x12\x0b\n\x07PCT_IAP\x10\x06\x12\x0c\n\x08PCT_PLAY\x10\x08\x12\x0e\n\nPCT_PAYPAL\x10\n\x12\r\n\tPCT_BOING\x10\x0b\x12\x10\n\x0cPCT_UNIONPAY\x10\x0c\x12\x0e\n\tPCT_AGENT\x10\xfd\x01\x12\x0f\n\nPCT_MANUAL\x10\xfe\x01\x12\x10\n\x0bPCT_DEVTEST\x10\xff\x01*i\n\x04Role\x12\n\n\x06R_NONE\x10\x00\x12\x0f\n\x0bR_SUPERUSER\x10\x01\x12\x08\n\x04R_OW\x10\x02\x12\x08\n\x04R_VP\x10\x03\x12\x08\n\x04R_MA\x10\x04\x12\t\n\x05R_CA1\x10\x05\x12\t\n\x05R_CA2\x10\x06\x12\x07\n\x03R_R\x10\x07\x12\x07\n\x03R_U\x10\x08*]\n\x0eNameplateStyle\x12\x0b\n\x07NS_NONE\x10\x00\x12\x0e\n\nNS_STYLE_1\x10\x01\x12\x0e\n\nNS_STYLE_2\x10\x02\x12\x0e\n\nNS_STYLE_3\x10\x03\x12\x0e\n\nNS_STYLE_4\x10\x04*E\n\x12PlayerResourceType\x12\x0c\n\x08PRT_NONE\x10\x00\x12\x15\n\x11PRT_FIRST_ACCOUNT\x10\x01\x12\n\n\x06PRT_WX\x10\x02*f\n\x19\x41ttitudeDegreesStatusType\x12\x13\n\x0f\x41\x44ST_BOTH_EVERY\x10\x00\x12\x17\n\x13\x41\x44ST_OPPOSITE_EVERY\x10\x01\x12\x1b\n\x17\x41\x44ST_OPPOSITE_NOTENOUGH\x10\x02*u\n\nCMediaType\x12\x13\n\x0f\x43MediaType_None\x10\x00\x12\x12\n\x0e\x43MediaType_Png\x10\x01\x12\x12\n\x0e\x43MediaType_Gif\x10\x02\x12\x14\n\x10\x43MediaType_Video\x10\x03\x12\x14\n\x10\x43MediaType_Audio\x10\x04*w\n\x11\x44\x65viceConnectOper\x12\x0c\n\x08\x44\x43S_None\x10\x00\x12\x12\n\x0e\x44\x43S_Requesting\x10\x01\x12\x0f\n\x0b\x44\x43S_Receive\x10\x02\x12\x0e\n\nDCS_Refuse\x10\x03\x12\x0f\n\x0b\x44\x43S_Timeout\x10\x04\x12\x0e\n\nDCS_Cancel\x10\x05*\xa7\x01\n\x0b\x44\x65viceCmdId\x12\x11\n\rDC_DeviceZero\x10\x00\x12\x14\n\x0e\x44\x43_DeviceLogin\x10\x99\x98\x1f\x12\x1e\n\x18\x44\x43_MessageConnectOperate\x10\x9a\x98\x1f\x12\x1c\n\x16\x44\x43_MessageStatusUpdate\x10\x9b\x98\x1f\x12\x1a\n\x14\x44\x43_DeviceShareStatus\x10\x9c\x98\x1f\x12\x15\n\x0f\x44\x43_SingoConnect\x10\xb9\xa5%*L\n\nTaskStatus\x12\x0b\n\x07TS_None\x10\x00\x12\x11\n\rTS_Processing\x10\x01\x12\x0e\n\nTS_Success\x10\x02\x12\x0e\n\nTS_Failure\x10\x03*N\n\x08TaskType\x12\x0b\n\x07TT_None\x10\x00\x12\x0c\n\x08TT_Image\x10\x01\x12\x0c\n\x08TT_Video\x10\x02\x12\x0c\n\x08TT_Audio\x10\x03\x12\x0b\n\x07TT_Text\x10\x04*C\n\tLabelType\x12\x0b\n\x07LT_NONE\x10\x00\x12\x0b\n\x07LT_POST\x10\x01\x12\x0e\n\nLT_Gallery\x10\x02\x12\x0c\n\x08LT_Group\x10\x03*N\n\x08\x41igcType\x12\x0b\n\x07\x41T_NONE\x10\x00\x12\x0c\n\x08\x41T_IMAGE\x10\x01\x12\x0c\n\x08\x41T_VIDEO\x10\x02\x12\x0c\n\x08\x41T_AUDIO\x10\x03\x12\x0b\n\x07\x41T_TEXT\x10\x04\x42\x06\xa2\x02\x03PB3b\x06proto3')
 
 _COMMONERR = DESCRIPTOR.enum_types_by_name['CommonErr']
 CommonErr = enum_type_wrapper.EnumTypeWrapper(_COMMONERR)
 _SEXTYPE = DESCRIPTOR.enum_types_by_name['SexType']
 SexType = enum_type_wrapper.EnumTypeWrapper(_SEXTYPE)
 _OWNERINROOM = DESCRIPTOR.enum_types_by_name['OwnerInRoom']
 OwnerInRoom = enum_type_wrapper.EnumTypeWrapper(_OWNERINROOM)
@@ -75,22 +75,14 @@
 TaskStatus = enum_type_wrapper.EnumTypeWrapper(_TASKSTATUS)
 _TASKTYPE = DESCRIPTOR.enum_types_by_name['TaskType']
 TaskType = enum_type_wrapper.EnumTypeWrapper(_TASKTYPE)
 _LABELTYPE = DESCRIPTOR.enum_types_by_name['LabelType']
 LabelType = enum_type_wrapper.EnumTypeWrapper(_LABELTYPE)
 _AIGCTYPE = DESCRIPTOR.enum_types_by_name['AigcType']
 AigcType = enum_type_wrapper.EnumTypeWrapper(_AIGCTYPE)
-_MODULE = DESCRIPTOR.enum_types_by_name['Module']
-Module = enum_type_wrapper.EnumTypeWrapper(_MODULE)
-_WIDGETTYPE = DESCRIPTOR.enum_types_by_name['WidgetType']
-WidgetType = enum_type_wrapper.EnumTypeWrapper(_WIDGETTYPE)
-_CALCULATEMODE = DESCRIPTOR.enum_types_by_name['CalculateMode']
-CalculateMode = enum_type_wrapper.EnumTypeWrapper(_CALCULATEMODE)
-_CHARGECATETYPE = DESCRIPTOR.enum_types_by_name['ChargeCateType']
-ChargeCateType = enum_type_wrapper.EnumTypeWrapper(_CHARGECATETYPE)
 ErrCodeNone = 0
 ErrCodeRedis = 10001
 ErrCodeMysql = 10002
 ErrCodeFrequency = 10003
 ErrCodeParam = 10004
 ErrCodeNoMatchObj = 10005
 ErrCodeBusy = 10006
@@ -310,33 +302,19 @@
 TT_Video = 2
 TT_Audio = 3
 TT_Text = 4
 LT_NONE = 0
 LT_POST = 1
 LT_Gallery = 2
 LT_Group = 3
-LT_Comment = 4
-LT_Lora = 5
-LT_Client = 6
 AT_NONE = 0
 AT_IMAGE = 1
 AT_VIDEO = 2
 AT_AUDIO = 3
 AT_TEXT = 4
-M_None = 0
-M_Subscribe = 1
-WT_None = 0
-WT_General = 1
-WT_SD = 2
-WT_Lora = 3
-CM_None = 0
-CM_Single = 1
-CM_Minute = 2
-CCT_Normal = 0
-CCT_ActCard = 1
 
 
 _PLAYER = DESCRIPTOR.message_types_by_name['Player']
 _USERINFO = DESCRIPTOR.message_types_by_name['UserInfo']
 _PLAYERINFO = DESCRIPTOR.message_types_by_name['PlayerInfo']
 _BAGITEM = DESCRIPTOR.message_types_by_name['BagItem']
 _AGODAKEY = DESCRIPTOR.message_types_by_name['AgodaKey']
@@ -634,25 +612,17 @@
   _DEVICECMDID._serialized_start=7893
   _DEVICECMDID._serialized_end=8060
   _TASKSTATUS._serialized_start=8062
   _TASKSTATUS._serialized_end=8138
   _TASKTYPE._serialized_start=8140
   _TASKTYPE._serialized_end=8218
   _LABELTYPE._serialized_start=8220
-  _LABELTYPE._serialized_end=8331
-  _AIGCTYPE._serialized_start=8333
-  _AIGCTYPE._serialized_end=8411
-  _MODULE._serialized_start=8413
-  _MODULE._serialized_end=8450
-  _WIDGETTYPE._serialized_start=8452
-  _WIDGETTYPE._serialized_end=8517
-  _CALCULATEMODE._serialized_start=8519
-  _CALCULATEMODE._serialized_end=8577
-  _CHARGECATETYPE._serialized_start=8579
-  _CHARGECATETYPE._serialized_end=8628
+  _LABELTYPE._serialized_end=8287
+  _AIGCTYPE._serialized_start=8289
+  _AIGCTYPE._serialized_end=8367
   _PLAYER._serialized_start=25
   _PLAYER._serialized_end=400
   _USERINFO._serialized_start=403
   _USERINFO._serialized_end=532
   _PLAYERINFO._serialized_start=535
   _PLAYERINFO._serialized_end=878
   _BAGITEM._serialized_start=880
```

### Comparing `mecord-cli-0.1.87/mecord/rpcinput_pb2.py` & `mecord-cli-0.1.9/mecord/rpcinput_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.87/mecord/script_template/main.py` & `mecord-cli-0.1.9/mecord/script_template/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 def main(cmd_opts):
     if cmd_opts.run == None or cmd_opts.out == None:
         print("args fail!")
         return
     
     if os.path.exists(cmd_opts.run):
-        with open(cmd_opts.run, 'r', encoding='UTF-8') as f:
+        with open(cmd_opts.run, 'r') as f:
             data = json.load(f)
     result = runTask(data)
     with open(cmd_opts.out, 'w') as f:
         json.dump(result, f)
 
 if __name__ == '__main__':
+    subprocess.run(f"mecord widget add {os.getcwd()}", stdout=None)
     main(cmd_opts)
```

### Comparing `mecord-cli-0.1.87/mecord/script_template/run.py` & `mecord-cli-0.1.9/mecord/script_template/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,13 +23,13 @@
     demoReturnText = "hello world"
     
     resultDic["result"].append({
         "type" : "text",
         "content": [ 
             demoReturnText
         ],
-        "extension" : {
+        "extention" : {
             "info": "",
             "cover_url": ""
         }
     })
     return resultDic
```

### Comparing `mecord-cli-0.1.87/mecord/uauth_common_pb2.py` & `mecord-cli-0.1.9/mecord/uauth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.87/mecord/uauth_ext_pb2.py` & `mecord-cli-0.1.9/mecord/uauth_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.87/mecord/user_status_ext_pb2.py` & `mecord-cli-0.1.9/mecord/user_status_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.87/mecord/widget_template/MekongJS.js.py` & `mecord-cli-0.1.9/mecord/widget_template/MekongJS.js.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.87/mecord/widget_template/icon.png.py` & `mecord-cli-0.1.9/mecord/widget_template/icon.png.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.87/mecord/widget_template/index.html.py` & `mecord-cli-0.1.9/mecord/widget_template/index.html.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.87/mecord/xy_pb.py` & `mecord-cli-0.1.9/mecord/xy_pb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,327 +1,235 @@
 import json
 import hashlib
 import time
-import socket
 import requests
-import urllib3
-import os
-import random
 
 from mecord import uauth_common_pb2 
 from mecord import uauth_ext_pb2 
 from mecord import common_ext_pb2 
 from mecord import aigc_ext_pb2 
 from mecord import rpcinput_pb2 
 from mecord import store 
 from mecord import utils 
 from mecord import constant 
 
+uuid = utils.generate_unique_id()
+
 def _aigc_post(request, function):
-    domain = None
-    token = None
-    if store.is_product():
-        domain = "https://api.mecordai.com/proxymsg"
-        token = "NDl8NWU5OGI1ODk4N2ExNTZmZWE1MmI4YzM3MTNjNjI0MDd8ZjI2MzYwZTA2ZWVkODg0Y2ZlNjZlZTBlNzVhZDM1OWY="
-    else:
-        domain = "https://mecord-beta.2tianxin.com/proxymsg"
-        token = store.token()
-    return _post(url=domain, 
+    return _post(url="https://mecord-beta.2tianxin.com/proxymsg", 
                  objStr="mecord.aigc.AigcExtObj", 
                  request=request, 
-                 function=function,
-                 token=token)
-
-def _post(url, objStr, request, function, token):
+                 function=function)
+    
+def _common_post(request, function):
+    return _post(url="https://beta.xiaohuxi.cn/proxymsg", 
+                 objStr="mizacommon.uauth.AuthExtObj", 
+                 request=request, 
+                 function=function)
+    
+def _post(url, objStr, request, function):
     req = request.SerializeToString()
     opt = {
         "lang": "zh-Hans",
         "region": "CN",
         "appid": "80",
         "application": "mecord",
         "version": "1.0",
-        "X-Token": token,
+        "X-Token": store.token(),
         "uid": "1",
     }
     input_req = rpcinput_pb2.RPCInput(obj=objStr, func=function, req=req, opt=opt)
-    try:
-        requests.adapters.DEFAULT_RETRIES = 2
-        s = requests.session()
-        s.keep_alive = False
-        s.headers.update({'Connection':'close'})
-        res = s.post(url=url, data=input_req.SerializeToString())
-        res.close()
-        pb_rsp = rpcinput_pb2.RPCOutput()
-        pb_rsp.ParseFromString(res.content)
-        s.close()
-    except UnicodeDecodeError as e:
-        return -1, f"url decode error : {e}", "" 
-    except socket.timeout as e:
-        return -1, "mecord server timeout", "" 
-    except Exception as e:
-        print(f'''mecord server error
-url={url}
-func={function}
-token={token}
-
-exception={e}
-''')
-        return -1, str(e), "" 
+    res = requests.post(url=url, data=input_req.SerializeToString())
+    pb_rsp = rpcinput_pb2.RPCOutput()
+    pb_rsp.ParseFromString(res.content)
     if pb_rsp.ret == 0:
         return 0, "", pb_rsp.rsp
     else:
-        print(f'''request err_code={pb_rsp.ret} err_desc={pb_rsp.desc}
-url={url}
-func={function}
-token={token}
-
-req=
-{request}
-
-respose=
-{res.content}
-''')
+        # print(pb_rsp)
         return pb_rsp.ret, pb_rsp.desc, "" 
     
-def GetTask():
+
+def GetQrcodeLoginCode():
+    req = uauth_ext_pb2.GetQrcodeLoginCodeReq()
+    req.login_type = uauth_common_pb2.UauthLoginType.LT_QRCODE_SCAN
+    req.device_type = uauth_common_pb2.UauthDeviceType.DT_WINDOWS_PC
+    req.device_id = uuid
+    req.u_meng_device_id = ""
+
+    rsp = uauth_ext_pb2.GetQrcodeLoginCodeRes()
+    r1, r2, r3 = _common_post(req, "GetQrcodeLoginCode")
+    if r1 != 0:
+        print(r2)
+        return None
+    rsp.ParseFromString(r3)
+    s = rsp.login_code
+    return s
+
+def CheckLoginLoop(code):
+    req = uauth_ext_pb2.GetQrcodeLoginStatusReq()
+    req.login_code = code
+    req.device_id = uuid
+    req.u_meng_device_id = ""
+
+    rsp = uauth_ext_pb2.GetQrcodeLoginStatusRes()
+    r1, r2, r3 = _common_post(req, "GetQrcodeLoginStatus")
+    if r1 != 0:
+        print(r2)
+        return 0
+    rsp.ParseFromString(r3)
+    if rsp.status == uauth_ext_pb2.GetQrcodeLoginStatus.SUCCESS:
+        sp = store.Store()
+        data = sp.read()
+        data["uid"] = rsp.commonSignInRes.user_id
+        data["token"] = rsp.commonSignInRes.login_token
+        data["nickname"] = rsp.userNickname
+        data["icon"] = rsp.userIconUrl
+        sp.write(data)
+        return 1
+    elif rsp.status == uauth_ext_pb2.GetQrcodeLoginStatus.EXPIRED or rsp.status == uauth_ext_pb2.GetQrcodeLoginStatus.CANCEL:
+        return 0
+    else:
+        return -1
+    
+def GetTask(token):
     req = aigc_ext_pb2.GetTaskReq()
-    req.version = constant.app_version
-    req.DeviceKey = utils.generate_unique_id()
+    req.DeviceKey = uuid
     map = store.widgetMap()
     for it in map:
-        if isinstance(map[it], (dict)):
-            if map[it]["isBlock"] == False:
-                req.widgets.append(it)
-        else:
-            req.widgets.append(it)
-    if store.is_product():
-        req.token = "NDl8NWU5OGI1ODk4N2ExNTZmZWE1MmI4YzM3MTNjNjI0MDd8ZjI2MzYwZTA2ZWVkODg0Y2ZlNjZlZTBlNzVhZDM1OWY="
-    else:
-        req.token = store.token()
-    req.limit = store.multitaskNum()
+        req.widgets.append(it)
+    req.token = token
+    req.limit = 1
     extInfo = store.readDeviceInfo()
     extInfo["app_version"] = constant.app_version
     extInfo["app_bulld_number"] = constant.app_bulld_number
     extInfo["app_name"] = constant.app_name
     req.extend = json.dumps(extInfo)
 
     rsp = aigc_ext_pb2.GetTaskRes()
     r1, r2, r3 = _aigc_post(req, "GetTask")
     if r1 != 0:
+        print(r2)
         return []
     rsp.ParseFromString(r3)
     datas = []
     for it in rsp.list:
         datas.append({
             "taskUUID": it.taskUUID,
             "pending_count": rsp.count - rsp.limit,
             "config": it.config,
             "data": it.data,
         })
     return datas
 
 def TaskNotify(taskUUID, status, msg, dataStr):
     req = aigc_ext_pb2.TaskNotifyReq()
-    req.version = constant.app_version
     req.taskUUID = taskUUID
     if status:
         req.taskStatus = common_ext_pb2.TaskStatus.TS_Success
     else:
         req.taskStatus = common_ext_pb2.TaskStatus.TS_Failure
     req.failReason = msg
     req.data = dataStr
-    
 
     rsp = aigc_ext_pb2.TaskNotifyRes()
     r1, r2, r3 = _aigc_post(req, "TaskNotify")
     if r1 != 0:
+        print(r2)
         return False
     rsp.ParseFromString(r3)
     return True
 
-def DeviceUnbind():
-    req = aigc_ext_pb2.AigcDeviceUnBindReq()
-    req.deviceToken = store.token()
-
-    rsp = aigc_ext_pb2.AigcDeviceUnBindRes()
-    r1, r2, r3 = _aigc_post(req, "DeviceUnBind")
-    if r1 != 0:
-        return False
-    rsp.ParseFromString(r3)
-    return False
-
 def GetAigcDeviceInfo():
     req = aigc_ext_pb2.AigcDeviceInfoReq()
-    req.version = constant.app_version
-    req.deviceKey = utils.generate_unique_id()
-    extInfo = store.readDeviceInfo()
-    extInfo["app_version"] = constant.app_version
-    extInfo["app_bulld_number"] = constant.app_bulld_number
-    extInfo["app_name"] = constant.app_name
-    req.extend = json.dumps(extInfo)
+    req.deviceKey = uuid
 
     rsp = aigc_ext_pb2.AigcDeviceInfoRes()
     r1, r2, r3 = _aigc_post(req, "DeviceInfo")
     if r1 != 0:
-        if r1 != 11000:
-            print(f'get DeviceInfo failed: {r1} {r2}')
+        print(r2)
         return False
     rsp.ParseFromString(r3)
-    
+    print(f"====={rsp}")
     if len(rsp.groupUUID) > 0:
         sp = store.Store()
         data = sp.read()
         data["groupUUID"] = rsp.groupUUID
         data["token"] = rsp.token
         if rsp.isCreateWidget == True:
             data["isCreateWidget"] = rsp.isCreateWidget
         sp.write(data)
         return True
     return False
 
 def CreateWidgetUUID():
-    req = aigc_ext_pb2.ApplyWidgetReq()
-    rsp = aigc_ext_pb2.ApplyWidgetRes()
-    r1, r2, r3 = _aigc_post(req, "ApplyWidget")
+    req = aigc_ext_pb2.CreateWidgetReq()
+    rsp = aigc_ext_pb2.CreateWidgetRes()
+    r1, r2, r3 = _aigc_post(req, "CreateWidget")
     if r1 != 0:
+        print(r2)
         return ""
     rsp.ParseFromString(r3)
     return rsp.widgetUUID
 
-def DeleteWidget(widgetid):
-    req = aigc_ext_pb2.DeleteAigcWidgetReq()
-    req.widgetUUID = widgetid
-    req.deviceToken = store.token()
-    rsp = aigc_ext_pb2.DeleteAigcWidgetRes()
-    r1, r2, r3 = _aigc_post(req, "DeleteWidget")
-    if r1 != 0:
-        return False
-    rsp.ParseFromString(r3)
-    return True
-
-def GetTaskCount(widgetid):
-    req = aigc_ext_pb2.TaskCountReq()
-    req.deviceToken = store.token()
-    rsp = aigc_ext_pb2.TaskCountRes()
-    r1, r2, r3 = _aigc_post(req, "TaskCount")
-    if r1 != 0:
-        return []
-    rsp.ParseFromString(r3)
-    datas = []
-    for it in rsp.items:
-        datas.append({
-            "widgetUUID": it.widgetUUID,
-            "taskCount": it.taskCount
-        })
-    return datas
-
-def RemoteWidgetList(widgetid):
-    req = aigc_ext_pb2.AigcWidgetListReq()
-    req.deviceToken = store.token()
-    rsp = aigc_ext_pb2.AigcWidgetListRes()
-    r1, r2, r3 = _aigc_post(req, "WidgetList")
-    if r1 != 0:
-        return []
-    rsp.ParseFromString(r3)
-    datas = []
-    for it in rsp.items:
-        datas.append({
-            "uuid": it.uuid,
-            "name": it.name,
-            "updated_at": it.updated_at,
-        })
-    return datas
-
-def ExpansionWithToken(token):
-    req = aigc_ext_pb2.AigcDeviceExpansionReq()
-    req.DeviceToken = token
-    req.DeviceKey = utils.generate_unique_id()
-
-    rsp = aigc_ext_pb2.AigcDeviceExpansionRes()
-    r1, r2, r3 = _aigc_post(req, "DeviceExpansion")
-    if r1 == 11000:
-        return False, r1
-    elif r1 != 0:
-        return ""
-    rsp.ParseFromString(r3)
-
-    if len(rsp.groupUUID) > 0:
-        sp = store.Store()
-        data = sp.read()
-        data["groupUUID"] = rsp.groupUUID
-        data["token"] = rsp.deviceToken
-        sp.write(data)
-        return True, 0
-    return False, -1
- 
 def GetOssUrl(ext):
     req = aigc_ext_pb2.UploadFileUrlReq()
-    if store.is_product():
-        req.token = "NDl8NWU5OGI1ODk4N2ExNTZmZWE1MmI4YzM3MTNjNjI0MDd8ZjI2MzYwZTA2ZWVkODg0Y2ZlNjZlZTBlNzVhZDM1OWY="
-    else:
-        req.token = store.token()
-    req.version = constant.app_version
+    req.token = store.token()
+    req.version = constant.app_bulld_number
     req.fileExt = ext
 
     rsp = aigc_ext_pb2.UploadFileUrlRes()
     r1, r2, r3 = _aigc_post(req, "UploadFileUrl")
     if r1 != 0:
-        return "", ""
+        print(r2)
+        return ""
     rsp.ParseFromString(r3)
     return rsp.url, rsp.contentType
-   
+    
 def GetWidgetOssUrl(widgetid):
     req = aigc_ext_pb2.UploadWidgetUrlReq()
-    req.version = constant.app_version
     req.widgetUUID = widgetid
 
     rsp = aigc_ext_pb2.UploadWidgetUrlRes()
     r1, r2, r3 = _aigc_post(req, "UploadWidgetUrl")
     if r1 != 0:
-        return "", ""
+        print(r2)
+        return ""
     rsp.ParseFromString(r3)
     return rsp.url, rsp.contentType
 
 def WidgetUploadEnd(url):
     req = aigc_ext_pb2.UploadWidgetReq()
-    req.version = constant.app_version
     req.fileUrl = url
     
     rsp = aigc_ext_pb2.UploadWidgetRes()
     r1, r2, r3 = _aigc_post(req, "UploadWidget")
     if r1 != 0:
+        print(r2)
         return 0
     rsp.ParseFromString(r3)
     return rsp.checkId
+
+# def PublishWidget(widgetid, oss_path):
+#     req = aigc_ext_pb2.UploadWidgetReq()
+#     req.fileUrl = oss_path
+
+#     rsp = aigc_ext_pb2.UploadWidgetRes()
+#     rsp.ParseFromString(_aigc_post(req, "UploadWidget"))
+#     return rsp.uploadId
     
 def UploadWidgetCheck(checkId):
     req = aigc_ext_pb2.UploadWidgetCheckReq()
-    req.version = constant.app_version
     req.checkId = checkId
 
     rsp = aigc_ext_pb2.UploadWidgetCheckRes()
     r1, r2, r3 = _aigc_post(req, "UploadWidgetCheck")
     if r1 != 0:
+        print(r2)
         return 0
     rsp.ParseFromString(r3)
     if rsp.status == aigc_ext_pb2.UploadWidgetStatus.UWS_SUCCESS:
         return 1
     elif rsp.status == aigc_ext_pb2.UploadWidgetStatus.UWS_FAILURE:
-        print(f"widget pulish fail msg => {rsp.failReason}")
+        print(f"failReason = {rsp.failReason}")
         return 0
     else:
         return -1
-
-def UploadMarketModel(name, cover, model_url, type, taskuuid):
-    req = aigc_ext_pb2.MarketModelCreateWithTaskReq()
-    req.name = name
-    req.cover = cover
-    req.url = model_url
-    req.type = type
-    req.TaskUUID = taskuuid
-
-    rsp = aigc_ext_pb2.MarketModelCreateWithTaskRes()
-    r1, r2, r3 = _aigc_post(req, "MarketModelCreateWithTask")
-    if r1 != 0:
-        return 0
-    rsp.ParseFromString(r3)
-    return True
```

### Comparing `mecord-cli-0.1.87/mecord/xy_user.py` & `mecord-cli-0.1.9/mecord/xy_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,32 +40,33 @@
     
     def logout(self):
         store.clear()
         self.logined = False
 
     def loginIfNeed(self):
         if xy_pb.GetAigcDeviceInfo():
+            print("login success")
             self.checkLoginStatus()
 
     #     if self.isLogin() == False:
     #         #need login
     #         logincode = xy_pb.GetQrcodeLoginCode()
     #         if logincode:
-    #             logincode_encoded = base64.b64encode(bytes(logincode, encoding='UTF-8')).decode(encoding='UTF-8').replace("==","fuckEqual")
+    #             logincode_encoded = base64.b64encode(bytes(logincode, 'utf-8')).decode('utf-8').replace("==","fuckEqual")
     #             uuid = utils.generate_unique_id()
     #             qrcode = f"https://main_page.html?action=scan&code={logincode_encoded}&deviceCode=143383612&deviceId={uuid}"
     #             utils.displayQrcode(qrcode)
     #             # qrcode_terminal.draw(qrcode)
     #             # print(qrcode)
     #             # utils.displayQRcodeOnTerminal(qrcode)
-    #             self.checkLoginComplete(logincode)
-    #             print("waiting for scan qrcode & login complete ~~~")
+    #             self.checkLoginComplate(logincode)
+    #             print("waiting for scan qrcode & login complate ~~~")
 
-    # def checkLoginComplete(self, qrcode):
+    # def checkLoginComplate(self, qrcode):
     #     rst = xy_pb.CheckLoginLoop(qrcode)
     #     if rst == 1: #success
     #         print("login success")
     #         self.logined = True
     #     elif rst == -1:
-    #         threading.Timer(1, self.checkLoginComplete, (qrcode, )).start()
+    #         threading.Timer(1, self.checkLoginComplate, (qrcode, )).start()
     #     else: #fail
     #         print("login fail !!!")
```

### Comparing `mecord-cli-0.1.87/mecord_cli.egg-info/SOURCES.txt` & `mecord-cli-0.1.9/mecord_cli.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 LICENSE
 README.md
 setup.py
 mecord/__init__.py
 mecord/aigc_ext_pb2.py
-mecord/capability_provider.py
 mecord/common_ext_pb2.py
 mecord/constant.py
+mecord/ftp_upload.py
 mecord/main.py
 mecord/mecord_service.py
 mecord/mecord_widget.py
-mecord/progress_monitor.py
 mecord/rpcinput_pb2.py
 mecord/store.py
 mecord/uauth_common_pb2.py
 mecord/uauth_ext_pb2.py
 mecord/upload.py
 mecord/user_status_ext_pb2.py
 mecord/utils.py
 mecord/xy_pb.py
+mecord/xy_socket.py
 mecord/xy_user.py
-mecord/public_tools/__init__.py
-mecord/public_tools/decorator_tools.py
 mecord/script_template/__init__.py
-mecord/script_template/launch.py
 mecord/script_template/main.py
 mecord/script_template/run.py
 mecord/widget_template/MekongJS.js.py
 mecord/widget_template/__init__.py
 mecord/widget_template/config.json.py
 mecord/widget_template/icon.png.py
 mecord/widget_template/index.html.py
```

