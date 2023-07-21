# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.6.1.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.6.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.6.2.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.6.1.tar` & `nonebot_plugin_talk_with_chatgpt-0.6.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10755 2023-06-27 15:17:02.686329 nonebot_plugin_talk_with_chatgpt-0.6.1/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0    14035 2023-06-06 06:18:10.409339 nonebot_plugin_talk_with_chatgpt-0.6.1/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     6397 2023-06-06 06:12:19.089000 nonebot_plugin_talk_with_chatgpt-0.6.1/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_chatgpt-0.6.1/nonebot_plugin_talk_with_chatgpt/HYWenHei-85W.ttf
--rw-r--r--   0        0        0      994 2023-06-28 03:41:50.273493 nonebot_plugin_talk_with_chatgpt-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6040 2023-06-28 03:42:12.597928 nonebot_plugin_talk_with_chatgpt-0.6.1/README.md
--rw-r--r--   0        0        0     6978 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    10755 2023-06-27 15:17:02.686329 nonebot_plugin_talk_with_chatgpt-0.6.2/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0    14035 2023-06-06 06:18:10.409339 nonebot_plugin_talk_with_chatgpt-0.6.2/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     6491 2023-07-21 03:41:30.636256 nonebot_plugin_talk_with_chatgpt-0.6.2/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_chatgpt-0.6.2/nonebot_plugin_talk_with_chatgpt/HYWenHei-85W.ttf
+-rw-r--r--   0        0        0      994 2023-07-21 03:42:37.363277 nonebot_plugin_talk_with_chatgpt-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6178 2023-07-21 03:43:10.970723 nonebot_plugin_talk_with_chatgpt-0.6.2/README.md
+-rw-r--r--   0        0        0     7112 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.6.2/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.6.1/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.6.2/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.6.1/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.6.2/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.6.1/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.6.2/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,21 @@
         if operation == "rename" or operation == "delete":
             return ""
         # 响应码
         resp_code = resp.status_code
         # 先存着结果，如果报错了用于判断
         err_msg = resp.text
         # 提取回答
-        json_data = loads(resp.text.split("\n\n")[-3][6:])
+        pre_data = resp.text.split("\n\n")
+        json_data = loads(pre_data[pre_data.index("data: [DONE]") - 2][6:])
         # 保存新的会话id
         # if not var.session_data[id][0]:
         var.session_data[id][0] = json_data["conversation_id"]
         var.session_data[id][1] = json_data["message"]["id"]
+
         # 尝试重命名（需api支持）
         if new_talk:
             await handle_req(id, "", "rename")
         result: str = json_data["message"]["content"]["parts"][0]
 
     except Exception as e:
         # 会话丢失
@@ -113,15 +115,15 @@
             return await handle_req(id, req_text, operation)
         # 真的出错了
         err_header = "响应结果异常！" if resp_code else "访问接口出错！"
         code_text = f"\n响应码: {resp_code}" if resp_code else ""
         err_type_text = "" if resp_code else f"\n错误类型: {repr(e)}"
         content_text = f"\n响应内容: {err_msg}" if resp_code else ""
         content_text = (
-            f"{content_text[:300]}\n（内容过长已截断）"
+            f"{content_text[:300]}\n（中间内容过多，忽略）\n{content_text[-300:]}"
             if len(content_text) > 300
             else content_text
         )
         result = err_header + code_text + err_type_text + content_text
 
     return result
 
@@ -173,8 +175,8 @@
     # 按行开画，c是计算写到第几行
     c = 0
     for line in lines:
         draw.text((10, 6 + line_height * c), line, font=font, fill=black_color)
         c += 1
     img_bytes = BytesIO()
     image.save(img_bytes, format="jpeg")
-    return img_bytes
+    return img_bytes
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.6.1/nonebot_plugin_talk_with_chatgpt/HYWenHei-85W.ttf` & `nonebot_plugin_talk_with_chatgpt-0.6.2/nonebot_plugin_talk_with_chatgpt/HYWenHei-85W.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.6.1/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.6.1"
+version = "0.6.2"
 description = "Nonebot2 基于accessToken登录的ChatGPT聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.6.1/README.md` & `nonebot_plugin_talk_with_chatgpt-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -106,17 +106,21 @@
 ## 插件命令（均可修改！） 
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
-| /chatgpt | 设置预设（人格），设置后会重置对话 |
+| /chatgpt | 如果talk_with_chatgpt_all_group_enable为false，则用该命令启用 |
 
 ## 更新日志
+### 2023/7/21 \[v0.6.2]
+
+* [修复无法响应的问题](https://github.com/nikissXI/nonebot_plugins/issues/29)
+
 ### 2023/6/28 \[v0.6.1]
 
 * 新增配置项 talk_with_chatgpt_send_with_img 和 talk_with_chatgpt_ban_word
 
 ### 2023/5/30 \[v0.5.0]
 
 * 更换了自带预设“猫娘”的内容，新增配置项 talk_with_chatgpt_all_group_enable 和 talk_with_chatgpt_group_enable_cmd ，新增命令/chatgpt
```

#### html2text {}

```diff
@@ -58,17 +58,19 @@
 talk_with_chatgpt_data = talk_with_chatgpt.json #
 å¦æä½¿ç¨å¾çåå¤ï¼å­ä½å¤§å° talk_with_chatgpt_font_size = 18 ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /chatgpt |
-è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-6/28 \[v0.6.1] * æ°å¢éç½®é¡¹ talk_with_chatgpt_send_with_img å
-talk_with_chatgpt_ban_word ### 2023/5/30 \[v0.5.0] *
+å¦ætalk_with_chatgpt_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | ##
+æ´æ°æ¥å¿ ### 2023/7/21 \[v0.6.2] * [ä¿®å¤æ æ³ååºçé®é¢](https://
+github.com/nikissXI/nonebot_plugins/issues/29) ### 2023/6/28 \[v0.6.1] *
+æ°å¢éç½®é¡¹ talk_with_chatgpt_send_with_img å talk_with_chatgpt_ban_word
+### 2023/5/30 \[v0.5.0] *
 æ´æ¢äºèªå¸¦é¢è®¾âç«å¨âçåå®¹ï¼æ°å¢éç½®é¡¹
 talk_with_chatgpt_all_group_enable å talk_with_chatgpt_group_enable_cmd
 ï¼æ°å¢å½ä»¤/chatgpt ### 2023/5/29 \[v0.4.3] *
 [æ¯ææææºå¨äººååºå½ä»¤](https://github.com/nikissXI/
 nonebot_plugins/issues/22) ### 2023/5/18 \[v0.4.2] *
 [ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢](https://github.com/nikissXI/
 nonebot_plugins/issues/21) ### 2023/4/22 \[v0.4.1] *
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.6.1/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.6.1
+Version: 0.6.2
 Summary: Nonebot2 基于accessToken登录的ChatGPT聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -130,17 +130,21 @@
 ## 插件命令（均可修改！） 
 | 指令 | 说明 |
 |:-----:|:----:|
 | /talk | 开始对话，默认群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
-| /chatgpt | 设置预设（人格），设置后会重置对话 |
+| /chatgpt | 如果talk_with_chatgpt_all_group_enable为false，则用该命令启用 |
 
 ## 更新日志
+### 2023/7/21 \[v0.6.2]
+
+* [修复无法响应的问题](https://github.com/nikissXI/nonebot_plugins/issues/29)
+
 ### 2023/6/28 \[v0.6.1]
 
 * 新增配置项 talk_with_chatgpt_send_with_img 和 talk_with_chatgpt_ban_word
 
 ### 2023/5/30 \[v0.5.0]
 
 * 更换了自带预设“猫娘”的内容，新增配置项 talk_with_chatgpt_all_group_enable 和 talk_with_chatgpt_group_enable_cmd ，新增命令/chatgpt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.6.1
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.6.2
 Summary: Nonebot2 åºäºaccessTokenç»å½çChatGPTèå¤©æä»¶ Home-page:
 https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt License: MIT Author: nikissXI Author-email:
 1299577815@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -73,17 +73,19 @@
 talk_with_chatgpt_data = talk_with_chatgpt.json #
 å¦æä½¿ç¨å¾çåå¤ï¼å­ä½å¤§å° talk_with_chatgpt_font_size = 18 ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /chatgpt |
-è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-6/28 \[v0.6.1] * æ°å¢éç½®é¡¹ talk_with_chatgpt_send_with_img å
-talk_with_chatgpt_ban_word ### 2023/5/30 \[v0.5.0] *
+å¦ætalk_with_chatgpt_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | ##
+æ´æ°æ¥å¿ ### 2023/7/21 \[v0.6.2] * [ä¿®å¤æ æ³ååºçé®é¢](https://
+github.com/nikissXI/nonebot_plugins/issues/29) ### 2023/6/28 \[v0.6.1] *
+æ°å¢éç½®é¡¹ talk_with_chatgpt_send_with_img å talk_with_chatgpt_ban_word
+### 2023/5/30 \[v0.5.0] *
 æ´æ¢äºèªå¸¦é¢è®¾âç«å¨âçåå®¹ï¼æ°å¢éç½®é¡¹
 talk_with_chatgpt_all_group_enable å talk_with_chatgpt_group_enable_cmd
 ï¼æ°å¢å½ä»¤/chatgpt ### 2023/5/29 \[v0.4.3] *
 [æ¯ææææºå¨äººååºå½ä»¤](https://github.com/nikissXI/
 nonebot_plugins/issues/22) ### 2023/5/18 \[v0.4.2] *
 [ä¿®å¤ä¼è¯ä¸¢å¤±ä¸éç½®çé®é¢](https://github.com/nikissXI/
 nonebot_plugins/issues/21) ### 2023/4/22 \[v0.4.1] *
```

