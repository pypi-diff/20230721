# Comparing `tmp/assemblyai-0.8.1.tar.gz` & `tmp/assemblyai-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.8.1.tar", last modified: Fri Jun  9 14:51:54 2023, max compression
+gzip compressed data, was "assemblyai-0.9.0.tar", last modified: Tue Jun 13 19:40:46 2023, max compression
```

## Comparing `assemblyai-0.8.1.tar` & `assemblyai-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.189179 assemblyai-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 14:51:43.000000 assemblyai-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-06-09 14:51:54.189179 assemblyai-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13762 2023-06-09 14:51:43.000000 assemblyai-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.185179 assemblyai-0.8.1/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    48658 2023-06-09 14:51:43.000000 assemblyai-0.8.1/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.185179 assemblyai-0.8.1/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 14:51:54.000000 assemblyai-0.8.1/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:51:54.189179 assemblyai-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-09 14:51:43.000000 assemblyai-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.185179 assemblyai-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:54.189179 assemblyai-0.8.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_auto_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_content_safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_entity_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_sentiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-09 14:51:43.000000 assemblyai-0.8.1/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:40:46.558751 assemblyai-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 19:40:32.000000 assemblyai-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-06-13 19:40:46.558751 assemblyai-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-06-13 19:40:32.000000 assemblyai-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:40:46.554751 assemblyai-0.9.0/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-13 19:40:32.000000 assemblyai-0.9.0/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-13 19:40:32.000000 assemblyai-0.9.0/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-13 19:40:32.000000 assemblyai-0.9.0/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-13 19:40:32.000000 assemblyai-0.9.0/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23409 2023-06-13 19:40:32.000000 assemblyai-0.9.0/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49027 2023-06-13 19:40:32.000000 assemblyai-0.9.0/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:40:46.554751 assemblyai-0.9.0/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-06-13 19:40:46.000000 assemblyai-0.9.0/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-13 19:40:46.000000 assemblyai-0.9.0/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:40:46.000000 assemblyai-0.9.0/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 19:40:46.000000 assemblyai-0.9.0/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 19:40:46.000000 assemblyai-0.9.0/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:40:46.558751 assemblyai-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-13 19:40:32.000000 assemblyai-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:40:46.554751 assemblyai-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:40:46.558751 assemblyai-0.9.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_auto_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_auto_highlights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_content_safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_entity_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_iab_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_redact_pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_sentiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-13 19:40:32.000000 assemblyai-0.9.0/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.8.1/LICENSE` & `assemblyai-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/PKG-INFO` & `assemblyai-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.8.1
+Version: 0.9.0
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -266,15 +266,15 @@
 <details>
   <summary>PII Redact a Transcript</summary>
 
 ```python
 import assemblyai as aai
 
 config = aai.TranscriptionConfig()
-config.set_pii_redact(
+config.set_redact_pii(
   # What should be redacted
   policies=[
       aai.PIIRedactionPolicy.credit_card_number,
       aai.PIIRedactionPolicy.email_address,
       aai.PIIRedactionPolicy.location,
       aai.PIIRedactionPolicy.person_name,
       aai.PIIRedactionPolicy.phone_number,
@@ -283,14 +283,16 @@
   substitution=aai.PIISubstitutionPolicy.hash,
 )
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
 ```
 
+[Read more about PII redaction here.](https://www.assemblyai.com/docs/Models/pii_redaction)
+
 </details>
 <details>
   <summary>Summarize the content of a transcript over time</summary>
 
 ```python
 import assemblyai as aai
 
@@ -349,30 +351,30 @@
 transcript = transcriber.transcribe(
   "https://example.org/audio.mp3",
   config=aai.TranscriptionConfig(content_safety=True)
 )
 
 
 # Get the parts of the transcript which were flagged as sensitive
-for result in transcript.content_safety_labels.results:
+for result in transcript.content_safety.results:
   print(result.text)  # sensitive text snippet
   print(result.timestamp.start)
   print(result.timestamp.end)
 
   for label in result.labels:
     print(label.label)  # content safety category
     print(label.confidence) # model's confidence that the text is in this category
     print(label.severity) # severity of the text in relation to the category
 
 # Get the confidence of the most common labels in relation to the entire audio file
-for label, confidence in transcript.content_safety_labels.summary.items():
+for label, confidence in transcript.content_safety.summary.items():
   print(f"{confidence * 100}% confident that the audio contains {label}")
 
 # Get the overall severity of the most common labels in relation to the entire audio file
-for label, severity_confidence in transcript.content_safety_labels.severity_score_summary.items():
+for label, severity_confidence in transcript.content_safety.severity_score_summary.items():
   print(f"{severity_confidence.low * 100}% confident that the audio contains low-severity {label}")
   print(f"{severity_confidence.medium * 100}% confident that the audio contains mid-severity {label}")
   print(f"{severity_confidence.high * 100}% confident that the audio contains high-severity {label}")
 
 ```
 
 [Read more about the content safety categories.](https://www.assemblyai.com/docs/Models/content_moderation#all-labels-supported-by-the-model)
@@ -395,15 +397,15 @@
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe(
   "https://example.org/audio.mp3",
   config=aai.TranscriptionConfig(sentiment_analysis=True)
 )
 
-for sentiment_result in transcript.sentiment_analysis_results:
+for sentiment_result in transcript.sentiment_analysis:
   print(sentiment_result.text)
   print(sentiment_result.sentiment)  # POSITIVE, NEUTRAL, or NEGATIVE
   print(sentiment_result.confidence)
   print(f"Timestamp: {sentiment_result.timestamp.start} - {sentiment_result.timestamp.end}")
 ```
 
 If `speaker_labels` is also enabled, then each sentiment analysis result will also include a `speaker` field.
@@ -411,15 +413,15 @@
 ```python
 # ...
 
 config = aai.TranscriptionConfig(sentiment_analysis=True, speaker_labels=True)
 
 # ...
 
-for sentiment_result in transcript.sentiment_analysis_results:
+for sentiment_result in transcript.sentiment_analysis:
   print(sentiment_result.speaker)
 ```
 
 [Read more about sentiment analysis here.](https://www.assemblyai.com/docs/Models/sentiment_analysis)
 
 </details>
 <details>
@@ -439,14 +441,66 @@
   print(entity.type) # i.e. EntityType.person
   print(f"Timestamp: {entity.start} - {entity.end}")
 ```
 
 [Read more about entity detection here.](https://www.assemblyai.com/docs/Models/entity_detection)
 
 </details>
+<details>
+  <summary>Detect Topics in a Transcript (IAB Classification)</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(iab_categories=True)
+)
+
+# Get the parts of the transcript that were tagged with topics
+for result in transcript.iab_categories.results:
+  print(result.text)
+  print(f"Timestamp: {result.timestamp.start} - {result.timestamp.end}")
+  for label in result.labels:
+    print(label.label)  # topic
+    print(label.relevance)  # how relevant the label is for the portion of text
+
+# Get a summary of all topics in the transcript
+for label, relevance in transcript.iab_categories.summary.items():
+  print(f"Audio is {relevance * 100}% relevant to {label}")
+```
+
+[Read more about IAB classification here.](https://www.assemblyai.com/docs/Models/iab_classification)
+
+</details>
+<details>
+  <summary>Identify Important Words and Phrases in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(auto_highlights=True)
+)
+
+for result in transcript.auto_highlights.results:
+  print(result.text) # the important phrase
+  print(result.rank) # relevancy of the phrase
+  print(result.count) # number of instances of the phrase
+  for timestamp in result.timestamps:
+    print(f"Timestamp: {timestamp.start} - {timestamp.end}")
+
+```
+
+[Read more about auto highlights here.](https://www.assemblyai.com/docs/Models/key_phrases)
+
+</details>
 
 ---
 
 ## Playgrounds
 
 Visit one of our Playgrounds:
 
@@ -503,7 +557,17 @@
 Currently, the SDK provides two ways to transcribe audio files.
 
 The synchronous approach halts the application's flow until the transcription has been completed.
 
 The asynchronous approach allows the application to continue running while the transcription is being processed. The caller receives a [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html) object which can be used to check the status of the transcription at a later time.
 
 You can identify those two approaches by the `_async` suffix in the `Transcriber`'s method name (e.g. `transcribe` vs `transcribe_async`).
+
+## Polling Intervals
+
+By default we poll the `Transcript`'s status each `3s`. In case you would like to adjust that interval:
+
+```python
+import assemblyai as aai
+
+aai.settings.polling_interval = 1.0
+```
```

### Comparing `assemblyai-0.8.1/README.md` & `assemblyai-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 <details>
   <summary>PII Redact a Transcript</summary>
 
 ```python
 import assemblyai as aai
 
 config = aai.TranscriptionConfig()
-config.set_pii_redact(
+config.set_redact_pii(
   # What should be redacted
   policies=[
       aai.PIIRedactionPolicy.credit_card_number,
       aai.PIIRedactionPolicy.email_address,
       aai.PIIRedactionPolicy.location,
       aai.PIIRedactionPolicy.person_name,
       aai.PIIRedactionPolicy.phone_number,
@@ -253,14 +253,16 @@
   substitution=aai.PIISubstitutionPolicy.hash,
 )
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
 ```
 
+[Read more about PII redaction here.](https://www.assemblyai.com/docs/Models/pii_redaction)
+
 </details>
 <details>
   <summary>Summarize the content of a transcript over time</summary>
 
 ```python
 import assemblyai as aai
 
@@ -319,30 +321,30 @@
 transcript = transcriber.transcribe(
   "https://example.org/audio.mp3",
   config=aai.TranscriptionConfig(content_safety=True)
 )
 
 
 # Get the parts of the transcript which were flagged as sensitive
-for result in transcript.content_safety_labels.results:
+for result in transcript.content_safety.results:
   print(result.text)  # sensitive text snippet
   print(result.timestamp.start)
   print(result.timestamp.end)
 
   for label in result.labels:
     print(label.label)  # content safety category
     print(label.confidence) # model's confidence that the text is in this category
     print(label.severity) # severity of the text in relation to the category
 
 # Get the confidence of the most common labels in relation to the entire audio file
-for label, confidence in transcript.content_safety_labels.summary.items():
+for label, confidence in transcript.content_safety.summary.items():
   print(f"{confidence * 100}% confident that the audio contains {label}")
 
 # Get the overall severity of the most common labels in relation to the entire audio file
-for label, severity_confidence in transcript.content_safety_labels.severity_score_summary.items():
+for label, severity_confidence in transcript.content_safety.severity_score_summary.items():
   print(f"{severity_confidence.low * 100}% confident that the audio contains low-severity {label}")
   print(f"{severity_confidence.medium * 100}% confident that the audio contains mid-severity {label}")
   print(f"{severity_confidence.high * 100}% confident that the audio contains high-severity {label}")
 
 ```
 
 [Read more about the content safety categories.](https://www.assemblyai.com/docs/Models/content_moderation#all-labels-supported-by-the-model)
@@ -365,15 +367,15 @@
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe(
   "https://example.org/audio.mp3",
   config=aai.TranscriptionConfig(sentiment_analysis=True)
 )
 
-for sentiment_result in transcript.sentiment_analysis_results:
+for sentiment_result in transcript.sentiment_analysis:
   print(sentiment_result.text)
   print(sentiment_result.sentiment)  # POSITIVE, NEUTRAL, or NEGATIVE
   print(sentiment_result.confidence)
   print(f"Timestamp: {sentiment_result.timestamp.start} - {sentiment_result.timestamp.end}")
 ```
 
 If `speaker_labels` is also enabled, then each sentiment analysis result will also include a `speaker` field.
@@ -381,15 +383,15 @@
 ```python
 # ...
 
 config = aai.TranscriptionConfig(sentiment_analysis=True, speaker_labels=True)
 
 # ...
 
-for sentiment_result in transcript.sentiment_analysis_results:
+for sentiment_result in transcript.sentiment_analysis:
   print(sentiment_result.speaker)
 ```
 
 [Read more about sentiment analysis here.](https://www.assemblyai.com/docs/Models/sentiment_analysis)
 
 </details>
 <details>
@@ -409,14 +411,66 @@
   print(entity.type) # i.e. EntityType.person
   print(f"Timestamp: {entity.start} - {entity.end}")
 ```
 
 [Read more about entity detection here.](https://www.assemblyai.com/docs/Models/entity_detection)
 
 </details>
+<details>
+  <summary>Detect Topics in a Transcript (IAB Classification)</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(iab_categories=True)
+)
+
+# Get the parts of the transcript that were tagged with topics
+for result in transcript.iab_categories.results:
+  print(result.text)
+  print(f"Timestamp: {result.timestamp.start} - {result.timestamp.end}")
+  for label in result.labels:
+    print(label.label)  # topic
+    print(label.relevance)  # how relevant the label is for the portion of text
+
+# Get a summary of all topics in the transcript
+for label, relevance in transcript.iab_categories.summary.items():
+  print(f"Audio is {relevance * 100}% relevant to {label}")
+```
+
+[Read more about IAB classification here.](https://www.assemblyai.com/docs/Models/iab_classification)
+
+</details>
+<details>
+  <summary>Identify Important Words and Phrases in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(auto_highlights=True)
+)
+
+for result in transcript.auto_highlights.results:
+  print(result.text) # the important phrase
+  print(result.rank) # relevancy of the phrase
+  print(result.count) # number of instances of the phrase
+  for timestamp in result.timestamps:
+    print(f"Timestamp: {timestamp.start} - {timestamp.end}")
+
+```
+
+[Read more about auto highlights here.](https://www.assemblyai.com/docs/Models/key_phrases)
+
+</details>
 
 ---
 
 ## Playgrounds
 
 Visit one of our Playgrounds:
 
@@ -473,7 +527,17 @@
 Currently, the SDK provides two ways to transcribe audio files.
 
 The synchronous approach halts the application's flow until the transcription has been completed.
 
 The asynchronous approach allows the application to continue running while the transcription is being processed. The caller receives a [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html) object which can be used to check the status of the transcription at a later time.
 
 You can identify those two approaches by the `_async` suffix in the `Transcriber`'s method name (e.g. `transcribe` vs `transcribe_async`).
+
+## Polling Intervals
+
+By default we poll the `Transcript`'s status each `3s`. In case you would like to adjust that interval:
+
+```python
+import assemblyai as aai
+
+aai.settings.polling_interval = 1.0
+```
```

### Comparing `assemblyai-0.8.1/assemblyai/__init__.py` & `assemblyai-0.9.0/assemblyai/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 from .client import Client
 from .lemur import Lemur
 from .transcriber import Transcriber, Transcript, TranscriptGroup
 from .types import (
     AssemblyAIError,
+    AutohighlightResponse,
+    AutohighlightResult,
+    Chapter,
+    ContentSafetyLabel,
+    ContentSafetyLabelResult,
+    ContentSafetyResponse,
+    ContentSafetySeverityScore,
+    Entity,
+    EntityType,
+    IABLabelResult,
+    IABResponse,
+    IABResult,
     LanguageCode,
     LemurError,
     LemurModel,
     LemurQuestion,
     LemurQuestionResult,
     Paragraph,
     PIIRedactionPolicy,
     PIISubstitutionPolicy,
     RawTranscriptionConfig,
     Sentence,
+    Sentiment,
+    SentimentType,
     Settings,
+    StatusResult,
     SummarizationModel,
     SummarizationType,
     Timestamp,
     TranscriptError,
     TranscriptionConfig,
     TranscriptStatus,
     Utterance,
@@ -30,23 +45,40 @@
 settings = Settings()
 """Global settings object that applies to all classes that use the `Client` class."""
 
 
 __all__ = [
     # types
     "AssemblyAIError",
+    "AutohighlightResponse",
+    "AutohighlightResult",
+    "Chapter",
     "Client",
+    "ContentSafetyLabel",
+    "ContentSafetyLabelResult",
+    "ContentSafetyResponse",
+    "ContentSafetySeverityScore",
+    "Entity",
+    "EntityType",
+    "IABLabelResult",
+    "IABResponse",
+    "IABResult",
     "LanguageCode",
     "Lemur",
     "LemurError",
     "LemurModel",
     "LemurQuestion",
     "LemurQuestionResult",
+    "PIIRedactionPolicy",
+    "PIISubstitutionPolicy",
     "Sentence",
+    "Sentiment",
+    "SentimentType",
     "Settings",
+    "StatusResult",
     "SummarizationModel",
     "SummarizationType",
     "Timestamp",
     "Transcriber",
     "TranscriptionConfig",
     "Transcript",
     "TranscriptError",
```

### Comparing `assemblyai-0.8.1/assemblyai/api.py` & `assemblyai-0.9.0/assemblyai/api.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/assemblyai/client.py` & `assemblyai-0.9.0/assemblyai/client.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/assemblyai/lemur.py` & `assemblyai-0.9.0/assemblyai/lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/assemblyai/transcriber.py` & `assemblyai-0.9.0/assemblyai/transcriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,29 +208,49 @@
     def summary(self) -> Optional[str]:
         "The summarization of the transcript"
 
         return self._impl.transcript.summary
 
     @property
     def chapters(self) -> Optional[List[types.Chapter]]:
+        "The list of auto-chapters results"
+
         return self._impl.transcript.chapters
 
     @property
-    def content_safety_labels(self) -> Optional[types.ContentSafetyResponse]:
+    def content_safety(self) -> Optional[types.ContentSafetyResponse]:
+        "The results from the content safety analysis"
+
         return self._impl.transcript.content_safety_labels
 
     @property
-    def sentiment_analysis_results(self) -> Optional[List[types.Sentiment]]:
+    def sentiment_analysis(self) -> Optional[List[types.Sentiment]]:
+        "The list of sentiment analysis results"
+
         return self._impl.transcript.sentiment_analysis_results
 
     @property
     def entities(self) -> Optional[List[types.Entity]]:
+        "The list of entity detection results"
+
         return self._impl.transcript.entities
 
     @property
+    def iab_categories(self) -> Optional[types.IABResponse]:
+        "The results from the IAB category detection"
+
+        return self._impl.transcript.iab_categories_result
+
+    @property
+    def auto_highlights(self) -> Optional[types.AutohighlightResponse]:
+        "The results from the auto-highlights model"
+
+        return self._impl.transcript.auto_highlights_result
+
+    @property
     def status(self) -> types.TranscriptStatus:
         "The current status of the transcript"
 
         return self._impl.transcript.status
 
     @property
     def error(self) -> Optional[str]:
```

### Comparing `assemblyai-0.8.1/assemblyai/types.py` & `assemblyai-0.9.0/assemblyai/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
-from pydantic import BaseModel, BaseSettings, Extra
+from pydantic import BaseModel, BaseSettings, Extra, Field
 from typing_extensions import Self
 
 
 class AssemblyAIError(Exception):
     """
     Base exception for all AssemblyAI errors
     """
@@ -33,15 +33,15 @@
 
     http_timeout: float = 15.0
     "The default HTTP timeout for general requests"
 
     base_url: str = "https://api.assemblyai.com/v2"
     "The base URL for the AssemblyAI API"
 
-    polling_interval: float = 1.0
+    polling_interval: float = Field(default=3.0, gte=0.1)
     "The default polling interval for long-running requests (e.g. polling the `Transcript`'s status)"
 
     class Config:
         env_prefix = "assemblyai_"
 
 
 class TranscriptStatus(str, Enum):
@@ -344,16 +344,16 @@
 
     content_safety: Optional[bool]
     "Enable Content Safety Detection."
 
     content_safety_confidence: Optional[int]
     "The minimum confidence level for a content safety label to be produced."
 
-    # iab_categories: bool = False
-    # "Enable Topic Detection."
+    iab_categories: Optional[bool]
+    "Enable Topic Detection."
 
     custom_spelling: Optional[List[Dict[str, List[str]]]]
     "Customize how words are spelled and formatted using to and from values"
 
     disfluencies: Optional[bool]
     "Transcribe Filler Words, like 'umm', in your media file."
 
@@ -369,16 +369,16 @@
     summarization: Optional[bool]
     "Enable Summarization"
     summary_model: Optional[SummarizationModel]
     "The summarization model to use in case `summarization` is enabled"
     summary_type: Optional[SummarizationType]
     "The summarization type to use in case `summarization` is enabled"
 
-    # auto_highlights: bool = False
-    # "Detect important phrases and words in your transcription text."
+    auto_highlights: Optional[bool]
+    "Detect important phrases and words in your transcription text."
 
     language_detection: Optional[bool]
     """
     Identify the dominant language that's spoken in an audio file, and route the file to the appropriate model for the detected language.
 
     Automatic Language Detection is supported for the following languages:
 
@@ -408,30 +408,30 @@
         audio_start_from: Optional[int] = None,
         audio_end_at: Optional[int] = None,
         word_boost: List[str] = [],
         boost_param: Optional[WordBoost] = None,
         filter_profanity: Optional[bool] = None,
         redact_pii: Optional[bool] = None,
         redact_pii_audio: Optional[bool] = None,
-        redact_pii_policies: Optional[PIIRedactionPolicy] = None,
+        redact_pii_policies: Optional[List[PIIRedactionPolicy]] = None,
         redact_pii_sub: Optional[PIISubstitutionPolicy] = None,
         speaker_labels: Optional[bool] = None,
         speakers_expected: Optional[int] = None,
         content_safety: Optional[bool] = None,
         content_safety_confidence: Optional[int] = None,
-        # iab_categories: bool = False,
+        iab_categories: Optional[bool] = None,
         custom_spelling: Optional[Dict[str, Union[str, Sequence[str]]]] = None,
         disfluencies: Optional[bool] = None,
         sentiment_analysis: Optional[bool] = None,
         auto_chapters: Optional[bool] = None,
         entity_detection: Optional[bool] = None,
         summarization: Optional[bool] = None,
         summary_model: Optional[SummarizationModel] = None,
         summary_type: Optional[SummarizationType] = None,
-        # auto_highlights: bool = False,
+        auto_highlights: Optional[bool] = None,
         language_detection: Optional[bool] = None,
         raw_transcription_config: Optional[RawTranscriptionConfig] = None,
     ) -> None:
         """
         Args:
             language_code: The language of your audio file. Possible values are found in Supported Languages.
             punctuate: Enable Automatic Punctuation
@@ -442,15 +442,15 @@
             webhook_auth_header_value: The value of the `webhook_auth_header_name` that is sent when the `webhoook_url` is being called.
             audio_start_from: The point in time, in milliseconds, to begin transcription from in your media file.
             audio_end_at: The point in time, in milliseconds, to stop transcribing in your media file.
             word_boost: A list of custom vocabulary to boost accuracy for.
             boost_param: The weight to apply to words/phrases in the word_boost array.
             filter_profanity: Filter profanity from the transcribed text.
             redact_pii: Redact PII from the transcribed text.
-            redact_pii_audio: Generate a copy of the original media file with spoken PII 'beeped' out.
+            redact_pii_audio: Generate a copy of the original media file with spoken PII 'beeped' out (new audio only available for 24 hours).
             redact_pii_policies: The list of PII Redaction policies to enable.
             redact_pii_sub: The replacement logic for detected PII.
             speaker_labels: Enable Speaker Diarization.
             speakers_expected: The number of speakers you expect to hear in your audio file. Up to 10 speakers are supported.
             content_safety: Enable Content Safety Detection.
             iab_categories: Enable Topic Detection.
             custom_spelling: Customize how words are spelled and formatted using to and from values.
@@ -490,26 +490,26 @@
             redact_pii,
             redact_pii_audio,
             redact_pii_policies,
             redact_pii_sub,
         )
         self.set_speaker_diarization(speaker_labels, speakers_expected)
         self.set_content_safety(content_safety, content_safety_confidence)
-        # self.iab_categories = iab_categories
+        self.iab_categories = iab_categories
         self.set_custom_spelling(custom_spelling, override=True)
         self.disfluencies = disfluencies
         self.sentiment_analysis = sentiment_analysis
         self.auto_chapters = auto_chapters
         self.entity_detection = entity_detection
         self.set_summarize(
             summarization,
             summary_model,
             summary_type,
         )
-        # self.auto_highlights = auto_highlights
+        self.auto_highlights = auto_highlights
         self.language_detection = language_detection
 
     @property
     def raw(self) -> RawTranscriptionConfig:
         return self._raw_transcription_config
 
     # region: Getters/Setters
@@ -693,25 +693,25 @@
         self._raw_transcription_config.content_safety = enable
         self._raw_transcription_config.content_safety_confidence = (
             content_safety_confidence
         )
 
         return self
 
-    # @property
-    # def iab_categories(self) -> bool:
-    #     "Returns the status of the Topic Detection feature."
+    @property
+    def iab_categories(self) -> Optional[bool]:
+        "Returns the status of the Topic Detection feature."
 
-    #     return self._raw_transcription_config.iab_categories
+        return self._raw_transcription_config.iab_categories
 
-    # @iab_categories.setter
-    # def iab_categories(self, enable: bool) -> None:
-    #     "Enable Topic Detection feature."
+    @iab_categories.setter
+    def iab_categories(self, enable: Optional[bool]) -> None:
+        "Enable Topic Detection feature."
 
-    #     self._raw_transcription_config.iab_categories = enable
+        self._raw_transcription_config.iab_categories = enable
 
     @property
     def custom_spelling(self) -> Optional[Dict[str, List[str]]]:
         "Returns the current set custom spellings."
 
         if self._raw_transcription_config.custom_spelling is None:
             return None
@@ -792,25 +792,25 @@
 
     @property
     def summary_type(self) -> Optional[SummarizationType]:
         "Returns the type of the Summarization feature."
 
         return self._raw_transcription_config.summary_type
 
-    # @property
-    # def auto_highlights(self) -> bool:
-    #     "Returns whether the Auto Highlights feature is enabled or not."
+    @property
+    def auto_highlights(self) -> Optional[bool]:
+        "Returns whether the Auto Highlights feature is enabled or not."
 
-    #     return self._raw_transcription_config.auto_highlights
+        return self._raw_transcription_config.auto_highlights
 
-    # @auto_highlights.setter
-    # def auto_highlights(self, enable: bool) -> None:
-    #     "Detect important phrases and words in your transcription text."
+    @auto_highlights.setter
+    def auto_highlights(self, enable: Optional[bool]) -> None:
+        "Detect important phrases and words in your transcription text."
 
-    #     self._raw_transcription_config.auto_highlights = enable
+        self._raw_transcription_config.auto_highlights = enable
 
     @property
     def language_detection(self) -> Optional[bool]:
         "Returns whether Automatic Language Detection is enabled or not."
 
         return self._raw_transcription_config.language_detection
 
@@ -955,37 +955,40 @@
         self._raw_transcription_config.word_boost = words
         self._raw_transcription_config.boost_param = boost
 
         return self
 
     def set_redact_pii(
         self,
-        enable: bool = True,
-        redact_audio: bool = False,
-        policies: List[PIIRedactionPolicy] = [],
-        substitution: PIISubstitutionPolicy = PIISubstitutionPolicy.hash,
+        enable: Optional[bool] = True,
+        redact_audio: Optional[bool] = None,
+        policies: Optional[List[PIIRedactionPolicy]] = None,
+        substitution: Optional[PIISubstitutionPolicy] = None,
     ) -> Self:
         """
         Enables Personal Identifiable Information (PII) Redaction feature.
 
         Args:
             enable: whether to enable or disable the PII Redaction feature.
-            redact_audio: Generate a copy of the original media file with spoken PII 'beeped' out.
+            redact_audio: Generate a copy of the original media file with spoken PII 'beeped' out. NOTE: The copy is available for 24h
             policies: A list of PII redaction policies to enable.
             substitution: The replacement logic for detected PII (`PIISubstutionPolicy.hash` by default).
         """
 
         if not enable:
             self._raw_transcription_config.redact_pii = None
             self._raw_transcription_config.redact_pii_audio = None
             self._raw_transcription_config.redact_pii_policies = None
             self._raw_transcription_config.redact_pii_sub = None
 
             return self
 
+        if not policies:
+            raise ValueError("You must provide at least one PII redaction policy.")
+
         self._raw_transcription_config.redact_pii = True
         self._raw_transcription_config.redact_pii_audio = redact_audio
         self._raw_transcription_config.redact_pii_policies = policies
         self._raw_transcription_config.redact_pii_sub = substitution
 
         return self
 
@@ -1354,16 +1357,16 @@
 
     content_safety: Optional[bool]
     "Enable Content Safety Detection."
 
     content_safety_confidence: Optional[int]
     "The minimum confidence level for a content safety label to be produced."
 
-    # iab_categories: bool = False
-    # "Enable Topic Detection."
+    iab_categories: Optional[bool]
+    "Enable Topic Detection."
 
     custom_spelling: Optional[List[Dict[str, Union[str, List[str]]]]]
     "Customize how words are spelled and formatted using to and from values"
 
     disfluencies: Optional[bool]
     "Transcribe Filler Words, like 'umm', in your media file."
 
@@ -1379,16 +1382,16 @@
     summarization: Optional[bool]
     "Enable Summarization"
     summary_model: Optional[SummarizationModel]
     "The summarization model to use in case `summarization` is enabled"
     summary_type: Optional[SummarizationType]
     "The summarization type to use in case `summarization` is enabled"
 
-    # auto_highlights: bool = False
-    # "Detect important phrases and words in your transcription text."
+    auto_highlights: Optional[bool]
+    "Detect important phrases and words in your transcription text."
 
     language_detection: Optional[bool]
     """
     Identify the dominant language that's spoken in an audio file, and route the file to the appropriate model for the detected language.
 
     Automatic Language Detection is supported for the following languages:
 
@@ -1441,36 +1444,39 @@
     "The status code we received from your server when delivering your webhook"
     webhook_auth: Optional[bool]
     "Whether the webhook was sent with an HTTP authentication header"
 
     summary: Optional[str]
     "The summarization of the transcript"
 
-    # auto_highlights_result: Optional[AutohighlightResponse] = None
-    # "The list of results when enabling Automatic Transcript Highlights"
+    auto_highlights_result: Optional[AutohighlightResponse]
+    "The list of results when enabling Automatic Transcript Highlights"
 
     content_safety_labels: Optional[ContentSafetyResponse]
     "The list of results when Content Safety is enabled"
 
-    # iab_categories_result: Optional[IABResponse] = None
-    # "The list of results when Topic Detection is enabled"
+    iab_categories_result: Optional[IABResponse]
+    "The list of results when Topic Detection is enabled"
 
     chapters: Optional[List[Chapter]]
     "When Auto Chapters is enabled, the list of Auto Chapters results"
 
     sentiment_analysis_results: Optional[List[Sentiment]]
     "When Sentiment Analysis is enabled, the list of Sentiment Analysis results"
 
     entities: Optional[List[Entity]]
     "When Entity Detection is enabled, the list of detected Entities"
 
     def __init__(self, **data: Any):
         # cleanup the response before creating the object
-        # if data.get("iab_categories_result") == {}:
-        #     data["iab_categories_result"] = None
+        if data.get("iab_categories_result") == {} or (
+            not data.get("iab_categories")
+            and data.get("iab_categories_result", {}).get("status") == "unavailable"
+        ):
+            data["iab_categories_result"] = None
 
         if data.get("content_safety_labels") == {} or (
             not data.get("content_safety")
             and data.get("content_safety_labels", {}).get("status") == "unavailable"
         ):
             data["content_safety_labels"] = None
```

### Comparing `assemblyai-0.8.1/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.9.0/assemblyai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.8.1
+Version: 0.9.0
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -266,15 +266,15 @@
 <details>
   <summary>PII Redact a Transcript</summary>
 
 ```python
 import assemblyai as aai
 
 config = aai.TranscriptionConfig()
-config.set_pii_redact(
+config.set_redact_pii(
   # What should be redacted
   policies=[
       aai.PIIRedactionPolicy.credit_card_number,
       aai.PIIRedactionPolicy.email_address,
       aai.PIIRedactionPolicy.location,
       aai.PIIRedactionPolicy.person_name,
       aai.PIIRedactionPolicy.phone_number,
@@ -283,14 +283,16 @@
   substitution=aai.PIISubstitutionPolicy.hash,
 )
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
 ```
 
+[Read more about PII redaction here.](https://www.assemblyai.com/docs/Models/pii_redaction)
+
 </details>
 <details>
   <summary>Summarize the content of a transcript over time</summary>
 
 ```python
 import assemblyai as aai
 
@@ -349,30 +351,30 @@
 transcript = transcriber.transcribe(
   "https://example.org/audio.mp3",
   config=aai.TranscriptionConfig(content_safety=True)
 )
 
 
 # Get the parts of the transcript which were flagged as sensitive
-for result in transcript.content_safety_labels.results:
+for result in transcript.content_safety.results:
   print(result.text)  # sensitive text snippet
   print(result.timestamp.start)
   print(result.timestamp.end)
 
   for label in result.labels:
     print(label.label)  # content safety category
     print(label.confidence) # model's confidence that the text is in this category
     print(label.severity) # severity of the text in relation to the category
 
 # Get the confidence of the most common labels in relation to the entire audio file
-for label, confidence in transcript.content_safety_labels.summary.items():
+for label, confidence in transcript.content_safety.summary.items():
   print(f"{confidence * 100}% confident that the audio contains {label}")
 
 # Get the overall severity of the most common labels in relation to the entire audio file
-for label, severity_confidence in transcript.content_safety_labels.severity_score_summary.items():
+for label, severity_confidence in transcript.content_safety.severity_score_summary.items():
   print(f"{severity_confidence.low * 100}% confident that the audio contains low-severity {label}")
   print(f"{severity_confidence.medium * 100}% confident that the audio contains mid-severity {label}")
   print(f"{severity_confidence.high * 100}% confident that the audio contains high-severity {label}")
 
 ```
 
 [Read more about the content safety categories.](https://www.assemblyai.com/docs/Models/content_moderation#all-labels-supported-by-the-model)
@@ -395,15 +397,15 @@
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe(
   "https://example.org/audio.mp3",
   config=aai.TranscriptionConfig(sentiment_analysis=True)
 )
 
-for sentiment_result in transcript.sentiment_analysis_results:
+for sentiment_result in transcript.sentiment_analysis:
   print(sentiment_result.text)
   print(sentiment_result.sentiment)  # POSITIVE, NEUTRAL, or NEGATIVE
   print(sentiment_result.confidence)
   print(f"Timestamp: {sentiment_result.timestamp.start} - {sentiment_result.timestamp.end}")
 ```
 
 If `speaker_labels` is also enabled, then each sentiment analysis result will also include a `speaker` field.
@@ -411,15 +413,15 @@
 ```python
 # ...
 
 config = aai.TranscriptionConfig(sentiment_analysis=True, speaker_labels=True)
 
 # ...
 
-for sentiment_result in transcript.sentiment_analysis_results:
+for sentiment_result in transcript.sentiment_analysis:
   print(sentiment_result.speaker)
 ```
 
 [Read more about sentiment analysis here.](https://www.assemblyai.com/docs/Models/sentiment_analysis)
 
 </details>
 <details>
@@ -439,14 +441,66 @@
   print(entity.type) # i.e. EntityType.person
   print(f"Timestamp: {entity.start} - {entity.end}")
 ```
 
 [Read more about entity detection here.](https://www.assemblyai.com/docs/Models/entity_detection)
 
 </details>
+<details>
+  <summary>Detect Topics in a Transcript (IAB Classification)</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(iab_categories=True)
+)
+
+# Get the parts of the transcript that were tagged with topics
+for result in transcript.iab_categories.results:
+  print(result.text)
+  print(f"Timestamp: {result.timestamp.start} - {result.timestamp.end}")
+  for label in result.labels:
+    print(label.label)  # topic
+    print(label.relevance)  # how relevant the label is for the portion of text
+
+# Get a summary of all topics in the transcript
+for label, relevance in transcript.iab_categories.summary.items():
+  print(f"Audio is {relevance * 100}% relevant to {label}")
+```
+
+[Read more about IAB classification here.](https://www.assemblyai.com/docs/Models/iab_classification)
+
+</details>
+<details>
+  <summary>Identify Important Words and Phrases in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(auto_highlights=True)
+)
+
+for result in transcript.auto_highlights.results:
+  print(result.text) # the important phrase
+  print(result.rank) # relevancy of the phrase
+  print(result.count) # number of instances of the phrase
+  for timestamp in result.timestamps:
+    print(f"Timestamp: {timestamp.start} - {timestamp.end}")
+
+```
+
+[Read more about auto highlights here.](https://www.assemblyai.com/docs/Models/key_phrases)
+
+</details>
 
 ---
 
 ## Playgrounds
 
 Visit one of our Playgrounds:
 
@@ -503,7 +557,17 @@
 Currently, the SDK provides two ways to transcribe audio files.
 
 The synchronous approach halts the application's flow until the transcription has been completed.
 
 The asynchronous approach allows the application to continue running while the transcription is being processed. The caller receives a [`concurrent.futures.Future`](https://docs.python.org/3/library/concurrent.futures.html) object which can be used to check the status of the transcription at a later time.
 
 You can identify those two approaches by the `_async` suffix in the `Transcriber`'s method name (e.g. `transcribe` vs `transcribe_async`).
+
+## Polling Intervals
+
+By default we poll the `Transcript`'s status each `3s`. In case you would like to adjust that interval:
+
+```python
+import assemblyai as aai
+
+aai.settings.polling_interval = 1.0
+```
```

### Comparing `assemblyai-0.8.1/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.9.0/assemblyai.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 assemblyai.egg-info/requires.txt
 assemblyai.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/factories.py
 tests/unit/test_auto_chapters.py
+tests/unit/test_auto_highlights.py
 tests/unit/test_client.py
 tests/unit/test_config.py
 tests/unit/test_content_safety.py
 tests/unit/test_domains.py
 tests/unit/test_entity_detection.py
+tests/unit/test_iab_categories.py
 tests/unit/test_lemur.py
+tests/unit/test_redact_pii.py
 tests/unit/test_sentiment_analysis.py
 tests/unit/test_summarization.py
 tests/unit/test_transcriber.py
 tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.8.1/setup.py` & `assemblyai-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.8.1",
+    version="0.9.0",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.8.1/tests/unit/factories.py` & `assemblyai-0.9.0/tests/unit/factories.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/tests/unit/test_auto_chapters.py` & `assemblyai-0.9.0/tests/unit/test_auto_chapters.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/tests/unit/test_content_safety.py` & `assemblyai-0.9.0/tests/unit/test_content_safety.py`

 * *Files 12% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         httpx_mock,
         mock_response=factories.generate_dict_factory(
             factories.TranscriptCompletedResponseFactory
         )(),
         config=aai.TranscriptionConfig(),
     )
     assert request_body.get("content_safety") is None
-    assert transcript.content_safety_labels is None
+    assert transcript.content_safety is None
 
 
 def test_content_safety_enabled(httpx_mock: HTTPXMock):
     """
     Tests that including `content_safety=True` in the `TranscriptionConfig`
     will result in `content_safety=True` in the request body, and that the
     response is properly parsed into a `Transcript` object
@@ -151,28 +151,28 @@
     )
 
     # Check that request body was properly defined
     assert request_body.get("content_safety") == True
 
     # Check that transcript was properly parsed from JSON response
     assert transcript.error is None
-    assert transcript.content_safety_labels is not None
+    assert transcript.content_safety is not None
 
     # Verify status
-    assert transcript.content_safety_labels.status == aai.types.StatusResult.success
+    assert transcript.content_safety.status == aai.types.StatusResult.success
 
     # Verify results
-    assert transcript.content_safety_labels.results is not None
-    assert len(transcript.content_safety_labels.results) > 0
-    assert len(transcript.content_safety_labels.results) == len(
+    assert transcript.content_safety.results is not None
+    assert len(transcript.content_safety.results) > 0
+    assert len(transcript.content_safety.results) == len(
         mock_response["content_safety_labels"]["results"]
     )
     for response_result, transcript_result in zip(
         mock_response["content_safety_labels"]["results"],
-        transcript.content_safety_labels.results,
+        transcript.content_safety.results,
     ):
         assert transcript_result.text == response_result["text"]
 
         assert (
             transcript_result.timestamp.start == response_result["timestamp"]["start"]
         )
         assert transcript_result.timestamp.end == response_result["timestamp"]["end"]
@@ -183,41 +183,41 @@
             response_result["labels"], transcript_result.labels
         ):
             assert transcript_label.label == response_label["label"]
             assert transcript_label.confidence == response_label["confidence"]
             assert transcript_label.severity == response_label["severity"]
 
     # Verify summary
-    assert transcript.content_safety_labels.summary is not None
-    assert len(transcript.content_safety_labels.summary) > 0
-    assert len(transcript.content_safety_labels.summary) == len(
+    assert transcript.content_safety.summary is not None
+    assert len(transcript.content_safety.summary) > 0
+    assert len(transcript.content_safety.summary) == len(
         mock_response["content_safety_labels"]["summary"]
     )
     for response_summary_items, transcript_summary_items in zip(
         mock_response["content_safety_labels"]["summary"].items(),
-        transcript.content_safety_labels.summary.items(),
+        transcript.content_safety.summary.items(),
     ):
         response_summary_key, response_summary_value = response_summary_items
         transcript_summary_key, transcript_summary_value = transcript_summary_items
 
         assert transcript_summary_key == response_summary_key
         assert transcript_summary_value == response_summary_value
 
     # Verify severity score summary
-    assert transcript.content_safety_labels.severity_score_summary is not None
-    assert len(transcript.content_safety_labels.severity_score_summary) > 0
-    assert len(transcript.content_safety_labels.severity_score_summary) == len(
+    assert transcript.content_safety.severity_score_summary is not None
+    assert len(transcript.content_safety.severity_score_summary) > 0
+    assert len(transcript.content_safety.severity_score_summary) == len(
         mock_response["content_safety_labels"]["severity_score_summary"]
     )
     for (
         response_severity_score_summary_items,
         transcript_severity_score_summary_items,
     ) in zip(
         mock_response["content_safety_labels"]["severity_score_summary"].items(),
-        transcript.content_safety_labels.severity_score_summary.items(),
+        transcript.content_safety.severity_score_summary.items(),
     ):
         (
             response_severity_score_summary_key,
             response_severity_score_summary_values,
         ) = response_severity_score_summary_items
         (
             transcript_severity_score_summary_key,
```

### Comparing `assemblyai-0.8.1/tests/unit/test_domains.py` & `assemblyai-0.9.0/tests/unit/test_domains.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/tests/unit/test_entity_detection.py` & `assemblyai-0.9.0/tests/unit/test_entity_detection.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/tests/unit/test_lemur.py` & `assemblyai-0.9.0/tests/unit/test_lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/tests/unit/test_sentiment_analysis.py` & `assemblyai-0.9.0/tests/unit/test_sentiment_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         httpx_mock,
         mock_response=factories.generate_dict_factory(
             factories.TranscriptCompletedResponseFactory
         )(),
         config=aai.TranscriptionConfig(),
     )
     assert request_body.get("sentiment_analysis") is None
-    assert transcript.sentiment_analysis_results is None
+    assert transcript.sentiment_analysis is None
 
 
 def test_sentiment_analysis_enabled(httpx_mock: HTTPXMock):
     """
     Tests that including `sentiment_analysis=True` in the `TranscriptionConfig`
     will result in `sentiment_analysis=True` in the request body, and that the
     response is properly parsed into a `Transcript` object
@@ -102,23 +102,23 @@
 
     # Check that request body was properly defined
     assert request_body.get("sentiment_analysis") == True
 
     # Check that transcript was properly parsed from JSON response
     assert transcript.error is None
 
-    assert transcript.sentiment_analysis_results is not None
-    assert len(transcript.sentiment_analysis_results) > 0
-    assert len(transcript.sentiment_analysis_results) == len(
+    assert transcript.sentiment_analysis is not None
+    assert len(transcript.sentiment_analysis) > 0
+    assert len(transcript.sentiment_analysis) == len(
         mock_response["sentiment_analysis_results"]
     )
 
     for response_sentiment_result, transcript_sentiment_result in zip(
         mock_response["sentiment_analysis_results"],
-        transcript.sentiment_analysis_results,
+        transcript.sentiment_analysis,
     ):
         assert transcript_sentiment_result.text == response_sentiment_result["text"]
         assert transcript_sentiment_result.start == response_sentiment_result["start"]
         assert transcript_sentiment_result.end == response_sentiment_result["end"]
         assert (
             transcript_sentiment_result.confidence
             == response_sentiment_result["confidence"]
```

### Comparing `assemblyai-0.8.1/tests/unit/test_summarization.py` & `assemblyai-0.9.0/tests/unit/test_summarization.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/tests/unit/test_transcriber.py` & `assemblyai-0.9.0/tests/unit/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.8.1/tests/unit/test_transcript.py` & `assemblyai-0.9.0/tests/unit/test_transcript.py`

 * *Files identical despite different names*

