# Comparing `tmp/ffmpeg_media_type-0.0.5.tar.gz` & `tmp/ffmpeg_media_type-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_media_type-0.0.5.tar", max compression
+gzip compressed data, was "ffmpeg_media_type-0.0.6.tar", max compression
```

## Comparing `ffmpeg_media_type-0.0.5.tar` & `ffmpeg_media_type-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1066 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/LICENSE
--rw-r--r--   0        0        0     4904 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/README.md
--rw-r--r--   0        0        0     1589 2023-07-14 21:03:14.467695 ffmpeg_media_type-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      186 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/__init__.py
--rw-r--r--   0        0        0    89367 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.2.json
--rw-r--r--   0        0        0    91003 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.3.json
--rw-r--r--   0        0        0    92339 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.4.json
--rw-r--r--   0        0        0    94852 2023-07-14 21:02:53.703172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.0.json
--rw-r--r--   0        0        0    95951 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.1.json
--rw-r--r--   0        0        0    97292 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.2.json
--rw-r--r--   0        0        0   100111 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.3.json
--rw-r--r--   0        0        0   106316 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.4.json
--rw-r--r--   0        0        0   107177 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-5.0.json
--rw-r--r--   0        0        0   109161 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-5.1.json
--rw-r--r--   0        0        0   120284 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-6.0.json
--rw-r--r--   0        0        0     3778 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/info.py
--rw-r--r--   0        0        0      378 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/main.py
--rw-r--r--   0        0        0        0 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/py.typed
--rw-r--r--   0        0        0        0 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/__init__.py
--rw-r--r--   0        0        0     5951 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/ffmpeg.py
--rw-r--r--   0        0        0     2977 2023-07-14 21:02:53.707172 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/table.py
--rw-r--r--   0        0        0     1790 2023-07-14 21:02:53.807174 ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/wiki_ext.py
--rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 ffmpeg_media_type-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4904 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/README.md
+-rw-r--r--   0        0        0     1589 2023-07-21 08:55:23.612316 ffmpeg_media_type-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      186 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/__init__.py
+-rw-r--r--   0        0        0      763 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/__init__.py
+-rw-r--r--   0        0        0    89367 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-3.2.json
+-rw-r--r--   0        0        0    91003 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-3.3.json
+-rw-r--r--   0        0        0    92339 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-3.4.json
+-rw-r--r--   0        0        0    94852 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.0.json
+-rw-r--r--   0        0        0    95951 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.1.json
+-rw-r--r--   0        0        0    97292 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.2.json
+-rw-r--r--   0        0        0   100111 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.3.json
+-rw-r--r--   0        0        0   106316 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.4.json
+-rw-r--r--   0        0        0   107177 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-5.0.json
+-rw-r--r--   0        0        0   109161 2023-07-21 08:55:00.459939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-5.1.json
+-rw-r--r--   0        0        0   120284 2023-07-21 08:55:00.463939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-6.0.json
+-rw-r--r--   0        0        0     3657 2023-07-21 08:55:00.463939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/info.py
+-rw-r--r--   0        0        0      378 2023-07-21 08:55:00.463939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 08:55:00.463939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/py.typed
+-rw-r--r--   0        0        0        0 2023-07-21 08:55:00.463939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/utils/__init__.py
+-rw-r--r--   0        0        0     6977 2023-07-21 08:55:00.463939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/utils/ffmpeg.py
+-rw-r--r--   0        0        0      431 2023-07-21 08:55:00.463939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/utils/shell.py
+-rw-r--r--   0        0        0     2977 2023-07-21 08:55:00.463939 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/utils/table.py
+-rw-r--r--   0        0        0     1790 2023-07-21 08:55:00.567941 ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/utils/wiki_ext.py
+-rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 ffmpeg_media_type-0.0.6/PKG-INFO
```

### Comparing `ffmpeg_media_type-0.0.5/LICENSE` & `ffmpeg_media_type-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/README.md` & `ffmpeg_media_type-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/pyproject.toml` & `ffmpeg_media_type-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffmpeg-media-type"
-version = "0.0.5"
+version = "0.0.6"
 description = "ffmpeg-media-type is a Python library that utilizes FFmpeg to extract crucial details from media files, such as duration, width, and height. With seamless integration of 100% typehint support, it offers a user-friendly interface for easy access to media file information."
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "ffmpeg_media_type", from = "src" }]
 include = ["ffmpeg_media_type/py.typed", "ffmpeg_media_type/data/*.json"]
 exclude = ["**/tests"]
 keywords = ["ffmpeg", "ffprobe", "video", "image", "audio", "media", "mimetype", "mp4", "mp3", "mov", "webm"]
```

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.2.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-3.2.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.3.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-3.3.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-3.4.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-3.4.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.0.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.1.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.2.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.2.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.3.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.3.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-4.4.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-4.4.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-5.0.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-5.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-5.1.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-5.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/data/ffmpeg-6.0.json` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/data/ffmpeg-6.0.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/info.py` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
-import subprocess
 from typing import Literal
 from urllib.parse import urlparse
 
 from pydantic import BaseModel
 
-from .utils.ffmpeg import FFProbeInfo, ffprobe, load_cache
+from .utils.ffmpeg import FFProbeInfo, ffprobe, get_ffmpeg, load_cache
+from .utils.shell import call
 
 
 class MediaInfo(BaseModel):
     type: Literal["image", "video", "audio"]
 
     width: int | None = None
     height: int | None = None
@@ -17,35 +17,30 @@
 
     format: str | None = None
     size: int | None = None
     suggest_ext: str | None = None
 
 
 def generate_thumbnail(video_path: str, thumbnail_path: str, time_offset: float = 0) -> str:
-    ffmpeg_cmd = [
-        "ffmpeg",  # FFmpeg command
+    ffmpeg_cmd = get_ffmpeg() + [
         "-y",  # Overwrite output file if it exists
         "-i",
         video_path,  # Input video path
         "-ss",
         str(time_offset),  # Time offset (seek to the specified position)
         "-vframes",
         "1",  # Number of frames to output
         "-vf",
         "scale=320:-1",  # Thumbnail size (width: 320, height: proportional)
         "-q:v",
         "2",  # Quality (2 - high, 5 - low)
         thumbnail_path,  # Output thumbnail path
     ]
 
-    try:
-        subprocess.check_output(ffmpeg_cmd, stderr=subprocess.STDOUT)
-    except subprocess.CalledProcessError as e:
-        print("Error generating thumbnail:", e.output)
-        raise
+    call(ffmpeg_cmd)
 
     return thumbnail_path
 
 
 def _extract_file_extension(uri: str) -> str:
     parsed_uri = urlparse(uri)
     path = parsed_uri.path
@@ -58,14 +53,15 @@
     "png_pipe": ["png"],
     "svg_pipe": ["svg"],
     "tiff_pipe": ["tiff", "tif"],
     "bmp_pipe": ["bmp"],
     "gif_pipe": ["gif"],
     "jpeg_pipe": ["jpeg", "jpg"],
     "webp_pipe": ["webp"],
+    "mjpeg": ["jpg", "jpeg", "mjpeg"],
 }
 
 
 def _guess_media_info(
     uri: str,
     info: FFProbeInfo,
 ) -> MediaInfo:
@@ -91,15 +87,15 @@
         suggest_ext = current_ext
     elif common_exts:
         suggest_ext = common_exts[0]
     else:
         suggest_ext = None
 
     # NOTE: we classify gif as image
-    if not duration or format_name == "gif":
+    if not duration or format_name in ("gif", "mjpeg"):
         return MediaInfo(
             type="image",
             width=info.streams[0].width or 0,
             height=info.streams[0].height or 0,
             duration=duration or 0,
             format=format_name,
             size=info.format.size,
```

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/ffmpeg.py` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/utils/ffmpeg.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 import os
 import re
-import subprocess
 from functools import lru_cache
 from pathlib import Path
-from typing import Any
+from typing import Any, Literal
 
 from pydantic import BaseModel, Field
 
+from .shell import call
+
 
 class FFProbeFormat(BaseModel):
     filename: str | None = None
     duration: float | None = None
     format_name: str | None = None
     format_long_name: str | None = None
     start_time: float | None = None
@@ -89,19 +90,35 @@
     muxer_info = {
         "common_exts": [],
         "mime_type": "",
         "default_video_codec": "",
         "default_audio_codec": "",
     }
     if "E" in flag:
-        os.system(f"docker run jrottenberg/ffmpeg:{version}-scratch -h muxer={codec} > output 2>&1")
-        muxer_info.update(_parse_muxer_info(open("output").read()))
+        text = call(
+            [
+                "docker",
+                "run",
+                f"jrottenberg/ffmpeg:{version}-scratch",
+                "-h",
+                f"muxer={codec}",
+            ]
+        )
+        muxer_info.update(_parse_muxer_info(text))
     if "D" in flag:
-        os.system(f"docker run jrottenberg/ffmpeg:{version}-scratch -h demuxer={codec} > output 2>&1")
-        muxer_info.update(_parse_muxer_info(open("output").read()))
+        text = call(
+            [
+                "docker",
+                "run",
+                f"jrottenberg/ffmpeg:{version}-scratch",
+                "-h",
+                f"demuxer={codec}",
+            ]
+        )
+        muxer_info.update(_parse_muxer_info(text))
 
     # print(f"{codec=}, {muxer_info=}")
     return FFMpegSupport(
         demuxing_support="D" in flag,
         muxing_support="E" in flag,
         codec=codec,
         description=description,
@@ -117,32 +134,29 @@
 
         if support_infos:
             output.append(support_infos[0])
     return output
 
 
 def list_support_format(version: str) -> list[FFMpegSupport]:
-    os.system(f"docker run jrottenberg/ffmpeg:{version}-scratch -formats > format.txt 2>&1")
-
-    with open("format.txt") as ifile:
-        content = ifile.read()
+    content = call(["docker", "run", f"jrottenberg/ffmpeg:{version}-scratch", "-formats"])
 
     # print(f"FFMpeg version: {version}")
 
     support_infos = _extract_file_format(content)
     output = []
     for support_info in support_infos:
         flag, codec, description = support_info
         output.append(_get_muxer_info(version, flag, codec, description))
 
     return output
 
 
 def _cache_file(version: str) -> str:
-    major_minor_version = ".".join(version.split(".")[:2])
+    major_minor_version = get_ffmpeg_version("minor")
     return str(Path(__file__).parent.parent / "data" / f"ffmpeg-{major_minor_version}.json")
 
 
 def _generate_cache(version: str) -> None:
     infos = list_support_format(version)
 
     with open(_cache_file(version), "w") as ofile:
@@ -160,40 +174,83 @@
     output = {}
     for info in _load_cache(ffmpeg_version):
         output[info.codec] = info
 
     return output
 
 
+def get_ffprobe() -> list[str]:
+    version = os.environ.get("FFMPEG_DOCKER_VERSION")
+    if version:
+        return [
+            "docker",
+            "run",
+            "--entrypoint",
+            "ffprobe",
+            "-v",
+            f"{Path.cwd()}:/work",
+            "-w",
+            "/work",
+            f"jrottenberg/ffmpeg:{version}-scratch",
+        ]
+    return ["ffprobe"]
+
+
+def get_ffmpeg() -> list[str]:
+    version = os.environ.get("FFMPEG_DOCKER_VERSION")
+    if version:
+        return [
+            "docker",
+            "run",
+            "--entrypoint",
+            "ffmpeg",
+            "-v",
+            f"{Path.cwd()}:/work",
+            "-w",
+            "/work",
+            f"jrottenberg/ffmpeg:{version}-scratch",
+        ]
+    return ["ffmpeg"]
+
+
 @lru_cache
-def get_ffmpeg_version() -> str:
+def get_ffmpeg_version(mode: Literal["major", "minor", "patch"] = "patch") -> str:
+    result = call(get_ffmpeg() + ["-version"])
+
     try:
-        result = subprocess.run(["ffmpeg", "-version"], capture_output=True, text=True)
-        output_lines = result.stdout.strip().split("\n")
-        version_line = output_lines[0].strip()
-        version = version_line.split(" ")[2]
-        return version
-    except FileNotFoundError as e:
-        raise FileNotFoundError("FFmpeg not found") from e
+        m_version = re.findall(r"ffmpeg version ([\d\.]+)", result)
+        assert len(m_version) == 1, m_version
+        version = m_version[0]
+
+        v_parts = version.split(".")
+        assert len(v_parts) <= 3, f"version format error: {version}"
+
+        v_parts += ["0"] * (3 - len(v_parts))
+
+        if mode == "patch":
+            v_parts = v_parts[:3]
+        elif mode == "minor":
+            v_parts = v_parts[:2]
+        else:
+            v_parts = v_parts[:1]
+
+        return ".".join(v_parts)
+
+    except IndexError as e:
+        raise RuntimeError(f"FFmpeg version not found {result}") from e
 
 
 def ffprobe(input_url: str) -> FFProbeInfo:
     # Construct the FFprobe command with JSON output format
-    ffprobe_cmd = [
-        "ffprobe",
+    ffprobe_cmd = get_ffprobe() + [
         "-v",
         "error",
         "-show_format",
         "-show_streams",
         "-of",
         "json",
         input_url,
     ]
 
-    try:
-        # Execute the FFprobe command and capture the output
-        output = subprocess.check_output(ffprobe_cmd, stderr=subprocess.STDOUT)
-        output_str = output.decode("utf-8")  # Convert bytes to string
-        return FFProbeInfo(**json.loads(output_str))
-    except subprocess.CalledProcessError as e:
-        # print(f"FFprobe error: {e.output}")
-        raise
+    # Execute the FFprobe command and capture the output
+    output = call(ffprobe_cmd)
+    return FFProbeInfo(**json.loads(output))
```

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/table.py` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/utils/table.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/src/ffmpeg_media_type/utils/wiki_ext.py` & `ffmpeg_media_type-0.0.6/src/ffmpeg_media_type/utils/wiki_ext.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_media_type-0.0.5/PKG-INFO` & `ffmpeg_media_type-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-media-type
-Version: 0.0.5
+Version: 0.0.6
 Summary: ffmpeg-media-type is a Python library that utilizes FFmpeg to extract crucial details from media files, such as duration, width, and height. With seamless integration of 100% typehint support, it offers a user-friendly interface for easy access to media file information.
 Keywords: ffmpeg,ffprobe,video,image,audio,media,mimetype,mp4,mp3,mov,webm
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

