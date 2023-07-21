# Comparing `tmp/miniscope_io-0.1.0.tar.gz` & `tmp/miniscope_io-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniscope_io-0.1.0.tar", max compression
+gzip compressed data, was "miniscope_io-0.1.2.tar", max compression
```

## Comparing `miniscope_io-0.1.0.tar` & `miniscope_io-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    34523 2023-06-27 01:14:55.751020 miniscope_io-0.1.0/LICENSE
--rw-r--r--   0        0        0      140 2023-06-27 01:18:46.012470 miniscope_io-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-24 00:50:21.943019 miniscope_io-0.1.0/miniscope_io/__init__.py
--rw-r--r--   0        0        0      169 2023-06-24 04:22:42.793243 miniscope_io-0.1.0/miniscope_io/exceptions.py
--rw-r--r--   0        0        0     2312 2023-06-27 19:57:24.223173 miniscope_io-0.1.0/miniscope_io/formats.py
--rw-r--r--   0        0        0    11981 2023-06-27 20:16:50.788244 miniscope_io-0.1.0/miniscope_io/io.py
--rw-r--r--   0        0        0     4106 2023-06-27 20:21:48.250019 miniscope_io-0.1.0/miniscope_io/sdcard.py
--rw-r--r--   0        0        0       52 2023-06-24 01:08:40.857671 miniscope_io-0.1.0/miniscope_io/widgets.py
--rw-r--r--   0        0        0      865 2023-06-27 20:18:06.932430 miniscope_io-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 miniscope_io-0.1.0/setup.py
--rw-r--r--   0        0        0      918 1970-01-01 00:00:00.000000 miniscope_io-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-28 19:52:23.218929 miniscope_io-0.1.2/LICENSE
+-rw-r--r--   0        0        0      140 2023-06-28 19:52:23.218997 miniscope_io-0.1.2/README.md
+-rw-r--r--   0        0        0       34 2023-07-21 17:58:59.024895 miniscope_io-0.1.2/miniscope_io/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-21 17:58:59.025040 miniscope_io-0.1.2/miniscope_io/exceptions.py
+-rw-r--r--   0        0        0     2311 2023-06-28 19:52:23.332968 miniscope_io-0.1.2/miniscope_io/formats.py
+-rw-r--r--   0        0        0    14540 2023-07-21 17:58:59.025238 miniscope_io-0.1.2/miniscope_io/io.py
+-rw-r--r--   0        0        0     4058 2023-06-28 19:52:23.333144 miniscope_io-0.1.2/miniscope_io/sdcard.py
+-rw-r--r--   0        0        0    12157 2023-07-21 17:58:59.025378 miniscope_io-0.1.2/miniscope_io/uart_daq.py
+-rw-r--r--   0        0        0       52 2023-06-28 19:52:23.333201 miniscope_io-0.1.2/miniscope_io/widgets.py
+-rw-r--r--   0        0        0      994 2023-07-21 18:30:28.518491 miniscope_io-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 miniscope_io-0.1.2/PKG-INFO
```

### Comparing `miniscope_io-0.1.0/LICENSE` & `miniscope_io-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miniscope_io-0.1.0/miniscope_io/formats.py` & `miniscope_io-0.1.2/miniscope_io/formats.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         height             = 1,
         fs                 = 2,
         buffer_size        = 3,
         n_buffers_recorded = 4,
         n_buffers_dropped  = 5
     ),
     buffer = BufferHeaderPositions(
-        length               = 10,
+        length               = 0,
         linked_list          = 1,
         frame_num            = 2,
         buffer_count         = 3,
         frame_buffer_count   = 4,
         write_buffer_count   = 5,
         dropped_buffer_count = 6,
         timestamp            = 7,
```

### Comparing `miniscope_io-0.1.0/miniscope_io/io.py` & `miniscope_io-0.1.2/miniscope_io/io.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 I/O functions for the SD card
 """
-from typing import Union, BinaryIO, Optional
+from typing import Union, BinaryIO, Optional, Tuple, List
 from pathlib import Path
 import warnings
 
 import numpy as np
 
 from miniscope_io.sdcard import SDLayout, SDConfig, DataHeader
-from miniscope_io.exceptions import InvalidSDException
-from miniscope_io.loggers import init_logger
+from miniscope_io.exceptions import InvalidSDException, EndOfRecordingException
+
 
 
 class SDCard:
     """
     I/O for data on an SDCard
 
     an instance of :class:`.sdcard.SDLayout` (typically in :mod:`.formats` ) configures how
@@ -36,30 +36,28 @@
         self.drive = Path(drive).resolve()
         self.layout = layout
 
         # Private attributes used when the file reading context is entered
         self._config = None  # type: Optional[SDConfig]
         self._f = None  # type: Optional[BinaryIO]
         self._frame = None  # type: Optional[int]
+        self._frame_count = None # type: Optional[int]
         self._array = None  # type: Optional[np.ndarray]
         """
         n_pix x 1 array used to store pixels while reading buffers
         """
         self.positions = {}
         """
         A mapping between frame number and byte position in the video that makes for faster seeking :)
         
         As we read, we store the locations of each frame before reading it. Later, we can assign to
         `frame` to seek back to those positions. Assigning to `frame` works without caching position, but
         has to manually iterate through each frame.
         """
 
-        self.logger = init_logger(self)
-        self.logger.debug("BOOTED UP")
-
 
 
         # this doesn't seem to be true anymore? but the WRITE_KEYs are still in
         # both the firmware and reading code, just unused?
         #if not self.check_valid():
         #    raise InvalidSDException(f"The SD card at path {str(self.drive)} does not have the correct WRITEKEYs in its header!")
 
@@ -133,41 +131,77 @@
             self._f.seek(self.layout.sectors.data_pos, 0)
             self._frame = 0
 
         if frame > self.frame:
             for i in range(frame - self.frame):
                 self.skip()
 
+    @property
+    def frame_count(self) -> int:
+        """
+        Total number of frames in recording.
+
+        Inferred from :class:`~.sdcard.SDConfig.n_buffers_recorded` and
+        reading a single frame to get the number of buffers per frame.
+        """
+        if self._frame_count is None:
+            if self._f is None:
+                with self as self_open:
+                    frame, headers = self_open.read(return_header=True)
+
+            else:
+                # If we're already open, great, just return to the last frame
+                last_frame = self.frame
+                frame, headers = self.read(return_header=True)
+                self.frame = last_frame
+
+            self._frame_count = int(np.ceil(
+                (self.config.n_buffers_recorded + self.config.n_buffers_dropped) / len(headers)
+            ))
+
+        # if we have since read more frames than should be there, we update the frame count with a warning
+        max_pos = np.max(list(self.positions.keys()))
+        if max_pos > self._frame_count:
+            warnings.warn(f'Got more frames than indicated in card header, expected {self._frame_count} but got {max_pos}')
+            self._frame_count = int(max_pos)
+
+        return self._frame_count
+
+
+
     # --------------------------------------------------
     # Context Manager methods
     # --------------------------------------------------
 
-    def __enter__(self):
+    def __enter__(self) -> 'SDCard':
         if self._f is not None:
             raise RuntimeError("Cant enter context, and open the file twice!")
 
-        self.logger.info('entered context')
-
         # init private attrs
         # create an empty frame to hold our data!
         self._array = np.zeros(
             (self.config.width * self.config.height, 1),
             dtype=np.uint8
         )
         self._pixel_count = 0
         self._last_buffer_n = 0
         self._frame = 0
 
         self._f = open(self.drive, 'rb')
         # seek to the start of the data
         self._f.seek(self.layout.sectors.data_pos, 0)
+        # store the 0th frame position
+        self.positions[0] = self.layout.sectors.data_pos
+
+        return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self._f.close()
         self._f = None
+        self._frame = 0
 
     # --------------------------------------------------
     # read methods
     # --------------------------------------------------
     def _read_data_header(self, sd:BinaryIO) -> DataHeader:
         """
         Given an already open file buffer opened in bytes mode,
@@ -235,54 +269,78 @@
         return data
 
     def _trim(self, data:np.ndarray, expected_size:int) -> np.ndarray:
         """
         Trim or pad an array to match an expected size
         """
         if data.shape[0] != expected_size:
-            self.logger.warning(
+            warnings.warn(
                 f"Expected buffer data length: {expected_size}, got data with shape {data.shape}. Padding to expected length")
 
             # trim if too long
             if data.shape[0] > expected_size:
                 data = data[0:expected_size]
             # pad if too short
             else:
                 data = np.pad(data, (0, expected_size - data.shape[0]))
 
         return data
 
-    def read(self) -> np.ndarray:
+    def read(self, return_header:bool=False) -> Union[np.ndarray, Tuple[np.ndarray, List[DataHeader]]]:
         """
         Read a single frame
+
+        Arguments:
+            return_header (bool): If `True`, return headers from individual buffers (default `False`)
+
+        Return:
+            :class:`numpy.ndarray` , or a tuple(ndarray, List[:class:`~.DataHeader`]) if `return_header` is `True`
         """
         if self._f is None:
             raise RuntimeError('File is not open! Try entering the reader context by using it like `with sdcard:`')
 
         self._array[:] = 0
         pixel_count = 0
         last_buffer_n = 0
+        headers = []
         while True:
             # stash position before reading header
             last_position = self._f.tell()
-            header = self._read_data_header(self._f)
-            if header is None:
-                # end of file!
-                raise StopIteration("Reached the end of the video!")
+            try:
+                header = self._read_data_header(self._f)
+            except ValueError as e:
+                if 'read length must be non-negative' in str(e):
+                    # end of file! Value error thrown because the dataHeader will be blank,
+                    # and thus have a value of 0 for the header size, and we can't read 0 from the card.
+                    self._f.seek(last_position, 0)
+                    raise EndOfRecordingException("Reached the end of the video!")
+                else:
+                    raise e
+            except IndexError as e:
+                if 'index 0 is out of bounds for axis 0 with size 0' in str(e):
+                    # end of file if we are reading from a disk image without any additional space on disk
+                    raise EndOfRecordingException("Reached the end of the video!")
+                else:
+                    raise e
 
             if header.frame_buffer_count == 0 and last_buffer_n > 0:
                 # we are in the next frame!
                 # rewind to the beginning of the header, and return
                 # the last_position is the start of the header for this frame
                 self._f.seek(last_position, 0)
                 self._frame += 1
                 self.positions[self._frame] = last_position
-                return np.reshape(self._array, (self.config.width, self.config.height))
+                frame = np.reshape(self._array, (self.config.width, self.config.height))
+                if return_header:
+                    return frame, headers
+                else:
+                    return frame
 
             # grab buffer data and stash
+            headers.append(header)
             data = self._read_buffer(self._f, header)
             data = self._trim(data, header.data_length)
             self._array[pixel_count:pixel_count + header.data_length, 0] = data
             pixel_count += header.data_length
             last_buffer_n = header.frame_buffer_count
 
     def skip(self):
```

### Comparing `miniscope_io-0.1.0/miniscope_io/sdcard.py` & `miniscope_io-0.1.2/miniscope_io/sdcard.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 Data model for configuring an SD card. Will be instantiated in the constants module with
 specific values. This allows for the model to be reused across different miniscopes, and
 for consuming code to use a consistent, introspectable API
 """
 from typing import Optional
 from pydantic import BaseModel
 
-from miniscope_io.loggers import init_logger
-
 class SectorConfig(BaseModel):
     """
     Configuration of sector layout on the SD card.
 
     For each sector, one can retrieve the position with the attribute *_pos,
 
     Examples:
@@ -39,16 +37,14 @@
     Recording data starts here
     """
     size: int = 512
     """
     The size of an individual sector
     """
 
-
-
     def __getattr__(self, item:str) -> int:
         """
         Get positions by multiplying by sector size
         (__getattr__ is only called if the name can't be found, so we don't need to handle
         the base case of the existing attributes)
         """
         split = item.split('_')
```

### Comparing `miniscope_io-0.1.0/pyproject.toml` & `miniscope_io-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "miniscope_io"
-version = "0.1.0"
+version = "0.1.2"
 description = ""
-authors = ["sneakers-the-rat <JLSaunders987@gmail.com>"]
+authors = [
+    "sneakers-the-rat <JLSaunders987@gmail.com>",
+    "t-sasatani <sasatani.dev@gmail.com>",
+]
 readme = "README.md"
 packages = [{include = "miniscope_io"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 opencv-python = "^4.7.0.72"
 numpy = "^1.25.0"
 pydantic = "^1.10.9"
 ipywidgets = "^8.0.6"
 jupyter = "^1.0.0"
 matplotlib = "^3.7.1"
-rich = "^13.4.2"
-parse = "^1.19.1"
+coloredlogs = "^15.0.1"
+pyserial = "^3.5"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 
 [tool.poetry.group.tests]
 optional = true
@@ -38,7 +41,10 @@
 [tool.poetry.extras]
 tests = ["pytest"]
 docs = ["sphinx", "furo", "myst-parser"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+uart_image_capture = "miniscope_io.uart_daq:main"
```

### Comparing `miniscope_io-0.1.0/PKG-INFO` & `miniscope_io-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: miniscope-io
-Version: 0.1.0
+Version: 0.1.2
 Summary: 
 Author: sneakers-the-rat
 Author-email: JLSaunders987@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Provides-Extra: tests
+Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
-Requires-Dist: parse (>=1.19.1,<2.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
-Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: pyserial (>=3.5,<4.0)
 Description-Content-Type: text/markdown
 
 # miniscope-io
 
 (Demonstration project for a lab workshop on making modular, testable python code.
 Functionality not guaranteed
 -<3 jonny)
```

