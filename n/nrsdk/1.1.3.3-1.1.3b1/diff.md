# Comparing `tmp/nrsdk-1.1.3.3.tar.gz` & `tmp/nrsdk-1.1.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrsdk-1.1.3.3.tar", last modified: Fri Jul 21 06:47:42 2023, max compression
+gzip compressed data, was "nrsdk-1.1.3b1.tar", last modified: Thu Jul 20 06:13:23 2023, max compression
```

## Comparing `nrsdk-1.1.3.3.tar` & `nrsdk-1.1.3b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 06:47:42.359786 nrsdk-1.1.3.3/
--rw-rw-rw-   0        0        0      197 2023-07-21 06:47:42.358786 nrsdk-1.1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      881 2023-07-19 07:10:12.000000 nrsdk-1.1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 06:47:42.349833 nrsdk-1.1.3.3/nrsdk/
--rw-rw-rw-   0        0        0      149 2023-07-19 07:15:08.000000 nrsdk-1.1.3.3/nrsdk/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-07-19 07:10:12.000000 nrsdk-1.1.3.3/nrsdk/base.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:47:42.355786 nrsdk-1.1.3.3/nrsdk/lib/
--rw-rw-rw-   0        0        0  1871360 2023-07-20 04:03:39.000000 nrsdk-1.1.3.3/nrsdk/lib/QLNRSdk.dll
--rw-rw-rw-   0        0        0     1975 2023-07-19 07:10:12.000000 nrsdk-1.1.3.3/nrsdk/mcf_reader.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:47:42.358786 nrsdk-1.1.3.3/nrsdk/neuro_recorder/
--rw-rw-rw-   0        0        0     5312 2023-07-20 05:24:07.000000 nrsdk-1.1.3.3/nrsdk/neuro_recorder/__init__.py
--rw-rw-rw-   0        0        0     4484 2023-07-19 07:46:18.000000 nrsdk-1.1.3.3/nrsdk/nrparam.py
--rw-rw-rw-   0        0        0    12108 2023-07-21 06:33:22.000000 nrsdk-1.1.3.3/nrsdk/nrsdk.py
--rw-rw-rw-   0        0        0     1995 2023-07-19 07:10:12.000000 nrsdk-1.1.3.3/nrsdk/paradigm.py
--rw-rw-rw-   0        0        0      136 2023-07-19 07:10:12.000000 nrsdk-1.1.3.3/nrsdk/rsa.py
-drwxrwxrwx   0        0        0        0 2023-07-21 06:47:42.355786 nrsdk-1.1.3.3/nrsdk.egg-info/
--rw-rw-rw-   0        0        0      197 2023-07-21 06:47:42.000000 nrsdk-1.1.3.3/nrsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-07-21 06:47:42.000000 nrsdk-1.1.3.3/nrsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 06:47:42.000000 nrsdk-1.1.3.3/nrsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 06:13:23.000000 nrsdk-1.1.3.3/nrsdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-21 06:47:42.000000 nrsdk-1.1.3.3/nrsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 06:47:42.359786 nrsdk-1.1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      735 2023-07-21 06:47:27.000000 nrsdk-1.1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 06:13:23.961066 nrsdk-1.1.3b1/
+-rw-rw-rw-   0        0        0      197 2023-07-20 06:13:23.961066 nrsdk-1.1.3b1/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2023-07-19 07:10:12.000000 nrsdk-1.1.3b1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 06:13:23.954994 nrsdk-1.1.3b1/nrsdk/
+-rw-rw-rw-   0        0        0      149 2023-07-19 07:15:08.000000 nrsdk-1.1.3b1/nrsdk/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-07-19 07:10:12.000000 nrsdk-1.1.3b1/nrsdk/base.py
+drwxrwxrwx   0        0        0        0 2023-07-20 06:13:23.961066 nrsdk-1.1.3b1/nrsdk/lib/
+-rw-rw-rw-   0        0        0  1871360 2023-07-20 04:03:39.000000 nrsdk-1.1.3b1/nrsdk/lib/QLNRSdk.dll
+-rw-rw-rw-   0        0        0     1975 2023-07-19 07:10:12.000000 nrsdk-1.1.3b1/nrsdk/mcf_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-20 06:13:23.961066 nrsdk-1.1.3b1/nrsdk/neuro_recorder/
+-rw-rw-rw-   0        0        0     5312 2023-07-20 05:24:07.000000 nrsdk-1.1.3b1/nrsdk/neuro_recorder/__init__.py
+-rw-rw-rw-   0        0        0     4484 2023-07-19 07:46:18.000000 nrsdk-1.1.3b1/nrsdk/nrparam.py
+-rw-rw-rw-   0        0        0    12110 2023-07-20 06:04:03.000000 nrsdk-1.1.3b1/nrsdk/nrsdk.py
+-rw-rw-rw-   0        0        0     1995 2023-07-19 07:10:12.000000 nrsdk-1.1.3b1/nrsdk/paradigm.py
+-rw-rw-rw-   0        0        0      136 2023-07-19 07:10:12.000000 nrsdk-1.1.3b1/nrsdk/rsa.py
+drwxrwxrwx   0        0        0        0 2023-07-20 06:13:23.961066 nrsdk-1.1.3b1/nrsdk.egg-info/
+-rw-rw-rw-   0        0        0      197 2023-07-20 06:13:23.000000 nrsdk-1.1.3b1/nrsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-07-20 06:13:23.000000 nrsdk-1.1.3b1/nrsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 06:13:23.000000 nrsdk-1.1.3b1/nrsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 06:13:23.000000 nrsdk-1.1.3b1/nrsdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-20 06:13:23.000000 nrsdk-1.1.3b1/nrsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 06:13:23.961066 nrsdk-1.1.3b1/setup.cfg
+-rw-rw-rw-   0        0        0      571 2023-07-20 06:08:11.000000 nrsdk-1.1.3b1/setup.py
```

### Comparing `nrsdk-1.1.3.3/README.md` & `nrsdk-1.1.3b1/README.md`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3.3/nrsdk/base.py` & `nrsdk-1.1.3b1/nrsdk/base.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3.3/nrsdk/lib/QLNRSdk.dll` & `nrsdk-1.1.3b1/nrsdk/lib/QLNRSdk.dll`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3.3/nrsdk/mcf_reader.py` & `nrsdk-1.1.3b1/nrsdk/mcf_reader.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3.3/nrsdk/neuro_recorder/__init__.py` & `nrsdk-1.1.3b1/nrsdk/neuro_recorder/__init__.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3.3/nrsdk/nrparam.py` & `nrsdk-1.1.3b1/nrsdk/nrparam.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3.3/nrsdk/nrsdk.py` & `nrsdk-1.1.3b1/nrsdk/nrsdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,43 +50,43 @@
         self._assert_connected()
 
         # 字符串格式统一为dict
         if isinstance(param, str):
             param = json.loads(param)
 
         s = json.dumps(param, indent=4)
-        # print(s)
+        print(s)
 
         param_2 = c_char_p(s.encode('utf-8'))
         p_resp = (c_char * 512)(0)
         len = 512
         device_code = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
         res = -1
         try:
             res = _api.QLNR_StartStimulationEx(self.login_handle, param_2, p_resp, len, device_code)
-            # print("start stimulation {}".format(resp_result(res)))
-            # if res != _RESP_SUCCESS:
-            #     print(p_resp.value.decode("utf-8"))
+            print("start stimulation {}".format(resp_result(res)))
+            if res != _RESP_SUCCESS:
+                print(p_resp.value.decode("utf-8"))
         except Exception as e:
             print(e)
     
         return _SUCCESS if res == _RESP_SUCCESS else _FAIL
         
     #停止刺激
     def _stop_stimulation(self, device=None):
         self._assert_connected()
 
         p_resp = (c_char * 512)(0)
         len = 512
         device_code = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
         try:
             res = _api.QLNR_StopStimulationEx(self.login_handle, p_resp, len, device_code)
-            # print("stop stimulation {}".format(resp_result(res)))
-            # if res != _RESP_SUCCESS:
-            #     print(p_resp.value.decode("utf-8"))
+            print("stop stimulation {}".format(resp_result(res)))
+            if res != _RESP_SUCCESS:
+                print(p_resp.value.decode("utf-8"))
         except Exception as e:
             print(e)
         
         return _SUCCESS if res == _RESP_SUCCESS else _FAIL
         
     #获取上位机已连接的设备列表
     def _get_device_list(self):
@@ -95,15 +95,15 @@
         p_resp = (c_char * 512)(0)
         len1 = 512
         p_list = (c_char * 4096)(0)
         len2 = 4096
         res = -1
         try:
             res = _api.QLNR_GetDeviceListEx(self.login_handle, p_resp, len1, p_list, len2)
-            # print("get device list {}".format(resp_result(res)))
+            print("get device list {}".format(resp_result(res)))
             if res == _RESP_SUCCESS:
                 list = p_list.value.decode("utf-8")
                 return json.loads(list)
             else:
                 print(p_resp.value.decode("utf-8"))
         except Exception as e:
             print(e)
@@ -119,15 +119,15 @@
         len = 512
         res = -1
         p_ssid = c_char_p(ssid.encode('utf-8')) if ssid else c_char_p(None)
         p_skey = c_char_p(skey.encode('utf-8')) if skey else c_char_p(None)
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
         try:
             res = _api.QLNR_SetDeviceWifiConfigEx(self.login_handle, p_ssid, p_skey, p_resp, len, p_device)
-            # print("set wifi config {} for device[{}]".format(resp_result(res), device))
+            print("set wifi config {} for device[{}]".format(resp_result(res), device))
             if res != _RESP_SUCCESS:
                 print(p_resp.value.decode("utf-8"))
         except Exception as e:
             print(e)
         
         return _SUCCESS if res == _RESP_SUCCESS else _FAIL
 
@@ -138,21 +138,23 @@
         p_wifi_config = (c_char * 512)(0)
         wifi_config_len = 512
         p_resp = (c_char * 512)(0)
         len = 512
         res = -1
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
 
+        ssid = None
+        skey = None
         result = {}
         try:
             res = _api.QLNR_GetDeviceWifiConfigEx(self.login_handle, p_wifi_config, wifi_config_len, p_resp, len, p_device)
             print("get wifi config {} for device[{}]".format(resp_result(res), device))
             if res == _RESP_SUCCESS:
                 wifi_config = p_wifi_config.value.decode("utf-8")
-                # print(wifi_config)
+                print(wifi_config)
                 wifi_config = json.loads(wifi_config)
                 result["ssid"] = wifi_config["configssid"]
                 result["skey"] = wifi_config["configpassword"]
                 result["ssid_default"] = wifi_config["defaultssid"]
                 result["skey_default"] = wifi_config["defaultpassword"]
                 result["ssid_connected"] = wifi_config["currentssid"]
                 result["skey_connected"] = wifi_config["currentpassword"]
@@ -172,15 +174,15 @@
         p_resp = (c_char * 512)(0)
         len = 512
         res = -1
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
 
         try:
             res = _api.QLNR_SetDeviceResetEx(self.login_handle, p_resp, len, p_device)
-            # print("restart device {} for device[{}], resp: {}".format(resp_result(res), device, p_resp.value.decode("utf-8")))
+            print("restart device {} for device[{}], resp: {}".format(resp_result(res), device, p_resp.value.decode("utf-8")))
             
         except Exception as e:
             print(e)
         
         return res
 
     #事件标记
@@ -190,15 +192,15 @@
         p_resp = (c_char * 512)(0)
         len = 512
         res = -1
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
 
         try:
             res = _api.QLNR_SetTrigger(self.login_handle, event_id, p_resp, len, p_device)
-            # print("trigger {} for device[{}], resp: {}".format(resp_result(res), device, p_resp.value.decode("utf-8")))
+            print("trigger {} for device[{}], resp: {}".format(resp_result(res), device, p_resp.value.decode("utf-8")))
             
         except Exception as e:
             print(e)
         
         return res
 
     #开启信号采集（并记录到文件）
@@ -220,15 +222,15 @@
         p_resp = (c_char * 512)(0)
         len = 512
         res = -1
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
 
         try:
             res = _api.QLNR_StartCollectEx(self.login_handle, p_param, p_path, file_type, p_resp, len, p_device)
-            # print("start collection {} for device[{}], resp: {}".format(resp_result(res), device, p_resp.value.decode("utf-8")))
+            print("start collection {} for device[{}], resp: {}".format(resp_result(res), device, p_resp.value.decode("utf-8")))
             
         except Exception as e:
             print(e)
         
         return res
 
     #停止信号采集
@@ -238,15 +240,15 @@
         p_resp = (c_char * 512)(0)
         len = 512
         res = -1
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
 
         try:
             res = _api.QLNR_StopCollectEx(self.login_handle, p_resp, len, p_device)
-            # print("start collection {} for device[{}], resp: {}".format(resp_result(res), device, p_resp.value.decode("utf-8")))
+            print("start collection {} for device[{}], resp: {}".format(resp_result(res), device, p_resp.value.decode("utf-8")))
             
         except Exception as e:
             print(e)
         
         return res
         
 
@@ -257,15 +259,15 @@
         p_resp = (c_char * 512)(0)
         len1 = 512
         p_list = (c_char * 4096)(0)
         len2 = 4096
         res = -1
         try:
             res = _api.QLNR_GetPatientListEx(self.login_handle, p_resp, len1, p_list, len2)
-            # print("get subject list {}".format(resp_result(res)))
+            print("get subject list {}".format(resp_result(res)))
             if res == _RESP_SUCCESS:
                 list = p_list.value.decode("utf-8")
                 return json.loads(list)
             else:
                 print(p_resp.value.decode("utf-8"))
         except Exception as e:
             print(e)
@@ -280,58 +282,58 @@
         len1 = 512
         p_list = (c_char * 40960)(0)
         len2 = 40960
         res = -1
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
         try:
             res = _api.QLNR_GetParadigmListEx(self.login_handle, p_resp, len1, p_list, len2, p_device)
-            # print("get paradigm list {}".format(resp_result(res)))
+            print("get paradigm list {}".format(resp_result(res)))
             if res == _RESP_SUCCESS:
                 list = p_list.value.decode("utf-8")
                 return json.loads(list)
             else:
                 print(p_resp.value.decode("utf-8"))
         except Exception as e:
             print(e)
         
         return []
 
     #设置被试
     def _set_subject_select(self, subject_id, device=None):
         self._assert_connected()
-        # print(f"_set_subject_select(subject_id:{subject_id}, : device:{device})")
+        print(f"_set_subject_select(subject_id:{subject_id}, : device:{device})")
 
         p_resp = (c_char * 512)(0)
         len = 512
         res = -1
         p_subject_id = c_char_p(subject_id.encode('utf-8')) if subject_id else c_char_p(None)
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
         try:
             res = _api.QLNR_SetPatientEx(self.login_handle, p_subject_id, p_resp, len, p_device)
-            # print("_set_subject_select {} for device[{}]".format(resp_result(res), device))
+            print("_set_subject_select {} for device[{}]".format(resp_result(res), device))
             if res != _RESP_SUCCESS:
                 print(p_resp.value.decode("utf-8"))
         except Exception as e:
             print(e)
         
         return _SUCCESS if res == _RESP_SUCCESS else _FAIL
 
     #设置范式
     def _set_paradigm_select(self, paradigm_id, device=None):
         self._assert_connected()
-        # print(f"_set_paradigm_select(paradigm_id:{paradigm_id}, : device:{device})")
+        print(f"_set_paradigm_select(paradigm_id:{paradigm_id}, : device:{device})")
 
         p_resp = (c_char * 512)(0)
         len = 512
         res = -1
         p_paradigm_id = c_char_p(paradigm_id.encode('utf-8')) if paradigm_id else c_char_p(None)
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
         try:
             res = _api.QLNR_SetParadigmEx(self.login_handle, p_paradigm_id, p_resp, len, p_device)
-            # print("_set_paradigm_select {} for device[{}]".format(resp_result(res), device))
+            print("_set_paradigm_select {} for device[{}]".format(resp_result(res), device))
             if res != _RESP_SUCCESS:
                 print(p_resp.value.decode("utf-8"))
         except Exception as e:
             print(e)
         
         return _SUCCESS if res == _RESP_SUCCESS else _FAIL
```

### Comparing `nrsdk-1.1.3.3/nrsdk/paradigm.py` & `nrsdk-1.1.3b1/nrsdk/paradigm.py`

 * *Files identical despite different names*

