# Comparing `tmp/trdate-1.0.1.tar.gz` & `tmp/trdate-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trdate-1.0.1.tar", max compression
+gzip compressed data, was "trdate-1.0.2.tar", max compression
```

## Comparing `trdate-1.0.1.tar` & `trdate-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1114 2023-07-20 09:38:14.395566 trdate-1.0.1/LICENSE
--rw-r--r--   0        0        0      503 2023-07-21 12:49:41.140937 trdate-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       19 2023-07-20 13:15:49.355566 trdate-1.0.1/trdate/__init__.py
--rw-r--r--   0        0        0       66 2023-07-20 13:16:14.675566 trdate-1.0.1/trdate/code/__init__.py
--rw-r--r--   0        0        0     6085 2023-07-20 14:01:07.275566 trdate-1.0.1/trdate/code/date_utils.py
--rw-r--r--   0        0        0    15591 2023-07-21 12:45:41.040937 trdate-1.0.1/trdate/code/main.py
--rw-r--r--   0        0        0      294 2023-07-20 13:45:18.215566 trdate-1.0.1/trdate/code/utils.py
--rw-r--r--   0        0        0       56 2023-07-20 09:08:07.785566 trdate-1.0.1/trdate/tests/__init__.py
--rw-r--r--   0        0        0     2460 2023-07-20 13:18:40.085566 trdate-1.0.1/trdate/tests/test_date_utils.py
--rw-r--r--   0        0        0      213 2023-07-20 14:30:25.595566 trdate-1.0.1/trdate/tests/test_main.py
--rw-r--r--   0        0        0      361 2023-07-20 13:19:06.405566 trdate-1.0.1/trdate/tests/test_utils.py
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 trdate-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1114 2023-07-20 09:38:14.395566 trdate-1.0.2/LICENSE
+-rw-r--r--   0        0        0      503 2023-07-21 14:18:41.000937 trdate-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       19 2023-07-20 13:15:49.355566 trdate-1.0.2/trdate/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-20 13:16:14.675566 trdate-1.0.2/trdate/code/__init__.py
+-rw-r--r--   0        0        0     6085 2023-07-20 14:01:07.275566 trdate-1.0.2/trdate/code/date_utils.py
+-rw-r--r--   0        0        0    15959 2023-07-21 14:16:49.830937 trdate-1.0.2/trdate/code/main.py
+-rw-r--r--   0        0        0      294 2023-07-20 13:45:18.215566 trdate-1.0.2/trdate/code/utils.py
+-rw-r--r--   0        0        0       56 2023-07-20 09:08:07.785566 trdate-1.0.2/trdate/tests/__init__.py
+-rw-r--r--   0        0        0     2460 2023-07-20 13:18:40.085566 trdate-1.0.2/trdate/tests/test_date_utils.py
+-rw-r--r--   0        0        0      926 2023-07-21 14:16:38.780937 trdate-1.0.2/trdate/tests/test_main.py
+-rw-r--r--   0        0        0      361 2023-07-20 13:19:06.405566 trdate-1.0.2/trdate/tests/test_utils.py
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 trdate-1.0.2/PKG-INFO
```

### Comparing `trdate-1.0.1/LICENSE` & `trdate-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trdate-1.0.1/trdate/code/date_utils.py` & `trdate-1.0.2/trdate/code/date_utils.py`

 * *Files identical despite different names*

### Comparing `trdate-1.0.1/trdate/code/main.py` & `trdate-1.0.2/trdate/code/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,22 +29,22 @@
     `get_d`(self) -> datetime:
         Возвращает объект `datetime`, полученный из атрибутов `year`, `month`, `day`, `hour`, `minute` и `second`.
 
     `get_date_list`(self, line: str) -> List[datetime]:
         Метод для получения списка дат из строки `line` и обработки их.
     """
 
-    def __init__(self):
+    def __init__(self, _str=f'{dt.datetime.now().strftime("%Y-%m-%d %H:%M:%S")}'):
         self.year = dt.datetime.now().year
         self.month = dt.datetime.now().month
         self.day = dt.datetime.now().day
         self.hour = "00"
         self.minute = "00"
         self.second = "00"
-        self.list_array = self.splitLines("сегодня")
+        self.list_array = self.splitLines(_str)
 
     def __str__(self):
         return f"{self.list_array}"
 
     def stringLines(self, string):
         """
         Объединяет строки в переданном списке `string` в одну строку, разделяя пробелами.
@@ -103,15 +103,15 @@
         -------
         `list`
             Список с обработанными элементами, включающими год.
 
         Example
         -------
         >>> transform_date = TransFormDate()
-        >>> transform_date.list_array = ['элемент', 'год', '20', 'YY']
+        >>> transform_date.list_array = ["20", "1000", "23", "год"]
         >>> result = transform_date.yearLines()
         >>> print(result)
         ['элемент', '2020YY', '20YY']
         """
         for i, item in enumerate(self.list_array):
             if re.search(r"^год$", item):
                 self.year = f"20{self.list_array[i-1]}" if len(
@@ -156,39 +156,43 @@
             r"^октябр": 10,
             r"^ноябр": 11,
             r"^декабр": 12
         }
         for i, item in enumerate(self.list_array):
             for regex_pattern, month_num in dict_month.items():
                 if re.search(regex_pattern, item, re.IGNORECASE):
-                    self.list_array[i] = f"{month_num:02d}MM"
+                    self.list_array[i] = f"{month_num}MM"
                     self.month = month_num
-                    if i != 0 and re.search(r"\d|\d\d", self.list_array[i-1]):
+                    if i != 0 and re.search(r"^\d{1}$|^\d{2}$", self.list_array[i-1]):
                         self.day = self.list_array[i-1]
                         self.list_array[i-1] = f"{self.list_array[i-1]}DD"
-                    elif len(self.list_array) > i + 1 and re.search(r"\d|\d\d", self.list_array[i+1]):
+                    elif len(self.list_array) > i + 1 and re.search(r"^\d{1}$|^\d{2}$", self.list_array[i+1]):
                         self.day = self.list_array[i+1]
                         self.list_array[i+1] = f"{self.list_array[i+1]}DD"
                     return self.stringLines(self.list_array)
             if re.search(r"^вчера", item, re.IGNORECASE):
                 yesterday = dt.datetime.now() - dt.timedelta(days=1)
                 month_date = yesterday.strftime("%m")
                 day_date = yesterday.strftime("%d")
-                self.list_array[i] = f"{month_date}MM {day_date:02d}DD"
+                self.list_array[i] = f"{month_date}MM {day_date}DD"
                 self.month = month_date
                 self.day = day_date
                 return self.list_array
             elif re.search(r"^позавчера", item, re.IGNORECASE):
                 day_before_yesterday = dt.datetime.now() - dt.timedelta(days=2)
                 month_date = day_before_yesterday.strftime("%m")
                 day_date = day_before_yesterday.strftime("%d")
-                self.list_array[i] = f"{month_date}MM {day_date:02d}DD"
+                self.list_array[i] = f"{month_date}MM {day_date}DD"
                 self.month = month_date
                 self.day = day_date
                 return self.list_array
+            elif re.search(r"^числ", item, re.IGNORECASE):
+                self.list_array[i-1] = f"{self.list_array[i-1]}DD"
+                self.day = self.list_array[i-1]
+                return self.list_array
         return self.list_array
 
     def hourLines(self):
         """
         Метод для обработки списка строк и определения времени в формате часов и минут.
 
         Returns
@@ -254,24 +258,25 @@
                     elif int(self.list_array[i + 1]) == 12:
                         self.list_array[i +
                                         1] = int(self.list_array[i + 1]) - 12
                     self.hour = self.list_array[i+1]
                     self.list_array[i+1] = f"{self.list_array[i+1]}HH"
                     return self.list_array
             elif re.search(r"^(0?[1-9]|1[0-9]|2[0-3])$", item, re.IGNORECASE):
-                if len(self.list_array) > i + 2 and re.search(r"^\d{2}$", self.list_array[i + 1], re.IGNORECASE):
+                if len(self.list_array) > i + 2 and re.search(r"^\d{1}$|^\d{2}$", self.list_array[i + 1], re.IGNORECASE):
                     self.hour = self.list_array[i]
                     self.list_array[i] = f"{self.list_array[i]}HH"
                     self.minute = self.list_array[i+1]
                     self.list_array[i+1] = f"{self.list_array[i+1]}MI"
                     return self.list_array
-                elif len(self.list_array) > i+1 and re.search(r"^минут", self.list_array[i+1], re.IGNORECASE) == None:
+                elif len(self.list_array) > i+1 and re.search(r"^минут", self.list_array[i+1], re.IGNORECASE) == None and self.list_array[i+1] != '1000':
                     self.hour = self.list_array[i]
                     self.list_array[i] = f"{self.list_array[i]}HH"
                     return self.list_array
+        return self.list_array
 
     def minuteLines(self):
         """
         Ищет строки, начинающиеся с 'минут' в списке `list_array` и выполняет определенные действия.
 
         Returns
         -------
@@ -303,15 +308,15 @@
             Объект `datetime`, представляющий дату и время, соответствующие атрибутам класса.
         """
         date_string = f"{self.year}-{self.month}-{self.day} {self.hour}:{self.minute}:{self.second}"
         date_format = "%Y-%m-%d %H:%M:%S"
         parsed_date = dt.datetime.strptime(date_string, date_format)
         return parsed_date
 
-    def get_date_list(self, line):
+    def get_date_list(self, line="2021 января 1 1 1"):
         """
         Метод для получения списка дат из строки `line` и обработки их.
 
         Parameters
         ----------
         `line` : `str`
             Строка, содержащая даты в определенном формате.
@@ -344,9 +349,9 @@
             print(parsed_date)
         else:
             print(parsed_date)
 
 
 if __name__ == '__main__':
     ds = TransFormDate()
-    ds.get_date_list("2023 год июль 21")
-    print(ds)
+    ds.get_date_list("20 1000 23 год 3 июля 23 59")
+    print(ds)
```

### Comparing `trdate-1.0.1/trdate/tests/test_date_utils.py` & `trdate-1.0.2/trdate/tests/test_date_utils.py`

 * *Files identical despite different names*

