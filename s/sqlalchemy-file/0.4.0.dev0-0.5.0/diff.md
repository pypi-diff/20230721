# Comparing `tmp/sqlalchemy_file-0.4.0.dev0.tar.gz` & `tmp/sqlalchemy_file-0.5.0.tar.gz`

## Comparing `sqlalchemy_file-0.4.0.dev0.tar` & `sqlalchemy_file-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/__init__.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/base.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/exceptions.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/file.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/helpers.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/mutable_list.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/processors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/py.typed
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/storage.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/stored_file.py
--rw-r--r--   0        0        0    14650 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/types.py
--rw-r--r--   0        0        0     8276 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/validators.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/LICENSE
--rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/README.md
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 sqlalchemy_file-0.4.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/__init__.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/base.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/exceptions.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/file.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/helpers.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/mutable_list.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/processors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/py.typed
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/storage.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/stored_file.py
+-rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/types.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/sqlalchemy_file/validators.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/README.md
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7737 2020-02-02 00:00:00.000000 sqlalchemy_file-0.5.0/PKG-INFO
```

### Comparing `sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/base.py` & `sqlalchemy_file-0.5.0/sqlalchemy_file/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing
 from typing import Any
 
 
 class BaseFile(typing.Dict[str, Any]):
-    """
-    Base class for file object. It keeps information on a content related to a specific storage.
+    """Base class for file object.
+
+    It keeps information on a content related to a specific storage.
     It is a specialized dictionary that provides also attribute style access,
     the dictionary parent permits easy encoding/decoding to JSON.
 
     """
 
     def __getitem__(self, key: str) -> Any:
         return dict.__getitem__(self, key)
```

### Comparing `sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/exceptions.py` & `sqlalchemy_file-0.5.0/sqlalchemy_file/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 class ValidationError(Exception):
     """Base class for ValidationError
     Parameters:
         key: Current Column key
-        msg: Validation error message
+        msg: Validation error message.
     """
 
     def __init__(self, key: str, msg: str):  # pragma: no cover
-        super().__init__("{}: {}".format(key, msg))
+        super().__init__(f"{key}: {msg}")
         self.key = key
         self.msg = msg
 
 
 class SizeValidationError(ValidationError):
     pass
```

### Comparing `sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/file.py` & `sqlalchemy_file-0.5.0/sqlalchemy_file/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,21 @@
 from sqlalchemy_file.processors import Processor
 from sqlalchemy_file.storage import StorageManager
 from sqlalchemy_file.stored_file import StoredFile
 from sqlalchemy_file.validators import Validator
 
 
 class File(BaseFile):
-    """
-    Takes a file as content and uploads it to the appropriate storage
+    """Takes a file as content and uploads it to the appropriate storage
     according to the attached Column and file information into the
     database as JSON.
 
     Default attributes provided for all ``File`` include:
 
     Attributes:
-
         filename (str):  This is the name of the uploaded file
         file_id:   This is the generated UUID for the uploaded file
         upload_storage:   Name of the storage used to save the uploaded file
         path:            This is a  combination of `upload_storage` and `file_id` separated by
                         `/`. This will be use later to retrieve the file
         content_type:   This is the content type of the uploaded file
         uploaded_at (datetime):    This is the upload date in ISO format
@@ -65,38 +63,39 @@
                     "size": get_content_size_from_fileobj(self.original_content),
                     "files": [],
                 }
             )
             self._thaw()
 
     def apply_validators(self, validators: List[Validator], key: str = "") -> None:
-        """Apply validators to current file"""
+        """Apply validators to current file."""
         for validator in validators:
             validator.process(self, key)
 
     def apply_processors(
         self,
         processors: List[Processor],
         upload_storage: Optional[str] = None,
     ) -> None:
-        """Apply processors to current file"""
+        """Apply processors to current file."""
         for processor in processors:
             processor.process(self, upload_storage)
         self._freeze()
 
     def save_to_storage(self, upload_storage: Optional[str] = None) -> None:
-        """Save current file into provided `upload_storage`"""
+        """Save current file into provided `upload_storage`."""
         extra = self.get("extra", {})
         extra.update({"content_type": self.content_type})
 
         metadata = self.get("metadata", None)
         if metadata is not None:
             warnings.warn(
                 'metadata attribute is deprecated. Use extra={"meta_data": ...} instead',
                 DeprecationWarning,
+                stacklevel=1,
             )
             extra.update({"meta_data": metadata})
 
         if extra.get("meta_data", None) is None:
             extra["meta_data"] = {}
 
         extra["meta_data"].update(
@@ -107,41 +106,41 @@
             upload_storage,
             extra=extra,
             headers=self.get("headers", None),
         )
         self["file_id"] = stored_file.name
         self["upload_storage"] = upload_storage
         self["uploaded_at"] = datetime.utcnow().isoformat()
-        self["path"] = "{}/{}".format(upload_storage, stored_file.name)
+        self["path"] = f"{upload_storage}/{stored_file.name}"
         self["url"] = stored_file.get_cdn_url()
         self["saved"] = True
 
     def store_content(
         self,
         content: Any,
         upload_storage: Optional[str] = None,
         name: Optional[str] = None,
         metadata: Optional[Dict[str, Any]] = None,
         extra: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
     ) -> StoredFile:
         """Store content into provided `upload_storage`
-        with additional `metadata`. Can be use by processors
+        with additional `metadata`. Can be used by processors
         to store additional files.
         """
         name = name or str(uuid.uuid4())
         stored_file = StorageManager.save_file(
             name=name,
             content=content,
             upload_storage=upload_storage,
             metadata=metadata,
             extra=extra,
             headers=headers,
         )
-        self["files"].append("{}/{}".format(upload_storage, name))
+        self["files"].append(f"{upload_storage}/{name}")
         return stored_file
 
     def encode(self) -> Dict[str, Any]:
         return {k: v for k, v in self.items() if k not in ["original_content"]}
 
     @classmethod
     def decode(cls, data: Any) -> "File":
```

### Comparing `sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/helpers.py` & `sqlalchemy_file-0.5.0/sqlalchemy_file/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import json
 import mimetypes
 import os
 import re
 from builtins import RuntimeError
 from tempfile import SpooledTemporaryFile
-from typing import Any, Dict, Union
+from typing import Any, Dict, List, Union
 
 INMEMORY_FILESIZE = 1024 * 1024
 LOCAL_STORAGE_DRIVER_NAME = "Local Storage"
 
 
 def get_metadata_file_obj(metadata: Dict[str, Any]) -> "SpooledTemporaryFile[bytes]":
     f = SpooledTemporaryFile(INMEMORY_FILESIZE)
     f.write(json.dumps(metadata).encode())
     f.seek(0)
     return f
 
 
 def get_content_from_file_obj(fileobj: Any) -> Any:
-    """Provides a real file object from file content
+    """Provides a real file object from file content.
+
     Converts ``str`` and ``bytes`` to an actual file.
     """
     if isinstance(fileobj, (str, bytes)):
         f = SpooledTemporaryFile(INMEMORY_FILESIZE)
         f.write(fileobj.encode() if isinstance(fileobj, str) else fileobj)
         f.seek(0)
         return f
-    elif getattr(fileobj, "file", None) is not None:
+    if getattr(fileobj, "file", None) is not None:
         return fileobj.file
     return fileobj
 
 
 def get_filename_from_fileob(fileobj: Any) -> Any:
     if getattr(fileobj, "filename", None) is not None:
         return fileobj.filename
-    elif getattr(fileobj, "name", None) is not None:
+    if getattr(fileobj, "name", None) is not None:
         return os.path.basename(fileobj.name)
     return "unnamed"
 
 
 def get_content_type_from_fileobj(fileobj: Any, filename: str) -> Any:
     if getattr(fileobj, "content_type", None) is not None:
         return fileobj.content_type
@@ -60,17 +61,21 @@
         file.seek(pos)
         return size
     raise RuntimeError("Unable to determine the file's size.")  # pragma: no cover
 
 
 def convert_size(size: Union[str, int]) -> int:
     # convert size to number of bytes ex: 1k -> 1000; 1Ki->1024
-    if isinstance(size, int):
-        return size
-    elif isinstance(size, str):
+    if isinstance(size, str):
         pattern = re.compile(r"^(\d+)\s*(k|([KM]i?))$")
         m = re.fullmatch(pattern, size)
         if m is None:
             raise ValueError("Invalid size %s" % size)
         value, si, _ = m.groups()
         si_map = {"k": 1000, "K": 1000, "M": 1000**2, "Ki": 1024, "Mi": 1024**2}
         return int(value) * si_map[si]
+    return size
+
+
+def flatmap(lists: List[List[Any]]) -> List[Any]:
+    """Flattens a list of lists into a single list."""
+    return [value for _list in lists for value in _list]
```

### Comparing `sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/mutable_list.py` & `sqlalchemy_file-0.5.0/sqlalchemy_file/mutable_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 from sqlalchemy.ext.mutable import Mutable
 
 T = TypeVar("T", bound=Any)
 
 
 class MutableList(Mutable, typing.List[T]):
-    """
-    A list type that implements :class:`Mutable`.
+    """A list type that implements :class:`Mutable`.
 
     The :class:`MutableList` object implements a list that will
     emit change events to the underlying mapping when the contents of
     the list are altered, including when values are added or removed.
 
     This is a replication of default Mutablelist provide by SQLAlchemy.
     The difference here is the properties _removed which keep every element
@@ -28,16 +27,15 @@
     @classmethod
     def coerce(cls, key: Any, value: Any) -> Any:
         if not isinstance(value, MutableList):
             if isinstance(value, list):
                 return MutableList(value)
             # this call will raise ValueError
             return Mutable.coerce(key, value)  # pragma: no cover
-        else:
-            return value  # pragma: no cover
+        return value  # pragma: no cover
 
     @no_type_check
     def __reduce_ex__(self, proto):  # pragma: no cover
         return self.__class__, (list(self),)
 
     # needed for backwards compatibility with
     # older pickles
@@ -46,28 +44,22 @@
 
     def __setstate__(self, state: Any) -> None:  # pragma: no cover
         self[:] = state[0]
         self._removed = state[1]
 
     def __setitem__(self, index: Any, value: Any) -> None:
         """Detect list set events and emit change events."""
-        if isinstance(index, slice):
-            old_value = self[index]
-        else:
-            old_value = [self[index]]
+        old_value = self[index] if isinstance(index, slice) else [self[index]]
         list.__setitem__(self, index, value)
         self.changed()
         self._removed.extend(old_value)
 
     def __delitem__(self, index: Any) -> None:
         """Detect list del events and emit change events."""
-        if isinstance(index, slice):
-            old_value = self[index]
-        else:
-            old_value = [self[index]]
+        old_value = self[index] if isinstance(index, slice) else [self[index]]
         list.__delitem__(self, index)
         self.changed()
         self._removed.extend(old_value)
 
     def pop(self, *arg) -> "T":  # type: ignore
         result = list.pop(self, *arg)
         self.changed()
```

### Comparing `sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/processors.py` & `sqlalchemy_file-0.5.0/sqlalchemy_file/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,40 +6,36 @@
 from sqlalchemy_file.helpers import INMEMORY_FILESIZE
 
 if TYPE_CHECKING:
     from sqlalchemy_file.file import File
 
 
 class Processor:
-    """
-    Interface that must be implemented by file processors.
+    """Interface that must be implemented by file processors.
     Can be used to add additional data to the stored file or change it.
     When file processors are run the file has already been stored.
 
     """
 
     @abstractmethod
     def process(
         self, file: "File", upload_storage: Optional[str] = None
     ) -> None:  # pragma: no cover
-        """
-        Should be overridden in inherited class
+        """Should be overridden in inherited class
         Parameters:
             file: [File][sqlalchemy_file.file.File] object,
                 Use file.original_content to access uploaded file
             upload_storage: pass this to
                 [file.store_content()][sqlalchemy_file.file.File.store_content]
-                to attach additional files to the original file
+                to attach additional files to the original file.
         """
-        pass
 
 
 class ThumbnailGenerator(Processor):
-    """
-    Generate thumbnail from original content.
+    """Generate thumbnail from original content.
 
     The default thumbnail format and size are `PNG@128x128`, those can be changed
     by giving custom `thumbnail_size` and `thumbnail_format`
 
     !!! note
         ThumbnailGenerator will add additional data
         to the file object under the key `thumbnail`.
@@ -120,23 +116,23 @@
             {
                 "filename": file["filename"] + f".thumbnail{width}x{height}{ext}",
                 "content_type": content_type,
                 "width": width,
                 "height": height,
             }
         )
-        extra.update({"meta_data": metadata})
+        extra.update({"content_type": content_type, "meta_data": metadata})
         stored_file = file.store_content(
             output, upload_storage, extra=extra, headers=file.get("headers", None)
         )
         file.update(
             {
                 "thumbnail": {
                     "file_id": stored_file.name,
                     "width": width,
                     "height": height,
                     "upload_storage": upload_storage,
-                    "path": "{}/{}".format(upload_storage, stored_file.name),
+                    "path": f"{upload_storage}/{stored_file.name}",
                     "url": stored_file.get_cdn_url(),
                 }
             }
         )
```

### Comparing `sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/storage.py` & `sqlalchemy_file-0.5.0/sqlalchemy_file/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,71 @@
+import contextlib
 import warnings
-from typing import Any, Dict, Iterator, Optional
+from typing import Any, ClassVar, Dict, Iterator, Optional
 
 from libcloud.storage.base import Container
 from libcloud.storage.types import ObjectDoesNotExistError
 from sqlalchemy_file.helpers import LOCAL_STORAGE_DRIVER_NAME, get_metadata_file_obj
 from sqlalchemy_file.stored_file import StoredFile
 
 
 class StorageManager:
-    """
-    Takes care of managing the whole Storage environment for the application.
+    """Takes care of managing the whole Storage environment for the application.
 
     Use [add_storage][sqlalchemy_file.storage.StorageManager.add_storage] method
     to add new `libcloud.storage.base.Container`and associate a name which
     will be use later to retrieve this container.
 
     The first container will be used as default, to simplify code when you have
     only one container.
 
     Use associated name as `upload_storage` for [FileField][sqlalchemy_file.types.FileField]
     to store his files inside the corresponding container.
 
     """
 
-    _default_storage_name: Optional[str] = None
-    _storages: Dict[str, Container] = {}
+    _default_storage_name: ClassVar[Optional[str]] = None
+    _storages: ClassVar[Dict[str, Container]] = {}
 
     @classmethod
     def set_default(cls, name: str) -> None:
-        """Replaces the current application default storage"""
+        """Replaces the current application default storage."""
         if name not in cls._storages:
-            raise RuntimeError("{} storage has not been added".format(name))
+            raise RuntimeError(f"{name} storage has not been added")
         cls._default_storage_name = name
 
     @classmethod
     def get_default(cls) -> str:
-        """Gets the current application default storage"""
+        """Gets the current application default storage."""
         if cls._default_storage_name is None:
             raise RuntimeError("No default storage has been added")
         return cls._default_storage_name
 
     @classmethod
     def add_storage(cls, name: str, container: Container) -> None:
-        """Add new storage"""
+        """Add new storage."""
         assert isinstance(container, Container), "Invalid container"
         if name in cls._storages:
-            raise RuntimeError("Storage {} has already been added".format(name))
+            raise RuntimeError(f"Storage {name} has already been added")
         if cls._default_storage_name is None:
             cls._default_storage_name = name
         cls._storages[name] = container
 
     @classmethod
     def get(cls, name: Optional[str] = None) -> Container:
-        """
-        Gets the container instance associate to the name,
-        return default if name isn't provided
+        """Gets the container instance associate to the name,
+        return default if name isn't provided.
         """
         if name is None and cls._default_storage_name is None:
             raise RuntimeError("No default storage have been added")
-        elif name is None:
+        if name is None:
             name = cls._default_storage_name
         if name in cls._storages:
             return cls._storages[name]
-        raise RuntimeError("{} storage has not been added".format(name))
+        raise RuntimeError(f"{name} storage has not been added")
 
     @classmethod
     def save_file(
         cls,
         name: str,
         content: Iterator[bytes],
         upload_storage: Optional[str] = None,
@@ -74,14 +73,15 @@
         extra: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
     ) -> StoredFile:
         if metadata is not None:
             warnings.warn(
                 'metadata attribute is deprecated. Use extra={"meta_data": ...} instead',
                 DeprecationWarning,
+                stacklevel=1,
             )
             extra = {
                 "meta_data": metadata,
                 "content_type": metadata.get(
                     "content_type", "application/octet-stream"
                 ),
             }
@@ -106,34 +106,32 @@
                 iterator=content, object_name=name, extra=extra, headers=headers
             )
         )
 
     @classmethod
     def get_file(cls, path: str) -> StoredFile:
         """Retrieve the file with `provided` path,
-        path is expected to be `storage_name/file_id`
+        path is expected to be `storage_name/file_id`.
         """
         upload_storage, file_id = path.split("/")
         return StoredFile(StorageManager.get(upload_storage).get_object(file_id))
 
     @classmethod
     def delete_file(cls, path: str) -> bool:
-        """Delete the file with `provided` path
-        path is expected to be `storage_name/file_id`
+        """Delete the file with `provided` path.
+
+        The path is expected to be `storage_name/file_id`.
         """
         upload_storage, file_id = path.split("/")
         obj = StorageManager.get(upload_storage).get_object(file_id)
         if obj.driver.name == LOCAL_STORAGE_DRIVER_NAME:
             """Try deleting associated metadata file"""
-            try:
+            with contextlib.suppress(ObjectDoesNotExistError):
                 obj.container.get_object(f"{obj.name}.metadata.json").delete()
-            except ObjectDoesNotExistError:
-                pass
+
         return obj.delete()
 
     @classmethod
     def _clear(cls) -> None:
-        """
-        This is only for testing pourposes, resets the StorageManager
-        """
+        """This is only for testing pourposes, resets the StorageManager."""
         cls._default_storage_name = None
         cls._storages = {}
```

### Comparing `sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/types.py` & `sqlalchemy_file-0.5.0/sqlalchemy_file/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union
+from typing import Any, ClassVar, Dict, List, Optional, Set, Tuple, Type, Union
 
 from sqlalchemy import event, inspect, orm, types
 from sqlalchemy.engine import Connection, Dialect
 from sqlalchemy.orm import ColumnProperty, Mapper, Session, SessionTransaction
 from sqlalchemy.orm.attributes import get_history
 from sqlalchemy_file.file import File
+from sqlalchemy_file.helpers import flatmap
 from sqlalchemy_file.mutable_list import MutableList
 from sqlalchemy_file.processors import Processor, ThumbnailGenerator
 from sqlalchemy_file.storage import StorageManager
 from sqlalchemy_file.validators import ImageValidator, Validator
 
 
 class FileField(types.TypeDecorator):  # type: ignore
-
-    """
-    Provides support for storing attachments to **SQLAlchemy** models.
+    """Provides support for storing attachments to **SQLAlchemy** models.
 
     [FileField][sqlalchemy_file.types.FileField] can be used as a Column type to
     store files into the model. The actual file itself will be uploaded to a specific
     `libcloud.storage.base.Container`, and only the [File][sqlalchemy_file.file.File]
     information will be stored on the database as JSON.
 
     [FileField][sqlalchemy_file.types.FileField] is transaction aware, so it will delete
@@ -30,40 +29,39 @@
     Each file will be validated by provided validators before being saved into
     associate storage `libcloud.storage.base.Container` and can go through different
     processors before being saved in the database.
 
     """
 
     impl = types.JSON
-    cache_ok = True
+    cache_ok = False
 
     def __init__(
         self,
         *args: Tuple[Any],
         upload_storage: Optional[str] = None,
         validators: Optional[List[Validator]] = None,
         processors: Optional[List[Processor]] = None,
         upload_type: Type[File] = File,
         multiple: Optional[bool] = False,
         extra: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
         **kwargs: Dict[str, Any],
     ) -> None:
-        """
-        Parameters:
-              upload_storage: storage to use
-              validators: List of validators to apply
-              processors: List of validators to apply
-              upload_type: File class to use, could be
-                        used to set custom File class
-              multiple: Use this to save multiple files
-              extra: Extra attributes (driver specific)
-              headers: Additional request headers,
-                such as CORS headers. For example:
-                headers = {'Access-Control-Allow-Origin': 'http://mozilla.com'}
+        """Parameters:
+        upload_storage: storage to use
+        validators: List of validators to apply
+        processors: List of validators to apply
+        upload_type: File class to use, could be
+        used to set custom File class
+        multiple: Use this to save multiple files
+        extra: Extra attributes (driver specific)
+        headers: Additional request headers,
+        such as CORS headers. For example:
+        headers = {'Access-Control-Allow-Origin': 'http://mozilla.com'}.
         """
         super().__init__(*args, **kwargs)
         if processors is None:
             processors = []
         if validators is None:
             validators = []
         self.upload_storage = upload_storage
@@ -81,15 +79,15 @@
             return None
         if not self.multiple and not isinstance(
             value, self.upload_type
         ):  # pragma: no cover
             raise ValueError(f"Expected {self.upload_type}, received: {type(value)}")
         if self.multiple and not (
             isinstance(value, list)
-            and all([isinstance(v, self.upload_type) for v in value])
+            and all(isinstance(v, self.upload_type) for v in value)
         ):  # pragma: no cover
             raise ValueError(
                 f"Expected MutableList[{self.upload_type}], received: {type(value)}"
             )
         return [v.encode() for v in value] if self.multiple else value.encode()
 
     def process_result_value(
@@ -107,15 +105,15 @@
 
 
 class ImageField(FileField):
     """Inherits all attributes and methods from [FileField][sqlalchemy_file.types.FileField],
     but also validates that the uploaded object is a valid image.
     """
 
-    cache_ok = True
+    cache_ok = False
 
     def __init__(
         self,
         *args: Tuple[Any],
         upload_storage: Optional[str] = None,
         thumbnail_size: Optional[Tuple[int, int]] = None,
         image_validator: Optional[ImageValidator] = None,
@@ -123,28 +121,27 @@
         processors: Optional[List[Processor]] = None,
         upload_type: Type[File] = File,
         multiple: Optional[bool] = False,
         extra: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         **kwargs: Dict[str, Any],
     ) -> None:
-        """
-        Parameters:
-            upload_storage: storage to use
-            image_validator: ImageField use default image
-                  validator, Use this property to customize it.
-            thumbnail_size: If set, a thumbnail will be generated
-                from original image using [ThumbnailGenerator]
-                [sqlalchemy_file.processors.ThumbnailGenerator]
-            validators: List of additional validators to apply
-            processors: List of validators to apply
-            upload_type: File class to use, could be
-                        used to set custom File class
-            multiple: Use this to save multiple files
-            extra: Extra attributes (driver specific)
+        """Parameters
+        upload_storage: storage to use
+        image_validator: ImageField use default image
+        validator, Use this property to customize it.
+        thumbnail_size: If set, a thumbnail will be generated
+        from original image using [ThumbnailGenerator]
+        [sqlalchemy_file.processors.ThumbnailGenerator]
+        validators: List of additional validators to apply
+        processors: List of validators to apply
+        upload_type: File class to use, could be
+        used to set custom File class
+        multiple: Use this to save multiple files
+        extra: Extra attributes (driver specific).
         """
         if validators is None:
             validators = []
         if image_validator is None:
             image_validator = ImageValidator()
         if thumbnail_size is not None:
             if processors is None:
@@ -161,15 +158,15 @@
             extra=extra,
             headers=headers,
             **kwargs,
         )
 
 
 class FileFieldSessionTracker:
-    mapped_entities: Dict[Type[Any], List[str]] = {}
+    mapped_entities: ClassVar[Dict[Type[Any], List[str]]] = {}
 
     @classmethod
     def delete_files(cls, paths: Set[str], ctx: str) -> None:
         for path in paths:
             StorageManager.delete_file(path)
 
     @classmethod
@@ -186,28 +183,26 @@
 
     @classmethod
     def add_old_files_to_session(cls, session: Session, paths: List[str]) -> None:
         session._old_files = getattr(session, "_old_files", set())  # type: ignore
         session._old_files.update(paths)  # type: ignore
 
     @classmethod
-    def extract_files_from_history(
-        cls, data: List[Union[MutableList[File], File]]
-    ) -> List[str]:
+    def extract_files_from_history(cls, data: Union[Tuple[()], List[Any]]) -> List[str]:
         paths = []
         for item in data:
             if isinstance(item, list):
-                paths.extend([f["path"] for f in item])
+                paths.extend([f["files"] for f in item])
             elif isinstance(item, File):
-                paths.append(item["path"])
-        return paths
+                paths.append(item["files"])
+        return flatmap(paths)
 
     @classmethod
-    def _mapper_configured(cls, mapper: Mapper, class_: Any) -> None:
-        """Detect and listen all class with FileField Column"""
+    def _mapper_configured(cls, mapper: Mapper, class_: Any) -> None:  # type: ignore[type-arg]
+        """Detect and listen all class with FileField Column."""
         for mapper_property in mapper.iterate_properties:
             if isinstance(mapper_property, ColumnProperty) and isinstance(
                 mapper_property.columns[0].type, FileField
             ):
                 assert (
                     len(mapper_property.columns) == 1
                 ), "Multiple-column properties are not supported"
@@ -215,67 +210,66 @@
                     MutableList.associate_with_attribute(
                         getattr(class_, mapper_property.key)
                     )
                 cls.mapped_entities.setdefault(class_, []).append(mapper_property.key)
 
     @classmethod
     def _after_configured(cls) -> None:
-        for entity in cls.mapped_entities.keys():
+        for entity in cls.mapped_entities:
             event.listen(entity, "before_insert", cls._before_insert)
             event.listen(entity, "before_update", cls._before_update)
             event.listen(entity, "after_update", cls._after_update)
             event.listen(entity, "after_delete", cls._after_delete)
 
     @classmethod
     def _after_commit(cls, session: Session) -> None:
-        """After commit, old files are automatically deleted"""
+        """After commit, old files are automatically deleted."""
         cls.delete_files(getattr(session, "_old_files", set()), "after_commit")
         cls.clear_session(session)
 
     @classmethod
     def _after_soft_rollback(cls, session: Session, _: SessionTransaction) -> None:
-        """After rollback, new files are automatically deleted"""
+        """After rollback, new files are automatically deleted."""
         cls.delete_files(getattr(session, "_new_files", set()), "after_soft_rollback")
         cls.clear_session(session)
 
     @classmethod
-    def _after_delete(cls, mapper: Mapper, _: Connection, obj: Any) -> None:
-        """
-        After delete mark all linked files as old in order to delete
-        them when after session is committed
+    def _after_delete(cls, mapper: Mapper, _: Connection, obj: Any) -> None:  # type: ignore[type-arg]
+        """After delete mark all linked files as old in order to delete
+        them when after session is committed.
         """
         tracked_columns: List[str] = cls.mapped_entities.get(mapper.class_, [])
         for key in tracked_columns:
             value = getattr(obj, key)
             if value is not None:
                 cls.add_old_files_to_session(
                     inspect(obj).session,
-                    [
-                        f["path"]
-                        for f in (value if isinstance(value, list) else [value])
-                    ],
+                    flatmap(
+                        [
+                            f["files"]
+                            for f in (value if isinstance(value, list) else [value])
+                        ]
+                    ),
                 )
 
     @classmethod
-    def _after_update(cls, mapper: Mapper, _: Connection, obj: Any) -> None:
-        """
-        After update, mark all edited files as old
-        in order to delete them when after session is committed
+    def _after_update(cls, mapper: Mapper, _: Connection, obj: Any) -> None:  # type: ignore[type-arg]
+        """After update, mark all edited files as old
+        in order to delete them when after session is committed.
         """
         tracked_columns: List[str] = cls.mapped_entities.get(mapper.class_, [])
         for key in tracked_columns:
             history = get_history(obj, key)
             cls.add_old_files_to_session(
                 inspect(obj).session, cls.extract_files_from_history(history.deleted)
             )
 
     @classmethod
-    def _before_update(cls, mapper: Mapper, _: Connection, obj: Any) -> None:
-        """
-        Before updating values, validate and save files. For multiple fields,
+    def _before_update(cls, mapper: Mapper, _: Connection, obj: Any) -> None:  # type: ignore[type-arg]
+        """Before updating values, validate and save files. For multiple fields,
         mark all removed files as old, as _removed attribute will be
         reinitialised after update.
         """
         session = inspect(obj).session
         tracked_columns: List[str] = cls.mapped_entities.get(mapper.class_, [])
         for key in tracked_columns:
             value = getattr(obj, key)
@@ -285,53 +279,68 @@
                     setattr(obj, key, prepare_value)
                     history = get_history(obj, key)
                     cls.add_new_files_to_session(
                         session, cls.extract_files_from_history(history.added)
                     )
                 if isinstance(value, MutableList):
                     _removed = getattr(value, "_removed", ())
-                    cls.add_old_files_to_session(session, [f["path"] for f in _removed])
+                    cls.add_old_files_to_session(
+                        session, flatmap([f["files"] for f in _removed])
+                    )
 
     @classmethod
-    def _before_insert(cls, mapper: Mapper, _: Connection, obj: Any) -> None:
+    def _before_insert(cls, mapper: Mapper, _: Connection, obj: Any) -> None:  # type: ignore[type-arg]
         """Before inserting values, mark all created files as new. They will be
-        automatically removed when session rollback"""
-
+        automatically removed when session rollback.
+        """
         tracked_columns: List[str] = cls.mapped_entities.get(mapper.class_, [])
         for key in tracked_columns:
             value = getattr(obj, key)
             if value is not None:
                 setattr(obj, key, cls.prepare_file_attr(mapper, obj, key)[1])
                 history = get_history(obj, key)
                 cls.add_new_files_to_session(
                     inspect(obj).session, cls.extract_files_from_history(history.added)
                 )
 
     @classmethod
     def prepare_file_attr(
-        cls, mapper: Mapper, obj: Any, key: str
+        cls, mapper: Mapper, obj: Any, key: str  # type: ignore[type-arg]
     ) -> Tuple[bool, Union[File, List[File]]]:
-        """
-        Prepare file before saved to database, convert bytes and string,
-        saved file into the upload_storage, apply validators and processors
+        """Prepare file(s) for saving into the database by converting bytes or strings into
+        File objects, applying validators, uploading the file(s) to the upload storage,
+        and applying processors.
+
+        Arguments:
+            mapper (Mapper): The mapper instance associated with the object.
+            obj (Any): The object containing the file attribute.
+            key (str): The name of the file attribute.
+
+        Returns:
+            Tuple[bool, Union[File, List[File]]]: A tuple containing a boolean flag indicating
+            whether the file(s) were changed, and the prepared file object(s). If the column type
+            allows multiple files, the prepared file objects are returned as a list.
         """
         value = getattr(obj, key)
 
-        """Become True when it is new file for single field,
-        or when new items is added for multiple field"""
+        """
+        The `changed` flag becomes True in two cases:
+        1. For a single-field attribute, when a new file is assigned, replacing the previous file.
+        2. For a multiple-field attribute, when new file objects are added to the existing ones.
+        """
         changed = False
 
-        column_type = mapper.attrs.get(key).columns[0].type
+        column_type = mapper.attrs.get(key).columns[0].type  # type: ignore[misc,union-attr]
         assert isinstance(column_type, FileField)
         upload_type = column_type.upload_type
 
         prepared_values: List[File] = []
         for v in value if isinstance(value, list) else [value]:
             if not isinstance(v, upload_type):
-                v = upload_type(v)
+                v = upload_type(v)  # noqa: PLW2901
             if not getattr(v, "saved", False):
                 changed = True
                 v.apply_validators(column_type.validators, key)
             prepared_values.append(v)
 
         upload_storage = column_type.upload_storage or StorageManager.get_default()
         for value in prepared_values:
@@ -347,14 +356,14 @@
                 value.apply_processors(column_type.processors, upload_storage)
         return changed, (
             prepared_values if column_type.multiple else prepared_values[0]
         )
 
     @classmethod
     def setup(cls) -> None:
-        event.listen(orm.mapper, "mapper_configured", cls._mapper_configured)
-        event.listen(orm.mapper, "after_configured", cls._after_configured)
+        event.listen(orm.Mapper, "mapper_configured", cls._mapper_configured)
+        event.listen(orm.Mapper, "after_configured", cls._after_configured)
         event.listen(Session, "after_commit", cls._after_commit)
         event.listen(Session, "after_soft_rollback", cls._after_soft_rollback)
 
 
 FileFieldSessionTracker.setup()
```

### Comparing `sqlalchemy_file-0.4.0.dev0/sqlalchemy_file/validators.py` & `sqlalchemy_file-0.5.0/sqlalchemy_file/validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,37 +11,35 @@
 from sqlalchemy_file.helpers import convert_size
 
 if TYPE_CHECKING:
     from sqlalchemy_file.file import File
 
 
 class Validator:
-    """
-    Interface that must be implemented by file validators.
+    """Interface that must be implemented by file validators.
+
     File validators get executed before a file is stored on the database
     using one of the supported fields. Can be used to add additional data
     to file object or change it.
 
     """
 
     @abstractmethod
     def process(self, file: "File", attr_key: str) -> None:  # pragma: no cover
-        """
-        Should be overridden in inherited class
+        """Should be overridden in inherited class.
 
         Parameters:
            file: [File][sqlalchemy_file.file.File] object
            attr_key: current SQLAlchemy column key. Can be passed to
                [ValidationError][sqlalchemy_file.exceptions.ValidationError]
         """
-        pass
 
 
 class SizeValidator(Validator):
-    """Validate file maximum size
+    """Validate file maximum size.
 
     Attributes:
         max_size:
             If set, the size of the underlying file must
             be below this file size in order to be valid.
             The size of the file can be given in one of
             the following formats:
@@ -52,14 +50,15 @@
             | k          | kilobyte      | 1,000 bytes     | `200k`      |
             | M          | megabyte      | 1,000,000 bytes | `2M`        |
             | Ki         | kibibyte      | 1,024 bytes     | `32Ki`      |
             | Mi         | mebibyte      | 1,048,576 bytes | `8Mi`       |
 
             For more information, view
             [Wikipedia: Binary prefix](https://en.wikipedia.org/wiki/Binary_prefix)
+
     Example:
         ```Python
         class Attachment(Base):
             __tablename__ = "attachment"
 
             id = Column(Integer, autoincrement=True, primary_key=True)
             name = Column(String(50), unique=True)
@@ -75,16 +74,15 @@
         super().__init__()
         self.max_size = max_size
 
     def process(self, file: "File", attr_key: str) -> None:
         if file.size > convert_size(self.max_size):
             raise SizeValidationError(
                 attr_key,
-                "The file is too large (%s bytes). Allowed maximum size is %s."
-                % (file.size, self.max_size),
+                f"The file is too large ({file.size} bytes). Allowed maximum size is {self.max_size}.",
             )
 
 
 class ContentTypeValidator(Validator):
     """Validate file mimetype
     Attributes:
         allowed_content_types: If set, file `content_type`
@@ -115,21 +113,20 @@
     def process(self, file: "File", attr_key: str) -> None:
         if (
             self.allowed_content_types is not None
             and file.content_type not in self.allowed_content_types
         ):
             raise ContentTypeValidationError(
                 attr_key,
-                "File content_type %s is not allowed. Allowed content_types are: %s"
-                % (file.content_type, self.allowed_content_types),
+                f"File content_type {file.content_type} is not allowed. Allowed content_types are: {self.allowed_content_types}",
             )
 
 
 class ImageValidator(ContentTypeValidator):
-    """Default Validator for ImageField
+    """Default Validator for ImageField.
 
     Attributes:
         min_wh: Minimum allowed dimension (w, h).
         max_wh: Maximum allowed dimension (w, h).
         allowed_content_types: An iterable whose items are
                     allowed content types. Default is `image/*`
         min_aspect_ratio: Minimum allowed image aspect ratio.
```

### Comparing `sqlalchemy_file-0.4.0.dev0/LICENSE` & `sqlalchemy_file-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_file-0.4.0.dev0/README.md` & `sqlalchemy_file-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -97,26 +97,26 @@
 
     id = Column(Integer, autoincrement=True, primary_key=True)
     name = Column(String(50), unique=True)
     content = Column(FileField)
 
 
 # Configure Storage
-os.makedirs("/tmp/storage/attachment", 0o777, exist_ok=True)
-container = LocalStorageDriver("/tmp/storage").get_container("attachment")
+os.makedirs("./upload_dir/attachment", 0o777, exist_ok=True)
+container = LocalStorageDriver("./upload_dir").get_container("attachment")
 StorageManager.add_storage("default", container)
 
 # Save your model
 engine = create_engine(
     "sqlite:///example.db", connect_args={"check_same_thread": False}
 )
 Base.metadata.create_all(engine)
 
-with Session(engine) as session:
-    session.add(Attachment(name="attachment1", content=open("./example.txt", "rb")))
+with Session(engine) as session, open("./example.txt", "rb") as local_file:
+    session.add(Attachment(name="attachment1", content=local_file))
     session.add(Attachment(name="attachment2", content=b"Hello world"))
     session.add(Attachment(name="attachment3", content="Hello world"))
     file = File(content="Hello World", filename="hello.txt", content_type="text/plain")
     session.add(Attachment(name="attachment4", content=file))
     session.commit()
 
 ```
```

### Comparing `sqlalchemy_file-0.4.0.dev0/pyproject.toml` & `sqlalchemy_file-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -26,79 +26,92 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     "Topic :: Database",
     "Topic :: Database :: Database Engines/Servers",
 ]
 dependencies = [
-    "SQLAlchemy >=1.4, <1.5",
+    "SQLAlchemy >=1.4, <2.1",
     "apache-libcloud >=3.6, <3.8",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://jowilf.github.io/sqlalchemy-file"
 Documentation = "https://jowilf.github.io/sqlalchemy-file"
 Repository = "https://github.com/jowilf/sqlalchemy-file"
 Changelog = "https://jowilf.github.io/sqlalchemy-file/changelog/"
 
 [project.optional-dependencies]
 test = [
-    "pytest >=7.2.0, <7.3.0",
-    "mypy ==0.991",
-    "ruff ==0.0.215",
-    "black ==22.12.0",
-    "coverage >=7.0.0, <7.1.0",
+    "pytest >=7.2.0, <7.5.0",
+    "mypy ==1.4.1",
+    "ruff ==0.0.278",
+    "black ==23.7.0",
+    "coverage >=7.0.0, <7.3.0",
     "fasteners ==0.18",
     "PyMySQL[rsa] >=1.0.2, <1.1.0",
     "psycopg2-binary >=2.9.5, <3.0.0",
-    "Pillow >=9.4.0, <9.5.0",
-    "sqlmodel ==0.0.8",
-    "python-multipart ==0.0.5",
-    "fastapi >=0.92, <0.93",
+    "Pillow >=9.4.0, <10.1.0",
+    "python-multipart ==0.0.6",
+    "fastapi >=0.92, <0.96",
     "Flask >=2.2, <2.3",
     "Flask-SQLAlchemy >=3.0,<3.1"
 ]
 doc = [
     "mkdocs-material >=9.0.0, <10.0.0",
-    "mkdocstrings[python] >=0.19.0, <0.21.0"
+    "mkdocstrings[python] >=0.19.0, <0.23.0"
 ]
 dev = [
-    "pre-commit >=2.20.0, <3.0.0",
-    "uvicorn >=0.20.0, <0.21.0",
+    "pre-commit >=2.20.0, <4.0.0",
+    "uvicorn >=0.20.0, <0.22.0",
 ]
 
 [tool.hatch.envs.default]
 features = [
     "test",
     "dev"
 ]
 [tool.hatch.envs.default.scripts]
 format = [
-    "ruff sqlalchemy_file tests docs_src --fix",
+    "ruff sqlalchemy_file tests --fix",
     "black ."
 ]
 
 [tool.hatch.envs.test]
 features = [
     "test",
 ]
 [tool.hatch.envs.test.scripts]
 lint = [
     "mypy sqlalchemy_file",
     "ruff sqlalchemy_file tests",
     "black . --check"
 ]
-all = "coverage run -m pytest tests"
+run = "coverage run -m pytest tests"
 cov = [
     "coverage combine",
     "coverage report --show-missing",
     "coverage xml"
 ]
 
+[[tool.hatch.envs.test.matrix]]
+sqla_version = ["1.4.x", "2.0.x"]
+
+[tool.hatch.envs.test.overrides]
+matrix.sqla_version.dependencies = [
+    { value = "SQLAlchemy >=2.0, <2.1", if = ["2.0.x"] },
+    { value = "SQLAlchemy >=1.4, <1.5", if = ["1.4.x"] },
+    { value = "sqlmodel ==0.0.8", if = ["1.4.x"] },
+]
+matrix.sqla_version.scripts = [
+    { key = "run", value = 'coverage run -m pytest tests --ignore=tests/test_sqlmodel.py', if = ["2.0.x"] },
+    { key = "cov", value = '', if = ["2.0.x"] },
+]
+
 [tool.hatch.envs.docs]
 features = [
     "doc",
 ]
 [tool.hatch.envs.docs.scripts]
 serve = "mkdocs serve -a localhost:8080"
 build = "mkdocs build"
@@ -118,25 +131,47 @@
 [tool.coverage.run]
 parallel = true
 command_line = "-m pytest"
 source = ["sqlalchemy_file", "tests"]
 
 [tool.ruff]
 select = [
+    "B", # flake8-bugbear
+    "C4", # flake8-comprehensions
+    "C90", # mccabe
+    "D", # pydocstyle
     "E", # pycodestyle errors
-    "W", # pycodestyle warnings
+    "ERA", # eradicate
     "F", # pyflakes
     "I", # isort
-    "C", # flake8-comprehensions
-    "B", # flake8-bugbear
+    "N", # pep8-naming
+    "PIE", # flake8-pie,
+    "PLC", # pylint - convention
+    "PLE", # pylint - error
+    "PLW", # pylint - warning
+    "Q", # flake8-quotes
+    "RET", # flake8-return,
+    "RUF", # Ruff-specific rules
+    "SIM", # flake8-simplify
+    "UP", # pyupgrade
+    "W", # pycodestyle warnings
 ]
-ignore = ["E501", "B904", "B008"]
+ignore = ["E501", "B904", "B008", "D100", "D101", "D102", "D103", "D104", "D105", "D106", "D107", "D205"]
+target-version = "py38"
+
+[tool.ruff.pydocstyle]
+convention = "google"
 
 [tool.ruff.isort]
 known-third-party = ["sqlalchemy_file"]
 
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+"docs_src/**" = ["N999"]
+
 [tool.mypy]
 strict = true
+warn_unused_ignores = false
 
 [tool.hatch.build.targets.wheel]
 [tool.hatch.build.targets.sdist]
 include = ["sqlalchemy_file"]
```

### Comparing `sqlalchemy_file-0.4.0.dev0/PKG-INFO` & `sqlalchemy_file-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-file
-Version: 0.4.0.dev0
+Version: 0.5.0
 Summary: SQLAlchemy-file is a SQLAlchemy extension for attaching files to SQLAlchemy model and uploading them to various storage.
 Project-URL: Homepage, https://jowilf.github.io/sqlalchemy-file
 Project-URL: Documentation, https://jowilf.github.io/sqlalchemy-file
 Project-URL: Repository, https://github.com/jowilf/sqlalchemy-file
 Project-URL: Changelog, https://jowilf.github.io/sqlalchemy-file/changelog/
 Author-email: Jocelin Hounon <hounonj@gmail.com>
 License-Expression: MIT
@@ -23,36 +23,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: apache-libcloud<3.8,>=3.6
-Requires-Dist: sqlalchemy<1.5,>=1.4
+Requires-Dist: sqlalchemy<2.1,>=1.4
 Provides-Extra: dev
-Requires-Dist: pre-commit<3.0.0,>=2.20.0; extra == 'dev'
-Requires-Dist: uvicorn<0.21.0,>=0.20.0; extra == 'dev'
+Requires-Dist: pre-commit<4.0.0,>=2.20.0; extra == 'dev'
+Requires-Dist: uvicorn<0.22.0,>=0.20.0; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mkdocs-material<10.0.0,>=9.0.0; extra == 'doc'
-Requires-Dist: mkdocstrings[python]<0.21.0,>=0.19.0; extra == 'doc'
+Requires-Dist: mkdocstrings[python]<0.23.0,>=0.19.0; extra == 'doc'
 Provides-Extra: test
-Requires-Dist: black==22.12.0; extra == 'test'
-Requires-Dist: coverage<7.1.0,>=7.0.0; extra == 'test'
-Requires-Dist: fastapi<0.93,>=0.92; extra == 'test'
+Requires-Dist: black==23.7.0; extra == 'test'
+Requires-Dist: coverage<7.3.0,>=7.0.0; extra == 'test'
+Requires-Dist: fastapi<0.96,>=0.92; extra == 'test'
 Requires-Dist: fasteners==0.18; extra == 'test'
 Requires-Dist: flask-sqlalchemy<3.1,>=3.0; extra == 'test'
 Requires-Dist: flask<2.3,>=2.2; extra == 'test'
-Requires-Dist: mypy==0.991; extra == 'test'
-Requires-Dist: pillow<9.5.0,>=9.4.0; extra == 'test'
+Requires-Dist: mypy==1.4.1; extra == 'test'
+Requires-Dist: pillow<10.1.0,>=9.4.0; extra == 'test'
 Requires-Dist: psycopg2-binary<3.0.0,>=2.9.5; extra == 'test'
 Requires-Dist: pymysql[rsa]<1.1.0,>=1.0.2; extra == 'test'
-Requires-Dist: pytest<7.3.0,>=7.2.0; extra == 'test'
-Requires-Dist: python-multipart==0.0.5; extra == 'test'
-Requires-Dist: ruff==0.0.215; extra == 'test'
-Requires-Dist: sqlmodel==0.0.8; extra == 'test'
+Requires-Dist: pytest<7.5.0,>=7.2.0; extra == 'test'
+Requires-Dist: python-multipart==0.0.6; extra == 'test'
+Requires-Dist: ruff==0.0.278; extra == 'test'
 Description-Content-Type: text/markdown
 
 # sqlalchemy-file
 
 
 **SQLAlchemy-file** is a [SQLAlchemy](https://www.sqlalchemy.org/) extension for attaching files to SQLAlchemy model and
 uploading them to various storage such as Local Storage, Amazon S3, Rackspace CloudFiles, Google Storage and others
@@ -150,26 +149,26 @@
 
     id = Column(Integer, autoincrement=True, primary_key=True)
     name = Column(String(50), unique=True)
     content = Column(FileField)
 
 
 # Configure Storage
-os.makedirs("/tmp/storage/attachment", 0o777, exist_ok=True)
-container = LocalStorageDriver("/tmp/storage").get_container("attachment")
+os.makedirs("./upload_dir/attachment", 0o777, exist_ok=True)
+container = LocalStorageDriver("./upload_dir").get_container("attachment")
 StorageManager.add_storage("default", container)
 
 # Save your model
 engine = create_engine(
     "sqlite:///example.db", connect_args={"check_same_thread": False}
 )
 Base.metadata.create_all(engine)
 
-with Session(engine) as session:
-    session.add(Attachment(name="attachment1", content=open("./example.txt", "rb")))
+with Session(engine) as session, open("./example.txt", "rb") as local_file:
+    session.add(Attachment(name="attachment1", content=local_file))
     session.add(Attachment(name="attachment2", content=b"Hello world"))
     session.add(Attachment(name="attachment3", content="Hello world"))
     file = File(content="Hello World", filename="hello.txt", content_type="text/plain")
     session.add(Attachment(name="attachment4", content=file))
     session.commit()
 
 ```
```

