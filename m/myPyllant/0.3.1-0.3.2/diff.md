# Comparing `tmp/mypyllant-0.3.1.tar.gz` & `tmp/mypyllant-0.3.2.tar.gz`

## Comparing `mypyllant-0.3.1.tar` & `mypyllant-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.3.1/logo.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.3.1/requirements-dev.txt
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.3.1/run_pytest.sh
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 mypyllant-0.3.1/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    17950 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/api.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/export.py
--rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/py.typed
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/conftest.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/find_countries.py
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/generate_test_data.py
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/test_api.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/test_countries.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/test_export.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/test_generate_test_data.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/test_sample.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/update_sample.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/utils.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/current_system.json
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/device_buckets.json
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/time_zone.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.3.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.3.1/LICENSE
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mypyllant-0.3.1/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 mypyllant-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.3.2/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.3.2/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.3.2/run_pytest.sh
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.3.2/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    17950 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/api.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/export.py
+-rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_export.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/current_system.json
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/device_buckets.json
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/time_zone.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mypyllant-0.3.2/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 mypyllant-0.3.2/PKG-INFO
```

### Comparing `mypyllant-0.3.1/.pre-commit-config.yaml` & `mypyllant-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/logo.png` & `mypyllant-0.3.2/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/.github/workflows/build-test.yaml` & `mypyllant-0.3.2/.github/workflows/build-test.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,16 @@
   pull_request:
   schedule:
     - cron: "0 0 * * *"
 
 jobs:
   build:
     runs-on: ubuntu-latest
+    permissions:
+      id-token: write
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
           cache: pip
@@ -33,12 +35,10 @@
       - name: Build a binary wheel and a source tarball
         run: >-
           python -m
           build
           --sdist
           --wheel
           --outdir dist/
-      - name: Publish distribution 📦 to PyPI
+      - name: Publish distribution to PyPI
         if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
+        uses: pypa/gh-action-pypi-publish@release/v1
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mypyllant-0.3.1/src/myPyllant/api.py` & `mypyllant-0.3.2/src/myPyllant/api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/const.py` & `mypyllant-0.3.2/src/myPyllant/const.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/export.py` & `mypyllant-0.3.2/src/myPyllant/export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/models.py` & `mypyllant-0.3.2/src/myPyllant/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     @property
     def display_value(self) -> str:
         return self.value.replace("_", " ").title()
 
 
 class CircuitState(MyPyllantEnum):
     HEATING = "HEATING"
+    COOLING = "COOLING"
     STANDBY = "STANDBY"
 
 
 class DeviceDataBucketResolution(MyPyllantEnum):
     HOUR = "HOUR"
     DAY = "DAY"
     MONTH = "MONTH"
@@ -46,14 +47,15 @@
     QUICK_VETO = "QUICK_VETO"
     HOLIDAY = "HOLIDAY"
 
 
 class ZoneHeatingState(MyPyllantEnum):
     IDLE = "IDLE"
     HEATING_UP = "HEATING_UP"
+    COOLING_DOWN = "COOLING_DOWN"
 
 
 class DHWCurrentSpecialFunction(MyPyllantEnum):
     CYLINDER_BOOST = "CYLINDER_BOOST"
     REGULAR = "REGULAR"
 
 
@@ -83,16 +85,17 @@
     general: dict
     index: int
     is_active: bool
     is_cooling_allowed: bool
     zone_binding: str
     current_room_temperature: float | None
     current_special_function: ZoneCurrentSpecialFunction
-    desired_room_temperature_setpoint_heating: float
-    desired_room_temperature_setpoint: float
+    desired_room_temperature_setpoint_heating: float | None
+    desired_room_temperature_setpoint_cooling: float | None
+    desired_room_temperature_setpoint: float | None
     heating_state: ZoneHeatingState
     current_room_humidity: float | None
     heating: ZoneHeating
     associated_circuit_index: int | None
     quick_veto_start_date_time: datetime.datetime | None
     quick_veto_end_date_time: datetime.datetime | None
 
@@ -255,15 +258,15 @@
     def name_display(self) -> str:
         return self.name if self.name else self.product_name.title()
 
 
 class DeviceDataBucket(BaseModel):
     start_date: datetime.datetime
     end_date: datetime.datetime
-    value: float
+    value: float | None
 
 
 class DeviceData(BaseModel):
     def __init__(self, device: Device | None = None, **kwargs: Any) -> None:
         kwargs["data_from"] = kwargs.pop("from") if "from" in kwargs else None
         kwargs["data_to"] = kwargs.pop("to") if "to" in kwargs else None
         super().__init__(device=device, **kwargs)
```

### Comparing `mypyllant-0.3.1/src/myPyllant/sample.py` & `mypyllant-0.3.2/src/myPyllant/sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/utils.py` & `mypyllant-0.3.2/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/find_countries.py` & `mypyllant-0.3.2/src/myPyllant/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/generate_test_data.py` & `mypyllant-0.3.2/src/myPyllant/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/test_api.py` & `mypyllant-0.3.2/src/myPyllant/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/test_countries.py` & `mypyllant-0.3.2/src/myPyllant/tests/test_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/test_export.py` & `mypyllant-0.3.2/src/myPyllant/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/test_generate_test_data.py` & `mypyllant-0.3.2/src/myPyllant/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/update_sample.py` & `mypyllant-0.3.2/src/myPyllant/tests/update_sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/utils.py` & `mypyllant-0.3.2/src/myPyllant/tests/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/current_system.json` & `mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/device_buckets.json` & `mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/system.json` & `mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/.gitignore` & `mypyllant-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/LICENSE` & `mypyllant-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/README.md` & `mypyllant-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/pyproject.toml` & `mypyllant-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.1/PKG-INFO` & `mypyllant-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

