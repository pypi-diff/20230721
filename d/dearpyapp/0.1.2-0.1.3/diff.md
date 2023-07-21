# Comparing `tmp/dearpyapp-0.1.2-py3-none-win_amd64.whl.zip` & `tmp/dearpyapp-0.1.3-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 19644 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      460 b- defN 23-Mar-03 09:12 dearpyapp/__init__.py
--rw-rw-rw-  2.0 fat    10777 b- defN 23-Mar-03 09:12 dearpyapp/application.py
--rw-rw-rw-  2.0 fat     2328 b- defN 23-Mar-03 09:12 dearpyapp/colors.py
--rw-rw-rw-  2.0 fat     8761 b- defN 23-Mar-03 09:12 dearpyapp/themes.py
--rw-rw-rw-  2.0 fat     8209 b- defN 23-Mar-03 09:12 dearpyapp/utils.py
--rw-rw-rw-  2.0 fat      105 b- defN 23-Mar-03 09:12 dearpyapp/components/__init__.py
--rw-rw-rw-  2.0 fat    12649 b- defN 23-Mar-03 09:12 dearpyapp/components/log.py
--rw-rw-rw-  2.0 fat    12733 b- defN 23-Mar-03 09:12 dearpyapp/components/port_control.py
--rw-rw-rw-  2.0 fat     6455 b- defN 23-Mar-03 09:12 dearpyapp/components/tab.py
--rw-rw-rw-  2.0 fat     1096 b- defN 23-Mar-03 09:13 dearpyapp-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      864 b- defN 23-Mar-03 09:13 dearpyapp-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-Mar-03 09:13 dearpyapp-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Mar-03 09:13 dearpyapp-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1132 b- defN 23-Mar-03 09:13 dearpyapp-0.1.2.dist-info/RECORD
-14 files, 65677 bytes uncompressed, 17774 bytes compressed:  72.9%
+Zip file size: 19858 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      460 b- defN 23-Jul-21 07:57 dearpyapp/__init__.py
+-rw-rw-rw-  2.0 fat    10777 b- defN 23-Jul-21 07:57 dearpyapp/application.py
+-rw-rw-rw-  2.0 fat     2328 b- defN 23-Jul-21 07:57 dearpyapp/colors.py
+-rw-rw-rw-  2.0 fat     8883 b- defN 23-Jul-21 07:57 dearpyapp/themes.py
+-rw-rw-rw-  2.0 fat     9102 b- defN 23-Jul-21 07:57 dearpyapp/utils.py
+-rw-rw-rw-  2.0 fat      105 b- defN 23-Jul-21 07:57 dearpyapp/components/__init__.py
+-rw-rw-rw-  2.0 fat    12649 b- defN 23-Jul-21 07:57 dearpyapp/components/log.py
+-rw-rw-rw-  2.0 fat    12733 b- defN 23-Jul-21 07:57 dearpyapp/components/port_control.py
+-rw-rw-rw-  2.0 fat     6455 b- defN 23-Jul-21 07:57 dearpyapp/components/tab.py
+-rw-rw-rw-  2.0 fat     1096 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      864 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1132 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/RECORD
+14 files, 66692 bytes uncompressed, 17988 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: dearpyapp/components/port_control.py
 Comment: 
 
 Filename: dearpyapp/components/tab.py
 Comment: 
 
-Filename: dearpyapp-0.1.2.dist-info/LICENSE
+Filename: dearpyapp-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: dearpyapp-0.1.2.dist-info/METADATA
+Filename: dearpyapp-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: dearpyapp-0.1.2.dist-info/WHEEL
+Filename: dearpyapp-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: dearpyapp-0.1.2.dist-info/top_level.txt
+Filename: dearpyapp-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dearpyapp-0.1.2.dist-info/RECORD
+Filename: dearpyapp-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dearpyapp/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 from . import colors as c
 from .application import DpgApp, get_running_app
 from .themes import (
     dpg_get_color_theme,
     dpg_get_default_theme
 )
```

## dearpyapp/themes.py

```diff
@@ -104,14 +104,17 @@
             dpg.add_theme_color(dpg.mvThemeCol_PlotHistogram, c.BLUE_18)
             dpg.add_theme_color(dpg.mvThemeCol_PlotLines, c.BLUE_18)
             dpg.add_theme_color(dpg.mvThemeCol_Separator, c.GRAY_6)
 
         with dpg.theme_component(dpg.mvPlot):
             dpg.add_theme_color(dpg.mvThemeCol_WindowBg, c.GRAY_2)
 
+        with dpg.theme_component(dpg.mvDatePicker):
+            dpg.add_theme_color(dpg.mvThemeCol_Button, c.BLUE_12)
+
         with dpg.theme_component(dpg.mvText):
             dpg.add_theme_color(dpg.mvThemeCol_Text, c.GRAY_22)
 
         for item_type in (dpg.mvInputText, dpg.mvInputInt, dpg.mvInputFloat, dpg.mvCombo):
             with dpg.theme_component(item_type):
                 dpg.add_theme_color(dpg.mvThemeCol_FrameBg, c.GRAY_2)
                 dpg.add_theme_color(dpg.mvThemeCol_PopupBg, c.GRAY_2)
```

## dearpyapp/utils.py

```diff
@@ -15,23 +15,48 @@
     dpg.mvWindowAppItem: _top_container_name,
     dpg.mvChildWindow: 'mvChildWindow',
     dpg.mvGroup: 'mvGroup',
     dpg.mvTab: 'mvTab',
 }
 
 _not_container_name_lookup = {
+    dpg.mvImage: 'mvImage',
     dpg.mvInputText: 'mvInputText',
     dpg.mvText: 'mvText',
     dpg.mvCombo: 'mvCombo',
+    dpg.mvListbox: 'mvListbox',
+    dpg.mvCollapsingHeader: 'mvCollapsingHeader',
+    dpg.mvTabBar: 'mvTabBar',
+    dpg.mvTab: 'mvTab',
     dpg.mvMenuBar: 'mvMenuBar',
+    dpg.mvMenu: 'mvMenu',
+    dpg.mvMenuItem: 'mvMenuItem',
     dpg.mvDragFloat: 'mvDragFloat',
+    dpg.mvInputFloat: 'mvInputFloat',
+    dpg.mvSliderFloat: 'mvSliderFloat',
     dpg.mvDragInt: 'mvDragInt',
-    dpg.mvButton: 'mvButton',
+    dpg.mvInputInt: 'mvInputInt',
+    dpg.mvSliderInt: 'mvSliderInt',
     dpg.mvCheckbox: 'mvCheckbox',
+    dpg.mvButton: 'mvButton',
+    dpg.mvRadioButton: 'mvRadioButton',
+    dpg.mvImageButton: 'mvImageButton',
+    dpg.mvColorButton: 'mvColorButton',
     dpg.mvProgressBar: 'mvProgressBar',
+    dpg.mvTable: 'mvTable',
+    dpg.mvDatePicker: 'mvDatePicker',
+    dpg.mvTimePicker: 'mvTimePicker',
+    dpg.mvTreeNode: 'mvTreeNode',
+    dpg.mvPlot: 'mvPlot',
+    dpg.mvSimplePlot: 'mvSimplePlot',
+    dpg.mvSeparator: 'mvSeparator',
+    dpg.mvSpacer: 'mvSpacer',
+    dpg.mvColorEdit: 'mvColorEdit',
+    dpg.mvColorPicker: 'mvColorPicker',
+    dpg.mvTooltip: 'mvTooltip',
 }
 
 _item_type_lookup = {v: k for k, v in ChainMap(_container_name_lookup,
                                                _not_container_name_lookup).items()}
 
 
 @contextmanager
```

## Comparing `dearpyapp-0.1.2.dist-info/LICENSE` & `dearpyapp-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dearpyapp-0.1.2.dist-info/METADATA` & `dearpyapp-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearpyapp
-Version: 0.1.2
+Version: 0.1.3
 Summary: Wrapper for DearPyGui
 Home-page: https://github.com/means0nothing/DearPyApp
 Author: Pavel Shevcov
 Author-email: means0nothing@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

## Comparing `dearpyapp-0.1.2.dist-info/RECORD` & `dearpyapp-0.1.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-dearpyapp/__init__.py,sha256=u6hVk7-azeKDPWlMzPef_2Jjwle31CsoBukvrJ21tjw,460
+dearpyapp/__init__.py,sha256=-dGIQnU8MIMVQasr6iSKrYdr-qDPIbJChqg9DTLSckA,460
 dearpyapp/application.py,sha256=Nma4VawA6GPQaeAihsjy_2M_NzVgUAaeQosN-w7NqXo,10777
 dearpyapp/colors.py,sha256=MIeFfAmC3Gwjyaf6EcjzO1Byxte_g_QBi5q8X-AgOmA,2328
-dearpyapp/themes.py,sha256=J_soId9XNYzabrgnZFOixtVcTZIFPsBWrrm-GNz7XRA,8761
-dearpyapp/utils.py,sha256=D2hloJ73xH-Jg0-edVvGjmKDBB3mLOZfuUKw-5AX8lI,8209
+dearpyapp/themes.py,sha256=sEPZcvwAVxbqBqci87Q0v57IFJxaZSNVFD6YVs0XSgw,8883
+dearpyapp/utils.py,sha256=SDPunxOee-INsQavMk6wvIN76CYBPv6RgDHGULOnzq8,9102
 dearpyapp/components/__init__.py,sha256=DH-92pXUHLPgxHSIJlc06FsA_WzMvooPck47pkvssGg,105
 dearpyapp/components/log.py,sha256=nigCQlPxlIoLJL5MeSE0oldTUd4Fu_dUqgYdvhoWXzU,12649
 dearpyapp/components/port_control.py,sha256=Jo1Q5d8-xmFRo_p5zutt7iBjN0KepiuNgQCcSMw9rJQ,12733
 dearpyapp/components/tab.py,sha256=4yhD6xGGI4jKZpYlDoyM8bN700ZrEf5LT4YELA6MumU,6455
-dearpyapp-0.1.2.dist-info/LICENSE,sha256=KOI2v5c_M5MQQkVqxM4BBqmkZnNAh6PYV-3Q9pTInWE,1096
-dearpyapp-0.1.2.dist-info/METADATA,sha256=H04YJxbNhJxbx6OZgeCxipTYOKUpPZFMhNgqtT94ZuU,864
-dearpyapp-0.1.2.dist-info/WHEEL,sha256=AiyVnrmrEuW_cPqhPlarzpb5qtD8ITcBeZKvhXXgyN4,98
-dearpyapp-0.1.2.dist-info/top_level.txt,sha256=XwOBbr99GukN8XkQi7CxxSmYO32SNAfcDnXtKuKRT_k,10
-dearpyapp-0.1.2.dist-info/RECORD,,
+dearpyapp-0.1.3.dist-info/LICENSE,sha256=KOI2v5c_M5MQQkVqxM4BBqmkZnNAh6PYV-3Q9pTInWE,1096
+dearpyapp-0.1.3.dist-info/METADATA,sha256=RcLcprhabDmVOW_zLP0TFJXgI6Njko-X5tA21iZTjh4,864
+dearpyapp-0.1.3.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+dearpyapp-0.1.3.dist-info/top_level.txt,sha256=XwOBbr99GukN8XkQi7CxxSmYO32SNAfcDnXtKuKRT_k,10
+dearpyapp-0.1.3.dist-info/RECORD,,
```

