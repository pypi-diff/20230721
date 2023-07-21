# Comparing `tmp/rpa_cooperativa-1.0.64.tar.gz` & `tmp/rpa_cooperativa-1.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.64.tar", last modified: Tue Jul 18 13:24:54 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.65.tar", last modified: Fri Jul 21 19:22:33 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.64.tar` & `rpa_cooperativa-1.0.65.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 13:24:54.063764 rpa_cooperativa-1.0.64/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.64/LICENSE
--rw-rw-rw-   0        0        0     6969 2023-07-18 13:24:54.060636 rpa_cooperativa-1.0.64/PKG-INFO
--rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.64/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 13:24:53.876124 rpa_cooperativa-1.0.64/rpa_coop/
--rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.64/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:24:53.968459 rpa_cooperativa-1.0.64/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.64/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.64/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.64/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.64/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.64/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.64/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.64/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.64/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.64/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.64/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.64/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0   101525 2023-07-18 13:22:44.000000 rpa_cooperativa-1.0.64/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:24:54.053000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6969 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      581 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 13:24:53.000000 rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 13:24:54.064764 rpa_cooperativa-1.0.64/setup.cfg
--rw-rw-rw-   0        0        0     2350 2023-07-18 12:25:45.000000 rpa_cooperativa-1.0.64/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:22:33.658632 rpa_cooperativa-1.0.65/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.65/LICENSE
+-rw-rw-rw-   0        0        0     6969 2023-07-21 19:22:33.651748 rpa_cooperativa-1.0.65/PKG-INFO
+-rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.65/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 19:22:33.294012 rpa_cooperativa-1.0.65/rpa_coop/
+-rw-rw-rw-   0        0        0      613 2023-07-21 18:26:52.000000 rpa_cooperativa-1.0.65/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:22:33.573092 rpa_cooperativa-1.0.65/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.65/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.65/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.65/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.65/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.65/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.65/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.65/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.65/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.65/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.65/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.65/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0   104223 2023-07-21 19:21:58.000000 rpa_cooperativa-1.0.65/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-07-21 19:22:33.641473 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6969 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-07-21 19:22:32.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      581 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 19:22:31.000000 rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 19:22:33.659356 rpa_cooperativa-1.0.65/setup.cfg
+-rw-rw-rw-   0        0        0     2350 2023-07-21 18:39:53.000000 rpa_cooperativa-1.0.65/setup.py
```

### Comparing `rpa_cooperativa-1.0.64/LICENSE` & `rpa_cooperativa-1.0.65/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.64/PKG-INFO` & `rpa_cooperativa-1.0.65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.64
+Version: 1.0.65
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.64/README.md` & `rpa_cooperativa-1.0.65/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.64/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.65/rpa_coop/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,9 +14,10 @@
 numero_por_extenso = escrever_por_extenso.numero_por_extenso
 taxa_percentual_por_extenso = escrever_por_extenso.taxa_por_extenso
 gerador_de_codigo = Gerador_de_codigo()
 selenium = Selenium()
 mail = Emails()
 dia_util = Dia_util()
 adobe = Adobe()
+get_errors =  Get_errors()
```

### Comparing `rpa_cooperativa-1.0.64/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.65/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.64/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.65/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.64/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.65/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.64/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.65/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.64/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.65/rpa_coop/rpa_coop.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import ssl
 ssl._create_default_https_context = ssl._create_unverified_context
 
 user_site_packages = site.getusersitepackages()
 user_site_packages = user_site_packages.replace('Roaming', 'Local\\Programs').replace('site-packages','Lib\\site-packages')
 
 
-def gerador_pwd(palavra_chave:str, select_atributo='usuario', retorna_atributo=True, retorna_dicionario=False ,print_atributo=False, mostrar_todas_credenciais=False):
+def gerador_pwd(palavra_chave:str, select_atributo='usuario', retorna_atributo=True, retorna_dicionario=False ,print_atributo=False, mostrar_todas_credenciais=False, return_conex_fluid = False):
     '''
     usuario = gerador_pwd('fluid', 'usuario')\n
     print(usuario)\n
     '''
     import os
     import socket
     from cryptography.fernet import Fernet 
@@ -60,15 +60,14 @@
     if mostrar_todas_credenciais:
         sql = f"SELECT * FROM rpa_cofre_senhas"
         conex = create_engine(f'mysql+mysqlconnector://{user_planning}:{pw_bd_planning}@{ip_planning}/{db}', pool_recycle=3600)
         credenciais = pd.read_sql_query(sql, conex)
         credenciais = credenciais[['usuario', 'palavra_chave', 'sistema', 'tipo']]
         print('\nPALAVRAS CHAVES EXISTENTES - PARA ACESSO AS CREDENCIAIS')
         print(credenciais[['palavra_chave', 'sistema']])
-        return credenciais
     else:  
         sql = f'SELECT * FROM rpa_cofre_senhas WHERE palavra_chave like "%{palavra_chave_}%"'
         conex = create_engine(f'mysql+mysqlconnector://{user_planning}:{pw_bd_planning}@{ip_planning}/{db}', pool_recycle=3600)
         df = pd.read_sql_query(sql, conex)
         # print(df)
         credencial_atributos = {}
         df = df.drop(columns='id')
@@ -84,15 +83,17 @@
             pass
         credencial_atributos = df.to_dict(orient='records')
         credenciais = credencial_atributos[0]
         valor = credenciais.get(select_atributo)
         result = f'{select_atributo} : {valor}'
         if print_atributo: print(result)
         if retorna_atributo: return valor
-        return credenciais
+    if return_conex_fluid:
+        return credenciais, conex
+    return credenciais
 
 
 class Adobe:
     # https://secure.na1.adobesign.com/public/docs/restapi/v6#://
     def __init__(self):
         self.token_api_adobe = str(gerador_pwd('api_adobe', 'senha'))
         self.url_api_adobe = str(gerador_pwd('api_adobe', 'ip_host'))
@@ -1299,69 +1300,102 @@
         except Exception:
             pass
         
         user_acc = self.usuario_acc
         pw_acclient = self.senha_acc
          
         self.subprocess.Popen("C:\\Users\\Public\\Desktop\\AC Client.lnk",shell=True)
-        self.p.sleep(15)
+        time.sleep(5)
         
 
         # pegar retangulo da janela pelo titulo parcial
-        janela = self.p.getWindowsWithTitle('Aplicações Core - Login')[0]
-        janela.activate()
-
+        espera = 0
+        while espera < 26:
+            if espera == 25:
+                raise Exception('Nao conseguiu clicar na janela, Login ACC')
+            try:
+                self.janela_login = self.p.getWindowsWithTitle('Aplicações Core - Login')[0]
+                self.janela_login.activate()
+                espera = 0
+                break
+            except:
+                time.sleep(2)
+                espera = espera + 1
+           
+                
         self.p.press('tab')
         self.p.press('tab')
         # digitar usuario
         self.p.typewrite(user_acc)
         self.p.press('tab')
         self.p.typewrite(pw_acclient)
         self.p.press('tab')
         self.p.press('enter')
         print('passou do login')
 
-        self.p.sleep(12)
+        time.sleep(3)
         # pegar retangulo da janela pelo titulo parcial
-        janela = self.p.getWindowsWithTitle('AC Client')[0]
-        janela.activate()
-        janela.left
+        espera = 0
+        while espera < 26:
+            if espera == 25:
+                raise Exception('Nao conseguiu clicar na janela, Menu ACC')
+            try:
+                self.janela = self.p.getWindowsWithTitle('AC Client')[0]
+                self.janela.activate()
+                espera = 0
+                break
+            except:
+                time.sleep(2)
+                espera = espera + 1
+
         self.p.sleep(1)
         self.p.press('pgdn')
 
         # Selecionar o MENU SIAT
         posicao = 0
         pasta_imagens = user_site_packages +  '\\rpa_coop\\img\\'
         
                    
         
         if transacional:
-            self.p.moveTo(janela.left + 48, janela.top + 165)
+            self.p.moveTo(self.janela.left + 48, self.janela.top + 165)
             time.sleep(1)
             self.p.click()
             # self.p.doubleClick()
         else:
-            self.p.moveTo(janela.left + 48, janela.top + 245)
+            self.p.moveTo(self.janela.left + 48, self.janela.top + 245)
             self.p.click()
             # self.p.doubleClick()
         time.sleep(3)
             
    
 
         num_menu = 0
         self.janelas = []
-        self.janela_sacg = janela
-        self.janela_siat = janela
-        self.janela_siac = janela
+        # self.janela_sacg = self.janela
+        # self.janela_siat = self.janela
+        # self.janela_siac = self.janela
         
         opcoes = [x.upper() for x in opcoes]
         
         for menu in opcoes:
             time.sleep(2)
-            janela.activate()
+            espera = 0
+            while espera < 26:
+                if espera == 25:
+                    raise Exception('Nao conseguiu clicar na janela, Menu ACC')
+                try:
+                    self.janela = self.p.getWindowsWithTitle('AC Client')[0]
+                    self.janela.activate()
+                    espera = 0
+                    break
+                except:
+                    time.sleep(2)
+                    espera = espera + 1
+                
             self.p.press('pgdn')
             time.sleep(1)
             
             if menu == 'SACG':
                 # Abrir SACG
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png', confidence=0.9, minSearchTime=2.0)
@@ -1761,15 +1795,15 @@
             
         if ',' in taxa:
             valor_aux = taxa.split(',')
             valor_dir = valor_aux[0]
             valor_esq = valor_aux[1]
         else:
             valor_dir = taxa
-            valor_esq = '0'
+            valor_esq = '0'   
     
         if int(valor_dir) > 999: return 'erro, valor maximo 999,99 por cento'    
         if int(valor_dir) > 0:
             valor_dir_extenso = ''   
             valor_dir_extenso = self.calc_3digitos(valor_dir)
         else:
             valor_dir_extenso = 'zero'
@@ -1783,16 +1817,16 @@
             return valor_dir_extenso + ' por cento'
             
                     
     def numero_por_extenso(self, numero: float | str, monetario: bool = True, moeda_unit: str ='real', moeda_plural: str ='reais', nome_separador: str = 'virgula') -> str:
         '''valor_texto = numero_por_extenso(100306000000.01)\n
         cem bilhões e trezentos e seis milhões de reais e um centavo
         '''
-        C , num , centavos, cents = '0', str(numero), '', ''
-        
+        C , num , centavos, cents = '0', str(numero), '', '' 
+            
         def calc_centavos(cents: str):
             if int(cents[-2]) == 0 and int(cents[-1]) > 0: D = self.unidades[int(cents[-1])]
             elif int(cents[-2]) == 1 and int(cents[-1]) >= 0: D = self.especiais[int(cents[-1])]
             elif int(cents[-2]) > 1 and int(cents[-1]) == 0: D = self.dezenas[int(cents[-2])] 
             else: D = self.dezenas[int(cents[-2])] + ' e ' + self.unidades[int(cents[-1])]    
             return D
         
@@ -2213,15 +2247,44 @@
             dia_util_proximo = dia_us
         else:
             dia_util_proximo = dia_br
             
         return dia_util_proximo
         
         
-
+class Get_errors:
+    import traceback
+    import re
+        
+    def __init__(self):
+        pass
+    
+    def pegar_erro(self) -> str:
+        '''usar dentro do except do try, captura informações do erro'''
+        str_traceback = self.traceback.format_exc().replace('Traceback (most recent call last):', '').replace('^','').replace('~','').replace('File ','').replace('"','').replace("'","")
+        try:
+            dica1 = str(self.re.findall('line\s\d+', str_traceback)[0]).replace('line', 'linha') + ' em ' + str(self.re.findall('c:.+py', str_traceback)[0]).split('\\')[-1]
+        except:
+            dica1 = ''
+        try:
+            dica2 = str(self.re.findall('line\s\d+', str_traceback)[1]).replace('line', 'linha') + ' em ' + str(self.re.findall('c:.+py', str_traceback)[1]).split('\\')[-1]
+        except:
+            dica2 = ''
+        try:
+            list_traceback = str_traceback.splitlines()
+            erro = str(list_traceback[-3]).strip() + ' : ' + str(list_traceback[-1]).strip()
+            msg_log = f'{dica1} --> {str(list_traceback[2]).strip()} \n{dica2} --> {erro}'
+        except:
+            try:
+                list_traceback = str_traceback.splitlines()
+                msg_log = f'{dica1} --> {str(list_traceback[2]).strip()} \n{dica2}'
+            except:      
+                msg_log = f'{dica1} \n{dica2}'
+        msg_log = msg_log[:490]
+        return msg_log
```

### Comparing `rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.64
+Version: 1.0.65
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.64/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.65/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.64/setup.py` & `rpa_cooperativa-1.0.65/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.64",
+    version="1.0.65",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

