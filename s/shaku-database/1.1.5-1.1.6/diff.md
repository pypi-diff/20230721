# Comparing `tmp/shaku-database-1.1.5.tar.gz` & `tmp/shaku-database-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaku-database-1.1.5.tar", last modified: Tue Jul 11 09:10:42 2023, max compression
+gzip compressed data, was "shaku-database-1.1.6.tar", last modified: Fri Jul 21 03:37:52 2023, max compression
```

## Comparing `shaku-database-1.1.5.tar` & `shaku-database-1.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.467533 shaku-database-1.1.5/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.5/LICENSE
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-11 09:10:42.467350 shaku-database-1.1.5/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.5/README.md
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.464006 shaku-database-1.1.5/database/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.5/database/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.464536 shaku-database-1.1.5/database/bigquery/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.5/database/bigquery/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.5/database/bigquery/bq_sql_parser.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.5/database/bigquery/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.465004 shaku-database-1.1.5/database/cloud_sql/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.5/database/cloud_sql/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.5/database/cloud_sql/crud.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.465467 shaku-database-1.1.5/database/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:09:30.000000 shaku-database-1.1.5/database/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1580 2023-07-11 09:00:21.000000 shaku-database-1.1.5/database/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.465708 shaku-database-1.1.5/gdrive_gcs_toolkit/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/__init__.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.465937 shaku-database-1.1.5/gdrive_gcs_toolkit/cloud_storage/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/cloud_storage/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/cloud_storage/util.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.466328 shaku-database-1.1.5/gdrive_gcs_toolkit/google_shared_drive/
--rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/google_shared_drive/__init__.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)    11601 2023-07-10 06:30:13.000000 shaku-database-1.1.5/gdrive_gcs_toolkit/google_shared_drive/util.py
--rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-11 09:10:42.467573 shaku-database-1.1.5/setup.cfg
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-11 09:10:11.000000 shaku-database-1.1.5/setup.py
-drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:10:42.467173 shaku-database-1.1.5/shaku_database.egg-info/
--rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/PKG-INFO
--rw-r--r--   0 tongyuhao   (501) staff       (20)      666 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/SOURCES.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/dependency_links.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/requires.txt
--rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-11 09:10:42.000000 shaku-database-1.1.5/shaku_database.egg-info/top_level.txt
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.296779 shaku-database-1.1.6/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1069 2023-06-15 08:18:42.000000 shaku-database-1.1.6/LICENSE
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-21 03:37:52.296441 shaku-database-1.1.6/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     6192 2023-06-15 08:05:19.000000 shaku-database-1.1.6/README.md
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.284351 shaku-database-1.1.6/database/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.6/database/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.284939 shaku-database-1.1.6/database/bigquery/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.6/database/bigquery/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1452 2023-07-07 09:40:34.000000 shaku-database-1.1.6/database/bigquery/bq_sql_parser.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1683 2023-06-20 03:32:33.000000 shaku-database-1.1.6/database/bigquery/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.285319 shaku-database-1.1.6/database/cloud_sql/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-05-25 07:00:04.000000 shaku-database-1.1.6/database/cloud_sql/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1139 2023-06-16 06:51:48.000000 shaku-database-1.1.6/database/cloud_sql/crud.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.285683 shaku-database-1.1.6/database/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-11 09:09:30.000000 shaku-database-1.1.6/database/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1580 2023-07-11 09:00:21.000000 shaku-database-1.1.6/database/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.286078 shaku-database-1.1.6/gdrive_gcs_toolkit/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/__init__.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.286366 shaku-database-1.1.6/gdrive_gcs_toolkit/cloud_storage/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/cloud_storage/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1183 2023-07-07 09:40:26.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/cloud_storage/util.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.286890 shaku-database-1.1.6/gdrive_gcs_toolkit/google_shared_drive/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        0 2023-07-07 09:40:26.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/google_shared_drive/__init__.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)    13463 2023-07-21 03:36:50.000000 shaku-database-1.1.6/gdrive_gcs_toolkit/google_shared_drive/util.py
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       38 2023-07-21 03:37:52.296854 shaku-database-1.1.6/setup.cfg
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1169 2023-07-21 03:37:17.000000 shaku-database-1.1.6/setup.py
+drwxr-xr-x   0 tongyuhao   (501) staff       (20)        0 2023-07-21 03:37:52.288020 shaku-database-1.1.6/shaku_database.egg-info/
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     7323 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/PKG-INFO
+-rw-r--r--   0 tongyuhao   (501) staff       (20)      666 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/SOURCES.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)        1 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/dependency_links.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)     1044 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/requires.txt
+-rw-r--r--   0 tongyuhao   (501) staff       (20)       28 2023-07-21 03:37:52.000000 shaku-database-1.1.6/shaku_database.egg-info/top_level.txt
```

### Comparing `shaku-database-1.1.5/LICENSE` & `shaku-database-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.5/PKG-INFO` & `shaku-database-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.5
+Version: 1.1.6
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.5/README.md` & `shaku-database-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.5/database/bigquery/bq_sql_parser.py` & `shaku-database-1.1.6/database/bigquery/bq_sql_parser.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.5/database/bigquery/util.py` & `shaku-database-1.1.6/database/bigquery/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.5/database/cloud_sql/crud.py` & `shaku-database-1.1.6/database/cloud_sql/crud.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.5/database/cloud_storage/util.py` & `shaku-database-1.1.6/database/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.5/gdrive_gcs_toolkit/cloud_storage/util.py` & `shaku-database-1.1.6/gdrive_gcs_toolkit/cloud_storage/util.py`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.5/gdrive_gcs_toolkit/google_shared_drive/util.py` & `shaku-database-1.1.6/gdrive_gcs_toolkit/google_shared_drive/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,66 +12,78 @@
 class GDriveToolkit:
     def __init__(self, shared_drive_id, key_file_path):
         self.SCOPES = ['https://www.googleapis.com/auth/drive']
         self.KEY_FILE_PATH = key_file_path
         self.creds = service_account.Credentials.from_service_account_file(self.KEY_FILE_PATH, scopes=self.SCOPES)
         self.service = build('drive', 'v3', credentials=self.creds)
         self.shared_drive_id = shared_drive_id
+        self.folder_dict = self.__get_folder_hierarchy(self.shared_drive_id)
 
     def __get_path_info(self, path):
 
         # get the parts of path
         path_parts = Path(path)
 
         if '.' in path_parts.name:  # Check if the last part of path is a file
             path_parts = path_parts.parent
 
         # search the corresponding file id based on the path_parts name
-        file_id = self.shared_drive_id
-        file_name = 'default'
+        current_dict = self.folder_dict
+        folder_name = 'default'
+        folder_id = 'default'
         path_id_name_list = {}
         for path_part in path_parts.parts[1:]:
-            query = f" name = '{path_part}' and '{file_id}' in parents and mimeType='application/vnd.google-apps.folder' and trashed = false"
-            results = self.service.files().list(q=query, fields='files(id, name)',
-                                                supportsAllDrives=True,
-                                                includeItemsFromAllDrives=True,
-                                                driveId=self.shared_drive_id, corpora='drive').execute()
 
-            items = results.get('files', [])
+            if path_part in current_dict and "subfolders" != {}:
+                folder_id = current_dict[path_part]["id"]
+                folder_name = path_part
+                current_dict = current_dict[path_part]["subfolders"]
 
-            if not items:
 
-                parent_id = file_id
-                folder_metadata = {
-                    'name': path_part,
-                    'mimeType': 'application/vnd.google-apps.folder',
-                    'parents': [parent_id]
-                }
-                folder = self.service.files().create(body=folder_metadata,
-                                                     supportsAllDrives=True,
-                                                     fields='id').execute()
-                file_id = folder.get('id')
-            else:
-                file_id = items[0]['id']
-                file_name = items[0]['name']
+            elif path_part in current_dict and "subfolders" == {}:
+                folder_id = current_dict[path_part]["id"]
+                folder_name = path_part
 
-            path_id_name_list[file_name] = file_id
+        path_id_name_list[folder_name] = folder_id
 
         return path_id_name_list
 
+    def __get_folder_hierarchy(self, folder_id):
+
+        query = f" '{folder_id}' in parents and mimeType = 'application/vnd.google-apps.folder' and trashed = false"
+        results = self.service.files().list(q=query, spaces='drive',
+                                            fields='files(id, name)',
+                                            supportsAllDrives=True,
+                                            includeItemsFromAllDrives=True,
+                                            driveId=self.shared_drive_id, corpora='drive'
+                                            ).execute()
+
+        items = results.get("files", [])
+        folder_dict = {}
+        for item in items:
+            folder_id = item['id']
+            folder_name = item['name']
+            subfolder_dict = self.__get_folder_hierarchy(folder_id)
+            if subfolder_dict != {}:
+
+                folder_dict[folder_name] = {'id': folder_id, 'subfolders': subfolder_dict}
+            else:
+                folder_dict[folder_name] = {'id': folder_id, 'subfolders': {}}
+        return folder_dict
+
     def read_folder_files(self, path):
 
         # input the path and return the file name and file id
-        folder_list = self.__get_path_info(path)
+        folder_info = self.__get_path_info(path)
 
         path_parts = Path(path)
 
         folder_name = path_parts.name
 
-        folder_id = folder_list[folder_name]
+        folder_id = folder_info[folder_name]
 
         try:
 
             query = f" '{folder_id}' in parents and mimeType != 'application/vnd.google-apps.folder' and trashed = false"
             results = self.service.files().list(q=query, spaces='drive',
                                                 fields='files(id, name)',
                                                 supportsAllDrives=True,
@@ -95,22 +107,22 @@
         except HttpError as error:
             raise f'An error occurred:{error}'
         except Exception as error:
             raise f'An error occurred:{error}'
 
     def read_file(self, path) -> pd.DataFrame:
 
-        folder_list = self.__get_path_info(path)
+        folder_info = self.__get_path_info(path)
 
         path_parts = Path(path)
 
         folder_name = path_parts.parent.name
         file_name = path_parts.name
 
-        folder_id = folder_list[folder_name]
+        folder_id = folder_info[folder_name]
 
         # if the last part is file, read the file
         # if len(file_name) > 0:
         file = pd.DataFrame()
         dataframes = self.__file_loader(file_name, folder_id)
         for key in dataframes.keys():
             if file_name in key:
@@ -143,15 +155,14 @@
                     file_id = item['id']
                     request = self.service.files().get_media(fileId=file_id)
                     downloaded = io.BytesIO()
                     downloader = MediaIoBaseDownload(downloaded, request)
                     done = False
                     while done is False:
                         status, done = downloader.next_chunk()
-                        print(f"Download {int(status.progress() * 100)}%.")
                     downloaded.seek(0)
                     try:
                         if item['name'].endswith('.csv'):
                             df = pd.read_csv(downloaded)
                         else:
                             df = pd.read_excel(downloaded, engine='openpyxl')
                     except:
@@ -183,14 +194,17 @@
                 for f in ZIP.namelist():
                     if f != 'xl/styles.xml':
                         zf.write(f)
                 zf.write("xl/styles_new.xml")
 
     def move_file(self, file_name, old_path, new_path):
 
+        # check folders is existed, create it if not existed
+        self.__check_folder_exist(new_path)
+
         old_path_parts = Path(old_path)
         new_path_parts = Path(new_path)
 
         old_folder_name = old_path_parts.name
         new_folder_name = new_path_parts.name
 
         old_path_info = self.__get_path_info(old_path)
@@ -212,29 +226,32 @@
 
             print(f"Moving file: {file_name}")
 
             self.service.files().update(fileId=file_id,
                                         addParents=new_folder_id,
                                         removeParents=old_folder_id,
                                         fields="id,parents", supportsAllDrives=True).execute()
-            print(f"Successfully moved file: {file_name}")
+            print(f"Successfully moved file {file_name} to {new_path}")
         except HttpError as error:
             raise f'An error occurred:{error}'
         except Exception as e:
             raise f'An error occurred:{e}'
 
     def save_to_drive(self, df, file_name, path):
 
-        folder_list = self.__get_path_info(path)
+        # check folders is existed, create it if not existed
+        self.__check_folder_exist(path)
+
+        folder_info = self.__get_path_info(path)
 
         path_parts = Path(path)
 
         folder_name = path_parts.name
 
-        folder_id = folder_list[folder_name]
+        folder_id = folder_info[folder_name]
 
         file_extension = Path(file_name).suffix
 
         try:
 
             if file_extension == ".csv":
                 # .csv is textual data so use StringIO
@@ -285,7 +302,39 @@
                 self.service.files().create(body=file_metadata, media_body=media, fields='id',
                                             supportsAllDrives=True).execute()
 
                 print(f"'{file_name}' is saved")
 
         except Exception as e:
             raise f'An error occurred:{e}'
+
+    def __check_folder_exist(self, path):
+
+        current_dict = self.folder_dict
+        path_parts = Path(path)
+        flag = False
+
+        for path_part in path_parts.parts[1:]:
+
+            if path_part in current_dict:
+                parent_id = current_dict[path_part]['id']
+                if current_dict[path_part]["subfolders"]:
+                    current_dict = current_dict[path_part]["subfolders"]
+            else:
+                flag = True
+                file_metadata = {
+                    "name": path_part,
+                    'mimeType': 'application/vnd.google-apps.folder',
+                    'parents': [parent_id]
+                }
+                try:
+                    new_folder = self.service.files().create(body=file_metadata, fields="id",
+                                                             supportsAllDrives=True).execute()
+                    current_dict[path_part] = {"id": new_folder['id'], "subfolders": {}}
+                    parent_id = new_folder['id']
+                except HttpError as error:
+                    raise f'An error occurred:{error}'
+
+        if flag == True:
+            self.folder_dict = self.__get_folder_hierarchy(self.shared_drive_id)
+            print("some folders are not existed and have been created.")
+
```

### Comparing `shaku-database-1.1.5/setup.py` & `shaku-database-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = pathlib.Path(__file__).parent.resolve()
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 EX_INSTALL_REQUIRES = {s.strip().split('==')[0]: s.strip().split('==')[1] if len(s.strip().split('==')) > 1 else ""
                        for s in requirements.split("\n")}
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
 setup(
     name="shaku-database",
-    version="1.1.5",
+    version="1.1.6",
     author="hawktorng",
     author_email="hawktorng@shaku.com.tw",
     description="Shaku Database util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/hawktorng1/test_shaku",
     packages=find_packages(),
```

### Comparing `shaku-database-1.1.5/shaku_database.egg-info/PKG-INFO` & `shaku-database-1.1.6/shaku_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaku-database
-Version: 1.1.5
+Version: 1.1.6
 Summary: Shaku Database util
 Home-page: https://gitlab.com/hawktorng1/test_shaku
 Author: hawktorng
 Author-email: hawktorng@shaku.com.tw
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shaku-database-1.1.5/shaku_database.egg-info/SOURCES.txt` & `shaku-database-1.1.6/shaku_database.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shaku-database-1.1.5/shaku_database.egg-info/requires.txt` & `shaku-database-1.1.6/shaku_database.egg-info/requires.txt`

 * *Files identical despite different names*

