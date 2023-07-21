# Comparing `tmp/KwoksTool-0.0.8.tar.gz` & `tmp/KwoksTool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksTool-0.0.8.tar", last modified: Sat Jul  8 04:35:12 2023, max compression
+gzip compressed data, was "KwoksTool-0.0.9.tar", last modified: Sat Jul  8 07:12:36 2023, max compression
```

## Comparing `KwoksTool-0.0.8.tar` & `KwoksTool-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.504403 KwoksTool-0.0.8/KwoksTool/
-drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/KwoksTool/Spider/
--rw-rw-rw-   0        0        0    12009 2023-07-08 04:30:16.000000 KwoksTool-0.0.8/KwoksTool/Spider/stock.py
--rw-rw-rw-   0        0        0      927 2023-07-08 03:12:19.000000 KwoksTool-0.0.8/KwoksTool/__init__.py
--rw-rw-rw-   0        0        0       22 2023-07-08 04:34:53.000000 KwoksTool-0.0.8/KwoksTool/_version.py
--rw-rw-rw-   0        0        0    14458 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/function.py
--rw-rw-rw-   0        0        0      122 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/info.py
--rw-rw-rw-   0        0        0     1095 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/model.py
-drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/KwoksTool/source/
--rw-rw-rw-   0        0        0   199365 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/source/IpPool.py
--rw-rw-rw-   0        0        0     3737 2023-07-08 01:44:22.000000 KwoksTool-0.0.8/KwoksTool/spider.py
-drwxrwxrwx   0        0        0        0 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/KwoksTool.egg-info/
--rw-rw-rw-   0        0        0       56 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-08 04:35:12.000000 KwoksTool-0.0.8/KwoksTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-07-08 04:34:48.000000 KwoksTool-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 04:35:12.519997 KwoksTool-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 07:12:36.123437 KwoksTool-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-07-08 07:12:36.123437 KwoksTool-0.0.9/KwoksTool/
+drwxrwxrwx   0        0        0        0 2023-07-08 07:12:36.123437 KwoksTool-0.0.9/KwoksTool/Spider/
+-rw-rw-rw-   0        0        0    12224 2023-07-08 07:06:22.000000 KwoksTool-0.0.9/KwoksTool/Spider/stock.py
+-rw-rw-rw-   0        0        0      927 2023-07-08 06:55:47.000000 KwoksTool-0.0.9/KwoksTool/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-07-08 07:12:10.000000 KwoksTool-0.0.9/KwoksTool/_version.py
+-rw-rw-rw-   0        0        0    14458 2023-07-08 06:55:47.000000 KwoksTool-0.0.9/KwoksTool/function.py
+-rw-rw-rw-   0        0        0      122 2023-07-08 06:55:47.000000 KwoksTool-0.0.9/KwoksTool/info.py
+-rw-rw-rw-   0        0        0     1095 2023-07-08 06:55:47.000000 KwoksTool-0.0.9/KwoksTool/model.py
+drwxrwxrwx   0        0        0        0 2023-07-08 07:12:36.123437 KwoksTool-0.0.9/KwoksTool/source/
+-rw-rw-rw-   0        0        0   199365 2023-07-08 06:55:47.000000 KwoksTool-0.0.9/KwoksTool/source/IpPool.py
+-rw-rw-rw-   0        0        0     3737 2023-07-08 06:55:47.000000 KwoksTool-0.0.9/KwoksTool/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-08 07:12:36.123437 KwoksTool-0.0.9/KwoksTool.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-07-08 07:12:36.000000 KwoksTool-0.0.9/KwoksTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-07-08 07:12:36.000000 KwoksTool-0.0.9/KwoksTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 07:12:36.000000 KwoksTool-0.0.9/KwoksTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-08 07:12:36.000000 KwoksTool-0.0.9/KwoksTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 07:12:36.000000 KwoksTool-0.0.9/KwoksTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-07-08 07:12:36.123437 KwoksTool-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-07-08 07:09:31.000000 KwoksTool-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 07:12:36.123437 KwoksTool-0.0.9/setup.cfg
```

### Comparing `KwoksTool-0.0.8/KwoksTool/Spider/stock.py` & `KwoksTool-0.0.9/KwoksTool/Spider/stock.py`

 * *Files 5% similar despite different names*

```diff
@@ -229,14 +229,16 @@
                 file_date=pd.concat([file_date,ChoiceColumn((pd.read_excel(file_path)),[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10])])
             file_date=file_date.reset_index(drop=True)
             file_name=r'.\\'+num+'.xlsx'
             file_date.to_excel(os.path.join(result_path,file_name))
         for i in range(len(array)):
             Merge(array[i])
     def main(year,array,type,path,ip=ip):
+        print('懒得修复Bug的警告提示：\n当type类型为single时候，如果只是采集这个，会出问题。所以，函数类型的调用必须按照如下顺序：\n\
+        all->single->sum\n')
         if type=='all':
             DataCollectionPlate(year, ip=ip)
         elif type=='single':
             SpecificStocksData(array, year)
         elif type=='sum':
             sum()
             sum(path=path,num=array)
```

### Comparing `KwoksTool-0.0.8/KwoksTool/__init__.py` & `KwoksTool-0.0.9/KwoksTool/__init__.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.8/KwoksTool/function.py` & `KwoksTool-0.0.9/KwoksTool/function.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.8/KwoksTool/model.py` & `KwoksTool-0.0.9/KwoksTool/model.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.8/KwoksTool/source/IpPool.py` & `KwoksTool-0.0.9/KwoksTool/source/IpPool.py`

 * *Files identical despite different names*

### Comparing `KwoksTool-0.0.8/KwoksTool/spider.py` & `KwoksTool-0.0.9/KwoksTool/spider.py`

 * *Files identical despite different names*

