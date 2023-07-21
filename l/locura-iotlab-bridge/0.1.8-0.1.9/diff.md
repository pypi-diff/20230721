# Comparing `tmp/locura_iotlab_bridge-0.1.8.tar.gz` & `tmp/locura_iotlab_bridge-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locura_iotlab_bridge-0.1.8.tar", last modified: Mon Jun 19 16:57:32 2023, max compression
+gzip compressed data, was "locura_iotlab_bridge-0.1.9.tar", last modified: Mon Jun 19 17:19:25 2023, max compression
```

## Comparing `locura_iotlab_bridge-0.1.8.tar` & `locura_iotlab_bridge-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-19 16:57:32.420564 locura_iotlab_bridge-0.1.8/
--rw-r--r--   0 quentin   (1000) quentin   (1000)    21783 2022-12-12 13:41:17.000000 locura_iotlab_bridge-0.1.8/LICENSE
--rw-r--r--   0 quentin   (1000) quentin   (1000)      486 2023-06-19 16:57:32.420564 locura_iotlab_bridge-0.1.8/PKG-INFO
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-19 16:57:32.420564 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge/
--rw-r--r--   0 quentin   (1000) quentin   (1000)       49 2022-12-12 15:29:01.000000 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge/__init__.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)     1156 2023-04-27 14:49:52.000000 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge/helpers.py
--rwxr-xr-x   0 quentin   (1000) quentin   (1000)     7266 2023-06-19 16:51:24.000000 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge/locura_iotlab_bridge.py
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-19 16:57:32.420564 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)      486 2023-06-19 16:57:32.000000 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge.egg-info/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)      345 2023-06-19 16:57:32.000000 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-06-19 16:57:32.000000 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       27 2023-06-19 16:57:32.000000 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge.egg-info/requires.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       21 2023-06-19 16:57:32.000000 locura_iotlab_bridge-0.1.8/locura_iotlab_bridge.egg-info/top_level.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-06-19 16:57:32.420564 locura_iotlab_bridge-0.1.8/setup.cfg
--rw-r--r--   0 quentin   (1000) quentin   (1000)      718 2023-06-19 16:53:52.000000 locura_iotlab_bridge-0.1.8/setup.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-19 17:19:25.802248 locura_iotlab_bridge-0.1.9/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)    21783 2022-12-12 13:41:17.000000 locura_iotlab_bridge-0.1.9/LICENSE
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      486 2023-06-19 17:19:25.802248 locura_iotlab_bridge-0.1.9/PKG-INFO
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-19 17:19:25.802248 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       49 2022-12-12 15:29:01.000000 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge/__init__.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     1156 2023-04-27 14:49:52.000000 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge/helpers.py
+-rwxr-xr-x   0 quentin   (1000) quentin   (1000)     7266 2023-06-19 17:18:59.000000 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge/locura_iotlab_bridge.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-19 17:19:25.802248 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge.egg-info/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      486 2023-06-19 17:19:25.000000 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      345 2023-06-19 17:19:25.000000 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-06-19 17:19:25.000000 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       27 2023-06-19 17:19:25.000000 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge.egg-info/requires.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       21 2023-06-19 17:19:25.000000 locura_iotlab_bridge-0.1.9/locura_iotlab_bridge.egg-info/top_level.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-06-19 17:19:25.802248 locura_iotlab_bridge-0.1.9/setup.cfg
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      718 2023-06-19 17:19:13.000000 locura_iotlab_bridge-0.1.9/setup.py
```

### Comparing `locura_iotlab_bridge-0.1.8/LICENSE` & `locura_iotlab_bridge-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `locura_iotlab_bridge-0.1.8/locura_iotlab_bridge/helpers.py` & `locura_iotlab_bridge-0.1.9/locura_iotlab_bridge/helpers.py`

 * *Files identical despite different names*

### Comparing `locura_iotlab_bridge-0.1.8/locura_iotlab_bridge/locura_iotlab_bridge.py` & `locura_iotlab_bridge-0.1.9/locura_iotlab_bridge/locura_iotlab_bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             if rc == 5 :
                 print("Check MQTT credentials", file=sys.stderr)
             self.looping = False
             
         # subscribe on specific node topic
         for node in self.nodeList :
             topic = '{}/{}/in'.format(self.topicRoot, node)
-            self.subscribe(topic, 2)
+            self.subscribe(topic, 1)
             if self.verbose >= 1 : 
                 print("subscribed to", topic, file=sys.stderr)
         
     def on_message(self, client, userdata, msg) :
         # parse/convert node id from topic and create node identifier
         node = msg.topic.split('/')[2]
         if not self.rIDMap is None and node in self.rIDMap :
@@ -82,23 +82,23 @@
         
         # publish as raw data on testbed/node/+/out
         rawDict = {
             'timestamp':    now,
             'node_id':      identifier2,
             'payload':      line.strip('\r')
             }
-        self.publish('{}/{}/out'.format(self.topicRoot,identifier2), json.dumps(rawDict),2)
+        self.publish('{}/{}/out'.format(self.topicRoot,identifier2), json.dumps(rawDict),1)
         # attempt to json-ify the data, publish it on testbed/node/+/json_out
         try :
             jsonDict = {
                 'timestamp':    now,
                 'node_id':      identifier2,
                 'payload':      json.loads(line)
                 }
-            self.publish('{}/{}/out_json'.format(self.topicRoot,identifier2), json.dumps(rawDict),2)
+            self.publish('{}/{}/out_json'.format(self.topicRoot,identifier2), json.dumps(rawDict),1)
         except json.decoder.JSONDecodeError :
             pass
         if self.verbose >= 2 : 
             print(time.time(), "{} -> {}".format(identifier2, line), file=sys.stderr)
 
 if __name__ == '__main__':
```

### Comparing `locura_iotlab_bridge-0.1.8/setup.py` & `locura_iotlab_bridge-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='locura_iotlab_bridge',
-    version='0.1.8',    
+    version='0.1.9',    
     description='Bridge to connect LocURa MQTT ecosystem to IOT-LAB',
     url='https://gitlab.irit.fr/rmess/locura/infra/locura_iotlab_bridge',
     author='Quentin Vey',
     author_email='quentin.vey@irit.fr',
     license='CeCILL 2.1',
     packages=['locura_iotlab_bridge'],
     install_requires=['iotlabcli>=3.3.0',
```

