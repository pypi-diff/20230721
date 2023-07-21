# Comparing `tmp/mkdocs-blogging-plugin-2.2.8.tar.gz` & `tmp/mkdocs-blogging-plugin-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-blogging-plugin-2.2.8.tar", last modified: Tue Jun  6 13:09:50 2023, max compression
+gzip compressed data, was "mkdocs-blogging-plugin-2.2.9.tar", last modified: Thu Jun  8 08:20:41 2023, max compression
```

## Comparing `mkdocs-blogging-plugin-2.2.8.tar` & `mkdocs-blogging-plugin-2.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.400224 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-button-theme.html
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-card-theme.html
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags-index.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags-render.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags.html
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog.html
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/pagination.js
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 13:09:50.000000 mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:50.404224 mkdocs-blogging-plugin-2.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-06 13:09:31.000000 mkdocs-blogging-plugin-2.2.8/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:20:41.290237 mkdocs-blogging-plugin-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-08 08:20:41.290237 mkdocs-blogging-plugin-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:20:41.286236 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:20:41.290237 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog-button-theme.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog-card-theme.html
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog-tags-index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog-tags-render.html
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog-tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/pagination.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:20:41.286236 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-08 08:20:41.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-08 08:20:41.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:20:41.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 08:20:41.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 08:20:41.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 08:20:41.000000 mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:20:41.290237 mkdocs-blogging-plugin-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:20:41.290237 mkdocs-blogging-plugin-2.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-08 08:20:22.000000 mkdocs-blogging-plugin-2.2.9/tests/test_template.py
```

### Comparing `mkdocs-blogging-plugin-2.2.8/LICENSE` & `mkdocs-blogging-plugin-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/PKG-INFO` & `mkdocs-blogging-plugin-2.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-blogging-plugin
-Version: 2.2.8
+Version: 2.2.9
 Summary: Mkdocs plugin that generates a blog index page sorted by creation date.
 Author: Liang Yesheang
 Author-email: liang2kl@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/liang2kl/mkdocs-blogging-plugin
 Keywords: mkdocs blog plugin
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-blogging-plugin-2.2.8/README.md` & `mkdocs-blogging-plugin-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/config.py` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/plugin.py` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-button-theme.html` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog-button-theme.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-card-theme.html` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog-card-theme.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags-index.html` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog-tags-index.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog-tags-render.html` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog-tags-render.html`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/blog.html` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/blog.html`

 * *Files 1% similar despite different names*

```diff
@@ -115,54 +115,56 @@
     </div>
     <hr />
 </div>
 {{ caller() }}
 {%- endmacro %}
 {% endif %}
 
-<div class="pages">
-    {% for page_idx in range(0, page_num) %}
-        {% set pg_group = pages[page_idx*page_size:(page_idx + 1)*page_size] %}
-        <div class="page" id="page{{ page_idx + 1 }}">
+<div class = "md-typeset">
+    <div class="pages">
+        {% for page_idx in range(0, page_num) %}
+            {% set pg_group = pages[page_idx*page_size:(page_idx + 1)*page_size] %}
+            <div class="page" id="page{{ page_idx + 1 }}">
 
-            {% for pg in pg_group %}
-                {# Setting variables. #}
-                {% set url = pg.canonical_url %}
-                {% set title = pg.title %}
-                {% if pg.meta and pg.meta.title_full %}
-                    {% set title = pg.meta.title_full %}
-                {% endif %}
+                {% for pg in pg_group %}
+                    {# Setting variables. #}
+                    {% set url = pg.canonical_url %}
+                    {% set title = pg.title %}
+                    {% if pg.meta and pg.meta.title_full %}
+                        {% set title = pg.meta.title_full %}
+                    {% endif %}
 
-                {% set description = "" %}
-                {% if full_content %}
-                    {% set description = pg.content|safe %}
-                {% elif pg.meta.description %}
-                    {% set description = pg.meta.description|truncate %}
-                {% endif %}
+                    {% set description = "" %}
+                    {% if full_content %}
+                        {% set description = pg.content|safe %}
+                    {% elif pg.meta.description %}
+                        {% set description = pg.meta.description|truncate %}
+                    {% endif %}
+
+                    {% set time = "" %}
+                    {% if pg.meta and pg.meta["localized-time"] %}
+                        {% set time = pg.meta["localized-time"] %}
+                    {% endif %}
+                    
+                    {% call render_blog(title, description, time, url, pg) %}
+                    {% endcall %}
+                {% endfor %}
+            </div>
+        {% endfor %}
+    </div>
 
-                {% set time = "" %}
-                {% if pg.meta and pg.meta["localized-time"] %}
-                    {% set time = pg.meta["localized-time"] %}
+    <div class="blog-center {{'blog-hidden' if page_num == 1 else '' }}">
+        <div class="blog-pagination " id="blog-pagination">
+            {% for num in range(page_num) %}
+                {% if num == 0 %}
+                    {% set link = "" %}
+                {% else %}
+                    {% set link = "#blog-p" + (num + 1)|string %}
                 {% endif %}
-                
-                {% call render_blog(title, description, time, url, pg) %}
-                {% endcall %}
+                <a class="page-number" href="{{ link }}">{{ num + 1 }}</a>
             {% endfor %}
         </div>
-    {% endfor %}
-</div>
-
-<div class="blog-center {{'blog-hidden' if page_num == 1 else '' }}">
-    <div class="blog-pagination " id="blog-pagination">
-        {% for num in range(page_num) %}
-            {% if num == 0 %}
-                {% set link = "" %}
-            {% else %}
-                {% set link = "#blog-p" + (num + 1)|string %}
-            {% endif %}
-            <a class="page-number" href="{{ link }}">{{ num + 1 }}</a>
-        {% endfor %}
+        {% if show_total %}
+            <div>Total <b>{{ pages|count }}</b> posts.</div>
+        {% endif %}
     </div>
-    {% if show_total %}
-        <div>Total <b>{{ pages|count }}</b> posts.</div>
-    {% endif %}
-</div>
+</div>
```

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/templates/pagination.js` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/templates/pagination.js`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin/util.py` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/PKG-INFO` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-blogging-plugin
-Version: 2.2.8
+Version: 2.2.9
 Summary: Mkdocs plugin that generates a blog index page sorted by creation date.
 Author: Liang Yesheang
 Author-email: liang2kl@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/liang2kl/mkdocs-blogging-plugin
 Keywords: mkdocs blog plugin
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-blogging-plugin-2.2.8/mkdocs_blogging_plugin.egg-info/SOURCES.txt` & `mkdocs-blogging-plugin-2.2.9/mkdocs_blogging_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/setup.py` & `mkdocs-blogging-plugin-2.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     LONG_DESCRIPTION = file.read()
 
 with open("requirements.txt", "r") as file:
     DEPENDENCIES = file.readlines()
 
 setup(
     name="mkdocs-blogging-plugin",
-    version="2.2.8",
+    version="2.2.9",
     description="Mkdocs plugin that generates a blog index page sorted by creation date.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="mkdocs blog plugin",
     project_urls={
         "Source": "https://github.com/liang2kl/mkdocs-blogging-plugin"
     },
```

### Comparing `mkdocs-blogging-plugin-2.2.8/tests/test_config.py` & `mkdocs-blogging-plugin-2.2.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/tests/test_format.py` & `mkdocs-blogging-plugin-2.2.9/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `mkdocs-blogging-plugin-2.2.8/tests/test_template.py` & `mkdocs-blogging-plugin-2.2.9/tests/test_template.py`

 * *Files identical despite different names*

