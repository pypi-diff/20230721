# Comparing `tmp/rubiran-2.0.7.tar.gz` & `tmp/rubiran-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubiran-2.0.7.tar", last modified: Thu Jul 20 20:29:12 2023, max compression
+gzip compressed data, was "rubiran-2.1.0.tar", last modified: Thu Jul 20 22:26:22 2023, max compression
```

## Comparing `rubiran-2.0.7.tar` & `rubiran-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 20:29:12.382005 rubiran-2.0.7/
--rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.0.7/LICENCE
--rw-rw----   0 root         (0) everybody  (9997)     1593 2023-07-20 20:29:12.386005 rubiran-2.0.7/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.0.7/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 20:29:12.078005 rubiran-2.0.7/rubiran/
--rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.0.7/rubiran/An_Wb.py
--rw-rw----   0 root         (0) everybody  (9997)     1103 2023-07-20 20:26:39.000000 rubiran-2.0.7/rubiran/How.py
--rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.0.7/rubiran/Socket.py
--rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.0.7/rubiran/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    53857 2023-07-20 20:21:36.000000 rubiran-2.0.7/rubiran/client.py
--rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.0.7/rubiran/encryption.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 20:29:12.342005 rubiran-2.0.7/rubiran.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1593 2023-07-20 20:29:10.000000 rubiran-2.0.7/rubiran.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      270 2023-07-20 20:29:10.000000 rubiran-2.0.7/rubiran.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-20 20:29:10.000000 rubiran-2.0.7/rubiran.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-07-20 20:29:10.000000 rubiran-2.0.7/rubiran.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-20 20:29:12.406005 rubiran-2.0.7/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1837 2023-07-20 20:26:31.000000 rubiran-2.0.7/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 22:26:21.710005 rubiran-2.1.0/
+-rw-rw----   0 root         (0) everybody  (9997)     1086 2022-10-17 13:06:02.000000 rubiran-2.1.0/LICENCE
+-rw-rw----   0 root         (0) everybody  (9997)     1593 2023-07-20 22:26:21.718005 rubiran-2.1.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      167 2022-10-19 11:05:05.000000 rubiran-2.1.0/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 22:26:20.394005 rubiran-2.1.0/rubiran/
+-rw-rw----   0 root         (0) everybody  (9997)      789 2023-06-30 12:24:09.000000 rubiran-2.1.0/rubiran/An_Wb.py
+-rw-rw----   0 root         (0) everybody  (9997)     1100 2023-07-20 22:23:14.000000 rubiran-2.1.0/rubiran/How.py
+-rw-rw----   0 root         (0) everybody  (9997)     2416 2023-02-18 15:38:01.000000 rubiran-2.1.0/rubiran/Socket.py
+-rw-rw----   0 root         (0) everybody  (9997)       28 2022-10-18 18:06:54.000000 rubiran-2.1.0/rubiran/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    53696 2023-07-20 22:15:50.000000 rubiran-2.1.0/rubiran/client.py
+-rw-rw----   0 root         (0) everybody  (9997)     4079 2023-06-30 11:24:47.000000 rubiran-2.1.0/rubiran/encryption.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-20 22:26:21.542005 rubiran-2.1.0/rubiran.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1593 2023-07-20 22:26:19.000000 rubiran-2.1.0/rubiran.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      270 2023-07-20 22:26:19.000000 rubiran-2.1.0/rubiran.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-20 22:26:19.000000 rubiran-2.1.0/rubiran.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-07-20 22:26:19.000000 rubiran-2.1.0/rubiran.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-20 22:26:21.738005 rubiran-2.1.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1837 2023-07-20 22:22:15.000000 rubiran-2.1.0/setup.py
```

### Comparing `rubiran-2.0.7/LICENCE` & `rubiran-2.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.7/PKG-INFO` & `rubiran-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.7
+Version: 2.1.0
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
@@ -48,15 +48,15 @@
 ``` bash
 from rubiran import rubiran
 ```
 
 ### How to install the library
 
 ``` bash
-pip install rubiran==2.0.7
+pip install rubiran==2.1.0
 ```
 
 ### My ID in Rubika
 
 ``` bash
 @professor_102
 ```
```

### Comparing `rubiran-2.0.7/rubiran/An_Wb.py` & `rubiran-2.1.0/rubiran/An_Wb.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.7/rubiran/How.py` & `rubiran-2.1.0/rubiran/How.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,15 @@
       white = '\033[97m'
       bold = '\033[1m'
       underline = '\033[4m'
       black='\033[30m'
 
 class chup:
       x_coder = f"""{color.bold}
-{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.0.7
- 
+{color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐕𝐄𝐑𝐒𝐈𝐎𝐍  {color.red}2.1.0
 
 {color.white} [⏦] - {color.cyan} 𝐑𝐔𝐁𝐈𝐑𝐀𝐍 {color.yellow} 𝐂𝐎𝐏𝐘𝐑𝐈𝐆𝐇𝐓 (𝐂) {color.red} 2023 {color.green}𝐌𝐀𝐌𝐀𝐃 𝐂𝐎𝐃𝐄𝐑   
 
 {color.white} [⏦] - {color.cyan} 𝐃𝐄𝐕𝐄𝐋𝐎𝐏𝐄𝐑  {color.yellow} 𝐑𝐔𝐁𝐈𝐊𝐀 {color.red} 𝐂𝐇𝐀𝐍𝐍𝐄𝐋 : {color.green} @python_java_source
 
 {color.white}╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾╼╾
 """
```

### Comparing `rubiran-2.0.7/rubiran/Socket.py` & `rubiran-2.1.0/rubiran/Socket.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.7/rubiran/client.py` & `rubiran-2.1.0/rubiran/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1298,142 +1298,133 @@
 		while 1:
 			try:
 				return loads(self.enc.decrypt(loads(self.send_post_file(inData))["data_enc"])).get("data")
 				break
 			except: continue
 
 	def _uploadFile(self, file):
+		enc = encryption
 		if not "http" in file:
-			REQUES = rubiran._requestSendFile(self, file)
+			from requests import post
+			test = self._requestSendFile(file=file)
 			bytef = open(file,"rb").read()
-
-			hash_send = REQUES["access_hash_send"]
-			file_id = REQUES["id"]
-			url = REQUES["upload_url"]
-
+			id = test["id"]
+			dc_id = test["dc_id"]
+			access_hash_send = test["access_hash_send"]
+			url = test["upload_url"]
 			header = {
-					'access-hash-send':hash_send,
-					'auth':self.enc.changeAuthType(bot.Auth),
-					'file-id':str(file_id),
-					'chunk-size':str(len(bytef)),
-					"content-type": "application/octet-stream",
-					"content-length": str(len(bytef)),
-					"accept-encoding": "gzip",
-					"user-agent": "okhttp/3.12.1"
-				}
-
+				'access-hash-send':access_hash_send,
+				'auth':enc.changeAuthType(self.Auth),
+				'file-id':str(id),
+				'chunk-size':str(len(bytef)),
+				"content-type": "application/octet-stream",
+				"content-length": str(len(bytef)),
+				"accept-encoding": "gzip",
+				"user-agent": "okhttp/3.12.1"
+			}
+			
 			if len(bytef) <= 131072:
-				header["part-number"], header["total-part"] = "1","1"
-
+				header['part-number'],header['total-part'] = "1","1"
+		
 				while True:
 					try:
-						j = asyncio.run(post(url=url,data=bytef,headers=header))
-						j = loads(j)['data']['access_hash_rec']
+						r = post(url=url,data=bytef,headers=header).json()["data"]["access_hash_rec"]
 						break
-					except Exception as e:
-						continue
-
-				return [REQUES, j]
+					except:continue
+				return [test,r]
 			else:
-				t = round(len(bytef) / 131072 + 1)
+				t = len(bytef) // 131072 + 1
 				for i in range(1,t+1):
 					if i != t:
 						k = (i - 1) * 131072
 						header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
 						while True:
 							try:
-								o = asyncio.run(post(url=url,data=bytef[k:k + 131072],headers=header))
-								o = loads(o)['data']
+								response = post(url=url,data=bytef[k:k + 131072],headers=header).json()["data"]
+								
 								break
-							except Exception as e:
-								continue
+							except:continue
+					
 					else:
 						k = (i - 1) * 131072
-						header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
+						header["chunk-size"], header["part-number"], header["total-part"] = str(len(bytef[k:])), str(i),str(t)
+				
 						while True:
 							try:
-								
-								p = asyncio.run(post(url=url,data=bytef[k:],headers=header))
-								
-								p = loads(p)['data']['access_hash_rec']
+								response = post(data=bytef[k:],url=url,headers=header).json()
+						#response = loads(response)
 								break
-							except Exception as e:
-								continue
-						return [REQUES, p]
+							except:continue
+				return [test,response["data"]["access_hash_rec"]]
+
 		else:
-			REQUES = {
+			test = {
 				"method":"requestSendFile",
 				"input":{
 					"file_name": file.split("/")[-1],
 					"mime": file.split(".")[-1],
 					"size": len(get(file).content)
 			},
 			"client": SetClines.web
 		}
 
 		while 1:
 			try:
-				return loads(self.enc.decrypt(loads(self.send_post_file(REQUES))["data_enc"])).get("data")
+				return loads(self.enc.decrypt(loads(self.send_post_file(test))["data_enc"])).get("data")
 				break
 			except: continue
 
-			hash_send = REQUES["access_hash_send"]
-			file_id = REQUES["id"]
-			url = REQUES["upload_url"]
-			bytef = get(file).content
-
+			id = test["id"]
+			dc_id = test["dc_id"]
+			access_hash_send = test["access_hash_send"]
+			url = test["upload_url"]
 			header = {
-					'access-hash-send':hash_send,
-					'auth':self.enc.changeAuthType(bot.Auth),
-					'file-id':str(file_id),
-					'chunk-size':str(len(bytef)),
-					"content-type": "application/octet-stream",
-					"content-length": str(len(bytef)),
-					"accept-encoding": "gzip",
-					"user-agent": "okhttp/3.12.1"
-				}
-
+				'access-hash-send':access_hash_send,
+				'auth':enc.changeAuthType(self.Auth),
+				'file-id':str(id),
+				'chunk-size':str(len(bytef)),
+				"content-type": "application/octet-stream",
+				"content-length": str(len(bytef)),
+				"accept-encoding": "gzip",
+				"user-agent": "okhttp/3.12.1"
+			}
+			
 			if len(bytef) <= 131072:
-				header["part-number"], header["total-part"] = "1","1"
-
+				header['part-number'],header['total-part'] = "1","1"
+		
 				while True:
 					try:
-						j = asyncio.run(post(url=url,data=bytef,headers=header))
-						j = loads(j)['data']['access_hash_rec']
+						r = post(url=url,data=bytef,headers=header).json()["data"]["access_hash_rec"]
 						break
-					except Exception as e:
-						continue
-
-				return [REQUES, j]
+					except:continue
+				return [test,r]
 			else:
-				t = round(len(bytef) / 131072 + 1)
+				t = len(bytef) // 131072 + 1
 				for i in range(1,t+1):
 					if i != t:
 						k = (i - 1) * 131072
 						header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
 						while True:
 							try:
+								response = post(url=url,data=bytef[k:k + 131072],headers=header).json()["data"]
 								
-								o = asyncio.run(post(url=url,data=bytef[k:k + 131072],headers=header))
-								o = loads(o)['data']
 								break
-							except Exception as e:
-								continue
+							except:continue
+					
 					else:
 						k = (i - 1) * 131072
-						header["chunk-size"], header["part-number"], header["total-part"] = "131072", str(i),str(t)
+						header["chunk-size"], header["part-number"], header["total-part"] = str(len(bytef[k:])), str(i),str(t)
+				
 						while True:
 							try:
-								
-								p = asyncio.run(post(url=url,data=bytef[k:],headers=header))
-								p = loads(p)['data']['access_hash_rec']
+								response = post(data=bytef[k:],url=url,headers=header).json()
+						#response = loads(response)
 								break
-							except Exception as e:
-								continue
-						return [REQUES, p]
+							except:continue
+				return [test,response["data"]["access_hash_rec"]]
 
 
 	@staticmethod
 	def _getThumbInline(image_bytes:bytes):
 		import io, base64, PIL.Image
 		im = PIL.Image.open(io.BytesIO(image_bytes))
 		width, height = im.size
@@ -1594,15 +1585,15 @@
 				return loads(self.enc.decrypt(loads(self.send_post_file(inData))["data_enc"]))
 				break
 			except: continue
 
 
 	
 	                
-	def sendVoice(self, chat_id, file, time, caption=None, message_id=None):
+	def sendVoice(self, chat_id, file, caption=None, message_id=None):
 		uresponse = rubiran._uploadFile(self, file)
 		file_id = str(uresponse[0]["id"])
 		mime = file.split(".")[-1]
 		dc_id = uresponse[0]["dc_id"]
 		access_hash_rec = uresponse[1]
 		file_name = file.split("/")[-1]
 		size = str(len(get(file).content if "http" in file else open(file,"rb").read()))
@@ -1612,15 +1603,15 @@
 				"input":{
 					"file_inline": {
 						"dc_id": dc_id,
 						"file_id": file_id,
 						"type":"Voice",
 						"file_name": file_name,
 						"size": size,
-						"time": time,
+						"time": "6400",
 						"mime": mime,
 						"access_hash_rec": access_hash_rec,
 					},
 					"object_guid":chat_id,
 					"rnd":f"{randint(100000,999999999)}",
 					"reply_to_message_id":message_id
 				},
@@ -1716,36 +1707,36 @@
 	    "input":{
 	    "file_inline":{
 	    "access_hash_rec":access_hash_rec,
 	    "auto_play":False,
 	    "dc_id":dc_id,
 	    "file_id":file_id,
 	    "file_name":file_name,
-	    "height":426,
+	    "height":"360",
 	    "mime":mime,
 	    "size":size,
 	    "thumb_inline":thumbnail,
-	    "time":5241,
+	    "time":"6700",
 	    "type":"Gif",
-	    "width":424
+	    "width":"360"
 	    },
 	    "is_mute":False,
 	    "object_guid":chat_id,"rnd":f"{randint(100000,999999999)}",
 	    "reply_to_message_id":message_id
 	    
 	    },
 	    "client":SetClines.web
 	    }
 	    if caption != None: inData["input"]["text"] = caption
 	    while 1:
 	        try:
 	            return loads(self.enc.decrypt(loads(self.send_post_file(inData))["data_enc"]))
 	        except:continue
 	        
-	def sendMusic(self, chat_id, file, time, caption=None, message_id=None):
+	def sendMusic(self, chat_id, file, caption=None, message_id=None):
 		uresponse = rubiran._uploadFile(self, file)
 		file_id = str(uresponse[0]["id"])
 		mime = file.split(".")[-1]
 		dc_id = uresponse[0]["dc_id"]
 		access_hash_rec = uresponse[1]
 		file_name = file.split("/")[-1]
 		size = str(len(get(file).content if "http" in file else open(file,"rb").read()))
@@ -1756,15 +1747,15 @@
 					"file_inline": {
 						"dc_id": dc_id,
 						"file_id": file_id,
 						"type":"Music",
 						"music_performer":"",
 						"file_name": file_name,
 						"size": size,
-						"time": time,
+						"time": 6400,
 						"mime": mime,
 						"access_hash_rec": access_hash_rec,
 					},
 					"object_guid":chat_id,
 					"rnd":f"{randint(100000,999999999)}",
 					"reply_to_message_id":message_id
 				},
```

### Comparing `rubiran-2.0.7/rubiran/encryption.py` & `rubiran-2.1.0/rubiran/encryption.py`

 * *Files identical despite different names*

### Comparing `rubiran-2.0.7/rubiran.egg-info/PKG-INFO` & `rubiran-2.1.0/rubiran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubiran
-Version: 2.0.7
+Version: 2.1.0
 Summary: Another example of the library making the Rubik's robot
 Home-page: https://rubika.ir/python_java_source
 Author: mamadcoder
 Author-email: mamadcoder@gmail.com
 License: MIT
 Keywords: rubika,bot,robot,library,rubikalib,rubikalib.ml,rubikalib.ir,rubika.ir,Rubika,Python,Pyrubika,pyrubika
 Classifier: Development Status :: 3 - Alpha
@@ -48,15 +48,15 @@
 ``` bash
 from rubiran import rubiran
 ```
 
 ### How to install the library
 
 ``` bash
-pip install rubiran==2.0.7
+pip install rubiran==2.1.0
 ```
 
 ### My ID in Rubika
 
 ``` bash
 @professor_102
 ```
```

### Comparing `rubiran-2.0.7/setup.py` & `rubiran-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ``` bash
 from rubiran import rubiran
 ```
 
 ### How to install the library
 
 ``` bash
-pip install rubiran==2.0.7
+pip install rubiran==2.1.0
 ```
 
 ### My ID in Rubika
 
 ``` bash
 @professor_102
 ```
@@ -44,15 +44,15 @@
 ``` bash
 @python_java_source 
 ```
 """
 
 setup(
     name = "rubiran",
-    version = "2.0.7",
+    version = "2.1.0",
     author = "mamadcoder",
     author_email = "mamadcoder@gmail.com",
     description = ("Another example of the library making the Rubik's robot"),
     license = "MIT",
     keywords = ["rubika","bot","robot","library","rubikalib","rubikalib.ml","rubikalib.ir","rubika.ir","Rubika","Python","Pyrubika","pyrubika"],
     url = "https://rubika.ir/python_java_source",
     packages=['rubiran'],
```

