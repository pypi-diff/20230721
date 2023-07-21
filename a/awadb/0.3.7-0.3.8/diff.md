# Comparing `tmp/awadb-0.3.7-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/awadb-0.3.8-cp39-cp39-macosx_13_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 2524777 bytes, number of entries: 11
--rwxr-xr-x  2.0 unx  7224968 b- defN 23-Jul-17 07:44 awa.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx    43111 b- defN 23-Jul-17 07:42 awadb/__init__.py
--rw-r--r--  2.0 unx       99 b- defN 23-Jul-16 14:55 awadb/punctuation_marks_en.py
--rw-r--r--  2.0 unx    11484 b- defN 23-Jul-16 14:55 awadb/stop_words_en.py
--rw-r--r--  2.0 unx    13236 b- defN 23-Jul-16 14:55 awadb/words_stem_en.py
--rw-r--r--  2.0 unx     1116 b- defN 23-Jul-16 15:11 awadb/llm_embedding/__init__.py
--rw-r--r--  2.0 unx    15759 b- defN 23-Jul-17 07:44 awadb-0.3.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      363 b- defN 23-Jul-17 07:44 awadb-0.3.7.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-Jul-17 07:44 awadb-0.3.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-17 07:44 awadb-0.3.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Jul-17 07:44 awadb-0.3.7.dist-info/RECORD
-11 files, 7311132 bytes uncompressed, 2523311 bytes compressed:  65.5%
+Zip file size: 1625714 bytes, number of entries: 11
+-rwxr-xr-x  2.0 unx  4467800 b- defN 23-Jul-17 02:19 awa.cpython-39-darwin.so
+-rw-r--r--  2.0 unx    45524 b- defN 23-Jul-21 14:03 awadb/__init__.py
+-rw-r--r--  2.0 unx       99 b- defN 23-Jul-17 02:07 awadb/punctuation_marks_en.py
+-rw-r--r--  2.0 unx    11484 b- defN 23-Jul-17 02:07 awadb/stop_words_en.py
+-rw-r--r--  2.0 unx    13236 b- defN 23-Jul-17 02:07 awadb/words_stem_en.py
+-rw-r--r--  2.0 unx     1116 b- defN 23-Jun-16 06:33 awadb/llm_embedding/__init__.py
+-rw-r--r--  2.0 unx    15759 b- defN 23-Jul-21 14:47 awadb-0.3.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      344 b- defN 23-Jul-21 14:47 awadb-0.3.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-21 14:47 awadb-0.3.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-21 14:47 awadb-0.3.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      868 b- defN 23-Jul-21 14:47 awadb-0.3.8.dist-info/RECORD
+11 files, 4556348 bytes uncompressed, 1624268 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: awa.cpython-39-x86_64-linux-gnu.so
+Filename: awa.cpython-39-darwin.so
 Comment: 
 
 Filename: awadb/__init__.py
 Comment: 
 
 Filename: awadb/punctuation_marks_en.py
 Comment: 
@@ -12,23 +12,23 @@
 
 Filename: awadb/words_stem_en.py
 Comment: 
 
 Filename: awadb/llm_embedding/__init__.py
 Comment: 
 
-Filename: awadb-0.3.7.dist-info/LICENSE
+Filename: awadb-0.3.8.dist-info/LICENSE
 Comment: 
 
-Filename: awadb-0.3.7.dist-info/METADATA
+Filename: awadb-0.3.8.dist-info/METADATA
 Comment: 
 
-Filename: awadb-0.3.7.dist-info/WHEEL
+Filename: awadb-0.3.8.dist-info/WHEEL
 Comment: 
 
-Filename: awadb-0.3.7.dist-info/top_level.txt
+Filename: awadb-0.3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: awadb-0.3.7.dist-info/RECORD
+Filename: awadb-0.3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awadb/__init__.py

```diff
@@ -389,14 +389,16 @@
         elif field_type == FieldDataType.FLOAT:
             awadb_field.value = struct.pack("<f", field_value)
             awadb_field.datatype = awa.DataType.FLOAT
             self.AddField(field_name, awadb_field.datatype, is_index)
         elif field_type == FieldDataType.STRING:
             awadb_field.value = field_value
             awadb_field.datatype = awa.DataType.STRING
+            if field_name == "embedding_text":
+                is_index = False
             self.AddField(field_name, awadb_field.datatype, is_index)
 
         elif field_type == FieldDataType.VECTOR:
             if type(field_value).__name__ == "ndarray":
                 awadb_field.value = field_value.tobytes()
             else:
                 vec_value = np.array(field_value, dtype=np.dtype("float32"))
@@ -523,18 +525,24 @@
                     continue
                 fvec_names.append(field_name)
 
             ret = awa.DoSearch(self.using_table_engine, req, response)
             response.PackResults(fvec_names)
 
             search_result_vec = response.Results()
-            for search_result in search_result_vec:
+            search_result_index = 0
+            while search_result_index < search_result_vec.__len__():
+                search_result = search_result_vec[search_result_index]
+            #for search_result in search_result_vec:
                 items = search_result.result_items
-                for item in items:
+                item_index = 0
+                #for item in items:
+                while item_index < items.__len__():
                     i = 0
+                    item = items[item_index] 
                     l = item.names.__len__()
                     item_detail = {}
                     while i < l:
                         name = item.names[i]
                         if (
                             not_include_fields is not None
                             and name in not_include_fields
@@ -552,19 +560,25 @@
                             item_detail[name] = float_value
                         elif f_type == FieldDataType.STRING:
                             item_detail[name] = item.values[i]
                         elif f_type == FieldDataType.VECTOR:
                             vec_data = awa.FloatVec()
                             item.GetVecData(name, vec_data)
                             vec_result = []
-                            for each_vec_data in vec_data:
+                            vec_index = 0
+                            while vec_index < vec_data.__len__():
+                                each_vec_data = vec_data[vec_index]
+                            #for each_vec_data in vec_data:
                                 vec_result.append(each_vec_data)
+                                vec_index = vec_index + 1
                             item_detail[name] = vec_result
                         i = i + 1
                     docs_detail.append(item_detail)
+                    item_index = item_index + 1
+                search_result_index = search_result_index + 1
             return docs_detail
 
         doc_results = awa.DocsMap()
         ids_list = awa.StrVec()
         for key_id in ids:
             doc_results[key_id] = awa.Doc()
             ids_list.append(key_id)
@@ -572,44 +586,76 @@
         awa.GetDocs(self.using_table_engine, ids_list, doc_results)
 
         for key_id in ids:
             if doc_results[key_id].Key() == "-1":
                 continue
 
             doc_detail = {}
-            for field in doc_results[key_id].TableFields():
+            field_index = 0
+            while field_index < doc_results[key_id].TableFields().__len__():
+                field = doc_results[key_id].TableFields()[field_index]
+            #for field in doc_results[key_id].TableFields():
                 if not_include_fields is not None and field.name in not_include_fields:
+                    field_index = field_index + 1 
                     continue
                 if field.datatype == awa.DataType.INT:
                     int_value = int(field.value)
                     doc_detail[field.name] = int_value
                 elif field.datatype == awa.DataType.FLOAT:
                     float_value = float(field.value)
                     doc_detail[field.name] = float_value
                 elif field.datatype == awa.DataType.STRING:
                     doc_detail[field.name] = field.value
+                field_index = field_index + 1
 
-            for field in doc_results[key_id].VectorFields():
+            field_index = 0
+            while field_index < doc_results[key_id].VectorFields().__len__():
+                field = doc_results[key_id].VectorFields()[field_index]
+            #for field in doc_results[key_id].VectorFields():
                 if not_include_fields is not None and field.name in not_include_fields:
+                    field_index = field_index + 1 
                     continue
                 if field.datatype == awa.DataType.VECTOR:
                     vec_data = awa.FloatVec()
                     ret = field.GetVecData(vec_data)
                     if vec_data.__len__() == 0:
                         print("Get vector data error!")
                         break
 
                     vec_result = []
-                    for each_vec_data in vec_data:
+                    vec_index = 0
+                    while vec_index < vec_data.__len__():
+                        each_vec_data = vec_data[vec_index]
+                    #for each_vec_data in vec_data:
                         vec_result.append(each_vec_data)
+                        vec_index = vec_index + 1
                     doc_detail[field.name] = vec_result
+                field_index = field_index + 1
 
             docs_detail.append(doc_detail)
         return docs_detail
 
+    def EmbedQuery(
+        self,
+        text: str,
+        **kwargs: Any,
+    ):
+        #print('enter EmbedQuery....') 
+        #texts = []
+        #texts.append(text)
+        if self.llm is None: 
+            from awadb import llm_embedding
+            self.llm = llm_embedding.LLMEmbedding()
+        #print(text) 
+        return self.llm.Embedding(text)
+
+        #embeddings = self.llm.EmbeddingQuery(text)
+        #print(embeddings)
+        #return embeddings
+
     def __TextPreprocess(
         self,
         text: str,
         **kwargs: Any,
     ) -> Dict[str, int]:
         words = text.split()  # now just support english
         words_count_dict: Dict[str, int] = {}
@@ -1027,26 +1073,31 @@
         for field_name in self.tables_fields_names[self.using_table_name]:
             if field_name == "_id" or (
                 not_include_fields is not None and field_name in not_include_fields
             ):
                 continue
 
             fvec_names.append(field_name)
-
+ 
         ret = awa.DoSearch(self.using_table_engine, req, response)
         response.PackResults(fvec_names)
 
         search_result_vec = response.Results()
-        for search_result in search_result_vec:
+        search_result_index = 0 
+        while search_result_index < search_result_vec.__len__():
+            search_result = search_result_vec[search_result_index]
             result_per_request = {}
             result_per_request["ResultSize"] = search_result.result_items.__len__()
 
             result_items_list = []
             items = search_result.result_items
-            for item in items:
+            item_index = 0 
+            #for item in items:
+            while item_index < items.__len__():
+                item = items[item_index]
                 i = 0
                 l = item.names.__len__()
                 item_detail = {}
                 while i < l:
                     name = item.names[i]
                     if not_include_fields is not None and name in not_include_fields:
                         i = i + 1
@@ -1063,18 +1114,23 @@
                         item_detail[name] = float_value
                     elif f_type == FieldDataType.STRING:
                         item_detail[name] = item.values[i]
                     elif f_type == FieldDataType.VECTOR:
                         vec_data = awa.FloatVec()
                         item.GetVecData(name, vec_data)
                         vec_result = []
-                        for each_vec_data in vec_data:
+                        j = 0
+                        while j < vec_data.__len__():
+                            each_vec_data = vec_data[j]
                             vec_result.append(each_vec_data)
+                            j = j + 1
                         item_detail[name] = vec_result
                     i = i + 1
                 if not_include_fields is not None and "score" not in not_include_fields:
                     item_detail["score"] = item.score
                 result_items_list.append(item_detail)
+                item_index = item_index + 1
 
             result_per_request["ResultItems"] = result_items_list
             show_results.append(result_per_request)
+            search_result_index = search_result_index + 1
         return show_results
```

## Comparing `awadb-0.3.7.dist-info/LICENSE` & `awadb-0.3.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awadb-0.3.7.dist-info/RECORD` & `awadb-0.3.8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-awa.cpython-39-x86_64-linux-gnu.so,sha256=dhI6XGtNVYYdiOG5vH2Ii8vvxp_XOMZrFkRRebkZaLA,7224968
-awadb/__init__.py,sha256=K6RKugwWkA6bDyakYo3tepqh082wvVKCbB85SkrooA4,43111
+awa.cpython-39-darwin.so,sha256=-_OS5cRniSfxZWkzywJJmJFa6A-b9WB5QXeNx_SlUvQ,4467800
+awadb/__init__.py,sha256=2QHqJez2EyAmcLlaQ_UzfUsWzzIoNEpxR-Cpa-h-9qY,45524
 awadb/punctuation_marks_en.py,sha256=iGKZzDqYLn4BGtcJ_i6FLVxL7R434eN72fhH0J7fEqo,99
 awadb/stop_words_en.py,sha256=uMRjtiGmBs2d6JqYXmFA3ICFbL74Oc5QLg-e2ZWhQns,11484
 awadb/words_stem_en.py,sha256=NteZaVk7mq15tYus3BDs9opb-LCybbOXeFFZDiik5jc,13236
 awadb/llm_embedding/__init__.py,sha256=4bk7F1jZW5w3MnqK98ojMysgDFRAuRL0_kE61qE-G1A,1116
-awadb-0.3.7.dist-info/LICENSE,sha256=_C8nbg50jUKzeKYx7e0LufHTUvlTw6gtloKQTms7fKE,15759
-awadb-0.3.7.dist-info/METADATA,sha256=GVyUBcNGIS9AtVqXao3udPnBmfaxyclYtZTQ9pZrZXU,363
-awadb-0.3.7.dist-info/WHEEL,sha256=LrizK2MHoduzM5QxL2KpqaPs9dWHcHab3k-KJZvbHOw,108
-awadb-0.3.7.dist-info/top_level.txt,sha256=ZZiN74SXyPZTb-mYHlpTS950dK4saVYJ-xXHLZwjq74,10
-awadb-0.3.7.dist-info/RECORD,,
+awadb-0.3.8.dist-info/LICENSE,sha256=_C8nbg50jUKzeKYx7e0LufHTUvlTw6gtloKQTms7fKE,15759
+awadb-0.3.8.dist-info/METADATA,sha256=k7eOB4gzp-nV_Ts-ELW3DT0XAQTKscCwsqWYxszV3fg,344
+awadb-0.3.8.dist-info/WHEEL,sha256=zz32RjpDRYSYdgnx3Bklgj6suPtc_HuWpXLAJPsGhtU,108
+awadb-0.3.8.dist-info/top_level.txt,sha256=ZZiN74SXyPZTb-mYHlpTS950dK4saVYJ-xXHLZwjq74,10
+awadb-0.3.8.dist-info/RECORD,,
```

