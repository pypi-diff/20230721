# Comparing `tmp/trdate-1.0.0.tar.gz` & `tmp/trdate-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trdate-1.0.0.tar", max compression
+gzip compressed data, was "trdate-1.0.1.tar", max compression
```

## Comparing `trdate-1.0.0.tar` & `trdate-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1114 2023-07-20 09:38:14.395566 trdate-1.0.0/LICENSE
--rw-r--r--   0        0        0      503 2023-07-21 10:58:35.150937 trdate-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       19 2023-07-20 13:15:49.355566 trdate-1.0.0/trdate/__init__.py
--rw-r--r--   0        0        0       66 2023-07-20 13:16:14.675566 trdate-1.0.0/trdate/code/__init__.py
--rw-r--r--   0        0        0     6085 2023-07-20 14:01:07.275566 trdate-1.0.0/trdate/code/date_utils.py
--rw-r--r--   0        0        0    15340 2023-07-21 10:14:07.570937 trdate-1.0.0/trdate/code/main.py
--rw-r--r--   0        0        0      294 2023-07-20 13:45:18.215566 trdate-1.0.0/trdate/code/utils.py
--rw-r--r--   0        0        0       56 2023-07-20 09:08:07.785566 trdate-1.0.0/trdate/tests/__init__.py
--rw-r--r--   0        0        0     2460 2023-07-20 13:18:40.085566 trdate-1.0.0/trdate/tests/test_date_utils.py
--rw-r--r--   0        0        0      213 2023-07-20 14:30:25.595566 trdate-1.0.0/trdate/tests/test_main.py
--rw-r--r--   0        0        0      361 2023-07-20 13:19:06.405566 trdate-1.0.0/trdate/tests/test_utils.py
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 trdate-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1114 2023-07-20 09:38:14.395566 trdate-1.0.1/LICENSE
+-rw-r--r--   0        0        0      503 2023-07-21 12:49:41.140937 trdate-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       19 2023-07-20 13:15:49.355566 trdate-1.0.1/trdate/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-20 13:16:14.675566 trdate-1.0.1/trdate/code/__init__.py
+-rw-r--r--   0        0        0     6085 2023-07-20 14:01:07.275566 trdate-1.0.1/trdate/code/date_utils.py
+-rw-r--r--   0        0        0    15591 2023-07-21 12:45:41.040937 trdate-1.0.1/trdate/code/main.py
+-rw-r--r--   0        0        0      294 2023-07-20 13:45:18.215566 trdate-1.0.1/trdate/code/utils.py
+-rw-r--r--   0        0        0       56 2023-07-20 09:08:07.785566 trdate-1.0.1/trdate/tests/__init__.py
+-rw-r--r--   0        0        0     2460 2023-07-20 13:18:40.085566 trdate-1.0.1/trdate/tests/test_date_utils.py
+-rw-r--r--   0        0        0      213 2023-07-20 14:30:25.595566 trdate-1.0.1/trdate/tests/test_main.py
+-rw-r--r--   0        0        0      361 2023-07-20 13:19:06.405566 trdate-1.0.1/trdate/tests/test_utils.py
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 trdate-1.0.1/PKG-INFO
```

### Comparing `trdate-1.0.0/LICENSE` & `trdate-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trdate-1.0.0/trdate/code/date_utils.py` & `trdate-1.0.1/trdate/code/date_utils.py`

 * *Files identical despite different names*

### Comparing `trdate-1.0.0/trdate/code/main.py` & `trdate-1.0.1/trdate/code/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,54 +134,58 @@
         -------
         `list`
             Список строк, где месяцы заменены на числовой формат и добавлены метки '`MM`' и '`DD`'.
 
         Example
         -------
         >>> transform_date = TransFormDate()
-        >>> transform_date.list_array = ["января", "какой-то текст", "февраля", "еще текст", "декабря"]
+        >>> transform_date.list_array = ["2023", "год", "июль", "21"]
         >>> result = transform_date.monthLines()
         >>> print(result)
-        ['1MM', 'какой-то текст', '2MM', 'еще текст', '12MM']
+        ['2023YY', 'год', '07MM', '21DD']
         """
         dict_month = {
-            "января": "1",
-            "февраля": "2",
-            "марта": "3",
-            "апреля": "4",
-            "мая": "5",
-            "июня": "6",
-            "июля": "7",
-            "августа": "8",
-            "сентября": "9",
-            "октября": "10",
-            "ноября": "11",
-            "декабря": "12"
+            r"^январ": 1,
+            r"^феврал": 2,
+            r"^март": 3,
+            r"^апрел": 4,
+            r"^май": 5,
+            r"^июн": 6,
+            r"^июл": 7,
+            r"^август": 8,
+            r"^сентябр": 9,
+            r"^октябр": 10,
+            r"^ноябр": 11,
+            r"^декабр": 12
         }
         for i, item in enumerate(self.list_array):
-            if item in dict_month:
-                self.list_array[i] = f"{dict_month[item]}MM"
-                self.month = dict_month[item]
-                if i != 0:
-                    self.day = self.list_array[i-1]
-                    self.list_array[i-1] = f"{self.list_array[i-1]}DD"
+            for regex_pattern, month_num in dict_month.items():
+                if re.search(regex_pattern, item, re.IGNORECASE):
+                    self.list_array[i] = f"{month_num:02d}MM"
+                    self.month = month_num
+                    if i != 0 and re.search(r"\d|\d\d", self.list_array[i-1]):
+                        self.day = self.list_array[i-1]
+                        self.list_array[i-1] = f"{self.list_array[i-1]}DD"
+                    elif len(self.list_array) > i + 1 and re.search(r"\d|\d\d", self.list_array[i+1]):
+                        self.day = self.list_array[i+1]
+                        self.list_array[i+1] = f"{self.list_array[i+1]}DD"
                     return self.stringLines(self.list_array)
-            elif re.search(r"^вчера", item, re.IGNORECASE):
+            if re.search(r"^вчера", item, re.IGNORECASE):
                 yesterday = dt.datetime.now() - dt.timedelta(days=1)
                 month_date = yesterday.strftime("%m")
                 day_date = yesterday.strftime("%d")
-                self.list_array[i] = f"{month_date}MM {day_date}DD"
+                self.list_array[i] = f"{month_date}MM {day_date:02d}DD"
                 self.month = month_date
                 self.day = day_date
                 return self.list_array
-            elif re.search(r"позавчера", item, re.IGNORECASE):
+            elif re.search(r"^позавчера", item, re.IGNORECASE):
                 day_before_yesterday = dt.datetime.now() - dt.timedelta(days=2)
                 month_date = day_before_yesterday.strftime("%m")
                 day_date = day_before_yesterday.strftime("%d")
-                self.list_array[i] = f"{month_date}MM {day_date}DD"
+                self.list_array[i] = f"{month_date}MM {day_date:02d}DD"
                 self.month = month_date
                 self.day = day_date
                 return self.list_array
         return self.list_array
 
     def hourLines(self):
         """
@@ -256,15 +260,15 @@
             elif re.search(r"^(0?[1-9]|1[0-9]|2[0-3])$", item, re.IGNORECASE):
                 if len(self.list_array) > i + 2 and re.search(r"^\d{2}$", self.list_array[i + 1], re.IGNORECASE):
                     self.hour = self.list_array[i]
                     self.list_array[i] = f"{self.list_array[i]}HH"
                     self.minute = self.list_array[i+1]
                     self.list_array[i+1] = f"{self.list_array[i+1]}MI"
                     return self.list_array
-                elif re.search(r"^минут", self.list_array[i+1], re.IGNORECASE) == None:
+                elif len(self.list_array) > i+1 and re.search(r"^минут", self.list_array[i+1], re.IGNORECASE) == None:
                     self.hour = self.list_array[i]
                     self.list_array[i] = f"{self.list_array[i]}HH"
                     return self.list_array
 
     def minuteLines(self):
         """
         Ищет строки, начинающиеся с 'минут' в списке `list_array` и выполняет определенные действия.
@@ -305,29 +309,27 @@
 
     def get_date_list(self, line):
         """
         Метод для получения списка дат из строки `line` и обработки их.
 
         Parameters
         ----------
-        line : str
+        `line` : `str`
             Строка, содержащая даты в определенном формате.
 
         Returns
         -------
-        None
+        `None`
 
         Example
         -------
         >>> transform_date = TransFormDate()
-        >>> line = "2023-07-21, 2023-07-22, 2023-07-23"
+        >>> line = "2023 год июль 21"
         >>> transform_date.get_date_list(line)
-        2023-07-21
-        2023-07-22
-        2023-07-23
+        2023-07-21 00:00:00
         """
         self.list_array = self.splitLines(line)
         self.yearLines()
         self.monthLines()
         self.hourLines()
         self.minuteLines()
 
@@ -342,9 +344,9 @@
             print(parsed_date)
         else:
             print(parsed_date)
 
 
 if __name__ == '__main__':
     ds = TransFormDate()
-    ds.get_date_list("6 часов утра 34 минуты")
+    ds.get_date_list("2023 год июль 21")
     print(ds)
```

### Comparing `trdate-1.0.0/trdate/tests/test_date_utils.py` & `trdate-1.0.1/trdate/tests/test_date_utils.py`

 * *Files identical despite different names*

