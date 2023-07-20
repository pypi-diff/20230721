# Comparing `tmp/DeeptransTool-1.3.tar.gz` & `tmp/DeeptransTool-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeeptransTool-1.3.tar", last modified: Sat Oct 15 22:20:11 2022, max compression
+gzip compressed data, was "DeeptransTool-1.4.tar", last modified: Thu Jul 20 23:14:54 2023, max compression
```

## Comparing `DeeptransTool-1.3.tar` & `DeeptransTool-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-10-15 22:20:10.942139 DeeptransTool-1.3/
-drwxrwxrwx   0        0        0        0 2022-10-15 22:20:10.624139 DeeptransTool-1.3/DTT/
--rw-rw-rw-   0        0        0        0 2022-10-12 19:49:17.000000 DeeptransTool-1.3/DTT/__init__.py
--rw-rw-rw-   0        0        0    15655 2022-10-15 22:06:41.000000 DeeptransTool-1.3/DTT/deepLTranslate.py
-drwxrwxrwx   0        0        0        0 2022-10-15 22:20:10.881140 DeeptransTool-1.3/DeeptransTool.egg-info/
--rw-rw-rw-   0        0        0     7150 2022-10-15 22:20:10.000000 DeeptransTool-1.3/DeeptransTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2022-10-15 22:20:10.000000 DeeptransTool-1.3/DeeptransTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-15 22:20:10.000000 DeeptransTool-1.3/DeeptransTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-10-15 22:20:10.000000 DeeptransTool-1.3/DeeptransTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-10-15 22:20:10.000000 DeeptransTool-1.3/DeeptransTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2022-10-12 20:14:07.000000 DeeptransTool-1.3/LICENSE
--rw-rw-rw-   0        0        0     7150 2022-10-15 22:20:10.908141 DeeptransTool-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6609 2022-10-15 22:11:34.000000 DeeptransTool-1.3/README.md
--rw-rw-rw-   0        0        0       42 2022-10-15 22:20:10.944141 DeeptransTool-1.3/setup.cfg
--rw-rw-rw-   0        0        0      926 2022-10-15 22:10:18.000000 DeeptransTool-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 23:14:54.157331 DeeptransTool-1.4/
+drwxrwxrwx   0        0        0        0 2023-07-20 23:14:54.057217 DeeptransTool-1.4/DTT/
+-rw-rw-rw-   0        0        0        0 2023-07-20 21:18:38.000000 DeeptransTool-1.4/DTT/__init__.py
+-rw-rw-rw-   0        0        0    16476 2023-07-20 22:20:15.000000 DeeptransTool-1.4/DTT/deepLTranslate.py
+drwxrwxrwx   0        0        0        0 2023-07-20 23:14:54.142235 DeeptransTool-1.4/DeeptransTool.egg-info/
+-rw-rw-rw-   0        0        0     6552 2023-07-20 23:14:53.000000 DeeptransTool-1.4/DeeptransTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-07-20 23:14:53.000000 DeeptransTool-1.4/DeeptransTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 23:14:53.000000 DeeptransTool-1.4/DeeptransTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-20 23:14:53.000000 DeeptransTool-1.4/DeeptransTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-20 23:14:53.000000 DeeptransTool-1.4/DeeptransTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-07-20 21:18:38.000000 DeeptransTool-1.4/LICENSE
+-rw-rw-rw-   0        0        0     6552 2023-07-20 23:14:54.153324 DeeptransTool-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6011 2023-07-20 22:22:25.000000 DeeptransTool-1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 23:14:54.157331 DeeptransTool-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-07-20 22:33:17.000000 DeeptransTool-1.4/setup.py
```

### Comparing `DeeptransTool-1.3/DTT/deepLTranslate.py` & `DeeptransTool-1.4/DTT/deepLTranslate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,502 +1,504 @@
-# Selenium Imports!
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.support.ui import Select
-
-
-# Web Driver Import:
-from webdriver_manager.chrome import ChromeDriverManager
-
-
-# PDF reader.
-from PyPDF2 import PdfReader
-
-
-
-
-# Others Imports:
-import time
-import os
-
-
-
-
-
-def file_translate(route:str, string_characters = 4999, l_from = 'en', l_to = 'es', new_file = True, new_file_extension = 'txt'):
-    """
-       Use the world's "best translator" to translate files with python, and without API key.
-    
-    
-    Params
-    =======
-    
-    route: STR | Path of the file to translate.
-    
-    string_characters: INT | how many characters will contain the string to be translated (it is done by parts, by the limitation that has the same translator). Use at most 5000, and with margin of error.
-    
-    l_from: STR | Language of origin. Generally the first acronym of the original language is used! An example of this is "Español", its acronym being "es". If you have any doubts about the acronym of your source or target language, check the website DeepL.
-
-    l_to: STR | Target Language. Generally the first acronym of the original language is used! An example of this is "English", its acronym being "en". If you have any doubts about the acronym of your source or target language, check the website DeepL.
-
-    new_file: BOOL | If you want the translation of the file to be done on a new one, you should activate this option.
-
-    new_file_extension: STR | If the previous option is True (new_file), you have to provide a valid file extension for the new file. If it is not provided, your new extension will be assumed to be txt.
-
-
-    Return
-    =======
-
-    No return new values, only save the file!
-
-    
-    """
-    
-    # Sacar el nombre del archivo sin extensión.
-    file_without_extension = os.path.basename(route)[::-1]
-    file_without_extension = file_without_extension[file_without_extension.find('.'):][::-1][:-1]
-
-
-    # Ahora, por separado, sacamos la extensión del archivo.
-    extension_file = os.path.basename(route)[::-1]
-    extension = extension_file[:extension_file.find('.')][::-1]
-    
-
-
-    # Extensiones de texto validas que usaremos!
-    text_files_extensions = ['srt', 'txt', 'html', 'log', 'csv', 'pdf']
-
-
-
-    # ============================
-    # Exceptions!!
-
-    if string_characters >= 5000:
-        raise Exception('(MaxCharactersError, error 01) Sorry :(, we have limitations with the web, therefore, as maximum characters at a time, we can translate 4999 per string. What we do, is that we pass strings of this length to the browser, when we already split your text into small pieces.')
-
-    elif extension not in text_files_extensions:
-        raise ValueError('(FileExtensionError, error 03) The file you provided seems not to be a valid text file :c')
-
-
-    elif new_file_extension == 'pdf':
-        raise ValueError("(PDFCreateError, error 04) Sorry, we can't build a pdf from your main file (is pdf file) :( Choose as output of your new file, a valid plain text extension!")
-
-    elif new_file == False and extension == 'pdf':
-        raise ValueError('(PDFNewFileError, error 05) If you want to translate a pdf file, it is mandatory to create a new file :/. Fix this error by setting new_file to True.')
-    # ============================
-
-
-
-
-    if extension != 'pdf':
-        f = open(route, 'r+', encoding = 'utf-8')
-        lines = f.readlines()
-
-        f.close()
-
-    else:
-        print('(EXPERIMENTAL PDF FUNCTION ALERT!) Your file is a PDF! Remember, working with PDF files can lead to serious problems with how paragraphs and text are constructed, so you may experience line breaks and tab errors in your text.\n\n')
-
-
-
-        lines = []
-        pdf_r = PdfReader(route)
-        pdf_number_page = len(pdf_r.pages)
-
-        for page_n in list(range(0, pdf_number_page, 1)):
-            page = pdf_r.pages[page_n]
-
-
-            text = str(page.extract_text()).split('\n')
-
-            for line in text:
-                lines.append(line)
-
-
-    
-    lines_to_translate = []
-    raw_consult_url = f'https://www.deepl.com/translator#{l_from}/{l_to}/' # URL del traductor
-    raw_text = ''
-
-    
-    for raw_line in lines: # Inserto TODO en una sola linea. Esto para trabajar
-                           # mejor con la cantidad de carácteres.
-        raw_text = raw_text + str(raw_line)
-
-
-
-
-    if len(raw_text) > string_characters:
-        jumps = list(range(0, len(raw_text), string_characters)) # Generamos una lista con los 
-                                                                 # saltos necesarios de con saltos 
-                                                                 # de {string_characters}
-        
-        jumps.append(len(raw_text))
-        
-
-    else:
-        jumps = [0, len(raw_text)]
-
-        
-    
-    
-    
-    # ====================================
-
-    text_list = []
-    index_list = []
-    new_jumps = [0]
-
-    for ei, index_space in enumerate(raw_text):
-        if index_space == ' ':
-            index_list.append(ei)
-
-
-    for nj in jumps[1:]:
-        n_jumps = min(index_list, key = lambda x: abs(x - nj)) # Esto devuelve el indíce de los espacios!
-
-        nj_j = index_list[index_list.index(n_jumps) - 1] #! Con esto, lo que hacemos es acceder al espacio anterior del que nos devuelve el min. Es util porque lo que queremos es que NO pase de los 5000 carácteres.
-
-        new_jumps.append(nj_j)
-
-
-
-
-
-
-    # =====================================
-
-
-    for e, jump in enumerate(new_jumps[:-1]): # Separamos el string teniendo en cuenta los saltos.
-        
-        
-        if e != len(new_jumps) - 2:
-            text_list.append(raw_text[jump:new_jumps[e + 1]])   
-            
-        elif e == len(new_jumps) - 2:
-            text_list.append(raw_text[jump:])
-            
-            # print(len(raw_text[jump:]))
-
-
-    # =====================================
-
-
-    processed_list = []
-    
-    for string in text_list: # Remplazamos con los caracteres clave que usa DeepL. Luego usaremos
-                             # esto mismo, pero a la inversa, para obtener nuevamente el string
-                             # virgen.
-                
-        string = string.replace(' ', '%20') # Para los espacios!
-        string = string.replace(',', '%2C') # Para las comas.
-        string = string.replace('\ufeff', r'')
-        string = string.replace('\t', r'%20%20%20%20') # Para las tabulaciones
-        string = string.replace('\n', '%0A') # Para los saltos de linea!
-        string = string.replace('?', '%3F') # Para los signos de interrogación.
-        
-    
-        string = string.replace('<i>', '--i--') # Para éstas etiquetas, que al parecer daban bug.
-        string = string.replace('</i>', '--ci--') # Para éstas etiquetas, que al parecer daban bug.
-        string = string.replace('/', r'%5C%2F')
-        string = string.replace('\\', r'%5C%5C')
-        string = string.replace('\\', r'%5C%5C')
-        
-        
-        string = string.replace('-->', '--8') # Para este tipo de signo (o conjunto de singos) y que no de bug. Luego volvemos todo a la normalidad.
-        
-        
-
-        processed_list.append(string)
-
-    
-    
-    
-    # Generemos la URL de consulta con cada uno de los strings.
-    
-    urls_list = []
-    
-    for string_processed in processed_list:
-        url_pro = raw_consult_url + string_processed
-        urls_list.append(url_pro)
-    
-    chrome_options = Options()
-    chrome_options.headless = True # Para que se ejecute sin una interfaz grafica.
-    chrome_options.add_argument('--headless')
-    chrome_options.add_argument('--no-sandbox')
-    chrome_options.add_argument('--disable-dev-shm-usage')
-    chrome_options.add_argument('--version')
-    
-    
-    
-    text_translate = ''
-    
-    
-    print('Traduciendo archivo!!')
-
-    browser = webdriver.Chrome(ChromeDriverManager().install(), options = chrome_options)
-    
-    for link_part in urls_list:
-
-
-        browser.get(link_part)
-        
-        time.sleep(5) #TODO USAR ES NECESARIO. EL TIEMPO DE ESPERA PUEDE VARIAR, VER QUE TAL FUNCIONA CON UN TIEMPO MÁS BAJO. 
-
-        translate_save = browser.find_element(By.ID, 'target-dummydiv')
-
-        translate_text = translate_save.get_attribute('outerHTML')[translate_save.get_attribute('outerHTML').find('>') + 1:-8]
-
-
-        text_translate = text_translate + f' {translate_text}'
-
-
-
-
-
-    browser.get('http://deepl.com')
-    text_f = text_translate.strip()
-    
-    text_f = text_f.replace('--8', '-->') # Para los espacios!
-    text_f = text_f.replace('--i--', '<i>') # Para éstas etiquetas, que al parecer daban bug.
-    text_f = text_f.replace('--ci--', '</i>')
-
-
-
-
-    
-    # Si el usuario decide que quiere la traducción en un nuevo archivo, creamos el archivo.
-    if new_file == True:
-        if new_file_extension in text_files_extensions:
-            new_name = f'{os.path.dirname(route)}/[DTT] {file_without_extension}.{new_file_extension}'
-            new_f = open(new_name, 'w+')
-            new_f.close()
-
-
-            translate_web = open(new_name, 'wb+')
-            translate_web.write(text_f.encode())
-
-            translate_web.close()
-
-        else:
-            raise ValueError('(NewFileExtensionError, error 02): The text extension for the new file is wrong or does not exist! Check it.')
-
-        
-
-    else:
-        translate_web = open(route, 'wb+')
-        translate_web.truncate()
-        
-        translate_web.write(text_f.encode())
-        
-        
-        translate_web.close()
-
-
-
-    browser.close() # Se cierra el navegador para que no consuma recursos obviamente.
-    
-    
-    
-    print(f'\n\nSe ha traducido correctamente el archivo de texto {route}\n\n')
-
-
-
-
-
-
-def string_translate(text, string_characters = 4999, l_from = 'en', l_to = 'es'):
-    """
-    Use the world's "best translator" to translate any text and make use of it, without any restrictions!
-    
-    
-    Params
-    =======
-    
-    text: STR | Text to translate!
-    
-    string_characters: INT | how many characters will contain the string to be translated (it is done by parts, by the limitation that has the same translator). Use at most 5000, and with margin of error.
-    
-    l_from: STR | Language of origin. Generally the first acronym of the original language is used! An example of this is "Español", its acronym being "es".
-
-    l_to: STR | Target Language. Generally the first acronym of the original language is used! An example of this is "English", its acronym being "en".
-
-
-    Return
-    =======
-
-    Return the text translate.
-
-    
-    """
-
-
-
-    # ============================
-    # Exceptions!!
-
-    if string_characters >= 5000:
-        raise Exception('(MaxCharactersError, error 01) Sorry :(, we have limitations with the web, therefore, as maximum characters at a time, we can translate 4999 per string. What we do, is that we pass strings of this length to the browser, when we already split your text into small pieces.')
-
-    # ============================
-
-
-
-                                                                # saltos necesarios de con saltos 
-                                                                # de {string_characters}
-    
-    
-
-    if len(text) >= 5000: # A comparación con la función anterior, acá directamente espliteamos el texto, haciendo el proceso más rápido.
-        jumps = list(range(0, len(text), string_characters)) # Generamos una lista con los 
-        jumps.append(len(text))
-
-
-    else:
-        jumps = [0, len(text)]
-
-        
-    
-    # =====================================
-    
-    # ====================================
-
-    text_list = []
-    index_list = []
-    new_jumps = [0]
-
-    for ei, index_space in enumerate(text):
-        if index_space == ' ':
-            index_list.append(ei)
-
-
-    for nj in jumps[1:]:
-        n_jumps = min(index_list, key = lambda x: abs(x - nj)) # Esto devuelve el indíce de los espacios!
-
-        nj_j = index_list[index_list.index(n_jumps) - 1]
-
-        new_jumps.append(nj_j)
-
-
-
-
-
-
-    # =====================================
-
-
-    for e, jump in enumerate(new_jumps[:-1]): # Separamos el string teniendo en cuenta los saltos.
-        
-        
-        if e != len(new_jumps) - 2:
-            text_list.append(text[jump:new_jumps[e + 1]])   
-            
-        elif e == len(new_jumps) - 2:
-            text_list.append(text[jump:])
-            
-            # print(len(text[jump:]))
-
-
-    # =====================================
-
-
-    processed_list = []
-    
-    for string in text_list: # Remplazamos con los caracteres clave que usa DeepL. Luego usaremos
-                             # esto mismo, pero a la inversa, para obtener nuevamente el string
-                             # virgen.
-                
-        string = string.replace(' ', '%20') # Para los espacios!
-        string = string.replace(',', '%2C') # Para las comas.
-        string = string.replace('\ufeff', r'')
-        string = string.replace('\t', r'%20%20%20%20') # Para las tabulaciones
-        string = string.replace('\n', '%0A') # Para los saltos de linea!
-        string = string.replace('?', '%3F') # Para los signos de interrogación.
-        
-    
-        string = string.replace('<i>', '--i--') # Para éstas etiquetas, que al parecer daban bug.
-        string = string.replace('</i>', '--ci--') # Para éstas etiquetas, que al parecer daban bug.
-        string = string.replace('/', r'%5C%2F')
-        string = string.replace('\\', r'%5C%5C')
-        string = string.replace('\\', r'%5C%5C')
-        
-        
-        string = string.replace('-->', '--8') # Para este tipo de signo (o conjunto de singos) y que no de bug. Luego volvemos todo a la normalidad.
-        
-        
-
-        processed_list.append(string)
-
-    
-    
-    
-    raw_consult_url = f'https://www.deepl.com/translator#{l_from}/{l_to}/' # URL del traductor
-    # Generemos la URL de consulta con cada uno de los strings.
-    
-    urls_list = []
-    
-    for string_processed in processed_list:
-        url_pro = raw_consult_url + string_processed
-        urls_list.append(url_pro)
-        
-    # print(urls_list[-1])
-    
-        
-
-        
-        
-        # break # TODO: quitar este break.
-    
-
-    
-    
-    
-    chrome_options = Options()
-    chrome_options.headless = True # Para que se ejecute sin una interfaz grafica.
-    chrome_options.add_argument('--headless')
-    chrome_options.add_argument('--no-sandbox')
-    chrome_options.add_argument('--disable-dev-shm-usage')
-    chrome_options.add_argument('--version')
-    
-    
-    
-    text_translate = ''
-    
-    
-    
-    print('Traduciendo el texto!!')
-
-    browser = webdriver.Chrome(ChromeDriverManager().install(), options = chrome_options)
-    
-    for link_part in urls_list:
-        browser.get(link_part)
-        time.sleep(5) # USAR ES NECESARIO.
-
-        translate_save = browser.find_element(By.ID, 'target-dummydiv')
-
-        translate_text = translate_save.get_attribute('outerHTML')[translate_save.get_attribute('outerHTML').find('>') + 1:-8]
-
-
-        text_translate = text_translate + f' {translate_text}'
-
-
-
-
-        
-
-    text_f = text_translate.strip()
-    
-    text_f = text_f.replace('--8', '-->') # Para los espacios!
-    text_f = text_f.replace('--i--', '<i>') # Para éstas etiquetas, que al parecer daban bug.
-    text_f = text_f.replace('--ci--', '</i>') # Para las de cierre.
-    browser.close() # Se cierra el navegador para que no consuma recursos obviamente.
-
-
-
-    
-    
-    
-    print(f'\n\nSe ha traducido correctamente el texto!\n\n')
-
+# Selenium Imports!
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.support.ui import Select
+
+
+# Web Driver Import:
+from webdriver_manager.chrome import ChromeDriverManager
+
+
+# PDF reader.
+from PyPDF2 import PdfReader
+
+
+# BeautifulSoup. Con esta librería podemos de forma más sencilla el texto.
+from bs4 import BeautifulSoup
+
+
+
+# Others Imports:
+import time
+import os
+
+
+
+
+
+def file_translate(route:str, string_characters = 4999, l_from = 'en', l_to = 'es', new_file = True, new_file_extension = 'txt'):
+    """
+       Use the world's "best translator" to translate files with python, and without API key.
+    
+    
+    Params
+    =======
+    
+    route: STR | Path of the file to translate.
+    
+    string_characters: INT | how many characters will contain the string to be translated (it is done by parts, by the limitation that has the same translator). Use at most 5000, and with margin of error.
+    
+    l_from: STR | Language of origin. Generally the first acronym of the original language is used! An example of this is "Español", its acronym being "es". If you have any doubts about the acronym of your source or target language, check the website DeepL.
+
+    l_to: STR | Target Language. Generally the first acronym of the original language is used! An example of this is "English", its acronym being "en". If you have any doubts about the acronym of your source or target language, check the website DeepL.
+
+    new_file: BOOL | If you want the translation of the file to be done on a new one, you should activate this option.
+
+    new_file_extension: STR | If the previous option is True (new_file), you have to provide a valid file extension for the new file. If it is not provided, your new extension will be assumed to be txt.
+
+
+    Return
+    =======
+
+    No return new values, only save the file!
+
+    
+    """
+    
+    # Sacar el nombre del archivo sin extensión.
+    file_without_extension = os.path.basename(route)[::-1]
+    file_without_extension = file_without_extension[file_without_extension.find('.'):][::-1][:-1]
+
+
+    # Ahora, por separado, sacamos la extensión del archivo.
+    extension_file = os.path.basename(route)[::-1]
+    extension = extension_file[:extension_file.find('.')][::-1]
+    
+
+
+    # Extensiones de texto validas que usaremos!
+    text_files_extensions = ['srt', 'txt', 'html', 'log', 'csv', 'pdf']
+
+
+
+    # ============================
+    # Exceptions!!
+
+    if string_characters >= 5000:
+        raise Exception('(MaxCharactersError, error 01) Sorry :(, we have limitations with the web, therefore, as maximum characters at a time, we can translate 4999 per string. What we do, is that we pass strings of this length to the browser, when we already split your text into small pieces.')
+
+    elif extension not in text_files_extensions:
+        raise ValueError('(FileExtensionError, error 03) The file you provided seems not to be a valid text file :c')
+
+
+    elif new_file_extension == 'pdf':
+        raise ValueError("(PDFCreateError, error 04) Sorry, we can't build a pdf from your main file (is pdf file) :( Choose as output of your new file, a valid plain text extension!")
+
+    elif new_file == False and extension == 'pdf':
+        raise ValueError('(PDFNewFileError, error 05) If you want to translate a pdf file, it is mandatory to create a new file :/. Fix this error by setting new_file to True.')
+    # ============================
+
+
+
+
+    if extension != 'pdf':
+        f = open(route, 'r+', encoding = 'utf-8')
+        lines = f.readlines()
+
+        f.close()
+
+    else:
+        print('(EXPERIMENTAL PDF FUNCTION ALERT!) Your file is a PDF! Remember, working with PDF files can lead to serious problems with how paragraphs and text are constructed, so you may experience line breaks and tab errors in your text.\n\n')
+
+
+
+        lines = []
+        pdf_r = PdfReader(route)
+        pdf_number_page = len(pdf_r.pages)
+
+        for page_n in list(range(0, pdf_number_page, 1)):
+            page = pdf_r.pages[page_n]
+
+
+            text = str(page.extract_text()).split('\n')
+
+            for line in text:
+                lines.append(line)
+
+
+    
+    lines_to_translate = []
+    raw_consult_url = f'https://www.deepl.com/translator#{l_from}/{l_to}/' # URL del traductor
+    raw_text = ''
+
+    
+    for raw_line in lines: # Inserto TODO en una sola linea. Esto para trabajar
+                           # mejor con la cantidad de carácteres.
+        raw_text = raw_text + str(raw_line)
+
+
+
+
+    if len(raw_text) > string_characters:
+        jumps = list(range(0, len(raw_text), string_characters)) # Generamos una lista con los 
+                                                                 # saltos necesarios de con saltos 
+                                                                 # de {string_characters}
+        
+        jumps.append(len(raw_text))
+        
+
+    else:
+        jumps = [0, len(raw_text)]
+
+        
+    
+    
+    
+    # ====================================
+
+    text_list = []
+    index_list = []
+    new_jumps = [0]
+
+    for ei, index_space in enumerate(raw_text):
+        if index_space == ' ':
+            index_list.append(ei)
+
+
+    for nj in jumps[1:]:
+        n_jumps = min(index_list, key = lambda x: abs(x - nj)) # Esto devuelve el indíce de los espacios!
+
+        nj_j = index_list[index_list.index(n_jumps) - 1] #! Con esto, lo que hacemos es acceder al espacio anterior del que nos devuelve el min. Es util porque lo que queremos es que NO pase de los 5000 carácteres.
+
+        new_jumps.append(nj_j)
+
+
+
+
+
+
+    # =====================================
+
+
+    for e, jump in enumerate(new_jumps[:-1]): # Separamos el string teniendo en cuenta los saltos.
+        
+        
+        if e != len(new_jumps) - 2:
+            text_list.append(raw_text[jump:new_jumps[e + 1]])   
+            
+        elif e == len(new_jumps) - 2:
+            text_list.append(raw_text[jump:])
+            
+            # print(len(raw_text[jump:]))
+
+
+    # =====================================
+
+
+    processed_list = []
+    
+    for string in text_list: # Remplazamos con los caracteres clave que usa DeepL. Luego usaremos
+                             # esto mismo, pero a la inversa, para obtener nuevamente el string
+                             # virgen.
+                
+        string = string.replace(' ', '%20') # Para los espacios!
+        string = string.replace(',', '%2C') # Para las comas.
+        string = string.replace('\ufeff', r'')
+        string = string.replace('\t', r'%20%20%20%20') # Para las tabulaciones
+        string = string.replace('\n', '%0A') # Para los saltos de linea!
+        string = string.replace('?', '%3F') # Para los signos de interrogación.
+        
+    
+        string = string.replace('<i>', '--i--') # Para éstas etiquetas, que al parecer daban bug.
+        string = string.replace('</i>', '--ci--') # Para éstas etiquetas, que al parecer daban bug.
+        string = string.replace('/', r'%5C%2F')
+        string = string.replace('\\', r'%5C%5C')
+        string = string.replace('\\', r'%5C%5C')
+        
+        
+        string = string.replace('-->', '--8') # Para este tipo de signo (o conjunto de singos) y que no de bug. Luego volvemos todo a la normalidad.
+        
+        
+
+        processed_list.append(string)
+
+    
+    
+    
+    # Generemos la URL de consulta con cada uno de los strings.
+    
+    urls_list = []
+    
+    for string_processed in processed_list:
+        url_pro = raw_consult_url + string_processed
+        urls_list.append(url_pro)
+    
+    chrome_options = Options()
+    chrome_options.headless = True # Para que se ejecute sin una interfaz grafica.
+    chrome_options.add_argument('--headless')
+    chrome_options.add_argument('--no-sandbox')
+    chrome_options.add_argument('--disable-dev-shm-usage')
+    chrome_options.add_argument('--version')
+    
+    
+    
+    text_translate = ''
+    
+    
+    print('Traduciendo archivo!!')
+
+    browser = webdriver.Chrome(ChromeDriverManager().install(), options = chrome_options)
+    
+    for link_part in urls_list:
+
+
+        browser.get(link_part)
+        
+        time.sleep(5) #TODO USAR ES NECESARIO. EL TIEMPO DE ESPERA PUEDE VARIAR, VER QUE TAL FUNCIONA CON UN TIEMPO MÁS BAJO. 
+
+        translate_save = browser.find_element(By.CLASS_NAME, 'lmt__inner_textarea_container')
+        translate_save = translate_save[1]
+
+        translate_text = translate_save.get_attribute('outerHTML')[translate_save.get_attribute('outerHTML').find('>') + 1:-8]
+
+        soup = BeautifulSoup(translate_text)
+        translate_text = soup.find('p').getText()
+
+
+        text_translate = text_translate + f' {translate_text}'
+
+
+
+
+
+    browser.get('http://deepl.com')
+    text_f = text_translate.strip()
+    
+    text_f = text_f.replace('--8', '-->') # Para los espacios!
+    text_f = text_f.replace('--i--', '<i>') # Para éstas etiquetas, que al parecer daban bug.
+    text_f = text_f.replace('--ci--', '</i>')
+
+
+
+
+    
+    # Si el usuario decide que quiere la traducción en un nuevo archivo, creamos el archivo.
+    if new_file == True:
+        if new_file_extension in text_files_extensions:
+            new_name = f'{os.path.dirname(route)}/[DTT] {file_without_extension}.{new_file_extension}'
+            new_f = open(new_name, 'w+')
+            new_f.close()
+
+
+            translate_web = open(new_name, 'wb+')
+            translate_web.write(text_f.encode())
+
+            translate_web.close()
+
+        else:
+            raise ValueError('(NewFileExtensionError, error 02): The text extension for the new file is wrong or does not exist! Check it.')
+
+        
+
+    else:
+        translate_web = open(route, 'wb+')
+        translate_web.truncate()
+        
+        translate_web.write(text_f.encode())
+        
+        
+        translate_web.close()
+
+
+
+    browser.close() # Se cierra el navegador para que no consuma recursos obviamente.
+    
+    
+    
+    print(f'\n\nSe ha traducido correctamente el archivo de texto {route}\n\n')
+
+
+
+
+
+
+def string_translate(text, string_characters = 4999, l_from = 'en', l_to = 'es'):
+
+    """
+    Use the world's "best translator" to translate any text and make use of it, without any restrictions!
+    
+    
+    Params
+    =======
+    
+    text: STR | Text to translate!
+    
+    string_characters: INT | how many characters will contain the string to be translated (it is done by parts, by the limitation that has the same translator). Use at most 5000, and with margin of error.
+    
+    l_from: STR | Language of origin. Generally the first acronym of the original language is used! An example of this is "Español", its acronym being "es".
+
+    l_to: STR | Target Language. Generally the first acronym of the original language is used! An example of this is "English", its acronym being "en".
+
+
+    Return
+    =======
+
+    Return the text translate.
+
+    
+    """
+
+
+
+    # ============================
+    # Exceptions!!
+
+    if string_characters >= 5000:
+        raise Exception('(MaxCharactersError, error 01) Sorry :(, we have limitations with the web, therefore, as maximum characters at a time, we can translate 4999 per string. What we do, is that we pass strings of this length to the browser, when we already split your text into small pieces.')
+
+    # ============================
+
+
+
+                                                                # saltos necesarios de con saltos 
+                                                                # de {string_characters}
+    
+    
+
+    if len(text) >= 5000: # A comparación con la función anterior, acá directamente espliteamos el texto, haciendo el proceso más rápido.
+        jumps = list(range(0, len(text), string_characters)) # Generamos una lista con los 
+        jumps.append(len(text))
+
+
+    else:
+        jumps = [0, len(text)]
+
+        
+    
+    # =====================================
+    
+    # ====================================
+
+    text_list = []
+    index_list = []
+    new_jumps = [0]
+
+    for ei, index_space in enumerate(text):
+        if index_space == ' ':
+            index_list.append(ei)
+
+
+    for nj in jumps[1:]:
+        n_jumps = min(index_list, key = lambda x: abs(x - nj)) # Esto devuelve el indíce de los espacios!
+
+        nj_j = index_list[index_list.index(n_jumps) - 1]
+
+        new_jumps.append(nj_j)
+
+
+
+
+
+
+    # =====================================
+
+
+    for e, jump in enumerate(new_jumps[:-1]): # Separamos el string teniendo en cuenta los saltos.
+        
+        
+        if e != len(new_jumps) - 2:
+            text_list.append(text[jump:new_jumps[e + 1]])   
+            
+        elif e == len(new_jumps) - 2:
+            text_list.append(text[jump:])
+            
+            # print(len(text[jump:]))
+
+
+    # =====================================
+
+
+    processed_list = []
+    
+    for string in text_list: # Remplazamos con los caracteres clave que usa DeepL. Luego usaremos
+                             # esto mismo, pero a la inversa, para obtener nuevamente el string
+                             # virgen.
+                
+        string = string.replace(' ', '%20') # Para los espacios!
+        string = string.replace(',', '%2C') # Para las comas.
+        string = string.replace('\ufeff', r'')
+        string = string.replace('\t', r'%20%20%20%20') # Para las tabulaciones
+        string = string.replace('\n', '%0A') # Para los saltos de linea!
+        string = string.replace('?', '%3F') # Para los signos de interrogación.
+        
+    
+        string = string.replace('<i>', '--i--') # Para éstas etiquetas, que al parecer daban bug.
+        string = string.replace('</i>', '--ci--') # Para éstas etiquetas, que al parecer daban bug.
+        string = string.replace('/', r'%5C%2F')
+        string = string.replace('\\', r'%5C%5C')
+        string = string.replace('\\', r'%5C%5C')
+        
+        
+        string = string.replace('-->', '--8') # Para este tipo de signo (o conjunto de singos) y que no de bug. Luego volvemos todo a la normalidad.
+        
+        
+
+        processed_list.append(string)
+
+    
+    
+    
+    raw_consult_url = f'https://www.deepl.com/translator#{l_from}/{l_to}/' # URL del traductor
+    # Generemos la URL de consulta con cada uno de los strings.
+    
+    urls_list = []
+    
+    for string_processed in processed_list:
+        url_pro = raw_consult_url + string_processed
+        urls_list.append(url_pro)
+        
+
+    
+    
+    chrome_options = Options()
+    chrome_options.headless = True # Para que se ejecute sin una interfaz grafica.
+    chrome_options.add_argument('--headless')
+    chrome_options.add_argument('--no-sandbox')
+    chrome_options.add_argument('--disable-dev-shm-usage')
+    chrome_options.add_argument('--version')
+    
+    
+    
+    text_translate = ''
+    
+    
+    
+    print('Traduciendo el texto!!')
+
+    browser = webdriver.Chrome(ChromeDriverManager().install(), options = chrome_options)
+    
+    for link_part in urls_list:
+        browser.get(link_part)
+        time.sleep(5) # USAR ES NECESARIO.
+
+        translate_save = browser.find_elements(By.CLASS_NAME, 'lmt__inner_textarea_container')
+        translate_save = translate_save[1]
+
+        translate_text = translate_save.get_attribute('outerHTML')[translate_save.get_attribute('outerHTML').find('>') + 1:-8]
+
+        soup = BeautifulSoup(translate_text)
+        translate_text = soup.find('p').getText()
+
+        text_translate = text_translate + f' {translate_text}'
+
+
+
+
+        
+
+    text_f = text_translate.strip()
+    
+    text_f = text_f.replace('--8', '-->') # Para los espacios!
+    text_f = text_f.replace('--i--', '<i>') # Para éstas etiquetas, que al parecer daban bug.
+    text_f = text_f.replace('--ci--', '</i>') # Para las de cierre.
+    browser.close() # Se cierra el navegador para que no consuma recursos obviamente.
+
+
+
+    
+    
+    
+    print(f'\n\nSe ha traducido correctamente el texto!\n\n')
+
     return text_f
```

### Comparing `DeeptransTool-1.3/DeeptransTool.egg-info/PKG-INFO` & `DeeptransTool-1.4/DeeptransTool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: DeeptransTool
-Version: 1.3
+Version: 1.4
 Summary: Use the world's best translator (DeepL) to translate your text files or text itself!! All without having to provide your credit card or be limited by the API. 🐸
 Home-page: https://github.com/ElHaban3ro/DeeptransTool
 Author: ElHaban3ro
 Author-email: habanferd@gmail.com
 License: GPLv3
 Keywords: Translate,DeepL,Traduccion,API,Translation
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DeeptransTool
 
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-yellowgreen.svg?style=flat-square)](https://www.gnu.org/licenses/gpl-3.0.en.html) [![Python 3.10](https://img.shields.io/badge/Python-3.10-blue.svg?style=flat-square&logo=python)](https://www.python.org/downloads/release/python-310/) [![PyPi Package](https://img.shields.io/badge/PyPi_Package-pip_install_DeeptransTool-yellow.svg?style=flat-square&logo=pypi)](https://pypi.org/project/DeeptransTool/)
 
@@ -22,21 +22,19 @@
 ---
 The **perfect** module to make ***translations*** with no character limitations, ***no need to pay and no need to give your bank details*** to access the API of ***DeepL***. Translate the main ***text files*** (soon also pdf's) or give the ***text directly***!
 
 To fulfill the **purpose**, we make use of ***Selenium*** and the browser [Chrome](https://www.google.com/chrome/) therefore, it is ***necessary** to have the browser installed ***on your computer***. If you are on **windows**, download the ***latest version***, if you are on ***linux***, we recommend you to download [this](https://github.com/ElHaban3ro/DeeptransTool/blob/main/packages/google-chrome-linux64-105.0.5195.125.deb?raw=true) version. 
 
 
 
-## (v1.3) Â¿What's New?
+## (v1.4) Â¿What's New?
 ---
-- Support for reading and translating PDF's. (Remember that pdf's are a more complex file type than a simple txt or srt, therefore, when creating a new file you may experience line breaks that are not applicable or not applicable at all, this, because of how a pdf is composed). You can use the function to translate PDF's ONLY by creating a new file.
-- Error handling.
-- Support for more characters (it is a problem how some signs that are passed by the url are translated, therefore, signs like "/", are translated by the translator as "%5C%2F", and if they are not corrected, they can cause serious problems. I will be attentive to your feedback to add this kind of characters to the package so that they do not cause errors).
+- Apparently they changed the structure of how the deepl.com page is built, and therefore, the scrapper stopped working. It's fixed!
 
-- A better way to cut the text and pass it to DeepL (apparently, it sometimes caused errors due to words being cut off).
+- The scrapp system was changed in the text. We now use "Beautifulsoup4" which will prevent us from errors in the future!
 
 
 ## Functions
 ---
 
 #### - file_translate(route, string_characters, l_from, l_to, new_file, new_file_extension)
 > Use the world's "best translator" to translate files with python, and without API key.
```

### Comparing `DeeptransTool-1.3/LICENSE` & `DeeptransTool-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DeeptransTool-1.3/PKG-INFO` & `DeeptransTool-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: DeeptransTool
-Version: 1.3
+Version: 1.4
 Summary: Use the world's best translator (DeepL) to translate your text files or text itself!! All without having to provide your credit card or be limited by the API. 🐸
 Home-page: https://github.com/ElHaban3ro/DeeptransTool
 Author: ElHaban3ro
 Author-email: habanferd@gmail.com
 License: GPLv3
 Keywords: Translate,DeepL,Traduccion,API,Translation
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DeeptransTool
 
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-yellowgreen.svg?style=flat-square)](https://www.gnu.org/licenses/gpl-3.0.en.html) [![Python 3.10](https://img.shields.io/badge/Python-3.10-blue.svg?style=flat-square&logo=python)](https://www.python.org/downloads/release/python-310/) [![PyPi Package](https://img.shields.io/badge/PyPi_Package-pip_install_DeeptransTool-yellow.svg?style=flat-square&logo=pypi)](https://pypi.org/project/DeeptransTool/)
 
@@ -22,21 +22,19 @@
 ---
 The **perfect** module to make ***translations*** with no character limitations, ***no need to pay and no need to give your bank details*** to access the API of ***DeepL***. Translate the main ***text files*** (soon also pdf's) or give the ***text directly***!
 
 To fulfill the **purpose**, we make use of ***Selenium*** and the browser [Chrome](https://www.google.com/chrome/) therefore, it is ***necessary** to have the browser installed ***on your computer***. If you are on **windows**, download the ***latest version***, if you are on ***linux***, we recommend you to download [this](https://github.com/ElHaban3ro/DeeptransTool/blob/main/packages/google-chrome-linux64-105.0.5195.125.deb?raw=true) version. 
 
 
 
-## (v1.3) Â¿What's New?
+## (v1.4) Â¿What's New?
 ---
-- Support for reading and translating PDF's. (Remember that pdf's are a more complex file type than a simple txt or srt, therefore, when creating a new file you may experience line breaks that are not applicable or not applicable at all, this, because of how a pdf is composed). You can use the function to translate PDF's ONLY by creating a new file.
-- Error handling.
-- Support for more characters (it is a problem how some signs that are passed by the url are translated, therefore, signs like "/", are translated by the translator as "%5C%2F", and if they are not corrected, they can cause serious problems. I will be attentive to your feedback to add this kind of characters to the package so that they do not cause errors).
+- Apparently they changed the structure of how the deepl.com page is built, and therefore, the scrapper stopped working. It's fixed!
 
-- A better way to cut the text and pass it to DeepL (apparently, it sometimes caused errors due to words being cut off).
+- The scrapp system was changed in the text. We now use "Beautifulsoup4" which will prevent us from errors in the future!
 
 
 ## Functions
 ---
 
 #### - file_translate(route, string_characters, l_from, l_to, new_file, new_file_extension)
 > Use the world's "best translator" to translate files with python, and without API key.
```

### Comparing `DeeptransTool-1.3/README.md` & `DeeptransTool-1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,19 @@
 ---
 The **perfect** module to make ***translations*** with no character limitations, ***no need to pay and no need to give your bank details*** to access the API of ***DeepL***. Translate the main ***text files*** (soon also pdf's) or give the ***text directly***!
 
 To fulfill the **purpose**, we make use of ***Selenium*** and the browser [Chrome](https://www.google.com/chrome/) therefore, it is ***necessary** to have the browser installed ***on your computer***. If you are on **windows**, download the ***latest version***, if you are on ***linux***, we recommend you to download [this](https://github.com/ElHaban3ro/DeeptransTool/blob/main/packages/google-chrome-linux64-105.0.5195.125.deb?raw=true) version. 
 
 
 
-## (v1.3) ¿What's New?
+## (v1.4) ¿What's New?
 ---
-- Support for reading and translating PDF's. (Remember that pdf's are a more complex file type than a simple txt or srt, therefore, when creating a new file you may experience line breaks that are not applicable or not applicable at all, this, because of how a pdf is composed). You can use the function to translate PDF's ONLY by creating a new file.
-- Error handling.
-- Support for more characters (it is a problem how some signs that are passed by the url are translated, therefore, signs like "/", are translated by the translator as "%5C%2F", and if they are not corrected, they can cause serious problems. I will be attentive to your feedback to add this kind of characters to the package so that they do not cause errors).
+- Apparently they changed the structure of how the deepl.com page is built, and therefore, the scrapper stopped working. It's fixed!
 
-- A better way to cut the text and pass it to DeepL (apparently, it sometimes caused errors due to words being cut off).
+- The scrapp system was changed in the text. We now use "Beautifulsoup4" which will prevent us from errors in the future!
 
 
 ## Functions
 ---
 
 #### - file_translate(route, string_characters, l_from, l_to, new_file, new_file_extension)
 > Use the world's "best translator" to translate files with python, and without API key.
```

### Comparing `DeeptransTool-1.3/setup.py` & `DeeptransTool-1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 
 setup(
     name = 'DeeptransTool',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = ['DTT'],
-    version = '1.3',
+    version = '1.4',
     license = 'GPLv3',
     description = "Use the world's best translator (DeepL) to translate your text files or text itself!! All without having to provide your credit card or be limited by the API. 🐸",
     author = 'ElHaban3ro',
     author_email = 'habanferd@gmail.com',
     url = 'https://github.com/ElHaban3ro/DeeptransTool',
     keywords = ['Translate', 'DeepL', 'Traduccion', 'API', 'Translation'],
     classifiers = [
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.11'
     ],
-    install_requires=['selenium==4.5.0', 'webdriver-manager==3.8.3', 'PyPDF2']
+    install_requires=['selenium==4.5.0', 'webdriver-manager==3.8.3', 'PyPDF2', 'beautifulsoup4']
 )
```

