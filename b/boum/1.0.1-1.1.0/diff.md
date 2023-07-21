# Comparing `tmp/boum-1.0.1.tar.gz` & `tmp/boum-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boum-1.0.1.tar", max compression
+gzip compressed data, was "boum-1.1.0.tar", max compression
```

## Comparing `boum-1.0.1.tar` & `boum-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2022-12-08 14:21:18.220062 boum-1.0.1/LICENSE
--rw-r--r--   0        0        0     5676 2022-12-08 14:21:18.220062 boum-1.0.1/README.md
--rw-r--r--   0        0        0      121 2022-12-08 14:21:18.220062 boum-1.0.1/boum/api_client/constants.py
--rw-r--r--   0        0        0     9979 2022-12-08 14:21:18.224062 boum-1.0.1/boum/api_client/v1/client.py
--rw-r--r--   0        0        0     7853 2022-12-08 14:21:18.224062 boum-1.0.1/boum/api_client/v1/endpoint.py
--rw-r--r--   0        0        0     7095 2022-12-08 14:21:18.224062 boum-1.0.1/boum/api_client/v1/models.py
--rw-r--r--   0        0        0     4952 2022-12-08 14:21:18.224062 boum-1.0.1/boum/resources/device.py
--rw-r--r--   0        0        0      964 2022-12-08 14:21:18.224062 boum-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6554 1970-01-01 00:00:00.000000 boum-1.0.1/setup.py
--rw-r--r--   0        0        0     6260 1970-01-01 00:00:00.000000 boum-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-07-21 12:03:32.308042 boum-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5676 2023-07-21 12:03:32.308042 boum-1.1.0/README.md
+-rw-r--r--   0        0        0      121 2023-07-21 12:03:32.308042 boum-1.1.0/boum/api_client/constants.py
+-rw-r--r--   0        0        0    10507 2023-07-21 12:03:32.308042 boum-1.1.0/boum/api_client/v1/client.py
+-rw-r--r--   0        0        0     7853 2023-07-21 12:03:32.308042 boum-1.1.0/boum/api_client/v1/endpoint.py
+-rw-r--r--   0        0        0     7095 2023-07-21 12:03:32.308042 boum-1.1.0/boum/api_client/v1/models.py
+-rw-r--r--   0        0        0     5363 2023-07-21 12:03:32.308042 boum-1.1.0/boum/resources/device.py
+-rw-r--r--   0        0        0      964 2023-07-21 12:03:32.308042 boum-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6554 1970-01-01 00:00:00.000000 boum-1.1.0/setup.py
+-rw-r--r--   0        0        0     6260 1970-01-01 00:00:00.000000 boum-1.1.0/PKG-INFO
```

### Comparing `boum-1.0.1/LICENSE` & `boum-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boum-1.0.1/README.md` & `boum-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `boum-1.0.1/boum/api_client/v1/client.py` & `boum-1.1.0/boum/api_client/v1/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,18 +220,34 @@
         self._put()
 
     def delete(self):
         if self.is_resource:
             raise AttributeError('Cannot unclaim from a specific user')
         self._delete()
 
+class DevicesClaimedEndpoint(Endpoint):
+
+    # pylint: disable=useless-parent-delegation
+    def __get__(self, parent, owner: type) -> "DevicesClaimEndpoint":
+        return super().__get__(parent, owner)
+
+    def get(self) -> list[str] | DeviceModel:
+        response = self._get()
+        data = response.json()['data']
+        if self.is_collection:
+            return [d['id'] for d in data]
+
+        device_model = DeviceModel.from_payload(data)
+        return device_model
+
 
 class DevicesEndpoint(Endpoint):
     data = DevicesDataEndpoint('data')
     claim = DevicesClaimEndpoint('claim')
+    claimed = DevicesClaimedEndpoint('claimed')
 
     # pylint: disable=useless-parent-delegation
     def __get__(self, parent, owner: type) -> "DevicesEndpoint":
         return super().__get__(parent, owner)
 
     def post(self) -> str:
         if self.is_resource:
```

### Comparing `boum-1.0.1/boum/api_client/v1/endpoint.py` & `boum-1.1.0/boum/api_client/v1/endpoint.py`

 * *Files identical despite different names*

### Comparing `boum-1.0.1/boum/api_client/v1/models.py` & `boum-1.1.0/boum/api_client/v1/models.py`

 * *Files identical despite different names*

### Comparing `boum-1.0.1/boum/resources/device.py` & `boum-1.1.0/boum/resources/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,30 @@
         Returns
         -------
             list[str]
                 The device ids
         """
         return api_client.root.devices.get()
 
+    @staticmethod
+    def get_claimed_device_ids(api_client: ApiClient) -> list[str]:
+        """Get all claimed device ids
+
+        Parameters
+        ----------
+            api_client
+                The api client that handles the interaction with the api
+
+        Returns
+        -------
+            list[str]
+                The device ids
+        """
+        return api_client.root.devices.claimed.get()
+
     def set_desired_device_state(self, desired_device_state: DeviceStateModel):
         """
         Set the desired device state.
 
         Parameters
         ----------
             desired_device_state
```

### Comparing `boum-1.0.1/pyproject.toml` & `boum-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "boum"
-version = "1.0.1"
+version = "1.1.0"
 description = "SDK to interact with the boum API"
 authors = ["Marc Pfander <marc.pfander@boum.garden>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/boum-garden/sdk"
 
 [tool.poetry.dependencies]
@@ -24,15 +24,15 @@
 bandit = "^1.7.4"
 coverage = "^6.5.0"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.1.0"
 
 
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `boum-1.0.1/setup.py` & `boum-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'boum',
-    'version': '1.0.1',
+    'version': '1.1.0',
     'description': 'SDK to interact with the boum API',
     'long_description': "# Boum Python SDK\nStatus: ![GitHub Actions](https://github.com/boum-garden/sdk/actions/workflows/main.yml/badge.svg)\n\n## Overview\nThis project provides an api client to interact with the [Boum API](https://api.boum.us/swagger) and abstractions to \nsimplify interactions with the underlying resources.\n\n\n## Installation\nThe package is available on PyPI, and can be installed with pip or similar tools:\n\n```bash\n    python -m pip install boum\n    poetry add boum\n    pipenv install boum\n    ...\n```\n\n## Usage\n\n### API Client\nThe API client models the topology of the API and provides a class hierarchy that is organized in the same way as the \nendpoint paths. Email and password or a token are required to use it.\n\nThe client can either connect to the API with `client.connect()` and `client.disconnect()`methods or it can be used \nas a context manager as `with client: ...` In the former case the disconnect method should be called explicitly in the\nend.\n\n```python\n>>> from boum.api_client.v1.client import ApiClient\n>>> from boum.api_client.v1.models import DeviceModel\n>>> \n>>> client = ApiClient(email, password, base_url=base_url)\n>>> # or ApiClient(refresh_token='token', base_url=base_url)\n>>>\n>>> with client:\n...     # Get call to the devices collection\n...     device_ids = client.root.devices.get()\n...     # Get call to a specific device \n...     device_states = client.root.devices(device_id).get()\n...     # Patch call to a specific device\n...     client.root.devices(device_id).patch(DeviceModel())\n...     # Get call to a devices data\n...     data = client.root.devices(device_id).data.get()\n\n```\n\n\n### Resource Abstractions\nThe resource abstractions provide a more intuitive interface to interact with the underlying resources.\n\n```python\n>>> from datetime import time, datetime, timedelta\n>>> import pandas as pd\n>>> from boum.api_client.v1.client import ApiClient\n>>> from boum.resources.device import Device\n>>> from boum.api_client.v1.models import DeviceStateModel\n>>>\n>>> client = ApiClient(email, password, base_url=base_url)\n>>> # or ApiClient(refresh_token='token', base_url=base_url)\n>>>\n>>> with client:\n...    # Get available device ids\n...    device_ids = Device.get_device_ids(client)\n...    # Create a device instance\n...    device = Device(device_id, client)\n...    # Remove device claim\n...    # device.unclaim()\n...    # Claim a device\n...    # device.claim()\n...    # Set desired device state\n...    desired_device_State = DeviceStateModel(\n...        pump_state=True,\n...        refill_time=time(3, 32),\n...        refill_interval_days=3,\n...        max_pump_duration_minutes=5\n...    )\n...    device.set_desired_device_state(desired_device_State)\n...    # Get reported and desired device state\n...    reported, desired = device.get_device_states()\n...    # Get device telemetry data\n...    data = device.get_telemetry_data(start=datetime.now() - timedelta(days=1),\n...        end=datetime.now())\n...    # Convert telemetry data to pandas dataframe\n...    df = pd.DataFrame(data)\n\n```\n\n### Jupyter Notebook Demo\nA Jupyter notebook demo is available [here](https://github.com/boum-garden/sdk/blob/638d62836f5b8b2f169d186170c679d6a813867a/doc/boum-sdk-demo.ipynb).\n\n### Loging\nThe SDK uses the standard python logging module.\n\n## Development\n\n### Dependecy management\n[Poetry](https://python-poetry.org/) is used for depency management and publishing.\n\n### Versioning\nVersioning is done using [bumpver](https://pypi.org/project/bumpver/) \nwith [semantic versioning](https://semver.org/)\nWhen the version is updated, a new tag is created and pushed to the remote repository.\n\n\n### Testing\n\n#### Unit tests\nThese are completely self-contained and have no external dependencies.\n\nIMPORTANT: There are fixtures that model the API responses and expected calls. These mnust be kept up to date with\nthe API, otherwise the unit tests will not test the correct behavior.\n\n#### End-to-end tests\nThese test the entire flow from user facing python classes to the underlying api calls. They require an instance \n(fake or real) of the API to run against. They also require a registered user with a clamied device.\nAPI Base URL, email and password are required as environmental variables.\n\n```bash\n    BOUM_SDK_TEST_BASE_URL\n    BOUM_SDK_TEST_EMAIL\n    BOUM_SDK_TEST_PASSWORD\n    BOUM_SDK_TEST_DEVICE_ID\n    BOUM_SDK_TEST_USER_ID\n```\n\n#### Doctests\n\nPart of the end-to-end tests are document tests executed using \n[doctest](https://docs.python.org/3/library/doctest.html). \nThese tests ensure that all the examples in this README and in the docstrings are up-to-date and working.\n\n\n## CI/CD\n\n### Integration\n\nThe GitHub action workflow `.github/workflows/checks_on_push_to_branch.yml` is triggered on every push on a branch\nexcept main. It provides the following checks:\n\n- Unit and end-to-end/contract tests with pytest\n- Linting with pylint\n- Security checks with bandit\n\nThe repository settings require that all checks pass before a pull request can be merged.\n\n### Deployment\n\nThe GitHub action workflow `.github/workflows/deploy_on_push_to_main.yml` is triggered on every push to main. It runs a\ntest deployment to the test PyPI repository.\n\nThe GitHub action workflow `.github/workflows/deploy_on_release.yml` is triggered on a tag with the format `v*.*.*` and\nruns a deployment to the production PyPI. It is recommended to set these tags using the GitHub release feature. \n\n\n## Technical debt\n\n- Doctest requires a specific format to make examples in documentation executable. This makes the examples in this\n  README harder to copy and paste. There exist other packages and add-ons that could be used to make the examples easier \n  to manage.\n\n\n\n\n\n\n",
     'author': 'Marc Pfander',
     'author_email': 'marc.pfander@boum.garden',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/boum-garden/sdk',
```

### Comparing `boum-1.0.1/PKG-INFO` & `boum-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boum
-Version: 1.0.1
+Version: 1.1.0
 Summary: SDK to interact with the boum API
 Home-page: https://github.com/boum-garden/sdk
 License: MIT
 Author: Marc Pfander
 Author-email: marc.pfander@boum.garden
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

