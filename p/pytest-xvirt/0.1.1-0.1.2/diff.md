# Comparing `tmp/pytest-xvirt-0.1.1.tar.gz` & `tmp/pytest-xvirt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/simone/Documents/python/pytest-xvirt/dist/.tmp-fix0k9ry/pytest-xvirt-0.1.1.tar", last modified: Sun Jun 18 16:28:31 2023, max compression
+gzip compressed data, was "/home/simone/Documents/python/pytest-xvirt/dist/.tmp-nhnm_wcq/pytest-xvirt-0.1.2.tar", last modified: Fri Jul 21 14:47:43 2023, max compression
```

## Comparing `pytest-xvirt-0.1.1.tar` & `pytest-xvirt-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/
--rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     2046 2023-04-02 16:47:36.000000 pytest-xvirt-0.1.1/README.rst
--rw-rw-r--   0 simone    (1000) simone    (1000)      236 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/setup.cfg
--rw-rw-r--   0 simone    (1000) simone    (1000)     1708 2023-06-18 16:28:27.000000 pytest-xvirt-0.1.1/setup.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/
--rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)      550 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       32 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/entry_points.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-15 17:04:00.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/not-zip-safe
--rw-rw-r--   0 simone    (1000) simone    (1000)       14 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       19 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/top_level.txt
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/xvirt/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-15 17:01:26.000000 pytest-xvirt-0.1.1/src/xvirt/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      561 2023-05-14 17:39:36.000000 pytest-xvirt-0.1.1/src/xvirt/collectors.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/src/xvirt/empty/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-15 18:10:34.000000 pytest-xvirt-0.1.1/src/xvirt/empty/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1520 2023-05-14 17:23:30.000000 pytest-xvirt-0.1.1/src/xvirt/events.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      361 2023-05-10 19:17:10.000000 pytest-xvirt-0.1.1/src/xvirt/newhooks.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2605 2023-05-14 17:35:10.000000 pytest-xvirt-0.1.1/src/xvirt/plugin.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-06-18 16:28:31.000000 pytest-xvirt-0.1.1/tests/
--rw-rw-r--   0 simone    (1000) simone    (1000)     1485 2023-05-21 16:30:01.000000 pytest-xvirt-0.1.1/tests/test_collectors.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      873 2023-06-17 14:59:06.000000 pytest-xvirt-0.1.1/tests/test_end2end.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1571 2023-05-14 17:35:41.000000 pytest-xvirt-0.1.1/tests/test_newhook_notify.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2414 2023-06-17 15:02:22.000000 pytest-xvirt-0.1.1/tests/test_newhook_setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2046 2023-04-02 16:47:36.000000 pytest-xvirt-0.1.2/README.rst
+-rw-rw-r--   0 simone    (1000) simone    (1000)      236 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/setup.cfg
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1708 2023-07-21 14:46:49.000000 pytest-xvirt-0.1.2/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3248 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)      578 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       32 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/entry_points.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2023-04-15 17:04:00.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/not-zip-safe
+-rw-rw-r--   0 simone    (1000) simone    (1000)       14 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       19 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/top_level.txt
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/xvirt/
+-rw-rw-r--   0 simone    (1000) simone    (1000)      547 2023-07-20 14:54:06.000000 pytest-xvirt-0.1.2/src/xvirt/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      561 2023-05-14 17:39:36.000000 pytest-xvirt-0.1.2/src/xvirt/collectors.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/src/xvirt/empty/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2023-04-15 18:10:34.000000 pytest-xvirt-0.1.2/src/xvirt/empty/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1520 2023-05-14 17:23:30.000000 pytest-xvirt-0.1.2/src/xvirt/events.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1181 2023-07-21 14:31:51.000000 pytest-xvirt-0.1.2/src/xvirt/events_handler.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      202 2023-07-20 15:12:59.000000 pytest-xvirt-0.1.2/src/xvirt/newhooks.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2912 2023-07-21 14:29:29.000000 pytest-xvirt-0.1.2/src/xvirt/plugin.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2023-07-21 14:47:43.000000 pytest-xvirt-0.1.2/tests/
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1485 2023-05-21 16:30:01.000000 pytest-xvirt-0.1.2/tests/test_collectors.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      962 2023-07-21 14:34:52.000000 pytest-xvirt-0.1.2/tests/test_end2end.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1662 2023-07-20 15:12:59.000000 pytest-xvirt-0.1.2/tests/test_newhook_notify.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1705 2023-07-20 15:01:53.000000 pytest-xvirt-0.1.2/tests/test_newhook_setup.py
```

### Comparing `pytest-xvirt-0.1.1/PKG-INFO` & `pytest-xvirt-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xvirt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pytest plugin to virtualize test. For example to transparently running them on a remote box.
 Home-page: https://github.com/www-py/pytest-xvirt
 Author: Simone Giacomelli, Fabrizio Lamarca
 Author-email: simone.giacomelli@gmail.com, lamarca.fabrizio@gmail.com
 Maintainer: Simone Giacomelli
 Maintainer-email: simone.giacomelli@gmail.com
 License: Apache 2.0
```

### Comparing `pytest-xvirt-0.1.1/README.rst` & `pytest-xvirt-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.1/setup.py` & `pytest-xvirt-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-xvirt',
-    version='0.1.1',
+    version='0.1.2',
     author='Simone Giacomelli, Fabrizio Lamarca',
     author_email='simone.giacomelli@gmail.com, lamarca.fabrizio@gmail.com',
     maintainer='Simone Giacomelli',
     maintainer_email='simone.giacomelli@gmail.com',
     license='Apache 2.0',
     url='https://github.com/www-py/pytest-xvirt',
     description='A pytest plugin to virtualize test. For example to transparently running them on a remote box.',
```

### Comparing `pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/PKG-INFO` & `pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xvirt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pytest plugin to virtualize test. For example to transparently running them on a remote box.
 Home-page: https://github.com/www-py/pytest-xvirt
 Author: Simone Giacomelli, Fabrizio Lamarca
 Author-email: simone.giacomelli@gmail.com, lamarca.fabrizio@gmail.com
 Maintainer: Simone Giacomelli
 Maintainer-email: simone.giacomelli@gmail.com
 License: Apache 2.0
```

### Comparing `pytest-xvirt-0.1.1/src/pytest_xvirt.egg-info/SOURCES.txt` & `pytest-xvirt-0.1.2/src/pytest_xvirt.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/pytest_xvirt.egg-info/entry_points.txt
 src/pytest_xvirt.egg-info/not-zip-safe
 src/pytest_xvirt.egg-info/requires.txt
 src/pytest_xvirt.egg-info/top_level.txt
 src/xvirt/__init__.py
 src/xvirt/collectors.py
 src/xvirt/events.py
+src/xvirt/events_handler.py
 src/xvirt/newhooks.py
 src/xvirt/plugin.py
 src/xvirt/empty/__init__.py
 tests/test_collectors.py
 tests/test_end2end.py
 tests/test_newhook_notify.py
 tests/test_newhook_setup.py
```

### Comparing `pytest-xvirt-0.1.1/src/xvirt/collectors.py` & `pytest-xvirt-0.1.2/src/xvirt/collectors.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.1/src/xvirt/events.py` & `pytest-xvirt-0.1.2/src/xvirt/events.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.1/src/xvirt/plugin.py` & `pytest-xvirt-0.1.2/src/xvirt/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 from pathlib import Path
+from typing import List
 
 import pytest
 
+from xvirt import events_handler, XVirt
+
 
 @pytest.hookimpl
 def pytest_addhooks(pluginmanager):
     from xvirt import newhooks
 
     pluginmanager.add_hookspecs(newhooks)
 
 
 @pytest.hookimpl(tryfirst=True)
 def pytest_configure(config) -> None:
+    config.pluginmanager.register(XvirtPluginRemote(config), "xvirt-plugin-remote")
     xvirt_packages = []
-    config.hook.pytest_xvirt_setup(config=config, xvirt_packages=xvirt_packages)
-    xvirt_package = ''
-    if len(xvirt_packages) == 1:
-        xvirt_package = xvirt_packages[0]
-        # config.option.xvirt_package = xvirt_package
-    elif len(xvirt_packages) > 1:
-        raise Exception('multiple packages not supported')
+    xvirt_instances: List[XVirt] = config.hook.pytest_xvirt_setup(config=config, xvirt_packages=xvirt_packages)
+    instances_count = len(xvirt_instances)
+    if instances_count == 0:
+        return
+    if instances_count != 1:
+        raise Exception('multiple xvirt users not supported')
 
-    config.pluginmanager.register(XvirtPlugin(config, xvirt_package), "xvirt-plugin")
+    xvirt_instance = xvirt_instances[0]
+    xvirt_package = xvirt_instance.remote_path()
+    config.pluginmanager.register(XvirtPlugin(xvirt_instance, config, xvirt_package), "xvirt-plugin-server")
 
 
-class XvirtPlugin:
+class XvirtPluginRemote:
 
-    def __init__(self, config, xvirt_package) -> None:
+    def __init__(self, config) -> None:
         self._config = config
-        self._xvirt_collect_file_done = False
-        self._xvirt_package = xvirt_package
 
     @pytest.hookimpl
     def pytest_runtest_logreport(self, report):
         if report.when != 'call':
             return
         config = self._config
         data = config.hook.pytest_report_to_serializable(config=config, report=report)
-        import json
-        data_json = json.dumps(data)
         from .events import EvtRuntestLogreport
         event = EvtRuntestLogreport(data)
-        config.hook.pytest_xvirt_notify(event=event, config=config)
+        config.hook.pytest_xvirt_send_event(event_json=event.to_json(), config=config)
+
+
+class XvirtPlugin:
+
+    def __init__(self, xvirt_instance: XVirt, config, xvirt_package) -> None:
+        self._xvirt_instance = xvirt_instance
+        self._config = config
+        self._xvirt_collect_file_done = False
+        self._xvirt_package = xvirt_package
 
     @pytest.hookimpl
     def pytest_pycollect_makemodule(self, module_path, path, parent):
         if self.is_xvirt_package(module_path.parent):
             empty = Path(__file__).parent / 'empty'
             return pytest.Module.from_parent(parent, fspath=empty)
 
@@ -56,26 +66,24 @@
             return None
 
         if self._xvirt_collect_file_done:
             return
 
         self._xvirt_collect_file_done = True
 
-        result = parent.config.hook.pytest_xvirt_collect_file(file_path=file_path, path=path, parent=parent)
-        if len(result) == 0:
-            return None
-        assert len(result) == 1
-        return result[0]
+        self._xvirt_instance.run()
+        evt_handler_fun = events_handler.make(file_path, parent)
+        return evt_handler_fun(self._xvirt_instance)
 
     def is_xvirt_package(self, path):
         if self._xvirt_package == '':
             return False
         str_path = str(path)
         return str_path.startswith(self._xvirt_package)
 
 
 @pytest.hookimpl
 def pytest_collection_finish(session: pytest.Session):
     # if session.config.option.xvirt_mode == mode_controlled:
     from .events import EvtCollectionFinish
     event = EvtCollectionFinish([item.nodeid for item in session.items])
-    session.config.hook.pytest_xvirt_notify(event=event, config=session.config)
+    session.config.hook.pytest_xvirt_send_event(event_json=event.to_json(), config=session.config)
```

### Comparing `pytest-xvirt-0.1.1/tests/test_collectors.py` & `pytest-xvirt-0.1.2/tests/test_collectors.py`

 * *Files identical despite different names*

### Comparing `pytest-xvirt-0.1.1/tests/test_end2end.py` & `pytest-xvirt-0.1.2/tests/test_end2end.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from pathlib import Path
 
 from pytest import Pytester
 
 from tests.find_port import find_port
-from tests.test_newhook_setup import _setup__pytest_xvirt_setup
 
 parent = Path(__file__).parent
 
 
 def test(pytester: Pytester):
     def read_text(filename): return (parent / filename).read_text()
 
     # GIVEN
-    foo = pytester.mkpydir('foo')
-    (foo / 'some_test.py').write_text('def test_1(): pass\ndef test_2(): pass\ndef test_3(): 1/0')
+    virt = pytester.mkpydir('foo')
+    (virt / 'some_test.py').write_text('def test_1(): pass\ndef test_2(): pass\ndef test_3(): 1/0')
 
     additional = read_text('end2end_support_server.py') \
+        .replace('##xvirt_package_marker##', str(virt)) \
+        .replace('##finalize_marker##', 'finalize_was_called') \
         .replace('##end2end_support_client_marker##', read_text('end2end_support_client.py')) \
         .replace('1234567890', str(find_port()))  # this replaces work on 2 inception levels: server&client
 
-    _setup__pytest_xvirt_setup(pytester, foo, additional=additional)
+    pytester.makeconftest(additional)
 
     # WHEN
     result = pytester.runpytest()
 
     # THEN
     result.assert_outcomes(passed=2, failed=1)
+
+    assert (virt.parent / 'finalize_was_called').exists()
```

### Comparing `pytest-xvirt-0.1.1/tests/test_newhook_notify.py` & `pytest-xvirt-0.1.2/tests/test_newhook_notify.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pytest import Pytester
 
 
 def test_newhook_xvirt_notify(pytester: Pytester) -> None:
     pytester.makeconftest(
         f"""
-        def pytest_xvirt_notify(event, config):
-
+        from xvirt.events import Evt
+        def pytest_xvirt_send_event(event_json, config):
+            event = Evt.from_json(event_json)
             from xvirt.events import EvtCollectionFinish
             if isinstance(event, EvtCollectionFinish): 
                 stripped_ids = [x.split('::')[1] for x in event.node_ids]
                 print('\\nHOOK1: ' + ', '.join(stripped_ids))
                 for x in event.node_ids:
                     print('XVIRT: ' + x)
```

### Comparing `pytest-xvirt-0.1.1/tests/test_newhook_setup.py` & `pytest-xvirt-0.1.2/tests/test_newhook_setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,61 +18,43 @@
     _setup__pytest_xvirt_setup(pytester, sub)
 
     (remote / 'some_test.py').write_text('def test_1(): pass\ndef test_2(): pass')
     (sub / 'sub_test.py').write_text('even no valid python')
     pytester.runpytest().assert_outcomes(passed=2)
 
 
-def test_xvirt_collect(pytester: Pytester):
-    foo = pytester.mkpydir('foo')
-
-    (foo / 'sub_test.py').write_text('even no valid python')
-
-    nodeids = ['m_test.py::test_a', 'm_test.py::test_b', 'm_test.py::test_c']
-    nodeids_json = json.dumps(nodeids)
-    _setup__pytest_xvirt_setup(pytester, foo, additional=f"""
-
-def pytest_xvirt_collect_file(file_path, path, parent):   
-    from xvirt.collectors import VirtCollector
-    result = VirtCollector.from_parent(parent, name=file_path.name)
-    result.nodeid_array = {nodeids_json}
-    return result
-    """)
-
-    result = pytester.runpytest('-v')
-    stdout_lines = '\n'.join(result.stdout.lines)
-
-    for nodeid in nodeids:
-        assert nodeid in stdout_lines
-
-    result.assert_outcomes(passed=3)
-
-
-def test_xvirt_collect_should_not_be_called(pytester: Pytester):
+def test_xvirt_run_should_not_be_called(pytester: Pytester):
     bar = pytester.mkpydir('bar')
     (bar / 'bar_test.py').write_text('def test_bar(): pass')
 
-    foo = pytester.mkpydir('foo')
-    (foo / 'sub_test.py').write_text('even no valid python')
+    virt = pytester.mkpydir('virt')
+    (virt / 'sub_test.py').write_text('even no valid python')
 
-    _setup__pytest_xvirt_setup(pytester, foo, additional=f"""
-def pytest_xvirt_collect_file(file_path, path, parent):   
-    assert 'this should not be executed' == ''
+    _setup__pytest_xvirt_setup(pytester, virt, additional=f"""
+    def run(self):   
+        assert 'this should not be executed' == ''
     """)
 
     result = pytester.runpytest(f'{bar}/')
     result.assert_outcomes(passed=1)
 
 
 def _setup__pytest_xvirt_setup(pytester, remote, additional=''):
     """
     Writes a conftest.py file with a pytest_xvirt_setup hook
     :param remote: defines the remote path to be added to xvirt_packages
     :param additional: Additional conftest.py content
     """
     remote_str = str(remote)
-    content = f"""            
-def pytest_xvirt_setup(config, xvirt_packages):
-    xvirt_packages.append('{remote_str}')
+    content = f"""    
+from xvirt import XVirt
+
+def pytest_xvirt_setup(config):
+    return XvirtTest1()
+        
+class XvirtTest1(XVirt):
+
+    def remote_path(self) -> str:
+        return '{remote_str}'
     
 {additional}"""
     pytester.makeconftest(content)
```

