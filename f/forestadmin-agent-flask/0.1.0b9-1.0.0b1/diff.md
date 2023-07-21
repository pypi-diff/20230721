# Comparing `tmp/forestadmin_agent_flask-0.1.0b9.tar.gz` & `tmp/forestadmin_agent_flask-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_flask-0.1.0b9.tar", max compression
+gzip compressed data, was "forestadmin_agent_flask-1.0.0b1.tar", max compression
```

## Comparing `forestadmin_agent_flask-0.1.0b9.tar` & `forestadmin_agent_flask-1.0.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2022-12-07 16:22:25.605515 forestadmin_agent_flask-0.1.0b9/README.md
--rw-r--r--   0        0        0        0 2022-12-07 16:22:25.605515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/__init__.py
--rw-r--r--   0        0        0     5711 2022-12-07 16:22:25.605515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/agent.py
--rw-r--r--   0        0        0        0 2022-12-07 16:22:25.609515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/__init__.py
--rw-r--r--   0        0        0      582 2022-12-07 16:22:25.609515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/dispatcher.py
--rw-r--r--   0        0        0     1449 2022-12-07 16:22:25.609515 forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/requests.py
--rw-r--r--   0        0        0     1330 2022-12-07 16:22:42.049444 forestadmin_agent_flask-0.1.0b9/pyproject.toml
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 forestadmin_agent_flask-0.1.0b9/setup.py
--rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 forestadmin_agent_flask-0.1.0b9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/__init__.py
+-rw-r--r--   0        0        0     7476 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/agent.py
+-rw-r--r--   0        0        0      125 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/exception.py
+-rw-r--r--   0        0        0        0 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/__init__.py
+-rw-r--r--   0        0        0      581 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/dispatcher.py
+-rw-r--r--   0        0        0     1449 2023-07-21 14:38:11.871842 forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/requests.py
+-rw-r--r--   0        0        0     1797 2023-07-21 14:38:35.884063 forestadmin_agent_flask-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 forestadmin_agent_flask-1.0.0b1/PKG-INFO
```

### Comparing `forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/agent.py` & `forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 import asyncio
-from typing import Literal, Optional, Tuple, Union
+import os
+import sys
+from typing import Optional, Tuple, Union
+
+import pkg_resources
+
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
 
 from flask import Blueprint, request
+from flask.app import Flask
 from flask.wrappers import Request as FlaskRequest
 from flask.wrappers import Response as FlaskResponse
 from forestadmin.agent_toolkit.agent import Agent as BaseAgent
-from forestadmin.agent_toolkit.options import AgentMeta, Options
+from forestadmin.agent_toolkit.options import Options
 from forestadmin.agent_toolkit.resources.base import BaseResource
 from forestadmin.agent_toolkit.resources.collections.crud import LiteralMethod as CrudLiteralMethod
 from forestadmin.agent_toolkit.resources.security.resources import LiteralMethod as AuthLiteralMethod
 from forestadmin.agent_toolkit.utils.context import Request
+from forestadmin.agent_toolkit.utils.forest_schema.type import AgentMeta
+from forestadmin.flask_agent.exception import FlaskAgentException
 from forestadmin.flask_agent.utils.dispatcher import get_dispatcher_method
 from forestadmin.flask_agent.utils.requests import convert_request, convert_response
 
 
 class Agent(BaseAgent):
-
     META: AgentMeta = {
-        "liana": "forest-nodejs-agent",
-        "liana_version": "1.0.0",
-        "stack": {"database_type": "postgresql", "orm_version": "3.2.14"},
+        "liana": "agent-python",
+        "liana_version": pkg_resources.get_distribution("forestadmin-agent-flask").version.replace("b", "-beta."),
+        # .replace because poetry force 0.0.1b25 instead of 0.0.1-beta.25
+        # for more details:
+        # https://python-poetry.org/docs/master/faq/ : "Why does Poetry not adhere to semantic versioning?"
+        "stack": {"engine": "python", "engine_version": ".".join(map(str, [*sys.version_info[:3]]))},
     }
 
     def __init__(self, options: Options):
         super(Agent, self).__init__(options)
         self._blueprint: Optional[Blueprint] = None
-        self.loop = asyncio.get_event_loop()
+        self.loop = asyncio.new_event_loop()
 
     @property
     def blueprint(self) -> Blueprint:
         if not self._blueprint:
-            raise
+            raise FlaskAgentException("Flask agent must have the forest blueprint.")
         return self._blueprint
 
     @blueprint.setter
     def blueprint(self, blueprint: Blueprint):
         self._blueprint = blueprint
 
+    def register_blueprint(self, app: Flask):
+        self.options["schema_path"] = os.path.join(app.root_path, ".forestadmin-schema.json")
+        app.register_blueprint(self.blueprint, url_prefix="/forest")
+        self.loop.run_until_complete(self.start())
+
 
 def build_agent(options: Options) -> Agent:
     agent = Agent(options)
     agent.blueprint = build_blueprint(agent)
     return agent
 
 
@@ -48,19 +67,14 @@
     response.headers["Access-Control-Allow-Private-Network"] = "true"
     return response
 
 
 def build_blueprint(agent: Agent):  # noqa: C901
     blueprint = Blueprint("flask_forest", __name__)
     blueprint.after_request(_after_request)
-    crud_resource = agent.resources["crud"]
-    crud_related_resource = agent.resources["crud_related"]
-    auth_resource = agent.resources["authentication"]
-    stats_resource = agent.resources["stats"]
-    actions_resource = agent.resources["actions"]
 
     def _get_dispatch(
         request: FlaskRequest,
         method: Union[CrudLiteralMethod, AuthLiteralMethod, Literal["execute", "hook"], None] = None,
         detail: bool = False,
     ) -> Tuple[Request, Union[CrudLiteralMethod, AuthLiteralMethod, Literal["execute", "hook"]]]:
         if not method:
@@ -82,50 +96,66 @@
     async def index() -> FlaskResponse:  # type: ignore
         rsp = FlaskResponse()
         rsp.status = 200
         return rsp
 
     @blueprint.route("/authentication/callback", methods=["GET"])
     async def callback() -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, auth_resource, "callback")
+        return await _get_collection_response(request, agent.resources["authentication"], "callback")
 
     @blueprint.route("/_actions/<collection_name>/<int:action_name>/<slug>/hooks/load", methods=["POST"])
     async def load_hook(**_) -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, actions_resource, "hook")
+        return await _get_collection_response(request, agent.resources["actions"], "hook")
 
     @blueprint.route("/_actions/<collection_name>/<int:action_name>/<slug>/hooks/change", methods=["POST"])
     async def change_hook(**_) -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, actions_resource, "hook")
+        return await _get_collection_response(request, agent.resources["actions"], "hook")
 
     @blueprint.route("/_actions/<collection_name>/<int:action_name>/<slug>", methods=["POST"])
     async def actions(**_) -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, actions_resource, "execute")
+        return await _get_collection_response(request, agent.resources["actions"], "execute")
 
     @blueprint.route("/authentication", methods=["POST"])
     async def authentication() -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, auth_resource, "authenticate")
+        return await _get_collection_response(request, agent.resources["authentication"], "authenticate")
 
     @blueprint.route("/stats/<collection_name>", methods=["POST"])
     async def stats(**_) -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, stats_resource)
+        return await _get_collection_response(request, agent.resources["stats"])
+
+    @blueprint.route("/_charts/<chart_name>", methods=["POST", "GET"])
+    async def charts(**_) -> FlaskResponse:  # type: ignore
+        return await _get_collection_response(request, agent.resources["datasource_charts"])
+
+    @blueprint.route("/_charts/<collection_name>/<chart_name>", methods=["POST", "GET"])
+    async def charts_collection(**_) -> FlaskResponse:  # type: ignore
+        return await _get_collection_response(request, agent.resources["collection_charts"])
 
     @blueprint.route("/<collection_name>/count", methods=["GET"])
     async def count(**_) -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, crud_resource, "count")
+        return await _get_collection_response(request, agent.resources["crud"], "count")
 
     @blueprint.route("/<collection_name>/<pks>", methods=["GET", "PUT", "DELETE"])
     async def detail(**_) -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, crud_resource, detail=True)
+        return await _get_collection_response(request, agent.resources["crud"], detail=True)
 
     @blueprint.route("/<collection_name>", methods=["GET", "POST", "DELETE"])
-    async def list(**_) -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, crud_resource)
+    async def list_(**_) -> FlaskResponse:  # type: ignore
+        return await _get_collection_response(request, agent.resources["crud"])
 
     @blueprint.route("/<collection_name>/<pks>/relationships/<relation_name>", methods=["GET", "POST", "DELETE", "PUT"])
     async def list_related(**_) -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, crud_related_resource)
+        return await _get_collection_response(request, agent.resources["crud_related"])
 
     @blueprint.route("/<collection_name>/<pks>/relationships/<relation_name>/count", methods=["GET"])
     async def count_related(**_) -> FlaskResponse:  # type: ignore
-        return await _get_collection_response(request, crud_related_resource, "count")
+        return await _get_collection_response(request, agent.resources["crud_related"], "count")
+
+    @blueprint.route("/<collection_name>.csv", methods=["GET"])
+    async def csv(**_) -> FlaskResponse:  # type: ignore
+        return await _get_collection_response(request, agent.resources["crud"], "csv")
+
+    @blueprint.route("/<collection_name>/<pks>/relationships/<relation_name>.csv", methods=["GET"])
+    async def csv_related(**_) -> FlaskResponse:  # type: ignore
+        return await _get_collection_response(request, agent.resources["crud_related"], "csv")
 
     return blueprint
```

### Comparing `forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/dispatcher.py` & `forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from forestadmin.agent_toolkit.resources.collections.crud import LiteralMethod
 
 LIST_MAPPER: Dict[str, Dict[str, LiteralMethod]] = {
     "LIST": {
         "GET": "list",
         "POST": "add",
         "DELETE": "delete_list",
-        "PUT": "update_list",  # usefull for the related resources
+        "PUT": "update_list",  # useful for the related resources
     },
     "DETAIL": {"GET": "get", "PUT": "update", "DELETE": "delete"},
 }
 
 
 def get_dispatcher_method(request_method: str, detail: bool = False) -> LiteralMethod:
     key = "LIST"
```

### Comparing `forestadmin_agent_flask-0.1.0b9/forestadmin/flask_agent/utils/requests.py` & `forestadmin_agent_flask-1.0.0b1/forestadmin/flask_agent/utils/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-0.1.0b9/pyproject.toml` & `forestadmin_agent_flask-1.0.0b1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-flask"
-version = "0.1.0-beta.9"
+version = "1.0.0-beta.1"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 typing-extensions = "~=4.2"
 tzdata = "~=2022.6"
-flask = "~=2.2.0"
-forestadmin-datasource-toolkit = "^0.1.0-beta.9"
-forestadmin-agent-toolkit = "^0.1.0-beta.9"
+forestadmin-agent-toolkit = "^1.0.0-beta.1"
+forestadmin-datasource-toolkit = "^1.0.0-beta.1"
+Flask-Cors = "^3.0.8"
+
+[tool.poetry.dependencies.flask]
+extras = [ "async",]
+version = "^2.0.0"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~=0.2.1"
 python = "<3.9"
 extras = [ "tzdata",]
 
 [tool.poetry.group.test]
@@ -37,14 +41,16 @@
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "~=7.1"
 pytest-asyncio = "~=0.18"
 coverage = "~=6.5"
 freezegun = "~=1.2.0"
+pytest-cov = "^4.0.0"
+sqlalchemy = "^1.4.44"
 [[tool.poetry.group.test.dependencies.mock]]
 version = "4.0"
 python = "3.7"
 
 [tool.poetry.group.linter.dependencies]
 [[tool.poetry.group.linter.dependencies.flake8]]
 version = "~=5.0"
@@ -55,7 +61,19 @@
 python = ">=3.8.1"
 
 [tool.poetry.group.formatter.dependencies]
 black = "~=22.10"
 
 [tool.poetry.group.sorter.dependencies]
 isort = "~=3.6"
+
+[tool.poetry.group.test.dependencies.forestadmin-datasource-toolkit]
+path = "../datasource_toolkit"
+develop = true
+
+[tool.poetry.group.test.dependencies.forestadmin-datasource-sqlalchemy]
+path = "../datasource_sqlalchemy"
+develop = true
+
+[tool.poetry.group.test.dependencies.forestadmin-agent-toolkit]
+path = "../agent_toolkit"
+develop = true
```

