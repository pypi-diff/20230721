# Comparing `tmp/bamboo-engine-2.7.3.tar.gz` & `tmp/bamboo-engine-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bamboo-engine-2.7.3.tar", max compression
+gzip compressed data, was "bamboo-engine-2.8.0.tar", max compression
```

## Comparing `bamboo-engine-2.7.3.tar` & `bamboo-engine-2.8.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0     1069 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/LICENSE
--rw-r--r--   0        0        0      781 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/__init__.py
--rw-r--r--   0        0        0      768 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/__version__.py
--rw-r--r--   0        0        0    20711 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/api.py
--rw-r--r--   0        0        0      805 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/__init__.py
--rw-r--r--   0        0        0     6627 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/builder.py
--rw-r--r--   0        0        0      866 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/__init__.py
--rw-r--r--   0        0        0     2044 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/activity.py
--rw-r--r--   0        0        0     2379 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/base.py
--rw-r--r--   0        0        0     3546 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/data.py
--rw-r--r--   0        0        0     1285 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/event.py
--rw-r--r--   0        0        0     2166 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/builder/flow/gateway.py
--rw-r--r--   0        0        0     1650 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/config.py
--rw-r--r--   0        0        0     5573 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/context.py
--rw-r--r--   0        0        0    45316 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/engine.py
--rw-r--r--   0        0        0      853 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/__init__.py
--rw-r--r--   0        0        0    42073 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/interfaces.py
--rw-r--r--   0        0        0      898 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/__init__.py
--rw-r--r--   0        0        0     1501 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/event.py
--rw-r--r--   0        0        0     4795 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/handler.py
--rw-r--r--   0        0        0     9183 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/interrupt.py
--rw-r--r--   0        0        0     6627 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/node.py
--rw-r--r--   0        0        0    11555 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/eri/models/runtime.py
--rw-r--r--   0        0        0     1742 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/exceptions.py
--rw-r--r--   0        0        0     5934 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handler.py
--rw-r--r--   0        0        0     1407 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/__init__.py
--rw-r--r--   0        0        0     8106 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/conditional_parallel_gateway.py
--rw-r--r--   0        0        0     2282 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/converge_gateway.py
--rw-r--r--   0        0        0     7561 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/empty_end_event.py
--rw-r--r--   0        0        0     4946 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/empty_start_event.py
--rw-r--r--   0        0        0     7718 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/exclusive_gateway.py
--rw-r--r--   0        0        0     4399 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/executable_end_event.py
--rw-r--r--   0        0        0     3318 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/parallel_gateway.py
--rw-r--r--   0        0        0    22403 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/service_activity.py
--rw-r--r--   0        0        0     6642 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/handlers/subprocess.py
--rw-r--r--   0        0        0     9442 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/interrupt.py
--rw-r--r--   0        0        0     1810 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/local.py
--rw-r--r--   0        0        0    12434 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/metrics.py
--rw-r--r--   0        0        0     2214 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/states.py
--rw-r--r--   0        0        0      825 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/template/__init__.py
--rw-r--r--   0        0        0     1747 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/template/sandbox.py
--rw-r--r--   0        0        0     6822 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/template/template.py
--rw-r--r--   0        0        0      800 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/utils/__init__.py
--rw-r--r--   0        0        0      892 2023-06-16 07:00:31.816582 bamboo-engine-2.7.3/bamboo_engine/utils/boolrule/__init__.py
--rw-r--r--   0        0        0     9057 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/boolrule/boolrule.py
--rw-r--r--   0        0        0     1834 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/collections.py
--rw-r--r--   0        0        0      936 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/constants.py
--rw-r--r--   0        0        0    15396 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/graph.py
--rw-r--r--   0        0        0      879 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/host.py
--rw-r--r--   0        0        0     2092 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_safety.py
--rw-r--r--   0        0        0      778 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/__init__.py
--rw-r--r--   0        0        0     2361 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/checker.py
--rw-r--r--   0        0        0     1803 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/code_extract.py
--rw-r--r--   0        0        0      805 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/exceptions.py
--rw-r--r--   0        0        0     4159 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/visitors.py
--rw-r--r--   0        0        0      884 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/object.py
--rw-r--r--   0        0        0     2064 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/utils/string.py
--rw-r--r--   0        0        0      801 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/__init__.py
--rw-r--r--   0        0        0     1919 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/api.py
--rw-r--r--   0        0        0     2770 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/connection.py
--rw-r--r--   0        0        0    16793 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/gateway.py
--rw-r--r--   0        0        0     2507 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/rules.py
--rw-r--r--   0        0        0     2847 2023-06-16 07:00:31.820582 bamboo-engine-2.7.3/bamboo_engine/validator/utils.py
--rw-r--r--   0        0        0      742 2023-06-16 07:00:31.828582 bamboo-engine-2.7.3/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 bamboo-engine-2.7.3/setup.py
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 bamboo-engine-2.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/LICENSE
+-rw-r--r--   0        0        0      781 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/__init__.py
+-rw-r--r--   0        0        0      768 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/__version__.py
+-rw-r--r--   0        0        0    20711 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/api.py
+-rw-r--r--   0        0        0      805 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/builder/__init__.py
+-rw-r--r--   0        0        0     6627 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/builder/builder.py
+-rw-r--r--   0        0        0      866 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/builder/flow/__init__.py
+-rw-r--r--   0        0        0     2044 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/builder/flow/activity.py
+-rw-r--r--   0        0        0     2379 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/builder/flow/base.py
+-rw-r--r--   0        0        0     3546 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/builder/flow/data.py
+-rw-r--r--   0        0        0     1285 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/builder/flow/event.py
+-rw-r--r--   0        0        0     2166 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/builder/flow/gateway.py
+-rw-r--r--   0        0        0     1913 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/config.py
+-rw-r--r--   0        0        0     5573 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/context.py
+-rw-r--r--   0        0        0    45772 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/engine.py
+-rw-r--r--   0        0        0      853 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/eri/__init__.py
+-rw-r--r--   0        0        0    43745 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/eri/interfaces.py
+-rw-r--r--   0        0        0      898 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/eri/models/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/eri/models/event.py
+-rw-r--r--   0        0        0     4795 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/eri/models/handler.py
+-rw-r--r--   0        0        0     9183 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/eri/models/interrupt.py
+-rw-r--r--   0        0        0     6677 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/eri/models/node.py
+-rw-r--r--   0        0        0    11555 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/eri/models/runtime.py
+-rw-r--r--   0        0        0     1742 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/exceptions.py
+-rw-r--r--   0        0        0     5934 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handler.py
+-rw-r--r--   0        0        0     1407 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/__init__.py
+-rw-r--r--   0        0        0     8238 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/conditional_parallel_gateway.py
+-rw-r--r--   0        0        0     2282 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/converge_gateway.py
+-rw-r--r--   0        0        0     7619 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/empty_end_event.py
+-rw-r--r--   0        0        0     4946 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/empty_start_event.py
+-rw-r--r--   0        0        0     8290 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/exclusive_gateway.py
+-rw-r--r--   0        0        0     4399 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/executable_end_event.py
+-rw-r--r--   0        0        0     3318 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/parallel_gateway.py
+-rw-r--r--   0        0        0    22652 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/service_activity.py
+-rw-r--r--   0        0        0     6642 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/handlers/subprocess.py
+-rw-r--r--   0        0        0     9442 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/interrupt.py
+-rw-r--r--   0        0        0     1810 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/local.py
+-rw-r--r--   0        0        0    12434 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/metrics.py
+-rw-r--r--   0        0        0     2214 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/states.py
+-rw-r--r--   0        0        0      825 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/template/__init__.py
+-rw-r--r--   0        0        0     1747 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/template/sandbox.py
+-rw-r--r--   0        0        0     6822 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/template/template.py
+-rw-r--r--   0        0        0      800 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/__init__.py
+-rw-r--r--   0        0        0      892 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/boolrule/__init__.py
+-rw-r--r--   0        0        0     9057 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/boolrule/boolrule.py
+-rw-r--r--   0        0        0     1834 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/collections.py
+-rw-r--r--   0        0        0     1461 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/constants.py
+-rw-r--r--   0        0        0      166 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/expr.py
+-rw-r--r--   0        0        0    15396 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/graph.py
+-rw-r--r--   0        0        0      879 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/host.py
+-rw-r--r--   0        0        0     2092 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/mako_safety.py
+-rw-r--r--   0        0        0      778 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/__init__.py
+-rw-r--r--   0        0        0     2361 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/checker.py
+-rw-r--r--   0        0        0     1803 2023-07-21 03:27:25.250201 bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/code_extract.py
+-rw-r--r--   0        0        0      805 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/exceptions.py
+-rw-r--r--   0        0        0     4159 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/visitors.py
+-rw-r--r--   0        0        0      884 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/utils/object.py
+-rw-r--r--   0        0        0     2064 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/utils/string.py
+-rw-r--r--   0        0        0      801 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/validator/__init__.py
+-rw-r--r--   0        0        0     1919 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/validator/api.py
+-rw-r--r--   0        0        0     2770 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/validator/connection.py
+-rw-r--r--   0        0        0    16793 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/validator/gateway.py
+-rw-r--r--   0        0        0     2507 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/validator/rules.py
+-rw-r--r--   0        0        0     2847 2023-07-21 03:27:25.254201 bamboo-engine-2.8.0/bamboo_engine/validator/utils.py
+-rw-r--r--   0        0        0      742 2023-07-21 03:27:25.262201 bamboo-engine-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 bamboo-engine-2.8.0/setup.py
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 bamboo-engine-2.8.0/PKG-INFO
```

### Comparing `bamboo-engine-2.7.3/LICENSE` & `bamboo-engine-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/__version__.py` & `bamboo-engine-2.8.0/bamboo_engine/validator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-__version__ = "2.7.3"
+from .api import validate_and_process_pipeline  # noqa
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/api.py` & `bamboo-engine-2.8.0/bamboo_engine/api.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/builder/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/builder/builder.py` & `bamboo-engine-2.8.0/bamboo_engine/builder/builder.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/builder/flow/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/builder/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/builder/flow/activity.py` & `bamboo-engine-2.8.0/bamboo_engine/builder/flow/activity.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/builder/flow/base.py` & `bamboo-engine-2.8.0/bamboo_engine/builder/flow/base.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/builder/flow/data.py` & `bamboo-engine-2.8.0/bamboo_engine/builder/flow/data.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/builder/flow/event.py` & `bamboo-engine-2.8.0/bamboo_engine/builder/flow/event.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/builder/flow/gateway.py` & `bamboo-engine-2.8.0/bamboo_engine/builder/flow/gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/config.py` & `bamboo-engine-2.8.0/bamboo_engine/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
+from bamboo_engine.utils.constants import ExclusiveGatewayStrategy
+from bamboo_engine.utils.expr import default_expr_func
 
 # 引擎内部配置模块
 
 
 class Settings:
     """
     引擎全局配置对象
@@ -60,7 +62,11 @@
         "vars",
         "__import__",
     ]
 
     MAKO_SANDBOX_IMPORT_MODULES = {}
 
     RERUN_INDEX_OFFSET = 0
+
+    PIPELINE_EXCLUSIVE_GATEWAY_EXPR_FUNC = default_expr_func
+
+    PIPELINE_EXCLUSIVE_GATEWAY_STRATEGY = ExclusiveGatewayStrategy.ONLY.value
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/context.py` & `bamboo-engine-2.8.0/bamboo_engine/context.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/engine.py` & `bamboo-engine-2.8.0/bamboo_engine/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,24 +36,24 @@
     ExecuteKeyPoint,
     InterruptException,
     ScheduleInterrupter,
     ScheduleKeyPoint,
 )
 from .local import CurrentNodeInfo, clear_node_info, set_node_info
 from .metrics import (
+    ENGINE_EXECUTE_POST_PROCESS_DURATION,
+    ENGINE_EXECUTE_PRE_PROCESS_DURATION,
     ENGINE_NODE_EXECUTE_TIME,
     ENGINE_NODE_SCHEDULE_TIME,
     ENGINE_PROCESS_RUNNING_TIME,
     ENGINE_RUNNING_PROCESSES,
     ENGINE_RUNNING_SCHEDULES,
-    ENGINE_SCHEDULE_RUNNING_TIME,
-    ENGINE_EXECUTE_PRE_PROCESS_DURATION,
-    ENGINE_EXECUTE_POST_PROCESS_DURATION,
-    ENGINE_SCHEDULE_PRE_PROCESS_DURATION,
     ENGINE_SCHEDULE_POST_PROCESS_DURATION,
+    ENGINE_SCHEDULE_PRE_PROCESS_DURATION,
+    ENGINE_SCHEDULE_RUNNING_TIME,
     setup_gauge,
     setup_histogram,
 )
 from .utils.host import get_hostname
 from .utils.string import get_lower_case_name
 
 logger = logging.getLogger("bamboo_engine")
@@ -804,14 +804,16 @@
                     )
                     execute_result = interrupter.recover_point.execute_result
                 else:
                     handler = HandlerFactory.get_handler(node, self.runtime, interrupter)
                     ENGINE_EXECUTE_PRE_PROCESS_DURATION.labels(type=node.type.value, hostname=self._hostname).observe(
                         time.time() - engine_pre_execute_start_at
                     )
+                    # 进入节点
+                    self.runtime.node_enter(root_pipeline_id=root_pipeline_id, node_id=node.id)
                     execute_result = handler.execute(
                         process_info=process_info,
                         loop=loop,
                         inner_loop=inner_loop,
                         version=version,
                         recover_point=interrupter.recover_point,
                     )
@@ -826,14 +828,18 @@
                     execute_result.__dict__,
                 )
 
                 ENGINE_NODE_EXECUTE_TIME.labels(type=type_label, hostname=self._hostname).observe(
                     time.time() - execute_start
                 )
 
+                # 节点运行成功并且不需要进行调度
+                if not execute_result.should_sleep and execute_result.next_node_id != node.id:
+                    self.runtime.node_finish(root_pipeline_id=root_pipeline_id, node_id=node.id)
+
                 # 进程是否要进入睡眠
                 if execute_result.should_sleep:
                     self.runtime.sleep(process_id)
 
                 # 节点是否准备好进入调度
                 if execute_result.schedule_ready:
                     schedule = self.runtime.set_schedule(
@@ -1096,14 +1102,15 @@
                     schedule_id=schedule_id,
                     schedule_after=schedule_result.schedule_after,
                     headers=headers,
                 )
 
             if schedule_result.schedule_done:
                 self.runtime.finish_schedule(schedule_id)
+                self.runtime.node_finish(root_pipeline_id, node.id)
                 self.runtime.execute(
                     process_id=process_id,
                     node_id=schedule_result.next_node_id,
                     root_pipeline_id=process_info.root_pipeline_id,
                     parent_pipeline_id=process_info.top_pipeline_id,
                     headers=headers,
                 )
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/eri/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/eri/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/eri/interfaces.py` & `bamboo-engine-2.8.0/bamboo_engine/eri/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,37 +7,37 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-from datetime import datetime
 from abc import ABCMeta, abstractmethod
-from typing import List, Optional, Dict, Set, Any, Tuple
+from datetime import datetime
+from typing import Any, Dict, List, Optional, Set, Tuple
 
 from .models import (
-    ScheduleInterruptPoint,
-    State,
-    Node,
-    Schedule,
-    ScheduleType,
+    CallbackData,
+    ContextValue,
     Data,
     DataInput,
+    DispatchProcess,
+    ExecuteInterruptEvent,
+    ExecuteInterruptPoint,
     ExecutionData,
     ExecutionHistory,
     ExecutionShortHistory,
-    CallbackData,
+    Node,
     ProcessInfo,
-    SuspendedProcessInfo,
-    DispatchProcess,
-    ContextValue,
-    ExecuteInterruptPoint,
-    ExecuteInterruptEvent,
+    Schedule,
     ScheduleInterruptEvent,
+    ScheduleInterruptPoint,
+    ScheduleType,
+    State,
+    SuspendedProcessInfo,
 )
 
 # plugin interface
 
 __version__ = "7.1.0"
 
 
@@ -180,22 +180,24 @@
 
 class PluginManagerMixin:
     """
     插件管理接口，声明了插件（服务，可执行结束节点，变量）管理相关的接口
     """
 
     @abstractmethod
-    def get_service(self, code: str, version: str) -> Service:
+    def get_service(self, code: str, version: str, name: str = None) -> Service:
         """
         根据代号与版本获取特定服务对象实例
 
         :param code: 服务唯一代号
         :type code: str
         :param version: 服务版本
         :type version: str
+        :param name: 服务名
+        :type version: str
         :return: 服务对象实例
         :rtype: Service
         """
 
     @abstractmethod
     def get_executable_end_event(self, code: str) -> ExecutableEvent:
         """
@@ -227,14 +229,64 @@
         :param additional_data: 额外数据字典
         :type additional_data: dict
         :return: 变量实例
         :rtype: Variable
         """
 
 
+class EngineRuntimeHooksMixin:
+    def node_execute_fail(self, root_pipeline_id: str, node_id: str, ex_data: str):
+        """
+        节点execute方法异常需要执行的钩子
+        :param root_pipeline_id: 任务ID
+        :type node_id: str
+        :param node_id: 节点ID
+        :type node_id: str
+        :param ex_data: 异常信息
+        :type ex_data: str
+        """
+
+    def node_schedule_fail(self, root_pipeline_id: str, node_id: str, ex_data: str):
+        """
+        节点schedule方法异常需要执行的钩子
+        :param root_pipeline_id: 任务ID
+        :type node_id: str
+        :param node_id: 节点ID
+        :type node_id: str
+        :param ex_data: 异常信息
+        :type ex_data: str
+        """
+
+    def node_enter(self, root_pipeline_id: str, node_id: str):
+        """
+        进入节点前
+        :param root_pipeline_id: 任务ID
+        :type node_id: str
+        :param node_id: 节点ID
+        :type node_id: str
+        """
+
+    def node_finish(self, root_pipeline_id: str, node_id: str):
+        """
+        离开节点需要执行的钩子
+        :param root_pipeline_id: 任务ID
+        :type node_id: str
+        :param node_id: 节点ID
+        :type node_id: str
+        """
+
+    def pipeline_finish(self, pipeline_id: str):
+        """
+        pipeline 结束执行的钩子
+
+        :param pipeline_id: 流程 ID
+        :type pipeline_id: str
+        """
+
+
 class EngineAPIHooksMixin:
     """
     引擎 API 执行时调用的钩子相关接口声明
     """
 
     def pre_prepare_run_pipeline(
         self, pipeline: dict, root_pipeline_data: dict, root_pipeline_context: dict, subprocess_context: dict, **options
@@ -1465,26 +1517,36 @@
     @abstractmethod
     def handle_schedule_interrupt_event(self, event: ScheduleInterruptEvent):
         """
         schedule 中断事件出现后的处理钩子
         """
 
 
+class ConfigMixin:
+    @abstractmethod
+    def get_config(self, name):
+        """
+        获取配置
+        """
+
+
 class EngineRuntimeInterface(
     PluginManagerMixin,
     EngineAPIHooksMixin,
+    EngineRuntimeHooksMixin,
     TaskMixin,
     ProcessMixin,
     StateMixin,
     NodeMixin,
     ScheduleMixin,
     ContextMixin,
     DataMixin,
     ExecutionHistoryMixin,
     InterruptMixin,
+    ConfigMixin,
     metaclass=ABCMeta,
 ):
     @abstractmethod
     def prepare_run_pipeline(
         self, pipeline: dict, root_pipeline_data: dict, root_pipeline_context: dict, subprocess_context: dict, **options
     ) -> int:
         """
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/eri/models/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/eri/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/eri/models/event.py` & `bamboo-engine-2.8.0/bamboo_engine/eri/models/event.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/eri/models/handler.py` & `bamboo-engine-2.8.0/bamboo_engine/eri/models/handler.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/eri/models/interrupt.py` & `bamboo-engine-2.8.0/bamboo_engine/eri/models/interrupt.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/eri/models/node.py` & `bamboo-engine-2.8.0/bamboo_engine/eri/models/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         target_flows: List[str],
         target_nodes: List[str],
         targets: Dict[str, str],
         root_pipeline_id: str,
         parent_pipeline_id: str,
         can_skip: bool = True,
         can_retry: bool = True,
+        name: str = None
     ):
         """
 
         :param id: 节点 ID
         :type id: str
         :param type: 节点类型
         :type type: NodeType
@@ -76,14 +77,15 @@
         self.targets = targets
         self.target_flows = target_flows
         self.target_nodes = target_nodes
         self.root_pipeline_id = root_pipeline_id
         self.parent_pipeline_id = parent_pipeline_id
         self.can_skip = can_skip
         self.can_retry = can_retry
+        self.name = name
 
 
 class EmptyStartEvent(Node):
     pass
 
 
 class ConvergeGateway(Node):
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/eri/models/runtime.py` & `bamboo-engine-2.8.0/bamboo_engine/eri/models/runtime.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/exceptions.py` & `bamboo-engine-2.8.0/bamboo_engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handler.py` & `bamboo-engine-2.8.0/bamboo_engine/handler.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/conditional_parallel_gateway.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/conditional_parallel_gateway.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 import json
 import logging
 from typing import Optional
 
 from pyparsing import ParseException
 
-from bamboo_engine.utils.boolrule import BoolRule
-from bamboo_engine.template.template import Template
-from bamboo_engine.interrupt import ExecuteKeyPoint
-from bamboo_engine import states, metrics
-from bamboo_engine.eri import NodeType, ProcessInfo, ExecuteInterruptPoint
+from bamboo_engine import metrics, states
 from bamboo_engine.context import Context
-from bamboo_engine.handler import register_handler, NodeHandler, ExecuteResult
+from bamboo_engine.eri import ExecuteInterruptPoint, NodeType, ProcessInfo
+from bamboo_engine.handler import ExecuteResult, NodeHandler, register_handler
+from bamboo_engine.interrupt import ExecuteKeyPoint
+from bamboo_engine.template.template import Template
+from bamboo_engine.utils.constants import RuntimeSettings
 from bamboo_engine.utils.string import transform_escape_char
 
 logger = logging.getLogger("bamboo_engine")
 
 
 @register_handler(NodeType.ConditionalParallelGateway)
 class ConditionalParallelGatewayHandler(NodeHandler):
@@ -105,15 +105,16 @@
                 self.node.id,
                 c.evaluation,
                 resolved_evaluate,
                 hydrated_context,
             )
 
             try:
-                result = BoolRule(resolved_evaluate).test()
+                expr_func = self.runtime.get_config(RuntimeSettings.PIPELINE_EXCLUSIVE_GATEWAY_EXPR_FUNC.value)
+                result = expr_func(resolved_evaluate, hydrated_context)
                 logger.info(
                     "root_pipeline[%s] node(%s) %s test result: %s",
                     root_pipeline_id,
                     self.node.id,
                     resolved_evaluate,
                     result,
                 )
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/converge_gateway.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/converge_gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/empty_end_event.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/empty_end_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
 import logging
 from typing import Optional
 
-from bamboo_engine import states, metrics
+from bamboo_engine import metrics, states
 from bamboo_engine.config import Settings
-from bamboo_engine.eri import ProcessInfo, NodeType, ExecuteInterruptPoint
-from bamboo_engine.handler import register_handler, NodeHandler, ExecuteResult
 from bamboo_engine.context import Context
+from bamboo_engine.eri import ExecuteInterruptPoint, NodeType, ProcessInfo
+from bamboo_engine.handler import ExecuteResult, NodeHandler, register_handler
 from bamboo_engine.template.template import Template
 
 logger = logging.getLogger("bamboo_engine")
 
 
 @register_handler(NodeType.EmptyEndEvent)
 class EmptyEndEventHandler(NodeHandler):
@@ -152,14 +152,15 @@
                 to_state=states.FINISHED,
                 set_archive_time=True,
                 ignore_boring_set=recover_point is not None,
             )
 
             # root pipeline finish
             if root_pipeline_finished:
+                self.runtime.pipeline_finish(pipeline_id)
                 return ExecuteResult(
                     should_sleep=False,
                     schedule_ready=False,
                     schedule_type=None,
                     schedule_after=-1,
                     dispatch_processes=[],
                     next_node_id=None,
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/empty_start_event.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/empty_start_event.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/exclusive_gateway.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/exclusive_gateway.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 """
 import json
 import logging
 from typing import Optional
 
 from pyparsing import ParseException
 
-from bamboo_engine import states, metrics
+from bamboo_engine import metrics, states
 from bamboo_engine.context import Context
+from bamboo_engine.eri import ExecuteInterruptPoint, NodeType, ProcessInfo
+from bamboo_engine.handler import ExecuteResult, NodeHandler, register_handler
 from bamboo_engine.template import Template
-from bamboo_engine.handler import register_handler, NodeHandler, ExecuteResult
-from bamboo_engine.utils.boolrule import BoolRule
-from bamboo_engine.eri import NodeType, ProcessInfo, ExecuteInterruptPoint
-
+from bamboo_engine.utils.constants import ExclusiveGatewayStrategy, RuntimeSettings
 from bamboo_engine.utils.string import transform_escape_char
 
 logger = logging.getLogger("bamboo_engine")
 
 
 @register_handler(NodeType.ExclusiveGateway)
 class ExclusiveGatewayHandler(NodeHandler):
@@ -111,22 +110,30 @@
                 root_pipeline_id,
                 self.node.id,
                 c.evaluation,
                 resolved_evaluate,
                 hydrated_context,
             )
             try:
-                result = BoolRule(resolved_evaluate).test()
+                expr_func = self.runtime.get_config(RuntimeSettings.PIPELINE_EXCLUSIVE_GATEWAY_EXPR_FUNC.value)
+                result = expr_func(resolved_evaluate, hydrated_context)
                 logger.info(
                     "root_pipeline[%s] node(%s) %s test result: %s",
                     root_pipeline_id,
                     self.node.id,
                     resolved_evaluate,
                     result,
                 )
+
+                strategy = self.runtime.get_config(RuntimeSettings.PIPELINE_EXCLUSIVE_GATEWAY_STRATEGY.value)
+                # 如果策略是命中第一个，并且result为true, 则直接结束循环
+                if strategy == ExclusiveGatewayStrategy.FIRST.value and result:
+                    meet_conditions.append(c.name)
+                    meet_targets.append(c.target_id)
+                    break
             except ParseException as e:
                 logger.exception(f"[exclusive_gateway] evaluation parse error: {e}")
                 return self._execute_fail(
                     ex_data="evaluate[{}] fail with data[{}]："
                     "please check if some variable not exists or the expression is unsupported, "
                     "related reference is "
                     '<a href="https://boolrule.readthedocs.io/en/latest/expressions.html">boolrule</a>'.format(
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/executable_end_event.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/executable_end_event.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/parallel_gateway.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/parallel_gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/service_activity.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/service_activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,45 +11,44 @@
 specific language governing permissions and limitations under the License.
 """
 
 import logging
 import traceback
 from typing import Optional
 
-from bamboo_engine import states, metrics
+from bamboo_engine import metrics, states
 from bamboo_engine.config import Settings
-
 from bamboo_engine.context import Context
-from bamboo_engine.eri.models.interrupt import ScheduleInterruptPoint
-from bamboo_engine.interrupt import ExecuteKeyPoint, ScheduleKeyPoint
-from bamboo_engine.metrics import (
-    ENGINE_SCHEDULE_FAILED_COUNT,
-    ENGINE_EXECUTE_FAILED_COUNT,
-    ENGINE_EXECUTE_EXCEPTION_COUNT,
-    ENGINE_SCHEDULE_EXCEPTION_COUNT,
-)
-from bamboo_engine.template import Template
 from bamboo_engine.eri import (
-    ProcessInfo,
+    CallbackData,
     ContextValue,
     ContextValueType,
+    ExecuteInterruptPoint,
     ExecutionData,
-    CallbackData,
-    ScheduleType,
+    FancyDict,
     NodeType,
+    ProcessInfo,
     Schedule,
-    ExecuteInterruptPoint,
-    FancyDict,
+    ScheduleType,
 )
+from bamboo_engine.eri.models.interrupt import ScheduleInterruptPoint
 from bamboo_engine.handler import (
-    register_handler,
-    NodeHandler,
     ExecuteResult,
+    NodeHandler,
     ScheduleResult,
+    register_handler,
 )
+from bamboo_engine.interrupt import ExecuteKeyPoint, ScheduleKeyPoint
+from bamboo_engine.metrics import (
+    ENGINE_EXECUTE_EXCEPTION_COUNT,
+    ENGINE_EXECUTE_FAILED_COUNT,
+    ENGINE_SCHEDULE_EXCEPTION_COUNT,
+    ENGINE_SCHEDULE_FAILED_COUNT,
+)
+from bamboo_engine.template import Template
 
 logger = logging.getLogger("bamboo_engine")
 
 
 @register_handler(NodeType.ServiceActivity)
 class ServiceActivityHandler(NodeHandler):
     """
@@ -187,15 +186,15 @@
             execute_inputs.update(render_escape_inputs)
 
             # data prepare
             service_data = ExecutionData(inputs=execute_inputs, outputs={})
             root_pipeline_data = ExecutionData(inputs=root_pipeline_inputs, outputs={})
 
             # execute
-            service = self.runtime.get_service(code=self.node.code, version=self.node.version)
+            service = self.runtime.get_service(code=self.node.code, version=self.node.version, name=self.node.name)
             service.setup_runtime_attributes(
                 id=self.node.id,
                 version=version,
                 top_pipeline_id=top_pipeline_id,
                 root_pipeline_id=root_pipeline_id,
                 loop=loop,
                 inner_loop=inner_loop,
@@ -230,14 +229,15 @@
             try:
                 execute_success = service.execute(data=service_data, root_pipeline_data=root_pipeline_data)
             except Exception:
                 ENGINE_EXECUTE_EXCEPTION_COUNT.labels(type=node_type, hostname=self._hostname).inc()
                 ex_data = traceback.format_exc()
                 service_data.outputs.ex_data = ex_data
                 logger.warning("root_pipeline[%s]service execute fail: %s", process_info.root_pipeline_id, ex_data)
+                self.runtime.node_execute_fail(root_pipeline_id, self.node.id, ex_data=ex_data)
             logger.debug("root_pipeline[%s] service data after execute: %s", root_pipeline_id, service_data)
 
         if not execute_success:
             ENGINE_EXECUTE_FAILED_COUNT.labels(type=node_type, hostname=self._hostname).inc()
 
         with metrics.observe(
             metrics.ENGINE_NODE_EXECUTE_POST_PROCESS_DURATION, type=self.node.type.value, hostname=self._hostname
@@ -416,15 +416,15 @@
                 "root_pipeline[%s] node(%s) activity schedule data: %s, root inputs: %s",
                 root_pipeline_id,
                 self.node.id,
                 service_data,
                 root_pipeline_inputs,
             )
 
-            service = self.runtime.get_service(code=self.node.code, version=self.node.version)
+            service = self.runtime.get_service(code=self.node.code, version=self.node.version, name=self.node.name)
             service.setup_runtime_attributes(
                 id=self.node.id,
                 version=schedule.version,
                 top_pipeline_id=top_pipeline_id,
                 root_pipeline_id=root_pipeline_id,
                 loop=loop,
                 inner_loop=inner_loop,
@@ -452,14 +452,15 @@
                     data=service_data,
                     root_pipeline_data=root_pipeline_data,
                     callback_data=callback_data,
                 )
             except Exception:
                 ENGINE_SCHEDULE_EXCEPTION_COUNT.labels(type=node_type, hostname=self._hostname).inc()
                 service_data.outputs.ex_data = traceback.format_exc()
+                self.runtime.node_schedule_fail(root_pipeline_id, self.node.id, ex_data=traceback.format_exc())
             else:
                 is_schedule_done = service.is_schedule_done()
 
         if not schedule_success:
             ENGINE_SCHEDULE_FAILED_COUNT.labels(type=node_type, hostname=self._hostname).inc()
 
         with metrics.observe(
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/handlers/subprocess.py` & `bamboo-engine-2.8.0/bamboo_engine/handlers/subprocess.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/interrupt.py` & `bamboo-engine-2.8.0/bamboo_engine/interrupt.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/local.py` & `bamboo-engine-2.8.0/bamboo_engine/local.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/metrics.py` & `bamboo-engine-2.8.0/bamboo_engine/metrics.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/states.py` & `bamboo-engine-2.8.0/bamboo_engine/states.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/template/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/template/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/template/sandbox.py` & `bamboo-engine-2.8.0/bamboo_engine/template/sandbox.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/template/template.py` & `bamboo-engine-2.8.0/bamboo_engine/template/template.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/boolrule/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/boolrule/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/boolrule/boolrule.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/boolrule/boolrule.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/collections.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/collections.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/constants.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/object.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,12 @@
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
 
-from bamboo_engine.eri import ContextValueType
+class Representable:
+    def __str__(self):
+        return "<%s: %s>" % (self.__class__.__name__, self.__dict__)
 
-
-VAR_CONTEXT_MAPPING = {
-    "plain": ContextValueType.PLAIN,
-    "splice": ContextValueType.SPLICE,
-    "lazy": ContextValueType.COMPUTE,
-}
+    __repr__ = __str__
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/graph.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/graph.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/host.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/host.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/mako_safety.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/mako_safety.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/checker.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/checker.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/code_extract.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/code_extract.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/exceptions.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/mako_utils/visitors.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/mako_utils/visitors.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/utils/string.py` & `bamboo-engine-2.8.0/bamboo_engine/utils/string.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/validator/__init__.py` & `bamboo-engine-2.8.0/bamboo_engine/__version__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-from .api import validate_and_process_pipeline  # noqa
+__version__ = "2.8.0"
```

### Comparing `bamboo-engine-2.7.3/bamboo_engine/validator/api.py` & `bamboo-engine-2.8.0/bamboo_engine/validator/api.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/validator/connection.py` & `bamboo-engine-2.8.0/bamboo_engine/validator/connection.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/validator/gateway.py` & `bamboo-engine-2.8.0/bamboo_engine/validator/gateway.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/validator/rules.py` & `bamboo-engine-2.8.0/bamboo_engine/validator/rules.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/bamboo_engine/validator/utils.py` & `bamboo-engine-2.8.0/bamboo_engine/validator/utils.py`

 * *Files identical despite different names*

### Comparing `bamboo-engine-2.7.3/pyproject.toml` & `bamboo-engine-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bamboo-engine"
-version = "2.7.3"
+version = "2.8.0"
 description = "Bamboo-engine is a general-purpose workflow engine"
 authors = ["homholueng <homholueng@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">= 3.6, < 4"
 Werkzeug = "^1.0.0"
```

### Comparing `bamboo-engine-2.7.3/setup.py` & `bamboo-engine-2.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ['Mako>=1.1.4,<2.0.0',
  'Werkzeug>=1.0.0,<2.0.0',
  'prometheus-client>=0.9.0,<0.10.0',
  'pyparsing>=2.2.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'bamboo-engine',
-    'version': '2.7.3',
+    'version': '2.8.0',
     'description': 'Bamboo-engine is a general-purpose workflow engine',
     'long_description': 'None',
     'author': 'homholueng',
     'author_email': 'homholueng@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bamboo-engine-2.7.3/PKG-INFO` & `bamboo-engine-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamboo-engine
-Version: 2.7.3
+Version: 2.8.0
 Summary: Bamboo-engine is a general-purpose workflow engine
 License: MIT
 Author: homholueng
 Author-email: homholueng@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

