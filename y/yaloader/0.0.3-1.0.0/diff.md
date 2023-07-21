# Comparing `tmp/yaloader-0.0.3.tar.gz` & `tmp/yaloader-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaloader-0.0.3.tar", last modified: Thu May  5 12:57:17 2022, max compression
+gzip compressed data, was "yaloader-1.0.0.tar", last modified: Fri Jul 21 09:43:21 2023, max compression
```

## Comparing `yaloader-0.0.3.tar` & `yaloader-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,30 @@
-drwxr-xr-x   0 work      (1001) work      (1001)        0 2022-05-05 12:57:17.881145 yaloader-0.0.3/
--rw-r--r--   0 work      (1001) work      (1001)    34523 2020-11-16 09:49:42.000000 yaloader-0.0.3/LICENSE.txt
--rw-r--r--   0 work      (1001) work      (1001)      761 2022-05-05 12:57:17.881145 yaloader-0.0.3/PKG-INFO
--rw-r--r--   0 work      (1001) work      (1001)      108 2022-02-03 12:30:34.000000 yaloader-0.0.3/README.md
--rw-r--r--   0 work      (1001) work      (1001)      104 2022-01-30 16:28:49.000000 yaloader-0.0.3/pyproject.toml
--rw-r--r--   0 work      (1001) work      (1001)      876 2022-05-05 12:57:17.884478 yaloader-0.0.3/setup.cfg
-drwxr-xr-x   0 work      (1001) work      (1001)        0 2022-05-05 12:57:17.881145 yaloader-0.0.3/src/
-drwxr-xr-x   0 work      (1001) work      (1001)        0 2022-05-05 12:57:17.881145 yaloader-0.0.3/src/yaloader/
--rw-r--r--   0 work      (1001) work      (1001)      355 2022-05-05 12:52:09.000000 yaloader-0.0.3/src/yaloader/__init__.py
--rw-r--r--   0 work      (1001) work      (1001)    26605 2022-05-05 12:47:49.000000 yaloader-0.0.3/src/yaloader/main.py
--rw-r--r--   0 work      (1001) work      (1001)     1904 2022-02-03 10:10:53.000000 yaloader-0.0.3/src/yaloader/utils.py
-drwxr-xr-x   0 work      (1001) work      (1001)        0 2022-05-05 12:57:17.881145 yaloader-0.0.3/src/yaloader.egg-info/
--rw-r--r--   0 work      (1001) work      (1001)      761 2022-05-05 12:57:17.000000 yaloader-0.0.3/src/yaloader.egg-info/PKG-INFO
--rw-r--r--   0 work      (1001) work      (1001)      293 2022-05-05 12:57:17.000000 yaloader-0.0.3/src/yaloader.egg-info/SOURCES.txt
--rw-r--r--   0 work      (1001) work      (1001)        1 2022-05-05 12:57:17.000000 yaloader-0.0.3/src/yaloader.egg-info/dependency_links.txt
--rw-r--r--   0 work      (1001) work      (1001)      124 2022-05-05 12:57:17.000000 yaloader-0.0.3/src/yaloader.egg-info/requires.txt
--rw-r--r--   0 work      (1001) work      (1001)        9 2022-05-05 12:57:17.000000 yaloader-0.0.3/src/yaloader.egg-info/top_level.txt
+drwxr-xr-x   0 work      (1001) work      (1001)        0 2023-07-21 09:43:21.128922 yaloader-1.0.0/
+-rw-r--r--   0 work      (1001) work      (1001)    34523 2023-05-05 08:11:37.000000 yaloader-1.0.0/LICENSE.txt
+-rw-r--r--   0 work      (1001) work      (1001)      742 2023-07-21 09:43:21.128922 yaloader-1.0.0/PKG-INFO
+-rw-r--r--   0 work      (1001) work      (1001)      108 2023-05-05 08:11:37.000000 yaloader-1.0.0/README.md
+-rw-r--r--   0 work      (1001) work      (1001)      104 2023-07-19 15:15:27.000000 yaloader-1.0.0/pyproject.toml
+-rw-r--r--   0 work      (1001) work      (1001)      883 2023-07-21 09:43:21.128922 yaloader-1.0.0/setup.cfg
+drwxr-xr-x   0 work      (1001) work      (1001)        0 2023-07-21 09:43:21.125922 yaloader-1.0.0/src/
+drwxr-xr-x   0 work      (1001) work      (1001)        0 2023-07-21 09:43:21.127922 yaloader-1.0.0/src/yaloader/
+-rw-r--r--   0 work      (1001) work      (1001)     1132 2023-07-21 09:42:59.000000 yaloader-1.0.0/src/yaloader/__init__.py
+-rw-r--r--   0 work      (1001) work      (1001)     3606 2023-07-21 09:42:59.000000 yaloader-1.0.0/src/yaloader/base_config.py
+-rw-r--r--   0 work      (1001) work      (1001)    15503 2023-07-21 09:42:59.000000 yaloader-1.0.0/src/yaloader/config_loader.py
+-rw-r--r--   0 work      (1001) work      (1001)     6424 2023-07-21 09:42:59.000000 yaloader-1.0.0/src/yaloader/constructor.py
+-rw-r--r--   0 work      (1001) work      (1001)      497 2023-07-21 09:42:59.000000 yaloader-1.0.0/src/yaloader/dumper.py
+-rw-r--r--   0 work      (1001) work      (1001)     3269 2023-07-21 09:42:59.000000 yaloader-1.0.0/src/yaloader/loader.py
+-rw-r--r--   0 work      (1001) work      (1001)     1836 2023-07-21 09:42:59.000000 yaloader-1.0.0/src/yaloader/representer.py
+-rw-r--r--   0 work      (1001) work      (1001)      925 2023-07-21 09:42:59.000000 yaloader-1.0.0/src/yaloader/utils.py
+drwxr-xr-x   0 work      (1001) work      (1001)        0 2023-07-21 09:43:21.127922 yaloader-1.0.0/src/yaloader.egg-info/
+-rw-r--r--   0 work      (1001) work      (1001)      742 2023-07-21 09:43:21.000000 yaloader-1.0.0/src/yaloader.egg-info/PKG-INFO
+-rw-r--r--   0 work      (1001) work      (1001)      633 2023-07-21 09:43:21.000000 yaloader-1.0.0/src/yaloader.egg-info/SOURCES.txt
+-rw-r--r--   0 work      (1001) work      (1001)        1 2023-07-21 09:43:21.000000 yaloader-1.0.0/src/yaloader.egg-info/dependency_links.txt
+-rw-r--r--   0 work      (1001) work      (1001)      129 2023-07-21 09:43:21.000000 yaloader-1.0.0/src/yaloader.egg-info/requires.txt
+-rw-r--r--   0 work      (1001) work      (1001)        9 2023-07-21 09:43:21.000000 yaloader-1.0.0/src/yaloader.egg-info/top_level.txt
+drwxr-xr-x   0 work      (1001) work      (1001)        0 2023-07-21 09:43:21.128922 yaloader-1.0.0/tests/
+-rw-r--r--   0 work      (1001) work      (1001)     2900 2023-07-21 09:42:59.000000 yaloader-1.0.0/tests/test_caching.py
+-rw-r--r--   0 work      (1001) work      (1001)     2455 2023-07-21 09:42:59.000000 yaloader-1.0.0/tests/test_config_class.py
+-rw-r--r--   0 work      (1001) work      (1001)     5084 2023-07-21 09:42:59.000000 yaloader-1.0.0/tests/test_config_variables.py
+-rw-r--r--   0 work      (1001) work      (1001)     1534 2023-07-21 09:42:59.000000 yaloader-1.0.0/tests/test_construct_from_string.py
+-rw-r--r--   0 work      (1001) work      (1001)      718 2023-05-05 08:11:37.000000 yaloader-1.0.0/tests/test_file_load.py
+-rw-r--r--   0 work      (1001) work      (1001)      911 2023-07-21 09:42:59.000000 yaloader-1.0.0/tests/test_loads_decorator.py
+-rw-r--r--   0 work      (1001) work      (1001)     1616 2023-07-21 09:42:59.000000 yaloader-1.0.0/tests/test_overwriting_tags.py
```

### Comparing `yaloader-0.0.3/LICENSE.txt` & `yaloader-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yaloader-0.0.3/PKG-INFO` & `yaloader-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: yaloader
-Version: 0.0.3
+Version: 1.0.0
 Summary: A package loading class configurations from yaml files
 Home-page: https://github.com/DominikMa/yaloader
 Author: Dominik Mairhöfer
 Author-email: dominik@mairhoefer.xyz
 License: GNU AGPLv3
 Project-URL: Documentation, https://yaloader.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/DominikMa/yaloader/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE.txt
 
 # YaLoader - A YAML Configuration Loader
 
 The documentation will be [here](https://yaloader.readthedocs.io).
-
```

### Comparing `yaloader-0.0.3/setup.cfg` & `yaloader-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [options]
 package_dir = 
 	=src
 packages = 
 	yaloader
 python_requires = >=3.9
 install_requires = 
-	pydantic
+	pydantic >= 2.0
 	pyyaml
 
 [options.extras_require]
 docs = 
 	sphinx
 	jupyter-server
 	myst-nb
```

### Comparing `yaloader-0.0.3/src/yaloader/main.py` & `yaloader-1.0.0/src/yaloader/config_loader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,473 +1,264 @@
 from __future__ import annotations
 
 import datetime
-import functools
 import logging
-import textwrap
-import warnings
 from inspect import isclass
-from pathlib import PosixPath, WindowsPath, Path
-from typing import Dict, Tuple, Set, Iterator, Type, Union, List, Optional, Any, Callable
+from pathlib import PosixPath, Path
+from typing import Type, Dict, List, Any, Tuple, Set, Iterator, Union, Optional
 
 import yaml
-from pydantic import BaseModel, ValidationError, conint
-from pydantic.main import ModelMetaclass
-from yaml import MarkedYAMLError
+from pydantic import BaseModel, conint
 from yaml.constructor import ConstructorError
 from yaml.parser import ParserError
 
-from yaloader.utils import full_object_name, remove_missing_errors
+from yaloader import YAMLBaseConfig, YAMLConfigLoader, get_multi_constructor_for_vars, VarYAMLConfigBase
 
 logger = logging.getLogger(__name__)
 
 
-class YAMLValueError(MarkedYAMLError):
-    """Error of wrong values in the loaded yaml configs."""
-    pass
-
-
-class YAMLConfigLoader(yaml.SafeLoader):
-    """YAML loader for the configs."""
-    yaml_config_classes: Dict[str, Type[YAMLBaseConfig]] = {}
-
-    @classmethod
-    def add_config_constructor(cls, config_class: Type[YAMLBaseConfig],
-                               constructor, overwrite_tag: bool = False) -> None:
-        """Add a yaml config class with its constructor to the loader.
-
-        :param config_class: The config which should be added to the loader.
-        :param constructor: The constructor to load the class.
-        :param overwrite_tag: If true and an other config with the same tag is already registered
-                              the previous config for the same tag is overwritten.
-                              Else a RuntimeError is raised if the tag of the config is already registered.
-        :return:
-        """
-        tag = config_class.get_yaml_tag()
-        if tag.startswith('!!'):
-            raise RuntimeError(
-                f"The tag {tag} has the prefix !! and can therefore not be used by {full_object_name(config_class)}. "
-                f"Choose another tag for the yaml config class."
-            )
-
-        if tag in cls.yaml_constructors.keys():
-            # If tag is not in the registered yaml config classes,
-            # it is a tag of the SafeLoader and should not be overwritten.
-            if tag not in cls.yaml_config_classes:
-                raise RuntimeError(
-                    f"The tag {tag} is already registered and can not be used by {full_object_name(config_class)}. "
-                    f"Choose another tag for the yaml config class."
-                )
-
-            if not overwrite_tag:
-                raise RuntimeError(
-                    f"The tag {tag} is already registered by {full_object_name(cls.yaml_config_classes[tag])} "
-                    f"and can therefore not be used by {full_object_name(config_class)}. "
-                    f"Set overwrite_tag to True if you want to overwrite the existing tag "
-                    f"or choose another tag for one of the yaml config classes."
-                )
-            # Overwrite existing tag, while keeping is under a different tag.
-            old_constructor = cls.yaml_constructors[tag]
-            del cls.yaml_constructors[tag]
-            old_config_class = cls.yaml_config_classes[tag]
-            del cls.yaml_config_classes[tag]
-
-            old_config_class.set_yaml_tag(f"!{full_object_name(old_config_class)}")
-            cls.add_config_constructor(old_config_class, old_constructor)
-
-        cls.add_constructor(tag, constructor)
-
-        # TODO: Not quite sure if this makes sense. Copied from the original yaml loader.
-        if 'yaml_config_classes' not in cls.__dict__:
-            cls.yaml_config_classes = cls.yaml_config_classes.copy()
-        cls.yaml_config_classes[tag] = config_class
-
-
-class YAMLConfigDumper(yaml.SafeDumper):
-    """YAML dumper for the configs."""
-    exclude_unset: bool = True
-    """If True exclude all unset values when dumping the config. 
-    See https://pydantic-docs.helpmanual.io/usage/exporting_models/ for details."""
-    exclude_defaults: bool = True
-    """If True exclude all default values when dumping the config.
-    See https://pydantic-docs.helpmanual.io/usage/exporting_models/ for details."""
-
-
-def representer_posix_path(dumper: YAMLConfigDumper, data: PosixPath):
-    return dumper.represent_str(str(data.absolute()))
-
-
-def representer_windows_path(dumper: YAMLConfigDumper, data: WindowsPath):
-    return dumper.represent_str(str(data.absolute()))
-
-
-def representer_timedelta(dumper: YAMLConfigDumper, data: datetime.timedelta):
-    return dumper.represent_str(str(data))
-
-
-def representer_base_model(dumper: YAMLConfigDumper, data: BaseModel):
-    return dumper.represent_dict(data.dict())
-
-
-yaml.add_representer(PosixPath, representer_posix_path, Dumper=YAMLConfigDumper)
-yaml.add_representer(WindowsPath, representer_windows_path, Dumper=YAMLConfigDumper)
-yaml.add_representer(datetime.timedelta, representer_timedelta, Dumper=YAMLConfigDumper)
-yaml.add_multi_representer(BaseModel, representer_base_model, Dumper=YAMLConfigDumper)
-
-
-class YAMLConfigMetaclass(ModelMetaclass):
-    """Metaclass for the BaseConfig to automagically add constructor and representer to the loader and dumper."""
-
-    def __init__(cls: Type[YAMLBaseConfig], name, bases, attrs,
-                 loaded_class: Optional[Type] = None, overwrite_tag: bool = False,
-                 yaml_loader: Type[YAMLConfigLoader] = YAMLConfigLoader,
-                 yaml_dumper: Type[YAMLConfigDumper] = YAMLConfigDumper,
-                 **kwargs):
-        cls: Type[YAMLBaseConfig]  # For the IDE
-        super(YAMLConfigMetaclass, cls).__init__(name, bases, attrs, **kwargs)
-
-        # If there is an explict yaml tag given use it
-        if '_yaml_tag' in attrs:
-            cls.set_yaml_tag(attrs['_yaml_tag'])
-
-        # Set the _loaded_class attribute
-        if loaded_class is not None:
-            setattr(cls, "_loaded_class", loaded_class)
-
-        def constructor(loader: YAMLConfigLoader, node: yaml.MappingNode) -> YAMLBaseConfig:
-            """Construct the config object from a mapping."""
-            if not isinstance(node, yaml.MappingNode):
-                raise ParserError(f"While parsing the configuration for the tag {node.tag}", node.start_mark,
-                                  f"expected a mapping node, but found {node.id}")
-            # Get the mapping in a dictionary
-            mapping = loader.construct_mapping(node, deep=True)
-            # Construct an object of this config class WITHOUT validating the inputs
-            config_instance: YAMLBaseConfig = cls.construct(**mapping)
-            # Validate the inputs, but ignore missing errors
-            try:
-                cls.validate_config(config_instance, force_all=False)
-            except ValidationError as e:
-                raise YAMLValueError(f"Could not validate the configuration for the tag {node.tag}", node.start_mark,
-                                     textwrap.indent(str(e), 2 * ' '))
-            return config_instance
-
-        yaml_loader.add_config_constructor(cls, constructor, overwrite_tag=overwrite_tag)
-
-        def representer(dumper: YAMLConfigDumper, data: YAMLBaseConfig):
-            """Represent the config object as a mapping."""
-            # Get all keys which should be dumped
-            keys = set(data.dict(exclude_unset=dumper.exclude_unset, exclude_defaults=dumper.exclude_defaults).keys())
-
-            # Just for sorting the output:
-            # Get keys of iteration types
-            it_keys = set(filter(lambda k: isinstance(getattr(data, k), (list, tuple, dict)), keys))
-            keys = keys.difference(it_keys)
-
-            # Get keys of BaseConfig type
-            config_objects_keys = set(filter(lambda key: isinstance(getattr(data, key), YAMLBaseConfig), keys))
-            keys = keys.difference(config_objects_keys)
-
-            dump_dict = {k: getattr(data, k) for k in sorted(keys) + sorted(it_keys) + sorted(config_objects_keys)}
-            return dumper.represent_mapping(
-                cls.get_yaml_tag(),
-                dump_dict
-            )
-
-        yaml_dumper.add_representer(cls, representer)
-
-
-def loads(loaded_class: Type) -> Callable[[Type[YAMLBaseConfig]], Type[YAMLBaseConfig]]:
-    """A class decorator for yaml configs to add a simple load function for a given class.
-
-    A load function, which gets all attributes of the config
-    and creates an instance of the given class with them as key word arguments,
-    is added to the config.
-
-    :param loaded_class: The class which should be loaded by this
-    :return: The class decorator
-    """
-    warnings.warn('The loads decorator will be deprecated. '
-                  'Use the Metaclass argument loaded_class instead.', DeprecationWarning, stacklevel=2)
-
-    def decorate(cls: Type[YAMLBaseConfig]):
-        @functools.wraps(cls.load)
-        def load(self, *args, **kwargs):
-            return loaded_class(**dict(self))
-
-        setattr(cls, 'load', load)
-        return cls
-    return decorate
-
-
-class YAMLBaseConfig(BaseModel, metaclass=YAMLConfigMetaclass):
-    """The base class for all config objects which are loaded from or dumped to yaml files.
-
-    Each config from which an actual object can be created has to implement
-    the :meth:`YAMLBaseConfig.load()` method.
-    """
-    _loaded_class: Optional[Type] = None
-    """The class which is loaded by the configuration. 
-    Can be None if the loaded class is explicitly specified in the load method."""
-
-    class Config:
-        """Since yaml configs are used to create instances extra fields are forbidden."""
-        extra = 'forbid'
-        validate_assignment = True
-
-    @classmethod
-    def get_yaml_tag(cls) -> str:
-        """Return the configs yaml tag."""
-        cls._assure_has_yaml_tag()
-        return getattr(cls, f"_{cls.__name__}__yaml_tag", None)
-
-    @classmethod
-    def set_yaml_tag(cls, yaml_tag: Optional[str]) -> None:
-        """Set the yaml tag of the config.
-
-        A valid tag has to start with an exclamation mark.
-
-        :param yaml_tag: Optional string of the tag. If None the tag will be set to a default value.
-        """
-        setattr(cls, f"_{cls.__name__}__yaml_tag", yaml_tag)
-        cls._assure_has_yaml_tag()
-
-    @classmethod
-    def _assure_has_yaml_tag(cls) -> None:
-        """ Assert that the config has a valid yaml tag.
-
-        If the tag is not set yet, try to set it to a default value.
-        """
-        yaml_tag = getattr(cls, f"_{cls.__name__}__yaml_tag", None)
-        if yaml_tag is None or not isinstance(yaml_tag, str):
-            # Set yaml tag to default case: class name without `Config` suffix
-            class_name = cls.__name__
-            if not class_name.endswith("Config"):
-                raise RuntimeError(f"Config class {cls.__name__} has not yaml tag. "
-                                   f"If the tag should be derived automatically the "
-                                   f"class name has to end with `Config`")
-            class_name = class_name.removesuffix("Config")
-            yaml_tag = f"!{class_name}"
-        elif not yaml_tag.startswith("!"):
-            raise RuntimeError(f"The tag of config class {full_object_name(cls)} does not start with !")
-        setattr(cls, f"_{cls.__name__}__yaml_tag", yaml_tag)
-
-    def validate_config(self, force_all: bool = False) -> None:
-        """Validate a BaseConfig instance
-
-        If force_all is False do not raise an error on missing attributes.
-        Configs have to be correct but may be incomplete.
-
-        :param force_all: If True raise an error on missing attributes
-        """
-        try:
-            self.validate(dict(self))
-        except ValidationError as e:
-            if force_all:
-                raise
-            not_missing_errors = remove_missing_errors(e.raw_errors)
-            if len(not_missing_errors) > 0:
-                raise ValidationError(not_missing_errors, model=e.model)
-
-    def load(self, *args, **kwargs):
-        """Create the object the yaml config object is for.
-
-        This basic constructor uses all attributes of the config as kwargs for the loaded class.
-        """
-        if hasattr(self, '_loaded_class') and self._loaded_class is not None:
-            return self._loaded_class(**dict(self))
-        raise NotImplementedError
-
-    def __init_subclass__(cls, **kwargs):
-        if 'loaded_class' in kwargs:
-            kwargs.pop('loaded_class')
-        if 'overwrite_tag' in kwargs:
-            kwargs.pop('overwrite_tag')
-        if 'yaml_loader' in kwargs:
-            kwargs.pop('yaml_loader')
-        if 'yaml_dumper' in kwargs:
-            kwargs.pop('yaml_dumper')
-        super().__init_subclass__(**kwargs)
-
-
 class ConfigWithPriority(BaseModel):
     """Keep a loaded yaml config class together with its priority."""
+
     config: YAMLBaseConfig
     priority: conint(ge=0, le=100) = 0
 
 
 class ConfigLoader:
     """The loader which will keep track of all loaded yaml configs."""
 
-    def __init__(self, yaml_loader: Type[YAMLConfigLoader] = YAMLConfigLoader):
+    def __init__(self, yaml_loader: Type[YAMLConfigLoader] = YAMLConfigLoader, cacheing: bool = True):
         self.yaml_loader = yaml_loader
+        self.yaml_loader.add_multi_constructor(
+            tag_prefix="!ConfigVar",
+            multi_constructor=get_multi_constructor_for_vars(yaml_loader),
+        )
 
         # All loaded yaml configs with their priorities per tag
         self.configs_per_tag: Dict[str, List[ConfigWithPriority]] = {}
 
-    def deep_construct_from_config(self, config: Any, final: bool = False, auto_load: bool = False) -> Any:
+        self.cacheing = cacheing
+        self.cache = None if not cacheing else {}
+
+    def deep_construct_from_config(
+            self, config: YAMLBaseConfig, final: bool = False, auto_load: bool = False
+    ) -> Any:
         """Deeply construct the config based on a config object.
 
         :param config: The config which should be constructed
         :param final: If False missing values will be ignored
         :param auto_load: If True automatically call the :meth:`YAMLBaseConfig.load()` method on the loaded config
         :return: The constructed config
         """
-        if not isinstance(config, YAMLBaseConfig):
-            return self._deep_construct(config, final=final, auto_load=auto_load)
-        config: YAMLBaseConfig
         # Construct only the flat object
         config = self.flat_construct_from_config(config)
 
         # Deep construct every attribute
         for key, v in dict(config).items():
-            v = self._deep_construct(v, final=final, auto_load=auto_load)
+            v = self.deep_construct(v, final=final, auto_load=auto_load)
             setattr(config, key, v)
 
         # Ensure that the config is still correct (and complete if final is True)
         config.validate_config(force_all=final)
         if auto_load:
             return config.load()
         return config
 
-    def _deep_construct(self, v: Any, final: bool = False, auto_load: bool = False) -> Any:
+    def deep_construct(
+            self, v: Any, final: bool = False, auto_load: bool = False
+    ) -> Any:
         # If v is another config just recursive call deep construct
         if isinstance(v, YAMLBaseConfig):
             return self.deep_construct_from_config(v, final=final, auto_load=auto_load)
         # If v is a list, tuple or dict recursively call this method for every item
         elif isinstance(v, List):
-            return list([self._deep_construct(e, final=final, auto_load=auto_load) for e in v])
+            return list(
+                [self.deep_construct(e, final=final, auto_load=auto_load) for e in v]
+            )
         elif isinstance(v, Tuple):
-            return tuple((self._deep_construct(e, final=final, auto_load=auto_load) for e in v))
+            return tuple(
+                (self.deep_construct(e, final=final, auto_load=auto_load) for e in v)
+            )
         elif isinstance(v, Dict):
-            return {k: self._deep_construct(e, final=final, auto_load=auto_load) for k, e in v.items()}
+            return {
+                k: self.deep_construct(e, final=final, auto_load=auto_load)
+                for k, e in v.items()
+            }
         # If v is an unhandled type log a warning and return v itself
-        elif v is not None and not isinstance(v, (
-                int, float, str,
-                PosixPath,
-                datetime.timedelta, datetime.datetime
-        )):
-            logger.warning(f'Got type {type(v)} while deep construct of a yaml config which is not explicitly handled.')
+        elif v is not None and not isinstance(
+                v, (int, float, str, PosixPath, datetime.timedelta, datetime.datetime)
+        ):
+            logger.warning(
+                f"Got type {type(v)} while deep construct of a yaml config which is not explicitly handled."
+            )
         return v
 
     def flat_construct_from_config(self, config: YAMLBaseConfig) -> YAMLBaseConfig:
         """Construct the config based on a config object.
 
         :param config: The config which should be constructed
         :return: The constructed config
         """
         # Construct flat object from loaded configs
         tag_config = self.flat_construct_from_tag(config.get_yaml_tag())
 
         # Get the not explict configs attributes
         not_explict_config_attributes = {}
-        self.update_config_attributes(not_explict_config_attributes, [tag_config, config], explicit=False)
+        self.update_config_attributes(
+            not_explict_config_attributes, [tag_config, config], explicit=False
+        )
 
         # Get the explict configs attributes
         explicit_configs_attributes = {}
-        self.update_config_attributes(explicit_configs_attributes, [tag_config, config], explicit=True)
+        self.update_config_attributes(
+            explicit_configs_attributes, [tag_config, config], explicit=True
+        )
 
         # Update object from loaded config attributes with not explict and explict configs
         config_attributes = {}
         config_attributes.update(not_explict_config_attributes)
         config_attributes.update(explicit_configs_attributes)
-        constructed_config = config.construct(_fields_set=set(explicit_configs_attributes.keys()), **config_attributes)
+
+        # If the config is a variable construct using the base class
+        config_cls = tag_config.__class__
+        while issubclass(config_cls, VarYAMLConfigBase):
+            config_cls = config_cls.__base__
+
+        constructed_config = config_cls.model_construct(
+            _fields_set=set(explicit_configs_attributes.keys()), **config_attributes
+        )
 
         constructed_config.validate_config(force_all=False)
         return constructed_config
 
     def flat_construct_from_tag(self, tag: str) -> YAMLBaseConfig:
         """Construct the config for a tag.
 
-        This is not deep. If the config contains an other config the included one is NOT constructed!
+        This is not deep. If the config contains another config the included one is NOT constructed!
 
         This includes inheritance as following:
             - explict set fields go over not explict set fields
             - local field go over inherited fields
             - inherited explict field goes over local not explict field
             - if there are multiple base classes the most left is most important
             - for multiple yaml configs high priority goes over low priority
             - for multiple yaml configs with same priority order matters
 
         :param tag: The tag of the config which should be constructed
         :return: The constructed config
         """
+        if self.cacheing and tag in self.cache:
+            return self.cache[tag].model_copy()
         try:
-            default_config = self.yaml_loader.yaml_config_classes[tag].construct()
+            default_config = self.yaml_loader.yaml_config_classes[tag].model_construct()
         except KeyError as e:
-            raise RuntimeError(f"Can not load configs for {tag}! "
-                               f"It seems that no config is registered for that tag.") from e
-
-        configs_with_priority_for_tag = [ConfigWithPriority(config=default_config, priority=0)]
+            raise RuntimeError(
+                f"Can not load configs for {tag}! "
+                f"It seems that no config is registered for that tag."
+            ) from e
+
+        configs_with_priority_for_tag = [
+            ConfigWithPriority(config=default_config, priority=0)
+        ]
         configs_with_priority_for_tag += self.configs_per_tag.get(tag, [])
 
         # Sort pairs by priority (lowest first) and get the config
-        configs_with_priority_for_tag.sort(key=lambda configs_with_priority: configs_with_priority.priority)
-        configs_objects: List[YAMLBaseConfig] = list(map(lambda y: y.config, configs_with_priority_for_tag))
+        configs_with_priority_for_tag.sort(
+            key=lambda configs_with_priority: configs_with_priority.priority
+        )
+        configs_objects: List[YAMLBaseConfig] = list(
+            map(lambda y: y.config, configs_with_priority_for_tag)
+        )
 
         # Get the class of the config, make sure it is exactly one
-        configs_object_classes: Set[Type[YAMLBaseConfig]] = set(map(lambda o: o.__class__, configs_objects))
+        configs_object_classes: Set[Type[YAMLBaseConfig]] = set(
+            map(lambda o: o.__class__, configs_objects)
+        )
         if len(configs_object_classes) != 1:
-            raise RuntimeError(f"In the configs for the tag {tag} is more than one class.")
+            raise RuntimeError(
+                f"In the configs for the tag {tag} is more than one class."
+            )
         config_object_class = configs_object_classes.pop()
 
         # Get all config classes which it inherits from
         # noinspection PyTypeChecker
-        config_class_bases: Iterator[Type[YAMLBaseConfig]] = filter(lambda x: (isclass(x) and
-                                                                               issubclass(x, YAMLBaseConfig) and
-                                                                               not x == YAMLBaseConfig),
-                                                                    config_object_class.__bases__)
+        config_class_bases: Iterator[Type[YAMLBaseConfig]] = filter(
+            lambda x: (
+                    isclass(x) and issubclass(x, YAMLBaseConfig) and not x == YAMLBaseConfig
+            ),
+            config_object_class.__bases__,
+        )
 
-        # Construct all bases, in reversed order (first base has highest priority and should be at end of the list)
+        # Construct all bases, in reversed order (first base has the highest priority and should be at end of the list)
         # Construction MUST BE flat. Otherwise there might be circles.
-        constructed_config_bases: List[YAMLBaseConfig] = list(map(
-            lambda config_base: self.flat_construct_from_tag(config_base.get_yaml_tag()),
-            config_class_bases)
+        constructed_config_bases: List[YAMLBaseConfig] = list(
+            map(
+                lambda config_base: self.flat_construct_from_tag(
+                    config_base.get_yaml_tag()
+                ),
+                config_class_bases,
+            )
         )
         constructed_config_bases.reverse()
 
         # Construct not explict set config attributes
         not_explict_config_attributes = {}
         # Add all not explict set fields from the bases, starting with the most right base to left base
-        self.update_config_attributes(not_explict_config_attributes, constructed_config_bases, explicit=False)
+        self.update_config_attributes(
+            not_explict_config_attributes, constructed_config_bases, explicit=False
+        )
         # Add all not explict set fields from the loaded configs, starting with the lowest priority to the highest
-        self.update_config_attributes(not_explict_config_attributes, configs_objects, explicit=False)
+        self.update_config_attributes(
+            not_explict_config_attributes, configs_objects, explicit=False
+        )
 
         # Construct explict set config attributes
         explicit_config_attributes = {}
         # Add all explict set fields from the bases, starting with the most right base to left base
-        self.update_config_attributes(explicit_config_attributes, constructed_config_bases, explicit=True)
+        self.update_config_attributes(
+            explicit_config_attributes, constructed_config_bases, explicit=True
+        )
         # Add all explict set fields from the loaded configs, starting with the lowest priority to the highest
-        self.update_config_attributes(explicit_config_attributes, configs_objects, explicit=True)
+        self.update_config_attributes(
+            explicit_config_attributes, configs_objects, explicit=True
+        )
 
         # Overwrite not explict config attributes with explict ones
         config_attributes = {}
         config_attributes.update(not_explict_config_attributes)
         config_attributes.update(explicit_config_attributes)
         # Construct config object, set only fields from `explicit_config_attributes` to explict
-        constructed_config = config_object_class.construct(_fields_set=set(explicit_config_attributes.keys()),
-                                                           **config_attributes)
+        constructed_config = config_object_class.model_construct(
+            _fields_set=set(explicit_config_attributes.keys()), **config_attributes
+        )
 
         # Validate, but do not force all. Some base class might be not complete (and it don't has to)
         constructed_config.validate_config(force_all=False)
-        return constructed_config
+
+        if self.cacheing:
+            self.cache[tag] = constructed_config
+        return constructed_config.model_copy()
 
     @staticmethod
-    def update_config_attributes(config_attributes: dict, config_updates: List[YAMLBaseConfig], explicit: bool) -> None:
+    def update_config_attributes(
+            config_attributes: dict, config_updates: List[YAMLBaseConfig], explicit: bool
+    ) -> None:
         """Add config attributes from update configs to the current config attributes.
 
         If the field already exists overwrite it. So `config_updates` are lowest priority first.
 
         :param config_attributes: Dict of existing attributes of the config
         :param config_updates: List of configs from which the attributes should be updated
         :param explicit: If True use only explicit attributes. Else use only not explicit ones.
         """
         for update in config_updates:
             update_dict = dict(update)
-            fields = filter(lambda f: (f in update.__fields_set__) == explicit,
-                            update_dict.keys())
+            fields = filter(
+                lambda f: (f in update.model_fields_set) == explicit, update_dict.keys()
+            )
             for field in fields:
                 config_attributes[field] = update_dict[field]
 
     def add_config(self, config_with_priority: ConfigWithPriority):
         """Add a config object together with its priority to the loader."""
         config: YAMLBaseConfig = config_with_priority.config
         tag = config.get_yaml_tag()
@@ -476,82 +267,89 @@
         except KeyError:
             self.configs_per_tag[tag] = [config_with_priority]
 
     def add_single_config_string(self, string: str, priority):
         """Add a yaml string with a single config object."""
         config: YAMLBaseConfig = yaml.load(string, Loader=self.yaml_loader)
         if not isinstance(config, YAMLBaseConfig):
-            string = string.replace('\n', '\n\t')
-            raise ValueError(f"The given string is not a registered config:\n\n\t{string}")
+            string = string.replace("\n", "\n\t")
+            raise ValueError(
+                f"The given string is not a registered config:\n\n\t{string}"
+            )
         config_with_priority = ConfigWithPriority(config=config, priority=priority)
         self.add_config(config_with_priority)
 
     def add_config_data(self, config_data: List[Union[Dict, List]], priority=None):
         """Add multiple configs or priorities."""
         given_priority = priority
         for config_element in config_data:
-            if isinstance(config_element, Dict) and 'priority' in config_element:
-                priority = config_element['priority'] if given_priority is None else given_priority
+            if isinstance(config_element, Dict) and "priority" in config_element:
+                priority = (
+                    config_element["priority"]
+                    if given_priority is None
+                    else given_priority
+                )
             elif isinstance(config_element, List):
                 for config in config_element:
                     if isinstance(config, YAMLBaseConfig):
                         config_with_priority = ConfigWithPriority(
                             config=config,
-                            priority=priority if priority is not None else 0
+                            priority=priority if priority is not None else 0,
                         )
                         self.add_config(config_with_priority)
             else:
-                raise ValueError(f"Entries in the config files must be mapping containing a priority key "
-                                 f"or a list of configs.")
+                raise ValueError(
+                    f"Entries in the config files must be mapping containing a priority key "
+                    f"or a list of configs."
+                )
 
     def load_string(self, string, priority: Optional[int] = None):
         """Load a yaml string including multiple configs or priorities."""
         try:
-            config_data: List = yaml.load_all(string, Loader=self.yaml_loader)
+            config_data: List = list(yaml.load_all(string, Loader=self.yaml_loader))
         except (ParserError, ConstructorError) as e:
             raise e
         self.add_config_data(config_data, priority)
 
     def load_file(self, file_path: Path, priority: Optional[int] = None):
-        """ Load a yaml file including multiple configs or priorities."""
+        """Load a yaml file including multiple configs or priorities."""
         if not file_path.is_file():
-            if file_path.with_suffix('.yaml').is_file():
-                file_path = file_path.with_suffix('.yaml')
+            if file_path.with_suffix(".yaml").is_file():
+                file_path = file_path.with_suffix(".yaml")
             else:
-                raise FileNotFoundError(f'Could not find file {file_path}')
+                raise FileNotFoundError(f"Could not find file {file_path}")
 
         with open(file_path) as file:
             try:
-                config_data: List = yaml.load_all(file, Loader=self.yaml_loader)
-                # pyyaml lazy loads, so file needs to stay open
-                self.add_config_data(config_data, priority)
+                config_data: List = list(yaml.load_all(file, Loader=self.yaml_loader))
             except (ParserError, ConstructorError) as e:
                 raise e
+        self.add_config_data(config_data, priority)
 
     def load_directory(self, directory_path: Path, priority: Optional[int] = None):
         """Load all files ending with .yaml from a directory."""
         if not directory_path.is_dir():
             raise NotADirectoryError(f"{directory_path} is not a directory.")
         for file_path in sorted(directory_path.glob("*.yaml")):
             self.load_file(file_path, priority)
 
     def construct_from_string(self, string: str, auto_load: bool = False):
         """Construct the configuration for a yaml string with a single yaml config."""
         try:
             config: Any = yaml.load(string, Loader=self.yaml_loader)
         except (ParserError, ConstructorError) as e:
             raise e
-        return self.deep_construct_from_config(config, final=True, auto_load=auto_load)
+        return self.deep_construct(config, final=True, auto_load=auto_load)
 
     def construct_from_file(self, file_path: Path, auto_load: bool = False):
         """Construct the configuration for a yaml file with a single yaml config."""
         if not file_path.is_file():
-            if file_path.with_suffix('.yaml').is_file():
-                file_path = file_path.with_suffix('.yaml')
+            if file_path.with_suffix(".yaml").is_file():
+                file_path = file_path.with_suffix(".yaml")
             else:
                 raise FileNotFoundError(f'Could not find file "{file_path}"')
         with open(file_path) as file:
             try:
                 config: Any = yaml.load(file, Loader=self.yaml_loader)
             except (ParserError, ConstructorError) as e:
                 raise e
-        return self.deep_construct_from_config(config, final=True, auto_load=auto_load)
+        return self.deep_construct(config, final=True, auto_load=auto_load)
```

### Comparing `yaloader-0.0.3/src/yaloader.egg-info/PKG-INFO` & `yaloader-1.0.0/src/yaloader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: yaloader
-Version: 0.0.3
+Version: 1.0.0
 Summary: A package loading class configurations from yaml files
 Home-page: https://github.com/DominikMa/yaloader
 Author: Dominik Mairhöfer
 Author-email: dominik@mairhoefer.xyz
 License: GNU AGPLv3
 Project-URL: Documentation, https://yaloader.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/DominikMa/yaloader/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE.txt
 
 # YaLoader - A YAML Configuration Loader
 
 The documentation will be [here](https://yaloader.readthedocs.io).
-
```

