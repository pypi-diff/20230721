# Comparing `tmp/computex_cli-0.1.5.tar.gz` & `tmp/computex_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computex_cli-0.1.5.tar", max compression
+gzip compressed data, was "computex_cli-0.1.6.tar", max compression
```

## Comparing `computex_cli-0.1.5.tar` & `computex_cli-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      613 2023-06-21 04:23:16.786796 computex_cli-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/__init__.py
--rw-r--r--   0        0        0     6742 2023-06-21 06:12:00.930141 computex_cli-0.1.5/cxcli/cli.py
--rw-r--r--   0        0        0      911 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/config.py
--rw-r--r--   0        0        0      161 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/exc.py
--rw-r--r--   0        0        0        0 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/__init__.py
--rw-r--r--   0        0        0      950 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/auth.py
--rw-r--r--   0        0        0     2263 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/deployments.py
--rw-r--r--   0        0        0     1912 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/service.py
--rw-r--r--   0        0        0     1236 2023-06-21 04:23:16.786796 computex_cli-0.1.5/cxcli/services/users.py
--rw-r--r--   0        0        0      727 2023-06-21 06:14:11.268529 computex_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 computex_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1233 2023-07-21 20:12:11.066659 computex_cli-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/__init__.py
+-rw-r--r--   0        0        0     8944 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/cli.py
+-rw-r--r--   0        0        0      911 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/config.py
+-rw-r--r--   0        0        0      161 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/exc.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/auth.py
+-rw-r--r--   0        0        0     3065 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/deployments.py
+-rw-r--r--   0        0        0     1912 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/service.py
+-rw-r--r--   0        0        0     1236 2023-07-21 20:12:11.066659 computex_cli-0.1.6/cxcli/services/users.py
+-rw-r--r--   0        0        0      744 2023-07-21 20:12:11.070659 computex_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 computex_cli-0.1.6/PKG-INFO
```

### Comparing `computex_cli-0.1.5/cxcli/cli.py` & `computex_cli-0.1.6/cxcli/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import json
 from datetime import datetime, timezone
 from functools import wraps
+from pathlib import Path
 
 import click
 import docker
 import jwt
+import toml
 from click import ClickException
 from jwt.exceptions import ExpiredSignatureError
 
 from . import exc
 from .config import Config
 from .services.auth import AuthService
-from .services.deployments import DeployRequest, DeploymentServiceV1
+from .services.deployments import (
+    DeployRequest,
+    DeployServerlessRequest,
+    DeploymentServiceV1,
+)
 from .services.users import UserServiceV1
 
 
+_pyproject_toml = toml.load(Path(__file__).resolve().parent.parent / "pyproject.toml")
+
+
 def update_core_api_credentials(access_token, refresh_token):
     config = Config()
     with open(config.credentials_path, "w") as f:
         f.write(f"COMPUTEX_CORE_API_ACCESS_TOKEN={access_token}\n")
         f.write(f"COMPUTEX_CORE_API_REFRESH_TOKEN={refresh_token}\n")
 
 
@@ -78,14 +87,15 @@
             update_core_api_credentials(r.access_token, r.refresh_token)
         return f(*args, **kwargs)
 
     return inner
 
 
 @click.group()
+@click.version_option(version=_pyproject_toml["tool"]["poetry"]["version"])
 def cli():
     pass
 
 
 @cli.command()
 def info():
     config = Config()
@@ -149,14 +159,72 @@
         replicas=replicas,
     )
     DeploymentServiceV1().deploy(r)
     click.echo("Your app has successfully deployed.")
 
 
 @cli.command()
+@click.option("--app", help="Your app's name.")
+@click.option(
+    "--image", help="A container image name that has been pushed to ComputeX."
+)
+@click.option("--num-cpu-cores", default=4, help="Number of CPU cores.")
+@click.option("--num-gpu", default=1, help="Number of GPUs.")
+@click.option(
+    "--gpu", default="A40", help="The type of GPU you'd like to use."
+)  # TODO: Add listing of SKUs
+# @click.option(
+#     "--cpu", default="intel_xeon_v3", help="The type of CPU you'd like to use."
+# )
+@click.option("--memory", default=4, help="Memory in GB to allocate.")
+@click.option(
+    "--concurrency",
+    default=1,
+    help="Represents the number of simultaneous requests sent to a single backend pod at a given time. For GPU inference, this should usually be set to 1. For CPU-based non-blocking requests, this number can be reasonably high, i.e. 100.",
+)
+@click.option(
+    "--min-scale", default=0, help="Minimum concurrent serverless invocations."
+)
+@click.option(
+    "--max-scale", default=1, help="Maximum concurrent serverless invocations."
+)
+@click.option("--public", is_flag=True, default=False)
+@refresh_credentials
+def deploy_serverless(
+    app: str,
+    image: str,
+    num_cpu_cores: int,
+    num_gpu: int,
+    gpu: str,
+    # cpu: str,
+    memory: int,
+    concurrency: int,
+    min_scale: int,
+    max_scale: int,
+    public: bool,
+):
+    # TODO: Verify that image exists before deployment.
+    r = UserServiceV1().get_registry_credentials()
+    r = DeployServerlessRequest(
+        app_name=app,
+        container_image=f"{r.registry_host}/{r.registry_namespace}/{image}",
+        num_cpu_cores=num_cpu_cores,
+        num_gpu=num_gpu,
+        gpu=gpu,
+        # cpu_sku=cpu_sku,
+        memory=memory,
+        concurrency=concurrency,
+        min_scale=min_scale,
+        max_scale=max_scale,
+    )
+    DeploymentServiceV1().deploy_serverless(r, is_public=public)
+    click.echo("Your app has successfully deployed.")
+
+
+@cli.command()
 @refresh_credentials
 def list_deployments():
     deployments = DeploymentServiceV1().list()
     click.echo(json.dumps(deployments.dict(), indent=4))
 
 
 @cli.command()
```

### Comparing `computex_cli-0.1.5/cxcli/config.py` & `computex_cli-0.1.6/cxcli/config.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.5/cxcli/services/auth.py` & `computex_cli-0.1.6/cxcli/services/auth.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.5/cxcli/services/deployments.py` & `computex_cli-0.1.6/cxcli/services/deployments.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,28 @@
     # TODO: Share SKU enums from main repo.
     gpu: str
     # cpu: str
     memory: int
     replicas: int
 
 
+class DeployServerlessRequest(BaseModel):
+    app_name: str
+    container_image: str
+    num_cpu_cores: int
+    num_gpu: int
+    # TODO: Share SKU enums from main repo.
+    gpu: str
+    # cpu: str
+    memory: int
+    concurrency: int = 1
+    min_scale: int = 0
+    max_scale: int = 10
+
+
 class DeployResponse(BaseModel):
     app_name: str
 
 
 class DeleteResponse(BaseModel):
     # TODO: Needs better definition once the spec starts to settle.
     status: dict
@@ -44,14 +58,28 @@
     def deploy(self, deploy_request: DeployRequest) -> DeployResponse:
         r = self._post("/deploy", json=deploy_request.dict())
         # TODO: Add better status checks and failed login reporting.
         r.raise_for_status()
         j = r.json()
         return DeployResponse(app_name=j["app_name"])
 
+    def deploy_serverless(
+        self,
+        deploy_serverless_request: DeployServerlessRequest,
+        is_public: bool = False,
+    ) -> DeployResponse:
+        path = (
+            is_public and "/deploy_serverless_public_endpoint" or "/deploy_serverless"
+        )
+        r = self._post(path, json=deploy_serverless_request.dict())
+        # TODO: Add better status checks and failed login reporting.
+        r.raise_for_status()
+        j = r.json()
+        return DeployResponse(app_name=j["app_name"])
+
     def list(self) -> ListDeploymentsResponse:
         r = self._get("/deployments")
         # TODO: Add better status checks and failed login reporting.
         r.raise_for_status()
         j = r.json()
         return ListDeploymentsResponse(deployments=j["deployments"])
```

### Comparing `computex_cli-0.1.5/cxcli/services/service.py` & `computex_cli-0.1.6/cxcli/services/service.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.5/cxcli/services/users.py` & `computex_cli-0.1.6/cxcli/services/users.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.5/pyproject.toml` & `computex_cli-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "computex-cli"
-version = "0.1.5"
+version = "0.1.6"
 description = "ComputeX CLI tool"
 authors = ["Abate De Mey <abate@computex.ai>"]
 readme = "README.md"
 packages = [{include = "cxcli"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 click = "^8.1.3"
 requests = "^2.31.0"
 pydantic = "^1.10.9"
 python-dotenv = "^1.0.0"
 pyjwt = "^2.7.0"
 cryptography = "^41.0.1"
 docker = "^6.1.3"
+toml = "^0.10.2"
 
 [tool.poetry.scripts]
 cx = "cxcli.cli:cli"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
```

