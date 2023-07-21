# Comparing `tmp/waffle_box-0.0.1.tar.gz` & `tmp/waffle_box-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_box-0.0.1.tar", max compression
+gzip compressed data, was "waffle_box-0.0.2.tar", max compression
```

## Comparing `waffle_box-0.0.1.tar` & `waffle_box-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0        0 2023-07-14 05:15:26.242521 waffle_box-0.0.1/README.md
--rw-r--r--   0        0        0       86 2023-07-14 01:41:16.640933 waffle_box-0.0.1/app_manager/__init__.py
--rw-r--r--   0        0        0     2541 2023-07-14 04:59:41.095018 waffle_box-0.0.1/app_manager/app_manager.py
--rw-r--r--   0        0        0     2382 2023-07-14 05:13:38.744598 waffle_box-0.0.1/app_manager/app_structure.py
--rw-r--r--   0        0        0       83 2023-07-14 01:41:24.140847 waffle_box-0.0.1/maker_manager/__init__.py
--rw-r--r--   0        0        0      280 2023-07-14 05:14:21.447733 waffle_box-0.0.1/maker_manager/convert_option.py
--rw-r--r--   0        0        0     3395 2023-07-14 04:45:54.742709 waffle_box-0.0.1/maker_manager/maker_manager.py
--rw-r--r--   0        0        0      480 2023-07-14 03:50:47.131443 waffle_box-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 23:39:38.963988 waffle_box-0.0.1/waffle_box/__init__.py
--rw-r--r--   0        0        0     1088 2023-07-14 05:13:38.744598 waffle_box-0.0.1/waffle_box/bake_service.py
--rw-r--r--   0        0        0     2242 2023-07-14 04:21:26.806950 waffle_box-0.0.1/waffle_box/cli.py
--rw-r--r--   0        0        0     1896 2023-07-14 04:35:11.217038 waffle_box-0.0.1/waffle_box/convert_service.py
--rw-r--r--   0        0        0      759 2023-07-14 04:35:01.085209 waffle_box-0.0.1/waffle_box/pull_service.py
--rw-r--r--   0        0        0      384 1970-01-01 00:00:00.000000 waffle_box-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      647 2023-07-17 01:24:46.969274 waffle_box-0.0.2/README.md
+-rw-r--r--   0        0        0      141 2023-07-21 04:10:43.147871 waffle_box-0.0.2/app_manager/__init__.py
+-rw-r--r--   0        0        0     9018 2023-07-21 09:26:55.273182 waffle_box-0.0.2/app_manager/app_manager.py
+-rw-r--r--   0        0        0     2898 2023-07-21 06:59:24.736512 waffle_box-0.0.2/app_manager/app_structure.py
+-rw-r--r--   0        0        0     2060 2023-07-21 03:54:46.601453 waffle_box-0.0.2/app_manager/nvinfer_config_parser.py
+-rw-r--r--   0        0        0       83 2023-07-14 01:41:24.140847 waffle_box-0.0.2/maker_manager/__init__.py
+-rw-r--r--   0        0        0     2359 2023-07-21 06:58:47.380531 waffle_box-0.0.2/maker_manager/convert_option.py
+-rw-r--r--   0        0        0     9925 2023-07-21 09:06:57.535079 waffle_box-0.0.2/maker_manager/maker_manager.py
+-rw-r--r--   0        0        0      599 2023-07-21 09:27:26.724869 waffle_box-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-07-21 07:13:17.494080 waffle_box-0.0.2/waffle_box/__init__.py
+-rw-r--r--   0        0        0     2579 2023-07-14 06:58:20.777371 waffle_box-0.0.2/waffle_box/bake_service.py
+-rw-r--r--   0        0        0     4281 2023-07-21 09:24:44.814491 waffle_box-0.0.2/waffle_box/cli.py
+-rw-r--r--   0        0        0     5048 2023-07-21 08:48:35.416144 waffle_box-0.0.2/waffle_box/convert_service.py
+-rw-r--r--   0        0        0     2229 2023-07-21 09:08:04.510093 waffle_box-0.0.2/waffle_box/pull_service.py
+-rw-r--r--   0        0        0       67 2023-07-17 00:29:45.225470 waffle_box-0.0.2/waffle_box_exception/__init__.py
+-rw-r--r--   0        0        0     1512 2023-07-21 03:54:46.601453 waffle_box-0.0.2/waffle_box_exception/waffle_box_exception.py
+-rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 waffle_box-0.0.2/PKG-INFO
```

### Comparing `waffle_box-0.0.1/app_manager/app_structure.py` & `waffle_box-0.0.2/app_manager/app_structure.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,65 @@
 from maker_manager import ONNXConvConfigs
 
 from dataclasses import dataclass
 from typing import List
 from uuid import UUID
 from pathlib import Path
 
+
 @dataclass(frozen=True)
 class ModelInfo:
     """ 모델 정보
-    
+
     모델의 기본 정보를 저장한다. (변경 불가)
 
     # Attributes
     - id: UUID
         - model.json에 기술되어 있는 모델의 uuid
     - name: str
         - model.json에 기술되어 있는 모델의 이름
     - precision: str
         - 모델의 precision
         - fp32, fp16, int8 중 하나
+    - engine_file_name
+        - engine 파일 이름
+        - 보통 model.engine
+    - input_dims
+        - 모델의 input shape, x로 구분
+        - 예) 3x640x640
+    - batch_size
+        - 모델의 batch size
+        - Autocare-D는 기본적으로 dynamic batch를 가정하므로
+        모델에 적혀있는 batch-size는 max batch size로 간주한다.
     - path: Path
         - 모델 폴더 경로
 
     """
+
     id: UUID
     name: str
     precision: str
+    engine_file_name: str
+    input_dims: str
+    max_batch_size: int
     path: Path
 
     def to_onnx_config(self) -> ONNXConvConfigs:
         """ ONNX 파일을 trt 엔진 파일로 변환하는데 필요한 정보
 
         ONNX 파일을 trt 엔진 파일로 변환하는데 
         필요한 설정 값을 모델 정보에서 얻는다.
 
         """
-        return ONNXConvConfigs(precision=self.precision)
+        return ONNXConvConfigs(
+            precision=self.precision, 
+            input_shapes=self.input_dims,
+            max_batch=self.max_batch_size
+        )
+
 
 @dataclass(frozen=True)
 class AppStructure:
     """ App 구조 정보
 
     App의 구조 정보를 저장한다. (변경 불가)
 
@@ -58,38 +78,40 @@
 
     def find_model_by_id(self, id: UUID) -> ModelInfo | None:
         """ id 값으로 모델을 찾는다.
 
         # Parameters
         - id
             - 찾는 모델의 uuid
-        
+
         # Returns
         - ModelInfo
             - 입력한 id와 일치하는 모델
         - None
             - 입력한 id와 일치하는 모델을 찾지 못했을 때
+
         """
         for m in self.models:
             if m.id == id:
                 return m
-        
+
         return None
 
     def find_model_by_name(self, name: str) -> ModelInfo | None:
         """ 이름으로 모델을 찾는다.
 
         # Parameters
         - name
             - 찾는 모델의 이름
-        
+
         # Returns
         - ModelInfo
             - 입력한 이름과 일치하는 모델
         - None
             - 입력한 이름과 일치하는 모델을 찾지 못했을 때
+
         """
         for m in self.models:
             if m.name == name:
                 return m
-        
+
         return None
```

