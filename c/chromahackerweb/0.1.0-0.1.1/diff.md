# Comparing `tmp/chromahackerweb-0.1.0.tar.gz` & `tmp/chromahackerweb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromahackerweb-0.1.0.tar", max compression
+gzip compressed data, was "chromahackerweb-0.1.1.tar", max compression
```

## Comparing `chromahackerweb-0.1.0.tar` & `chromahackerweb-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-06-09 01:26:35.000000 chromahackerweb-0.1.0/README.md
--rw-r--r--   0        0        0     6148 2023-06-29 18:39:26.234949 chromahackerweb-0.1.0/chromahackerweb/.DS_Store
--rw-r--r--   0        0        0      853 2023-07-21 20:24:44.852717 chromahackerweb-0.1.0/chromahackerweb/__main__.py
--rw-r--r--   0        0        0     1824 2023-07-21 19:08:09.030974 chromahackerweb-0.1.0/chromahackerweb/static/script.js
--rw-r--r--   0        0        0     2399 2023-07-21 20:44:24.223814 chromahackerweb-0.1.0/chromahackerweb/static/style.css
--rw-r--r--   0        0        0      494 2023-07-21 20:33:05.082842 chromahackerweb-0.1.0/chromahackerweb/templates/index.html
--rw-r--r--   0        0        0      314 2023-07-21 17:45:44.919298 chromahackerweb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 chromahackerweb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-09 01:26:35.000000 chromahackerweb-0.1.1/README.md
+-rw-r--r--   0        0        0     6148 2023-06-29 18:39:26.234949 chromahackerweb-0.1.1/chromahackerweb/.DS_Store
+-rw-r--r--   0        0        0      837 2023-07-21 21:10:00.387886 chromahackerweb-0.1.1/chromahackerweb/__main__.py
+-rw-r--r--   0        0        0     1824 2023-07-21 19:08:09.030974 chromahackerweb-0.1.1/chromahackerweb/static/script.js
+-rw-r--r--   0        0        0     2399 2023-07-21 20:44:24.223814 chromahackerweb-0.1.1/chromahackerweb/static/style.css
+-rw-r--r--   0        0        0      494 2023-07-21 20:33:05.082842 chromahackerweb-0.1.1/chromahackerweb/templates/index.html
+-rw-r--r--   0        0        0      385 2023-07-21 21:11:11.676022 chromahackerweb-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 chromahackerweb-0.1.1/PKG-INFO
```

### Comparing `chromahackerweb-0.1.0/chromahackerweb/.DS_Store` & `chromahackerweb-0.1.1/chromahackerweb/.DS_Store`

 * *Files identical despite different names*

### Comparing `chromahackerweb-0.1.0/chromahackerweb/__main__.py` & `chromahackerweb-0.1.1/chromahackerweb/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,10 +26,10 @@
 
     return send_file('../wallpaper.' + OUTPUT, mimetype='image/' + OUTPUT)
 
 @app.route('/')
 def main():
     return render_template('index.html')
 
-if __name__ == '__main__':
+def run():
     webbrowser.open('http://localhost:5000')
     app.run()
```

### Comparing `chromahackerweb-0.1.0/chromahackerweb/static/script.js` & `chromahackerweb-0.1.1/chromahackerweb/static/script.js`

 * *Files identical despite different names*

### Comparing `chromahackerweb-0.1.0/chromahackerweb/static/style.css` & `chromahackerweb-0.1.1/chromahackerweb/static/style.css`

 * *Files identical despite different names*

