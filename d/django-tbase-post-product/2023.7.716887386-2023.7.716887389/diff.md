# Comparing `tmp/django_tbase_post_product-2023.7.716887386.tar.gz` & `tmp/django_tbase_post_product-2023.7.716887389.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.7.716887386.tar", last modified: Fri Jul  7 14:04:46 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.7.716887389.tar", last modified: Fri Jul  7 14:09:26 2023, max compression
```

## Comparing `django_tbase_post_product-2023.7.716887386.tar` & `django_tbase_post_product-2023.7.716887389.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.451896 django_tbase_post_product-2023.7.716887386/
--rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.7.716887386/MANIFEST.in
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-07 14:04:46.451896 django_tbase_post_product-2023.7.716887386/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1222 2023-06-05 15:40:41.000000 django_tbase_post_product-2023.7.716887386/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.441896 django_tbase_post_product-2023.7.716887386/django_tbase_post_product.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-07 14:04:46.000000 django_tbase_post_product-2023.7.716887386/django_tbase_post_product.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-07-07 14:04:46.000000 django_tbase_post_product-2023.7.716887386/django_tbase_post_product.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-07-07 14:04:46.000000 django_tbase_post_product-2023.7.716887386/django_tbase_post_product.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-07-07 14:04:46.000000 django_tbase_post_product-2023.7.716887386/django_tbase_post_product.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-07-07 14:04:46.000000 django_tbase_post_product-2023.7.716887386/django_tbase_post_product.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-07-07 14:04:46.451896 django_tbase_post_product-2023.7.716887386/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.7.716887386/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.441896 django_tbase_post_product-2023.7.716887386/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.716887386/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-07-07 14:04:14.000000 django_tbase_post_product-2023.7.716887386/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.716887386/tbase_post/apps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.441896 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.441896 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     4230 2023-07-07 14:00:03.000000 django_tbase_post_product-2023.7.716887386/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.7.716887386/tbase_post/sitemaps.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.431896 django_tbase_post_product-2023.7.716887386/tbase_post/static/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.451896 django_tbase_post_product-2023.7.716887386/tbase_post/static/images/
--rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.716887386/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
--rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.716887386/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.451896 django_tbase_post_product-2023.7.716887386/tbase_post/templates/
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.451896 django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/
--rw-r--r--   0 terry     (1000) terry     (1000)     3667 2023-07-02 16:58:12.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/article_list_by_tag.html
--rw-r--r--   0 terry     (1000) terry     (1000)     2127 2023-07-02 15:36:36.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/blog_index.html
--rw-r--r--   0 terry     (1000) terry     (1000)     5170 2023-07-02 16:55:04.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/detail.html
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.451896 django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/extras/
--rw-r--r--   0 terry     (1000) terry     (1000)      583 2023-07-02 15:28:54.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/extras/amazon_link.html
--rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-07-02 14:56:34.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/extras/last_update.html
--rw-r--r--   0 terry     (1000) terry     (1000)      366 2023-07-02 15:28:37.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/extras/related_post_by_tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      569 2023-07-02 16:41:58.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/extras/tags.html
--rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templates/sitemap.xml
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.451896 django_tbase_post_product-2023.7.716887386/tbase_post/templatetags/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templatetags/__init__.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:04:46.451896 django_tbase_post_product-2023.7.716887386/tbase_post/templatetags/__pycache__/
--rw-r--r--   0 terry     (1000) terry     (1000)      176 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     3444 2023-07-02 16:53:59.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
--rw-r--r--   0 terry     (1000) terry     (1000)     6225 2023-07-02 16:53:58.000000 django_tbase_post_product-2023.7.716887386/tbase_post/templatetags/post_extras.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.716887386/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      841 2023-07-02 14:42:11.000000 django_tbase_post_product-2023.7.716887386/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     4262 2023-07-02 17:03:03.000000 django_tbase_post_product-2023.7.716887386/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.7.716887389/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1222 2023-06-05 15:40:41.000000 django_tbase_post_product-2023.7.716887389/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.781842 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1544 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1689 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-07-07 14:09:26.000000 django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-26 20:53:14.000000 django_tbase_post_product-2023.7.716887389/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.716887389/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-07-07 14:04:14.000000 django_tbase_post_product-2023.7.716887389/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.716887389/tbase_post/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     4230 2023-07-07 14:00:03.000000 django_tbase_post_product-2023.7.716887389/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.7.716887389/tbase_post/sitemaps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.781842 django_tbase_post_product-2023.7.716887389/tbase_post/static/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/static/images/
+-rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.716887389/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.7.716887389/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templates/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/
+-rw-r--r--   0 terry     (1000) terry     (1000)     3667 2023-07-02 16:58:12.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/article_list_by_tag.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     2127 2023-07-02 15:36:36.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/blog_index.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     5170 2023-07-02 16:55:04.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/detail.html
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/
+-rw-r--r--   0 terry     (1000) terry     (1000)      583 2023-07-02 15:28:54.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/amazon_link.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-07-02 14:56:34.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/last_update.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      366 2023-07-02 15:28:37.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      569 2023-07-02 16:41:58.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templates/sitemap.xml
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-07-07 14:09:26.791842 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      176 2023-06-30 11:21:12.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3444 2023-07-02 16:53:59.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     6241 2023-07-07 14:08:47.000000 django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/post_extras.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.7.716887389/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      841 2023-07-02 14:42:11.000000 django_tbase_post_product-2023.7.716887389/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     4262 2023-07-02 17:03:03.000000 django_tbase_post_product-2023.7.716887389/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.7.716887386/PKG-INFO` & `django_tbase_post_product-2023.7.716887389/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_post_product
-Version: 2023.7.716887386
+Version: 2023.7.716887389
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.7.716887386/README.md` & `django_tbase_post_product-2023.7.716887389/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-post-product
-Version: 2023.7.716887386
+Version: 2023.7.716887389
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
```

### Comparing `django_tbase_post_product-2023.7.716887386/django_tbase_post_product.egg-info/SOURCES.txt` & `django_tbase_post_product-2023.7.716887389/django_tbase_post_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/setup.py` & `django_tbase_post_product-2023.7.716887389/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/admin.py` & `django_tbase_post_product-2023.7.716887389/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc` & `django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc` & `django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc` & `django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc` & `django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc` & `django_tbase_post_product-2023.7.716887389/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/models.py` & `django_tbase_post_product-2023.7.716887389/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg` & `django_tbase_post_product-2023.7.716887389/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/article_list_by_tag.html` & `django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/article_list_by_tag.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/blog_index.html` & `django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/blog_index.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/detail.html` & `django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/detail.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/extras/amazon_link.html` & `django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/amazon_link.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/templates/post/extras/tags.html` & `django_tbase_post_product-2023.7.716887389/tbase_post/templates/post/extras/tags.html`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc` & `django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/templatetags/post_extras.py` & `django_tbase_post_product-2023.7.716887389/tbase_post/templatetags/post_extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,18 +194,18 @@
     """
     
     
     """
     try:
 
         if exclude_pk==None:
-            page_obj = Post.objects.all().order_by('-pk').distinct()[:limit]
+            page_obj = Post.objects.all().order_by('-updated_on').distinct()[:limit]
         else:
             page_obj = Post.objects.all().exclude(
-                pk=exclude_pk).order_by('-pk').distinct()[:limit]
+                pk=exclude_pk).order_by('-updated_on').distinct()[:limit]
 
         # print("page_obj", page_obj)
         return {
             'state': True,
             'link': "context['home_link']",
             'title': "Last Update",
             "page_obj": page_obj,
```

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/urls.py` & `django_tbase_post_product-2023.7.716887389/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.7.716887386/tbase_post/views.py` & `django_tbase_post_product-2023.7.716887389/tbase_post/views.py`

 * *Files identical despite different names*

