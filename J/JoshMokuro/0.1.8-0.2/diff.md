# Comparing `tmp/JoshMokuro-0.1.8.tar.gz` & `tmp/JoshMokuro-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JoshMokuro-0.1.8.tar", last modified: Thu Jul 20 03:35:05 2023, max compression
+gzip compressed data, was "JoshMokuro-0.2.tar", last modified: Fri Jul 21 05:16:31 2023, max compression
```

## Comparing `JoshMokuro-0.1.8.tar` & `JoshMokuro-0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-20 03:35:05.727965 JoshMokuro-0.1.8/
-drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-20 03:35:05.723126 JoshMokuro-0.1.8/JoshMokuro.egg-info/
--rw-r--r--   0 jcancellier   (501) staff       (20)     1905 2023-07-20 03:35:05.000000 JoshMokuro-0.1.8/JoshMokuro.egg-info/PKG-INFO
--rw-r--r--   0 jcancellier   (501) staff       (20)      977 2023-07-20 03:35:05.000000 JoshMokuro-0.1.8/JoshMokuro.egg-info/SOURCES.txt
--rw-r--r--   0 jcancellier   (501) staff       (20)        1 2023-07-20 03:35:05.000000 JoshMokuro-0.1.8/JoshMokuro.egg-info/dependency_links.txt
--rw-r--r--   0 jcancellier   (501) staff       (20)       52 2023-07-20 03:35:05.000000 JoshMokuro-0.1.8/JoshMokuro.egg-info/entry_points.txt
--rw-r--r--   0 jcancellier   (501) staff       (20)      197 2023-07-20 03:35:05.000000 JoshMokuro-0.1.8/JoshMokuro.egg-info/requires.txt
--rw-r--r--   0 jcancellier   (501) staff       (20)       13 2023-07-20 03:35:05.000000 JoshMokuro-0.1.8/JoshMokuro.egg-info/top_level.txt
--rw-r--r--   0 jcancellier   (501) staff       (20)    35149 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/LICENSE
--rw-r--r--   0 jcancellier   (501) staff       (20)      103 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/MANIFEST.in
--rw-r--r--   0 jcancellier   (501) staff       (20)     1905 2023-07-20 03:35:05.727820 JoshMokuro-0.1.8/PKG-INFO
--rw-r--r--   0 jcancellier   (501) staff       (20)     3341 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/README.md
-drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-20 03:35:05.725304 JoshMokuro-0.1.8/mokuro/
--rw-r--r--   0 jcancellier   (501) staff       (20)      124 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/__init__.py
--rw-r--r--   0 jcancellier   (501) staff       (20)      113 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/__main__.py
-drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-20 03:35:05.725465 JoshMokuro-0.1.8/mokuro/assets/
-drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-20 03:35:05.727125 JoshMokuro-0.1.8/mokuro/assets/icons/
--rw-r--r--   0 jcancellier   (501) staff       (20)      284 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/icons/chevron-left-double-svgrepo-com.svg
--rw-r--r--   0 jcancellier   (501) staff       (20)      229 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/icons/chevron-left-svgrepo-com.svg
--rw-r--r--   0 jcancellier   (501) staff       (20)      283 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/icons/chevron-right-double-svgrepo-com.svg
--rw-r--r--   0 jcancellier   (501) staff       (20)      228 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/icons/chevron-right-svgrepo-com.svg
--rw-r--r--   0 jcancellier   (501) staff       (20)      282 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/icons/cross-svgrepo-com.svg
--rw-r--r--   0 jcancellier   (501) staff       (20)      342 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/icons/expand-svgrepo-com.svg
--rw-r--r--   0 jcancellier   (501) staff       (20)      378 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/icons/expand-width-svgrepo-com.svg
--rw-r--r--   0 jcancellier   (501) staff       (20)      482 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/icons/fullscreen-svgrepo-com.svg
--rw-r--r--   0 jcancellier   (501) staff       (20)      282 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/icons/menu-hamburger-svgrepo-com.svg
--rw-r--r--   0 jcancellier   (501) staff       (20)    32706 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/assets/panzoom.min.js
--rw-r--r--   0 jcancellier   (501) staff       (20)     1015 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/cache.py
--rw-r--r--   0 jcancellier   (501) staff       (20)      128 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/env.py
--rw-r--r--   0 jcancellier   (501) staff       (20)     3867 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/manga_page_ocr.py
--rw-r--r--   0 jcancellier   (501) staff       (20)    13025 2023-07-20 03:24:24.000000 JoshMokuro-0.1.8/mokuro/overlay_generator.py
--rw-r--r--   0 jcancellier   (501) staff       (20)     1587 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/run.py
--rw-r--r--   0 jcancellier   (501) staff       (20)    16831 2023-07-20 03:25:18.000000 JoshMokuro-0.1.8/mokuro/script.js
--rw-r--r--   0 jcancellier   (501) staff       (20)     5543 2023-07-20 03:23:00.000000 JoshMokuro-0.1.8/mokuro/styles.css
--rw-r--r--   0 jcancellier   (501) staff       (20)      706 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/mokuro/utils.py
--rw-r--r--   0 jcancellier   (501) staff       (20)       38 2023-07-20 03:35:05.728005 JoshMokuro-0.1.8/setup.cfg
--rw-r--r--   0 jcancellier   (501) staff       (20)     1177 2023-07-20 03:34:56.000000 JoshMokuro-0.1.8/setup.py
-drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-20 03:35:05.727571 JoshMokuro-0.1.8/tests/
--rw-r--r--   0 jcancellier   (501) staff       (20)        0 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/tests/__init__.py
--rw-r--r--   0 jcancellier   (501) staff       (20)      355 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/tests/generate_expected_results.py
--rw-r--r--   0 jcancellier   (501) staff       (20)      994 2023-07-20 03:19:29.000000 JoshMokuro-0.1.8/tests/test_mokuro.py
+drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-21 05:16:31.271655 JoshMokuro-0.2/
+drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-21 05:16:31.265704 JoshMokuro-0.2/JoshMokuro.egg-info/
+-rw-r--r--   0 jcancellier   (501) staff       (20)     1903 2023-07-21 05:16:31.000000 JoshMokuro-0.2/JoshMokuro.egg-info/PKG-INFO
+-rw-r--r--   0 jcancellier   (501) staff       (20)      977 2023-07-21 05:16:31.000000 JoshMokuro-0.2/JoshMokuro.egg-info/SOURCES.txt
+-rw-r--r--   0 jcancellier   (501) staff       (20)        1 2023-07-21 05:16:31.000000 JoshMokuro-0.2/JoshMokuro.egg-info/dependency_links.txt
+-rw-r--r--   0 jcancellier   (501) staff       (20)       48 2023-07-21 05:16:31.000000 JoshMokuro-0.2/JoshMokuro.egg-info/entry_points.txt
+-rw-r--r--   0 jcancellier   (501) staff       (20)      197 2023-07-21 05:16:31.000000 JoshMokuro-0.2/JoshMokuro.egg-info/requires.txt
+-rw-r--r--   0 jcancellier   (501) staff       (20)       13 2023-07-21 05:16:31.000000 JoshMokuro-0.2/JoshMokuro.egg-info/top_level.txt
+-rw-r--r--   0 jcancellier   (501) staff       (20)    35149 2023-07-20 04:51:17.000000 JoshMokuro-0.2/LICENSE
+-rw-r--r--   0 jcancellier   (501) staff       (20)      103 2023-07-20 04:51:17.000000 JoshMokuro-0.2/MANIFEST.in
+-rw-r--r--   0 jcancellier   (501) staff       (20)     1903 2023-07-21 05:16:31.271502 JoshMokuro-0.2/PKG-INFO
+-rw-r--r--   0 jcancellier   (501) staff       (20)     3341 2023-07-20 04:51:17.000000 JoshMokuro-0.2/README.md
+drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-21 05:16:31.268455 JoshMokuro-0.2/mokuro/
+-rw-r--r--   0 jcancellier   (501) staff       (20)      124 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/__init__.py
+-rw-r--r--   0 jcancellier   (501) staff       (20)      113 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/__main__.py
+drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-21 05:16:31.268639 JoshMokuro-0.2/mokuro/assets/
+drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-21 05:16:31.270559 JoshMokuro-0.2/mokuro/assets/icons/
+-rw-r--r--   0 jcancellier   (501) staff       (20)      284 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/icons/chevron-left-double-svgrepo-com.svg
+-rw-r--r--   0 jcancellier   (501) staff       (20)      229 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/icons/chevron-left-svgrepo-com.svg
+-rw-r--r--   0 jcancellier   (501) staff       (20)      283 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/icons/chevron-right-double-svgrepo-com.svg
+-rw-r--r--   0 jcancellier   (501) staff       (20)      228 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/icons/chevron-right-svgrepo-com.svg
+-rw-r--r--   0 jcancellier   (501) staff       (20)      282 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/icons/cross-svgrepo-com.svg
+-rw-r--r--   0 jcancellier   (501) staff       (20)      342 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/icons/expand-svgrepo-com.svg
+-rw-r--r--   0 jcancellier   (501) staff       (20)      378 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/icons/expand-width-svgrepo-com.svg
+-rw-r--r--   0 jcancellier   (501) staff       (20)      482 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/icons/fullscreen-svgrepo-com.svg
+-rw-r--r--   0 jcancellier   (501) staff       (20)      282 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/icons/menu-hamburger-svgrepo-com.svg
+-rw-r--r--   0 jcancellier   (501) staff       (20)    32706 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/assets/panzoom.min.js
+-rw-r--r--   0 jcancellier   (501) staff       (20)     1015 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/cache.py
+-rw-r--r--   0 jcancellier   (501) staff       (20)      128 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/env.py
+-rw-r--r--   0 jcancellier   (501) staff       (20)     3867 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/manga_page_ocr.py
+-rw-r--r--   0 jcancellier   (501) staff       (20)    13028 2023-07-21 05:06:22.000000 JoshMokuro-0.2/mokuro/overlay_generator.py
+-rw-r--r--   0 jcancellier   (501) staff       (20)     1587 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/run.py
+-rw-r--r--   0 jcancellier   (501) staff       (20)    18205 2023-07-21 05:09:43.000000 JoshMokuro-0.2/mokuro/script.js
+-rw-r--r--   0 jcancellier   (501) staff       (20)     5622 2023-07-21 05:07:11.000000 JoshMokuro-0.2/mokuro/styles.css
+-rw-r--r--   0 jcancellier   (501) staff       (20)      706 2023-07-20 04:51:17.000000 JoshMokuro-0.2/mokuro/utils.py
+-rw-r--r--   0 jcancellier   (501) staff       (20)       38 2023-07-21 05:16:31.271700 JoshMokuro-0.2/setup.cfg
+-rw-r--r--   0 jcancellier   (501) staff       (20)     1171 2023-07-21 05:16:25.000000 JoshMokuro-0.2/setup.py
+drwxr-xr-x   0 jcancellier   (501) staff       (20)        0 2023-07-21 05:16:31.271174 JoshMokuro-0.2/tests/
+-rw-r--r--   0 jcancellier   (501) staff       (20)        0 2023-07-20 04:51:17.000000 JoshMokuro-0.2/tests/__init__.py
+-rw-r--r--   0 jcancellier   (501) staff       (20)      355 2023-07-20 04:51:17.000000 JoshMokuro-0.2/tests/generate_expected_results.py
+-rw-r--r--   0 jcancellier   (501) staff       (20)      994 2023-07-20 04:51:17.000000 JoshMokuro-0.2/tests/test_mokuro.py
```

### Comparing `JoshMokuro-0.1.8/JoshMokuro.egg-info/PKG-INFO` & `JoshMokuro-0.2/JoshMokuro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JoshMokuro
-Version: 0.1.8
+Version: 0.2
 Summary: Browser reader for manga with selectable text
 Home-page: https://github.com/kha-white/mokuro
 Author: Maciej Budyś
 Author-email: kha-white@mail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `JoshMokuro-0.1.8/JoshMokuro.egg-info/SOURCES.txt` & `JoshMokuro-0.2/JoshMokuro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JoshMokuro-0.1.8/LICENSE` & `JoshMokuro-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `JoshMokuro-0.1.8/PKG-INFO` & `JoshMokuro-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JoshMokuro
-Version: 0.1.8
+Version: 0.2
 Summary: Browser reader for manga with selectable text
 Home-page: https://github.com/kha-white/mokuro
 Author: Maciej Budyś
 Author-email: kha-white@mail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `JoshMokuro-0.1.8/README.md` & `JoshMokuro-0.2/README.md`

 * *Files identical despite different names*

### Comparing `JoshMokuro-0.1.8/mokuro/assets/panzoom.min.js` & `JoshMokuro-0.2/mokuro/assets/panzoom.min.js`

 * *Files identical despite different names*

### Comparing `JoshMokuro-0.1.8/mokuro/cache.py` & `JoshMokuro-0.2/mokuro/cache.py`

 * *Files identical despite different names*

### Comparing `JoshMokuro-0.1.8/mokuro/manga_page_ocr.py` & `JoshMokuro-0.2/mokuro/manga_page_ocr.py`

 * *Files identical despite different names*

### Comparing `JoshMokuro-0.1.8/mokuro/overlay_generator.py` & `JoshMokuro-0.2/mokuro/overlay_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                 else:
                     with tag('link', rel='stylesheet', href='styles.css'):
                         pass
 
             with tag('body'):
                 self.top_menu(doc, tag, text, len(page_htmls))
 
-                with tag('div', id='trantext');
+                with tag('button', id='trantext'):
                     pass
 
                 with tag('div', id='dimOverlay'):
                     pass
 
                 with tag('div', id='popupAbout', klass='popup'):
                     if is_demo:
```

### Comparing `JoshMokuro-0.1.8/mokuro/run.py` & `JoshMokuro-0.2/mokuro/run.py`

 * *Files identical despite different names*

### Comparing `JoshMokuro-0.1.8/mokuro/script.js` & `JoshMokuro-0.2/mokuro/script.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -139,14 +139,60 @@
                 let textBoxes = document.querySelectorAll('.textBox');
                 for (let i = 0; i < textBoxes.length; i++) {
                     textBoxes[i].classList.remove('hovered');
                 }
             }
         }
     });
+
+    const trantext = document.getElementById("trantext")
+    trantext.addEventListener('click', function(e) {
+        trantext.classList.remove('fetchingError');
+        trantext.classList.add('fetching');
+
+        const trantextInner = trantext.childNodes[0];
+        const trantextText = trantextInner.innerHTML;
+
+        translateJapaneseToEnglish(trantextText)
+            .then(translatedText => {
+                trantextInner.innerHTML += '<p>' + translatedText + '</p>';
+                trantext.classList.remove('fetching');
+            })
+            .catch(error => {
+                trantext.classList.add('fetchingError');
+            })
+    })
+}
+
+async function translateJapaneseToEnglish(japaneseText) {
+    const data = {
+        "text": japaneseText,
+        "target_lang": "EN"
+    };
+
+    try {
+        const response = await fetch('https://deepl-proxy.fly.dev/api/v1/translate', {
+            method: 'POST',
+            body: JSON.stringify(data),
+            headers: {
+                "Content-Type": "application/json",
+            }
+        });
+
+        if (response.ok) {
+            const result = await response.json();
+            const translatedText = result.translations[0].text;
+            return translatedText;
+        } else {
+            throw new Error('Translation failed');
+        }
+    } catch (error) {
+        console.error('Error:', error.message);
+        return null;
+    }
 }
 
 function updateProperties() {
     if (state.textBoxBorders) {
         r.style.setProperty('--textBoxBorderHoverColor', 'rgba(237, 28, 36, 0.3)');
     } else {
         r.style.setProperty('--textBoxBorderHoverColor', 'rgba(0, 0, 0, 0)');
```

### Comparing `JoshMokuro-0.1.8/mokuro/styles.css` & `JoshMokuro-0.2/mokuro/styles.css`

 * *Files 2% similar despite different names*

```diff
@@ -268,14 +268,22 @@
     box-shadow: 0px 0px 8px 0px var(--color3a);
     transition: all 0.5s ease-out, max-width 0s ease-in;
     visibility: visible;
     opacity: 1;
     max-width: 100vw;
 }
 
+.fetchError {
+    border-color: red;
+}
+
+.fetching {
+    border-color: blue;
+}
+
 #dimOverlay {
     display: none;
     position: fixed;
     width: 100%;
     height: 100%;
     top: 0;
     left: 0;
```

### Comparing `JoshMokuro-0.1.8/mokuro/utils.py` & `JoshMokuro-0.2/mokuro/utils.py`

 * *Files identical despite different names*

### Comparing `JoshMokuro-0.1.8/setup.py` & `JoshMokuro-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 long_description = (Path(__file__).parent / "README.md").read_text('utf-8').split('# Installation')[0]
 
 setup(
     name="JoshMokuro",
-    version='0.1.8',
+    version='0.2',
     description="Browser reader for manga with selectable text",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kha-white/mokuro",
     author="Maciej Budyś",
     author_email="kha-white@mail.com",
     license="GPLv3",
@@ -36,11 +36,11 @@
         "torchvision>=0.8.1",
         "transformers>=4.25.0",
         "tqdm>=4.41.0",
         "yattag",
     ],
     entry_points={
         "console_scripts": [
-            "JoshMokuro=mokuro.__main__:main",
+            "mokuro=mokuro.__main__:main",
         ]
     },
 )
```

### Comparing `JoshMokuro-0.1.8/tests/test_mokuro.py` & `JoshMokuro-0.2/tests/test_mokuro.py`

 * *Files identical despite different names*

