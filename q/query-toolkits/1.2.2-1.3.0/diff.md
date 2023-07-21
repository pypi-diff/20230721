# Comparing `tmp/query_toolkits-1.2.2-py3-none-any.whl.zip` & `tmp/query_toolkits-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 2515022 bytes, number of entries: 18
+Zip file size: 2515100 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      845 b- defN 23-May-22 02:33 query_toolkits/__init__.py
 -rw-r--r--  2.0 unx    40836 b- defN 23-Mar-29 03:08 query_toolkits/error_correction.py
--rw-r--r--  2.0 unx    26728 b- defN 23-Jun-01 03:20 query_toolkits/extractor.py
+-rw-r--r--  2.0 unx    27111 b- defN 23-Jul-21 03:06 query_toolkits/extractor.py
 -rw-r--r--  2.0 unx      783 b- defN 23-Jun-01 03:18 query_toolkits/financial_index.txt
 -rw-r--r--  2.0 unx    16386 b- defN 23-Jun-01 04:01 query_toolkits/financial_index_full.txt
 -rw-r--r--  2.0 unx  1056198 b- defN 23-Feb-27 08:08 query_toolkits/fund_product.txt
 -rw-r--r--  2.0 unx    18015 b- defN 23-May-16 12:35 query_toolkits/index.txt
 -rw-------  2.0 unx 44320114 b- defN 23-Mar-29 02:13 query_toolkits/info.json
 -rw-r--r--  2.0 unx      153 b- defN 22-Oct-10 04:02 query_toolkits/keyword.txt
 -rw-r--r--  2.0 unx   634483 b- defN 22-Oct-12 02:15 query_toolkits/organization.txt
 -rw-r--r--  2.0 unx     9995 b- defN 23-May-16 12:30 query_toolkits/product.txt
 -rw-r--r--  2.0 unx     2237 b- defN 22-Aug-15 03:50 query_toolkits/unit_transform
 -rw-r--r--  2.0 unx     5453 b- defN 23-Mar-29 02:52 query_toolkits/utils.py
 -rw-------  2.0 unx   420676 b- defN 22-Oct-20 07:33 query_toolkits/weapon.txt
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-01 08:43 query_toolkits-1.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 08:43 query_toolkits-1.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-01 08:43 query_toolkits-1.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1534 b- defN 23-Jun-01 08:43 query_toolkits-1.2.2.dist-info/RECORD
-18 files, 46554773 bytes uncompressed, 2512522 bytes compressed:  94.6%
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-21 07:58 query_toolkits-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 07:58 query_toolkits-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-21 07:58 query_toolkits-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1534 b- defN 23-Jul-21 07:58 query_toolkits-1.3.0.dist-info/RECORD
+18 files, 46555156 bytes uncompressed, 2512600 bytes compressed:  94.6%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: query_toolkits/utils.py
 Comment: 
 
 Filename: query_toolkits/weapon.txt
 Comment: 
 
-Filename: query_toolkits-1.2.2.dist-info/METADATA
+Filename: query_toolkits-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: query_toolkits-1.2.2.dist-info/WHEEL
+Filename: query_toolkits-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: query_toolkits-1.2.2.dist-info/top_level.txt
+Filename: query_toolkits-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: query_toolkits-1.2.2.dist-info/RECORD
+Filename: query_toolkits-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## query_toolkits/extractor.py

```diff
@@ -53,28 +53,28 @@
                 return True
         elif type == "minute":
             if number_str in list(map(str, range(0, 61))) + special_num_list + ["00"]:
                 return True
         return False
 
 
-    def _fill_slot(self, text):
+    def _fill_slot(self, text, is_title=False):
         year = None
         month = None
         day = None
         hour = None
         second = None
         minute = None
         case_year = "(\d{4})年"
         case_month = "(\d{1,2})(月份|月)"
         case_day = "(\d{1,2})[日|号]"
         case_hour = "(\d{1,2})[点|时]"
         case_second = "(\d{1,2})(分钟|分)"
         case_minute = "(\d{1,2})秒"
-        key_year = {'今年': 0, '去年': -1, '前年': -2, "明年": 1, "前一年": -1, "大前年":-3}
+        key_year = dict() if is_title else {'今年': 0, '去年': -1, '前年': -2, "明年": 1, "前一年": -1, "大前年":-3}
         for key in key_year:
             if key in text:
                 year = str(datetime.now().year + key_year[key])
         res_year = re.search(case_year, text)
         res_month = re.search(case_month, text)
         res_day = re.search(case_day, text)
         res_hour = re.search(case_hour, text)
@@ -201,29 +201,35 @@
             day = int(elem[6:])
             if year >= 1949 and year <= 2100 and month in range(13) and day in range(32):
                 final_res.append((year, month, day))
         return final_res
 
 
     # 时间提取
-    def extract_time(self, text, cut_res):
+    def extract_time(self, text, cut_res, is_title=False):
         time_res = []
         date_list = []
         index_list = []
         # 字典键值对用冒号分割，每个键值对之间用逗号分割，整个字典包括在花括号{}中
         # dict.get(key, default=None)返回指定键的值，如果值不在字典中返回default值
-        key_date = utils.key_date
-        week_day = utils.week_day
+        if is_title:
+            key_date = dict()
+            week_day = dict()
+            pattern = "\d{4}年\d{1,2}月\d{1,2}[号|日]|\d{4}[-\./]\d{1,2}[-\./]\d{1,2}|"
+            "\d{4}年\d{1,2}月|\d{4}年|\d{4}-\d{1,2}|\d{4}\.\d{1,2}|\d{4}/\d{1,2}|"
+            "\d{2}[:：]\d{2}([:：]\d{2})?|\d{1,2}[点|时]\d{1,2}[分|分钟](\d{1,2}[秒])?"
+        else:
+            key_date = utils.key_date
+            week_day = utils.week_day
+            pattern =  "(去年|今年|前年|明年|前一年)?\d{1,2}月\d{1,2}[号|日]|\d{4}年\d{1,2}月\d{1,2}[号|日]|\d{4}[-\./]\d{1,2}[-\./]\d{1,2}|"
+            "\d{4}年\d{1,2}月|\d{4}年|\d{4}-\d{1,2}|\d{4}\.\d{1,2}|\d{4}/\d{1,2}|"
+            "\d{2}[:：]\d{2}([:：]\d{2})?|\d{1,2}[点|时]\d{1,2}[分|分钟](\d{1,2}[秒])?"
 
         # 检测英文写法日期8位数字
-        date_dig = re.finditer(
-            "(去年|今年|前年|明年|前一年)?\d{1,2}月\d{1,2}[号|日]|\d{4}年\d{1,2}月\d{1,2}[号|日]|\d{4}[-\./]\d{1,2}[-\./]\d{1,2}|"
-            "\d{4}年\d{1,2}月|\d{4}年|\d{4}-\d{1,2}|\d{4}\.\d{1,2}|\d{4}/\d{1,2}|"
-            "\d{2}[:：]\d{2}([:：]\d{2})?|\d{1,2}[点|时]\d{1,2}[分|分钟](\d{1,2}[秒])?",
-            text)
+        date_dig = re.finditer(pattern, text)
         if date_dig:
             for dd in date_dig:
                 date_list.append(dd.group(0))
                 index_list.append(dd.span())
         phrase = ""
         phrase_list = []
         for i, (k, v) in enumerate(cut_res):
@@ -242,15 +248,15 @@
             elif v not in ("m", "t", "x") and phrase != "":
                 phrase_list.append(phrase)
                 phrase = ""
         if phrase != "":
             phrase_list.append(phrase)
 
         result = list(filter(lambda x: x is not None, [self._check_time_valid(w) for w in time_res + date_list + phrase_list]))
-        final_res = [self._fill_slot(x) for x in result]
+        final_res = [self._fill_slot(x, is_title) for x in result]
         final_res = [x for x in final_res if x is not None]
         final_res_copy = final_res.copy()
         remove_set = set()
         final_res = []
         for i1, res1 in enumerate(final_res_copy):
             for i2 in range(i1, len(final_res_copy)):
                 res2 = final_res_copy[i2]
@@ -599,18 +605,18 @@
 
 
 
 
 
 
 
-# if __name__ == '__main__':
-#     import time
-#     import jieba.posseg as psg
-#     et = Extractor()
+if __name__ == '__main__':
+    import time
+    import jieba.posseg as psg
+    et = Extractor()
 #     cut_res = psg.cut("pe和市净率市盈率吃在2432净资产收益率在5%理财宝364天期470号 理财宝28天期580号中国平安贵州茅台SH000002 SH00000566")
 #     cut_words = [k for k,v in cut_res]
 #     print(cut_words)
 #     print(cut_words)
 #     res = et.extract_financial_index(cut_words)
 #     print(res)
 #     res = et.extract_fund_name(cut_words)
@@ -637,59 +643,61 @@
 #     res = et.extract_reference_no("银发〔2015〕324号/JR/T 0125-2015")
 #     print(res)
 #     print(datetime.today())
 #     start = time.time()
 #     # text = "2021-03-0914:00开庭审理杨峰？"
 #     # get_range_time_from_query(text)
 #     # exit(0)
-#     li = [
-#         '20161204',
-#         '23434455',
-#         '现在是20110809',
-#         '20110809oh',
-#         '上周六的股票',
-#         '我前天来的',
-#         '我今天到的',
-#         '12月26号的天气怎么样',
-#         '2020.10.03的2022.1.5利率是多少？',
-#         "周二的api是多少",
-#         "2018/1/1,利率",
-#         "现在，利率",
-#         "8月1日，利率",
-#         "9.8，利率",
-#         "第3026期，利率",
-#         "2019年7月1日的利率是多少",
-#         "2020年8月1日 利率",
-#         "8月1日 利率",
-#         "1月5日 利率",
-#         "2022年11月1日中国历史",
-#         "中国2021年9月18日历史",
-#         "利现在，率",
-#         "利2018/1/1,率",
-#         "利8月1日 率",
-#         "20年8月1日 利率",
-#         '的2022.1.5利率是多少？',
-#         '去年9月10日利率是多少？',
-#         '2020年12月利率是多少？',
-#         '2020.1/26利率是多少？',
-#         '利率2020.1/26是多少？',
-#         '利率是多少？2020.1/26',
-#         '利率2020.1月26是多少？',
-#         '利率2020年1月2日是多少？',
-#         '我可以9月10日利率是多少？',
-#         '2021-03-09 14:00开庭审理杨峰',
-#         '2021-03-0914:00开庭审理杨峰',
-#         '01-09 14:00开庭审理杨峰',
-#         '03 09 yuhuagangtie',
-#         '2022年11月12日 14:00开庭审理杨峰',
-#         '我上上周五的时候利率',
-#         '2015年3月5日 14：32到5月22日 13：00',
-#         '1993年5月28',
-#         '大前年',
-#         '达观数据']
-#     for text in li:
-#         cut_res = list(psg.cut(text))
-#         print(text)
-#         res = et.extract_time(text, cut_res)
-#         print(res)
+    li = [
+        '20161204',
+        '23434455',
+        '现在是20110809',
+        '20110809oh',
+        '上周六的股票',
+        '我前天来的',
+        '我今天到的',
+        '12月26号的天气怎么样',
+        '2020.10.03的2022.1.5利率是多少？',
+        "周二的api是多少",
+        "2018/1/1,利率",
+        "现在，利率",
+        "8月1日，利率",
+        "9.8，利率",
+        "第3026期，利率",
+        "2019年7月1日的利率是多少",
+        "2020年8月1日 利率",
+        "8月1日 利率",
+        "1月5日 利率",
+        "2022年11月1日中国历史",
+        "中国2021年9月18日历史",
+        "利现在，率",
+        "利2018/1/1,率",
+        "利8月1日 率",
+        "20年8月1日 利率",
+        '的2022.1.5利率是多少？',
+        '去年9月10日利率是多少？',
+        '2020年12月利率是多少？',
+        '2020.1/26利率是多少？',
+        '利率2020.1/26是多少？',
+        '利率是多少？2020.1/26',
+        '利率2020.1月26是多少？',
+        '利率2020年1月2日是多少？',
+        '我可以9月10日利率是多少？',
+        '2021-03-09 14:00开庭审理杨峰',
+        '2021-03-0914:00开庭审理杨峰',
+        '01-09 14:00开庭审理杨峰',
+        '03 09 yuhuagangtie',
+        '2022年11月12日 14:00开庭审理杨峰',
+        '我上上周五的时候利率',
+        '2015年3月5日 14：32到5月22日 13：00',
+        '1993年5月28',
+        '大前年',
+        '达观数据',
+        "1999年",
+    "上周五"]
+    for text in li:
+        cut_res = list(psg.cut(text))
+        print(text)
+        res = et.extract_time(text, cut_res, True)
+        print(res)
```

## Comparing `query_toolkits-1.2.2.dist-info/RECORD` & `query_toolkits-1.3.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 query_toolkits/__init__.py,sha256=EveacW4_39hG1bXQXu2-_iach21RtE1NVgSjXgmaDyE,845
 query_toolkits/error_correction.py,sha256=auit3b2ihsuWufmNixOrjC5CEjVrD2IiAzj461YrJUg,40836
-query_toolkits/extractor.py,sha256=SHgNMCmFPvJUiwF2k4IghZ6BUooPNmTxAvUgC6ftxv8,26728
+query_toolkits/extractor.py,sha256=b9k_ZW2WI_5YPRMiHcSAw-fvECK-hC3dpRoDg6AZ0Qg,27111
 query_toolkits/financial_index.txt,sha256=Lw12OQ50B8-vFD3W6H7uAFtAWkmHDx1az5PX9I5h98g,783
 query_toolkits/financial_index_full.txt,sha256=IreFvGQWJJtzT67BU8rSJcdonMSkbKPSz-IMzGwL8RY,16386
 query_toolkits/fund_product.txt,sha256=Fn3FPhk10KjtHkyXD0OHK8OttYjVtN4KRiTQ6X4c0uI,1056198
 query_toolkits/index.txt,sha256=W9_pC0bCTEVykwjwSI1Zi7gFFW94BrsvKdkzRBkhWBw,18015
 query_toolkits/info.json,sha256=BC85jy__r1H89WHSJqkmfKK0arna3MlP0V3cDvARo_w,44320114
 query_toolkits/keyword.txt,sha256=iFtkA8SUDbKViFYSg2YPP9RG_btJ35AlGor06ywy0A4,153
 query_toolkits/organization.txt,sha256=hRLDyvQKxw-_XgM2WEQ9MD3DvmanTluYu2Z6Se5JYro,634483
 query_toolkits/product.txt,sha256=PAWJ7YtTOydgsGcZ470hQ-wgXtYHMEDCFa23lKy1Zns,9995
 query_toolkits/unit_transform,sha256=yHFE7ydHauFdJy13GNCyYmNZy0gQWd0lYlvki_6OUD4,2237
 query_toolkits/utils.py,sha256=zPTVyjmxeioiND7PlUfCkUjMi50wKgcRghyzmo_20ig,5453
 query_toolkits/weapon.txt,sha256=rpGr_JynyYjrvnoM-swGLM1DLdxNKITUNJyfb_juw_E,420676
-query_toolkits-1.2.2.dist-info/METADATA,sha256=7jd7s_unoNo2upJnJ9g7ueSr5-vARsRehm1-_DrMTrY,230
-query_toolkits-1.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-query_toolkits-1.2.2.dist-info/top_level.txt,sha256=oX-XPh75LlcNrWWX-7EQ7ciThjo7m_iFQkriyWxvwCo,15
-query_toolkits-1.2.2.dist-info/RECORD,,
+query_toolkits-1.3.0.dist-info/METADATA,sha256=ckLYwdrztKGjqF25N6rzS3hyP5SFGnOo_-mLqV6_b5g,230
+query_toolkits-1.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+query_toolkits-1.3.0.dist-info/top_level.txt,sha256=oX-XPh75LlcNrWWX-7EQ7ciThjo7m_iFQkriyWxvwCo,15
+query_toolkits-1.3.0.dist-info/RECORD,,
```

