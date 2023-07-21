# Comparing `tmp/imsosorry-1.2.0.tar.gz` & `tmp/imsosorry-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsosorry-1.2.0.tar", last modified: Sun Jan 29 08:36:25 2023, max compression
+gzip compressed data, was "imsosorry-1.2.1.tar", last modified: Fri Jul 21 03:11:13 2023, max compression
```

## Comparing `imsosorry-1.2.0.tar` & `imsosorry-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 08:36:25.494594 imsosorry-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-29 08:36:07.000000 imsosorry-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-01-29 08:36:25.494594 imsosorry-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-29 08:36:07.000000 imsosorry-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-01-29 08:36:07.000000 imsosorry-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 08:36:25.494594 imsosorry-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 08:36:25.490594 imsosorry-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 08:36:25.494594 imsosorry-1.2.0/src/imsosorry/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-29 08:36:07.000000 imsosorry-1.2.0/src/imsosorry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-01-29 08:36:07.000000 imsosorry-1.2.0/src/imsosorry/uwuification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 08:36:25.494594 imsosorry-1.2.0/src/imsosorry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-01-29 08:36:25.000000 imsosorry-1.2.0/src/imsosorry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-29 08:36:25.000000 imsosorry-1.2.0/src/imsosorry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 08:36:25.000000 imsosorry-1.2.0/src/imsosorry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-29 08:36:25.000000 imsosorry-1.2.0/src/imsosorry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-29 08:36:25.000000 imsosorry-1.2.0/src/imsosorry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:11:13.930935 imsosorry-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 03:11:04.000000 imsosorry-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-21 03:11:13.926935 imsosorry-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-21 03:11:04.000000 imsosorry-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-21 03:11:04.000000 imsosorry-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 03:11:13.930935 imsosorry-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:11:13.926935 imsosorry-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:11:13.926935 imsosorry-1.2.1/src/imsosorry/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 03:11:04.000000 imsosorry-1.2.1/src/imsosorry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-21 03:11:04.000000 imsosorry-1.2.1/src/imsosorry/uwuification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:11:13.926935 imsosorry-1.2.1/src/imsosorry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-21 03:11:13.000000 imsosorry-1.2.1/src/imsosorry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-21 03:11:13.000000 imsosorry-1.2.1/src/imsosorry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 03:11:13.000000 imsosorry-1.2.1/src/imsosorry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 03:11:13.000000 imsosorry-1.2.1/src/imsosorry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 03:11:13.000000 imsosorry-1.2.1/src/imsosorry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:11:13.926935 imsosorry-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-21 03:11:04.000000 imsosorry-1.2.1/tests/test_uwuification.py
```

### Comparing `imsosorry-1.2.0/LICENSE` & `imsosorry-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imsosorry-1.2.0/src/imsosorry/uwuification.py` & `imsosorry-1.2.1/src/imsosorry/uwuification.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""The ancient arts of Uwuification"""
+"""The ancient arts of Uwuification."""
 
 from __future__ import annotations
 
 import random
 import re
 from functools import partial
 
@@ -13,14 +13,15 @@
     "love": "luv",
     "stupid": "baka",
     "idiot": "baka",
     "what": "nani",
     "meow": "nya~",
     "roar": "rawrr~",
 }
+"""A dict to match certain words for replacement words"""
 
 EMOJIS = [
     "rawr x3",
     "OwO",
     "UwU",
     "o.O",
     "-.-",
@@ -28,113 +29,120 @@
     "(⑅˘꒳˘)",
     "(ꈍᴗꈍ)",
     "(˘ω˘)",
     "(U ᵕ U❁)",
     "σωσ",
     "òωó",
     "(///ˬ///✿)",
-    "(U ﹏ U)",
+    "(U ﹏ U)",  # noqa: RUF001 - literally the point...
     "( ͡o ω ͡o )",
     "ʘwʘ",
     ":3",
     ":3",  # important enough to have twice
     "XD",
     "nyaa~~",
     "mya",
     ">_<",
     "😳",
     "🥺",
     "😳😳😳",
     "rawr",
     "^^",
     "^^;;",
-    "(ˆ ﻌ ˆ)♡",
+    "(ˆ ﻌ ˆ)♡",  # noqa: RUF001 - literally the point...
     "^•ﻌ•^",
     "/(^•ω•^)",
     "(✿oωo)",
 ]
+"""A list of emojis/emoticons to add."""
 
 REGEX_WORD_REPLACE = re.compile(r"(?<!w)[lr](?!w)")
+"""A wegex that to detect certain characters to change to "w"s."""
 
 REGEX_PUNCTUATION = re.compile(r"[.!?\r\n\t]")
+"""A regex to detect certain punctuation characters to emotify /(^•ω•^)"""
 
 REGEX_TILDE = re.compile(r"(?![^ ])(?<!\B)")
+"""A regex to find places to add tildes (~) to."""
 
 REGEX_STUTTER = re.compile(r"(\s)([a-zA-Z])")
+"""A regex to find words to stutter."""
 SUBSTITUTE_STUTTER = r"\g<1>\g<2>-\g<2>"
+"""A regex to add st-stuttering to strings."""
 
 REGEX_NYA = re.compile(r"n([aeou][^aeiou])")
+"""A regex to detect words with an n before a vowel to nyaify."""
 SUBSTITUTE_NYA = r"ny\1"
+"""A regex to to nyaify words."""
 
 
 def word_replace(text: str) -> str:
-    """Replaces words that are keys in the word replacement hash to the values specified."""
+    """Replace words that are keys in the word replacement hash to the values specified."""
     for word, replacement in WORD_REPLACE.items():
         text = text.replace(word, replacement)
     return text
 
 
 def char_replace(text: str) -> str:
     """Replace certain characters with 'w'."""
     return REGEX_WORD_REPLACE.sub("w", text)
 
 
 def stutter_replace(match: re.Match, strength: float = 0.0) -> str:
-    """Replaces a single character with a stuttered character."""
+    """Replace a single character with a stuttered character."""
     match_string = match.group()
     if random.random() < strength:
         return f"{match_string}-{match_string[-1]}"  # Stutter the last character
     return match_string
 
 
 def stutter(text: str, strength: float) -> str:
-    """Adds stuttering to a string."""
+    """Add stuttering to a string."""
     return REGEX_STUTTER.sub(partial(stutter_replace, strength=strength), text, 0)
 
 
 def nyaify(text: str) -> str:
-    """Nyaifies a string by adding a 'y' between an 'n' and a vowel."""
+    """Nyaify a string by adding a 'y' between an 'n' and a vowel."""
     return REGEX_NYA.sub(SUBSTITUTE_NYA, text, 0)
 
 
 def emoji_replace(match: re.Match, strength: float = 0.0) -> str:
-    """Replaces a punctuation character with an emoticon."""
+    """Replace a punctuation character with an emoticon."""
     match_string = match.group()
     if random.random() < strength:
         return f" {random.choice(EMOJIS)} "
     return match_string
 
 
 def emoji(text: str, strength: float) -> str:
-    """Replaces some punctuation with emoticons."""
+    """Replace some punctuation with emoticons."""
     return REGEX_PUNCTUATION.sub(partial(emoji_replace, strength=strength), text, 0)
 
 
-def tildes(match: re.Match, strength: float = 0.0):
-    """Adds some tildes to spaces."""
+def tildes(match: re.Match, strength: float = 0.0) -> str:
+    """Add some tildes to spaces."""
     match_string = match.group()
     if random.random() < strength:
         return "~"
     return match_string
 
 
 def tildify(text: str, strength: float) -> str:
-    """Adds some tildes to spaces."""
+    """Add some tildes to spaces."""
     return REGEX_TILDE.sub(partial(tildes, strength=strength), text, 0)
 
 
 def uwuify(
     text: str,
     *,
     stutter_strength: float = 0.2,
     emoji_strength: float = 0.1,
     tilde_strength: float = 0.1,
 ) -> str:
-    """Takes a string and returns an uwuified version of it."""
+    """Take a string and returns an uwuified version of it."""
     text = text.lower()
     text = word_replace(text)
     text = nyaify(text)
     text = char_replace(text)
     text = stutter(text, stutter_strength)
     text = emoji(text, emoji_strength)
-    text = tildify(text, tilde_strength)
-    return text
+    return tildify(text, tilde_strength)
```

