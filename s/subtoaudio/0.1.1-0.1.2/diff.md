# Comparing `tmp/subtoaudio-0.1.1.tar.gz` & `tmp/subtoaudio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtoaudio-0.1.1.tar", last modified: Mon Jul 17 23:08:57 2023, max compression
+gzip compressed data, was "subtoaudio-0.1.2.tar", last modified: Fri Jul 21 20:39:26 2023, max compression
```

## Comparing `subtoaudio-0.1.1.tar` & `subtoaudio-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 23:08:56.992974 subtoaudio-0.1.1/
--rw-rw-rw-   0        0        0    16725 2023-07-17 08:09:14.000000 subtoaudio-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2732 2023-07-17 23:08:56.992974 subtoaudio-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2084 2023-07-17 23:06:54.000000 subtoaudio-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 23:08:56.992974 subtoaudio-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-07-17 23:07:37.000000 subtoaudio-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 23:08:56.946174 subtoaudio-0.1.1/subtoaudio/
--rw-rw-rw-   0        0        0       34 2023-07-17 08:09:14.000000 subtoaudio-0.1.1/subtoaudio/__init__.py
--rw-rw-rw-   0        0        0     5037 2023-07-17 08:09:14.000000 subtoaudio-0.1.1/subtoaudio/subtoaudio.py
-drwxrwxrwx   0        0        0        0 2023-07-17 23:08:56.992974 subtoaudio-0.1.1/subtoaudio.egg-info/
--rw-rw-rw-   0        0        0     2732 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 20:39:26.888094 subtoaudio-0.1.2/
+-rw-rw-rw-   0        0        0    16725 2023-07-21 03:01:38.000000 subtoaudio-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2821 2023-07-21 20:39:26.883094 subtoaudio-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2163 2023-07-21 20:34:28.000000 subtoaudio-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-21 20:39:26.923094 subtoaudio-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      963 2023-07-21 20:35:59.000000 subtoaudio-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:39:26.823094 subtoaudio-0.1.2/subtoaudio/
+-rw-rw-rw-   0        0        0       34 2023-07-21 03:01:38.000000 subtoaudio-0.1.2/subtoaudio/__init__.py
+-rw-rw-rw-   0        0        0     5131 2023-07-21 03:01:38.000000 subtoaudio-0.1.2/subtoaudio/subtoaudio.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:39:26.878094 subtoaudio-0.1.2/subtoaudio.egg-info/
+-rw-rw-rw-   0        0        0     2821 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-21 20:39:25.000000 subtoaudio-0.1.2/subtoaudio.egg-info/top_level.txt
```

### Comparing `subtoaudio-0.1.1/LICENSE` & `subtoaudio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `subtoaudio-0.1.1/PKG-INFO` & `subtoaudio-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: subtoaudio
-Version: 0.1.1
-Summary: Generate audio or speech from any subtitle file
+Version: 0.1.2
+Summary: Subtitle to audio, generate speech from any subtitle file
 Home-page: https://github.com/bnsantoso/
 Author: Bagas NS
 Author-email: bagassantoso71@gmail.com
 License: MPL 2.0
 Keywords: subtitle,tts,text to audio,subtitle to audio,subtitle to speech
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/bnsantoso)
 
 # Subtitle to Audio
-Generate audio from any subtitle file using coqui-ai TTS.
+Subtitle to audio, generate audio from any subtitle file using Coqui-ai TTS and synchronize the audio timing according to subtitle time.
 
 ## Dependencies
 [ffmpeg](https://ffmpeg.org/), [pydub](https://github.com/jiaaro/pydub), [librosa](https://github.com/librosa/librosa), [coqui-ai TTS](https://github.com/coqui-ai/TTS/)
 
 ## Installation
 
 ```bash
```

### Comparing `subtoaudio-0.1.1/README.md` & `subtoaudio-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/bnsantoso)
 
 # Subtitle to Audio
-Generate audio from any subtitle file using coqui-ai TTS.
+Subtitle to audio, generate audio from any subtitle file using Coqui-ai TTS and synchronize the audio timing according to subtitle time.
 
 ## Dependencies
 [ffmpeg](https://ffmpeg.org/), [pydub](https://github.com/jiaaro/pydub), [librosa](https://github.com/librosa/librosa), [coqui-ai TTS](https://github.com/coqui-ai/TTS/)
 
 ## Installation
 
 ```bash
```

### Comparing `subtoaudio-0.1.1/setup.py` & `subtoaudio-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 with open("README.md", "r", encoding="utf-8") as readme_file:
     README = readme_file.read()
 
 setup(
     name="subtoaudio",
     packages=find_packages(exclude=[]),
-    version="0.1.1",
+    version="0.1.2",
     license="MPL 2.0",
-    description="Generate audio or speech from any subtitle file",
+    description="Subtitle to audio, generate speech from any subtitle file",
     author="Bagas NS",
     author_email="bagassantoso71@gmail.com",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bnsantoso/",
     install_requires=["TTS","pydub","librosa",],
     keywords=["subtitle", "tts", "text to audio", "subtitle to audio", "subtitle to speech",],
```

### Comparing `subtoaudio-0.1.1/subtoaudio/subtoaudio.py` & `subtoaudio-0.1.2/subtoaudio/subtoaudio.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,33 +58,36 @@
       pass
 
     if os.path.splitext(output_path)[1] != ".wav":
       output_path += ".wav"
 
     with tempfile.TemporaryDirectory() as temp_folder:
       print("Temporary folder:", temp_folder)
-      end_time = data[-1]['end_time']
-      base_duration = end_time + 10000
-      blank_base_audio = AudioSegment.silent(duration=base_duration)
 
       for entry_data in data:
         audio_path = f"{temp_folder}/{entry_data['audio_name']}"
         self.apitts.tts_to_file(f"{entry_data['text']}",
                                 file_path=audio_path,
                                 speaker=speaker,
                                 language=languages,
                                 speaker_wav=speaker_wav)
         audio_length = int(round(librosa.get_duration(path=audio_path),3) * 1000)
         entry_data['audio_length'] = audio_length
 
       for i in range(len(data)):
         if data[i]['audio_length'] > data[i]['sub_time']:
           shift_time = data[i]['audio_length'] - data[i]['sub_time'] + 50
-          data[i+1]['start_time'] += shift_time
-          data[i+1]['sub_time'] -= shift_time
+          if i + 1 < len(data):
+            data[i+1]['start_time'] += shift_time
+            data[i+1]['end_time'] += shift_time
+            data[i+1]['sub_time'] -= shift_time
+      
+      end_time = data[-1]['end_time']
+      base_duration = end_time + 10000
+      blank_base_audio = AudioSegment.silent(duration=base_duration)
 
       for entry_data in data:
         audio_path = f"{temp_folder}/{entry_data['audio_name']}"
         position = entry_data['start_time']
         overlay_audio = AudioSegment.from_file(audio_path)
         blank_base_audio = blank_base_audio.overlay(overlay_audio, position=position)
```

### Comparing `subtoaudio-0.1.1/subtoaudio.egg-info/PKG-INFO` & `subtoaudio-0.1.2/subtoaudio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: subtoaudio
-Version: 0.1.1
-Summary: Generate audio or speech from any subtitle file
+Version: 0.1.2
+Summary: Subtitle to audio, generate speech from any subtitle file
 Home-page: https://github.com/bnsantoso/
 Author: Bagas NS
 Author-email: bagassantoso71@gmail.com
 License: MPL 2.0
 Keywords: subtitle,tts,text to audio,subtitle to audio,subtitle to speech
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/bnsantoso)
 
 # Subtitle to Audio
-Generate audio from any subtitle file using coqui-ai TTS.
+Subtitle to audio, generate audio from any subtitle file using Coqui-ai TTS and synchronize the audio timing according to subtitle time.
 
 ## Dependencies
 [ffmpeg](https://ffmpeg.org/), [pydub](https://github.com/jiaaro/pydub), [librosa](https://github.com/librosa/librosa), [coqui-ai TTS](https://github.com/coqui-ai/TTS/)
 
 ## Installation
 
 ```bash
```

