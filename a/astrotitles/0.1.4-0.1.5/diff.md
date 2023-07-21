# Comparing `tmp/astrotitles-0.1.4.tar.gz` & `tmp/astrotitles-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrotitles-0.1.4.tar", last modified: Thu Jul 20 15:24:58 2023, max compression
+gzip compressed data, was "astrotitles-0.1.5.tar", last modified: Fri Jul 21 19:35:26 2023, max compression
```

## Comparing `astrotitles-0.1.4.tar` & `astrotitles-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:24:58.589514 astrotitles-0.1.4/
--rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1.4/LICENCE.txt
--rw-r--r--   0 ben        (501) staff       (20)     4596 2023-07-20 15:24:58.589586 astrotitles-0.1.4/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     4219 2023-07-20 15:20:44.000000 astrotitles-0.1.4/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:24:58.588636 astrotitles-0.1.4/astrotitles/
--rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1.4/astrotitles/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     1406 2023-07-20 15:21:10.000000 astrotitles-0.1.4/astrotitles/cli.py
--rw-r--r--   0 ben        (501) staff       (20)     2114 2023-07-20 15:11:23.000000 astrotitles-0.1.4/astrotitles/transcriber.py
--rw-r--r--   0 ben        (501) staff       (20)     1137 2023-07-20 13:42:14.000000 astrotitles-0.1.4/astrotitles/utils.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-20 15:24:58.589398 astrotitles-0.1.4/astrotitles.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     4596 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       52 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-20 15:24:58.000000 astrotitles-0.1.4/astrotitles.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-20 15:24:58.589829 astrotitles-0.1.4/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)      765 2023-07-20 15:24:12.000000 astrotitles-0.1.4/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-21 19:35:26.102488 astrotitles-0.1.5/
+-rw-r--r--   0 ben        (501) staff       (20)    34523 2023-07-19 22:08:12.000000 astrotitles-0.1.5/LICENCE.txt
+-rw-r--r--   0 ben        (501) staff       (20)     4701 2023-07-21 19:35:26.102573 astrotitles-0.1.5/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     4324 2023-07-21 19:22:36.000000 astrotitles-0.1.5/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-21 19:35:26.101386 astrotitles-0.1.5/astrotitles/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-07-19 22:07:36.000000 astrotitles-0.1.5/astrotitles/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     1422 2023-07-21 19:22:26.000000 astrotitles-0.1.5/astrotitles/cli.py
+-rw-r--r--   0 ben        (501) staff       (20)     2128 2023-07-21 19:29:40.000000 astrotitles-0.1.5/astrotitles/transcriber.py
+-rw-r--r--   0 ben        (501) staff       (20)     1145 2023-07-21 19:29:06.000000 astrotitles-0.1.5/astrotitles/utils.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-07-21 19:35:26.102374 astrotitles-0.1.5/astrotitles.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     4701 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      343 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       52 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)       20 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-07-21 19:35:26.000000 astrotitles-0.1.5/astrotitles.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       79 2023-07-21 19:35:26.102813 astrotitles-0.1.5/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)      765 2023-07-21 19:31:31.000000 astrotitles-0.1.5/setup.py
```

### Comparing `astrotitles-0.1.4/LICENCE.txt` & `astrotitles-0.1.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `astrotitles-0.1.4/PKG-INFO` & `astrotitles-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrotitles
-Version: 0.1.4
+Version: 0.1.5
 Summary: Automatically generate subtitles using the Astrotitles command line interface.
 Home-page: https://github.com/Astrotitles/cli
 Download-URL: https://github.com/Astrotitles/cli.git
 Author: Ben Webster
 License: AGPL-3.0
 Keywords: AI,Whisper AI,Subtitles
 Description-Content-Type: markdown
@@ -63,16 +63,16 @@
 The Astrotitles CLI is self-documented with ```--help``` content and examples for every command. You should start exploring the CLI by using the global ```--help``` option:
 
 ```sh
 astrotitles --help
 ```
 
 ```
-usage: astrotitles [-h] [--output OUTPUT] [--output-name OUTPUT_NAME]
-    [--max-chars MAX_CHARS] [--format FORMAT] [--model MODEL] input
+usage: astrotitles [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] 
+    [--format FORMAT] [--model MODEL] [--verbose VERBOSE] input
 
 Generate a srt/vtt subtitle file from audio/video file
 
 positional arguments:
   input                 Input audio/video file to be transcribed
 
 options:
@@ -80,14 +80,15 @@
   --output OUTPUT       Specify output directory for srt/vtt subtitle file
   --output-name OUTPUT_NAME
                         Specify output file name (no extension)
   --max-chars MAX_CHARS
                         Specify the maximum number of characters allowed per subtitle segment
   --format FORMAT       Specify subtitle format (default: .srt)
   --model MODEL         Whisper AI model to use for transcribing
+  --verbose VERBOSE     Print out progress of transcription process (default: True)
 
 Thanks for using Astrotitles CLI!
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1.4 Summary: Automatically
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.5 Summary: Automatically
 generate subtitles using the Astrotitles command line interface. Home-page:
 https://github.com/Astrotitles/cli Download-URL: https://github.com/
 Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
 AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
@@ -18,22 +18,23 @@
 via pip (github) ```sh pip install git+https://github.com/Astrotitles/cli.git
 ```
                                                                   (back_to_top)
  ## Usage The Astrotitles CLI is self-documented with ```--help``` content and
 examples for every command. You should start exploring the CLI by using the
 global ```--help``` option: ```sh astrotitles --help ``` ``` usage: astrotitles
 [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] [--
-format FORMAT] [--model MODEL] input Generate a srt/vtt subtitle file from
-audio/video file positional arguments: input Input audio/video file to be
-transcribed options: -h, --help show this help message and exit --output OUTPUT
-Specify output directory for srt/vtt subtitle file --output-name OUTPUT_NAME
-Specify output file name (no extension) --max-chars MAX_CHARS Specify the
-maximum number of characters allowed per subtitle segment --format FORMAT
-Specify subtitle format (default: .srt) --model MODEL Whisper AI model to use
-for transcribing Thanks for using Astrotitles CLI! ```
+format FORMAT] [--model MODEL] [--verbose VERBOSE] input Generate a srt/vtt
+subtitle file from audio/video file positional arguments: input Input audio/
+video file to be transcribed options: -h, --help show this help message and
+exit --output OUTPUT Specify output directory for srt/vtt subtitle file --
+output-name OUTPUT_NAME Specify output file name (no extension) --max-chars
+MAX_CHARS Specify the maximum number of characters allowed per subtitle segment
+--format FORMAT Specify subtitle format (default: .srt) --model MODEL Whisper
+AI model to use for transcribing --verbose VERBOSE Print out progress of
+transcription process (default: True) Thanks for using Astrotitles CLI! ```
                                                                   (back_to_top)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `astrotitles-0.1.4/README.md` & `astrotitles-0.1.5/astrotitles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: astrotitles
+Version: 0.1.5
+Summary: Automatically generate subtitles using the Astrotitles command line interface.
+Home-page: https://github.com/Astrotitles/cli
+Download-URL: https://github.com/Astrotitles/cli.git
+Author: Ben Webster
+License: AGPL-3.0
+Keywords: AI,Whisper AI,Subtitles
+Description-Content-Type: markdown
+License-File: LICENCE.txt
+
 <a name="readme-top"></a>
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
@@ -51,16 +63,16 @@
 The Astrotitles CLI is self-documented with ```--help``` content and examples for every command. You should start exploring the CLI by using the global ```--help``` option:
 
 ```sh
 astrotitles --help
 ```
 
 ```
-usage: astrotitles [-h] [--output OUTPUT] [--output-name OUTPUT_NAME]
-    [--max-chars MAX_CHARS] [--format FORMAT] [--model MODEL] input
+usage: astrotitles [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] 
+    [--format FORMAT] [--model MODEL] [--verbose VERBOSE] input
 
 Generate a srt/vtt subtitle file from audio/video file
 
 positional arguments:
   input                 Input audio/video file to be transcribed
 
 options:
@@ -68,14 +80,15 @@
   --output OUTPUT       Specify output directory for srt/vtt subtitle file
   --output-name OUTPUT_NAME
                         Specify output file name (no extension)
   --max-chars MAX_CHARS
                         Specify the maximum number of characters allowed per subtitle segment
   --format FORMAT       Specify subtitle format (default: .srt)
   --model MODEL         Whisper AI model to use for transcribing
+  --verbose VERBOSE     Print out progress of transcription process (default: True)
 
 Thanks for using Astrotitles CLI!
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
@@ -119,8 +132,8 @@
 [forks-shield]: https://img.shields.io/github/forks/Astrotitles/cli.svg?style=for-the-badge
 [forks-url]: https://github.com/Astrotitles/cli/network/members
 [stars-shield]: https://img.shields.io/github/stars/Astrotitles/cli.svg?style=for-the-badge
 [stars-url]: https://github.com/Astrotitles/cli/stargazers
 [issues-shield]: https://img.shields.io/github/issues/Astrotitles/cli.svg?style=for-the-badge
 [issues-url]: https://github.com/Astrotitles/cli/issues
 [license-shield]: https://img.shields.io/github/license/Astrotitles/cli.svg?style=for-the-badge
-[license-url]: https://github.com/Astrotitles/cli/blob/master/LICENSE.txt
+[license-url]: https://github.com/Astrotitles/cli/blob/master/LICENSE.txt
```

#### html2text {}

```diff
@@ -1,10 +1,15 @@
- [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![MIT License][license-shield]][license-url]
+Metadata-Version: 2.1 Name: astrotitles Version: 0.1.5 Summary: Automatically
+generate subtitles using the Astrotitles command line interface. Home-page:
+https://github.com/Astrotitles/cli Download-URL: https://github.com/
+Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
+AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
+[Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
+[forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
+[issues-url] [![MIT License][license-shield]][license-url]
                            **** Astrotitles CLI ****
 Automatically generate subtitles using the Astrotitles command line interface.
 
                  View_Web_App Â· Report_Bug Â· Request_Feature
 ## Getting Started Astrotitles CLI is a tool that allows you to generate a srt/
 vtt subtitle file from a audio/video file. Astrotitles has word-level
 timestamps, allowing you to control how many characters are in each subtitle
@@ -13,22 +18,23 @@
 via pip (github) ```sh pip install git+https://github.com/Astrotitles/cli.git
 ```
                                                                   (back_to_top)
  ## Usage The Astrotitles CLI is self-documented with ```--help``` content and
 examples for every command. You should start exploring the CLI by using the
 global ```--help``` option: ```sh astrotitles --help ``` ``` usage: astrotitles
 [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] [--
-format FORMAT] [--model MODEL] input Generate a srt/vtt subtitle file from
-audio/video file positional arguments: input Input audio/video file to be
-transcribed options: -h, --help show this help message and exit --output OUTPUT
-Specify output directory for srt/vtt subtitle file --output-name OUTPUT_NAME
-Specify output file name (no extension) --max-chars MAX_CHARS Specify the
-maximum number of characters allowed per subtitle segment --format FORMAT
-Specify subtitle format (default: .srt) --model MODEL Whisper AI model to use
-for transcribing Thanks for using Astrotitles CLI! ```
+format FORMAT] [--model MODEL] [--verbose VERBOSE] input Generate a srt/vtt
+subtitle file from audio/video file positional arguments: input Input audio/
+video file to be transcribed options: -h, --help show this help message and
+exit --output OUTPUT Specify output directory for srt/vtt subtitle file --
+output-name OUTPUT_NAME Specify output file name (no extension) --max-chars
+MAX_CHARS Specify the maximum number of characters allowed per subtitle segment
+--format FORMAT Specify subtitle format (default: .srt) --model MODEL Whisper
+AI model to use for transcribing --verbose VERBOSE Print out progress of
+transcription process (default: True) Thanks for using Astrotitles CLI! ```
                                                                   (back_to_top)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `astrotitles-0.1.4/astrotitles/cli.py` & `astrotitles-0.1.5/astrotitles/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     parser.add_argument("input", type=str, help="Input audio/video file to be transcribed")
 
     parser.add_argument("--output", type=str, default="./", help="Specify output directory for srt/vtt subtitle file")
     parser.add_argument("--output-name", type=str, help="Specify output file name (no extension)")
     parser.add_argument("--max-chars", type=checkPositive, help="Specify the maximum number of characters allowed per subtitle segment")
     parser.add_argument("--format", type=str, default="srt", choices=["srt", "vtt"], metavar="FORMAT", help="Specify subtitle format (default: .srt)")
     parser.add_argument("--model", type=str, default=Transcriber.defaultModel(), choices=Transcriber.availableModels(), metavar="MODEL", help="Whisper AI model to use for transcribing")
-    parser.add_argument("--verbose", type=str2bool, default=True, help="Print out progress of transcription process")
+    parser.add_argument("--verbose", type=str2bool, default=True, help="Print out progress of transcription process (default: True)")
 
     args = parser.parse_args().__dict__
 
     transcriber = Transcriber(args)
     transcriber.transcribe()
 
 if __name__ == "__main__":
```

### Comparing `astrotitles-0.1.4/astrotitles/transcriber.py` & `astrotitles-0.1.5/astrotitles/transcriber.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         warnings.filterwarnings("ignore")
         result = whisper.transcribe(model=model, audio=self.input, verbose=False)
         warnings.filterwarnings("default")
 
         outputFilePath = os.path.join(self.output, self.outputName)
 
         if os.path.exists(outputFilePath):
-            overrideOutputFilePrompt()
+            overrideOutputFilePrompt(outputFilePath)
 
 
         verbose(f"Writing subtitle file...", self.verbose)
         with open(outputFilePath, "w", encoding="utf-8") as outputFile:
             if self.format == "srt":
                 write_srt(self.getSubtitleData(result["segments"]), outputFile)
             else:
```

### Comparing `astrotitles-0.1.4/astrotitles/utils.py` & `astrotitles-0.1.5/astrotitles/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return f"subtitle_{str(time()).replace('.', '')}"
 
 
 def outputFileName(outputName: str, format: str) -> str:
     return f"{generateName() if outputName == None else outputName}.{format}"
 
 
-def verbose(msg: str, verbose: bool):
+def verbose(msg: str, verbose: bool) -> None:
     if (verbose):
         print(msg)
 
 
 def overrideOutputFilePrompt(outputFilePath: str) -> None:
     override = input("\nOutput file already exists. Override [y/n]: ")
```

### Comparing `astrotitles-0.1.4/astrotitles.egg-info/PKG-INFO` & `astrotitles-0.1.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: astrotitles
-Version: 0.1.4
-Summary: Automatically generate subtitles using the Astrotitles command line interface.
-Home-page: https://github.com/Astrotitles/cli
-Download-URL: https://github.com/Astrotitles/cli.git
-Author: Ben Webster
-License: AGPL-3.0
-Keywords: AI,Whisper AI,Subtitles
-Description-Content-Type: markdown
-License-File: LICENCE.txt
-
 <a name="readme-top"></a>
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
@@ -63,16 +51,16 @@
 The Astrotitles CLI is self-documented with ```--help``` content and examples for every command. You should start exploring the CLI by using the global ```--help``` option:
 
 ```sh
 astrotitles --help
 ```
 
 ```
-usage: astrotitles [-h] [--output OUTPUT] [--output-name OUTPUT_NAME]
-    [--max-chars MAX_CHARS] [--format FORMAT] [--model MODEL] input
+usage: astrotitles [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] 
+    [--format FORMAT] [--model MODEL] [--verbose VERBOSE] input
 
 Generate a srt/vtt subtitle file from audio/video file
 
 positional arguments:
   input                 Input audio/video file to be transcribed
 
 options:
@@ -80,14 +68,15 @@
   --output OUTPUT       Specify output directory for srt/vtt subtitle file
   --output-name OUTPUT_NAME
                         Specify output file name (no extension)
   --max-chars MAX_CHARS
                         Specify the maximum number of characters allowed per subtitle segment
   --format FORMAT       Specify subtitle format (default: .srt)
   --model MODEL         Whisper AI model to use for transcribing
+  --verbose VERBOSE     Print out progress of transcription process (default: True)
 
 Thanks for using Astrotitles CLI!
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
@@ -131,8 +120,8 @@
 [forks-shield]: https://img.shields.io/github/forks/Astrotitles/cli.svg?style=for-the-badge
 [forks-url]: https://github.com/Astrotitles/cli/network/members
 [stars-shield]: https://img.shields.io/github/stars/Astrotitles/cli.svg?style=for-the-badge
 [stars-url]: https://github.com/Astrotitles/cli/stargazers
 [issues-shield]: https://img.shields.io/github/issues/Astrotitles/cli.svg?style=for-the-badge
 [issues-url]: https://github.com/Astrotitles/cli/issues
 [license-shield]: https://img.shields.io/github/license/Astrotitles/cli.svg?style=for-the-badge
-[license-url]: https://github.com/Astrotitles/cli/blob/master/LICENSE.txt
+[license-url]: https://github.com/Astrotitles/cli/blob/master/LICENSE.txt
```

#### html2text {}

```diff
@@ -1,15 +1,10 @@
-Metadata-Version: 2.1 Name: astrotitles Version: 0.1.4 Summary: Automatically
-generate subtitles using the Astrotitles command line interface. Home-page:
-https://github.com/Astrotitles/cli Download-URL: https://github.com/
-Astrotitles/cli.git Author: Ben Webster License: AGPL-3.0 Keywords: AI,Whisper
-AI,Subtitles Description-Content-Type: markdown License-File: LICENCE.txt  [!
-[Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
-[forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
-[issues-url] [![MIT License][license-shield]][license-url]
+ [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
+shield]][issues-url] [![MIT License][license-shield]][license-url]
                            **** Astrotitles CLI ****
 Automatically generate subtitles using the Astrotitles command line interface.
 
                  View_Web_App Â· Report_Bug Â· Request_Feature
 ## Getting Started Astrotitles CLI is a tool that allows you to generate a srt/
 vtt subtitle file from a audio/video file. Astrotitles has word-level
 timestamps, allowing you to control how many characters are in each subtitle
@@ -18,22 +13,23 @@
 via pip (github) ```sh pip install git+https://github.com/Astrotitles/cli.git
 ```
                                                                   (back_to_top)
  ## Usage The Astrotitles CLI is self-documented with ```--help``` content and
 examples for every command. You should start exploring the CLI by using the
 global ```--help``` option: ```sh astrotitles --help ``` ``` usage: astrotitles
 [-h] [--output OUTPUT] [--output-name OUTPUT_NAME] [--max-chars MAX_CHARS] [--
-format FORMAT] [--model MODEL] input Generate a srt/vtt subtitle file from
-audio/video file positional arguments: input Input audio/video file to be
-transcribed options: -h, --help show this help message and exit --output OUTPUT
-Specify output directory for srt/vtt subtitle file --output-name OUTPUT_NAME
-Specify output file name (no extension) --max-chars MAX_CHARS Specify the
-maximum number of characters allowed per subtitle segment --format FORMAT
-Specify subtitle format (default: .srt) --model MODEL Whisper AI model to use
-for transcribing Thanks for using Astrotitles CLI! ```
+format FORMAT] [--model MODEL] [--verbose VERBOSE] input Generate a srt/vtt
+subtitle file from audio/video file positional arguments: input Input audio/
+video file to be transcribed options: -h, --help show this help message and
+exit --output OUTPUT Specify output directory for srt/vtt subtitle file --
+output-name OUTPUT_NAME Specify output file name (no extension) --max-chars
+MAX_CHARS Specify the maximum number of characters allowed per subtitle segment
+--format FORMAT Specify subtitle format (default: .srt) --model MODEL Whisper
+AI model to use for transcribing --verbose VERBOSE Print out progress of
+transcription process (default: True) Thanks for using Astrotitles CLI! ```
                                                                   (back_to_top)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `astrotitles-0.1.4/setup.py` & `astrotitles-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    version="0.1.4",
+    version="0.1.5",
     name="astrotitles",
     packages=find_packages(),
     license="AGPL-3.0",
     author="Ben Webster",
     url="https://github.com/Astrotitles/cli",
     download_url="https://github.com/Astrotitles/cli.git",
     keywords=["AI", "Whisper AI", "Subtitles"],
```

