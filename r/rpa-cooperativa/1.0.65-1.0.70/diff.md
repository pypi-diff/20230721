# Comparing `tmp/rpa_cooperativa-1.0.65.tar.gz` & `tmp/rpa_cooperativa-1.0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.65.tar", last modified: Fri Jul 21 19:22:33 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.70.tar", last modified: Fri Jul 21 19:52:08 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.65.tar` & `rpa_cooperativa-1.0.70.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 19:22:33.658632 rpa_cooperativa-1.0.65/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.65/LICENSE
--rw-rw-rw-   0        0        0     6969 2023-07-21 19:22:33.651748 rpa_cooperativa-1.0.65/PKG-INFO
--rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.65/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 19:22:33.294012 rpa_cooperativa-1.0.65/rpa_coop/
--rw-rw-rw-   0        0        0      613 2023-07-21 18:26:52.000000 rpa_cooperativa-1.0.65/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:22:33.573092 rpa_cooperativa-1.0.65/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.65/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.65/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.65/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.65/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.65/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.65/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.65/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.65/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.65/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.65/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.65/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0   104223 2023-07-21 19:21:58.000000 rpa_cooperativa-1.0.65/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:22:33.641473 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6969 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-21 19:22:32.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      581 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 19:22:33.659356 rpa_cooperativa-1.0.65/setup.cfg
--rw-rw-rw-   0        0        0     2350 2023-07-21 18:39:53.000000 rpa_cooperativa-1.0.65/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:52:08.836005 rpa_cooperativa-1.0.70/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.70/LICENSE
+-rw-rw-rw-   0        0        0     6969 2023-07-21 19:52:08.832936 rpa_cooperativa-1.0.70/PKG-INFO
+-rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.70/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 19:52:08.677143 rpa_cooperativa-1.0.70/rpa_coop/
+-rw-rw-rw-   0        0        0      613 2023-07-21 18:26:52.000000 rpa_cooperativa-1.0.70/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:52:08.774132 rpa_cooperativa-1.0.70/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.70/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.70/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.70/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.70/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.70/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.70/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.70/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.70/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.70/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.70/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.70/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0   104247 2023-07-21 19:51:34.000000 rpa_cooperativa-1.0.70/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:52:08.824759 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6969 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      581 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 19:52:08.000000 rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 19:52:08.837016 rpa_cooperativa-1.0.70/setup.cfg
+-rw-rw-rw-   0        0        0     2350 2023-07-21 19:51:09.000000 rpa_cooperativa-1.0.70/setup.py
```

### Comparing `rpa_cooperativa-1.0.65/LICENSE` & `rpa_cooperativa-1.0.70/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.65/PKG-INFO` & `rpa_cooperativa-1.0.70/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.65
+Version: 1.0.70
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.65/README.md` & `rpa_cooperativa-1.0.70/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.65/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.70/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.65/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.70/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.65/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.70/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.65/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.70/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.65/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.70/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.65/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.70/rpa_coop/rpa_coop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1375,26 +1375,26 @@
         # self.janela_siat = self.janela
         # self.janela_siac = self.janela
         
         opcoes = [x.upper() for x in opcoes]
         
         for menu in opcoes:
             time.sleep(2)
-            espera = 0
-            while espera < 26:
-                if espera == 25:
-                    raise Exception('Nao conseguiu clicar na janela, Menu ACC')
-                try:
-                    self.janela = self.p.getWindowsWithTitle('AC Client')[0]
-                    self.janela.activate()
-                    espera = 0
-                    break
-                except:
-                    time.sleep(2)
-                    espera = espera + 1
+            # espera = 0
+            # while espera < 26:
+            #     if espera == 25:
+            #         raise Exception('Nao conseguiu clicar na janela, Menu ACC')
+            #     try:
+            #         self.janela = self.p.getWindowsWithTitle('AC Client')[0]
+            #         self.janela.activate()
+            #         espera = 0
+            #         break
+            #     except:
+            #         time.sleep(2)
+            #         espera = espera + 1
                 
             self.p.press('pgdn')
             time.sleep(1)
             
             if menu == 'SACG':
                 # Abrir SACG
                 try:
```

### Comparing `rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.65
+Version: 1.0.70
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.70/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.65/setup.py` & `rpa_cooperativa-1.0.70/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.65",
+    version="1.0.70",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

