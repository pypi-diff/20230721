# Comparing `tmp/datawords-0.6.0.tar.gz` & `tmp/datawords-0.6.1.tar.gz`

## Comparing `datawords-0.6.0.tar` & `datawords-0.6.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.6.0/.pylintrc
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.6.0/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.6.0/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.6.0/readthedocs.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/_utils.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/constants.py
--rw-r--r--   0        0        0    12357 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/indexes.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/install_pytorch.py
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/models.py
--rw-r--r--   0        0        0    13822 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/parsers.py
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/ranking.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/utils.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/deepnlp/__init__.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/deepnlp/core.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/deepnlp/translators.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/deepnlp/translators2.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/deepnlp/utils.py
--rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/files/stop_en.txt
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/files/stop_es.txt
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.6.0/datawords/files/stop_pt.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/make.bat
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/source/api_reference.rst
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/source/conf.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/source/index.rst
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/source/introduction.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/source/api/deepnlp.rst
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/source/api/indexes.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/source/api/models.rst
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/source/api/parsers.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 datawords-0.6.0/docs/source/api/ranking.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 datawords-0.6.0/tests/shared.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 datawords-0.6.0/tests/test_indexes.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 datawords-0.6.0/tests/test_models.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 datawords-0.6.0/tests/test_parsers.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 datawords-0.6.0/tests/test_rankings.py
--rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.6.0/tests/texts.txt
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.6.0/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.6.0/LICENSE
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.6.0/NOTICE.md
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.6.0/README.md
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 datawords-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 datawords-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.6.1/.pylintrc
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.6.1/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.6.1/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.6.1/readthedocs.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/_utils.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/constants.py
+-rw-r--r--   0        0        0    12357 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/indexes.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/install_pytorch.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/models.py
+-rw-r--r--   0        0        0    14532 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/parsers.py
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/ranking.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/utils.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/deepnlp/__init__.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/deepnlp/core.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/deepnlp/translators.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/deepnlp/translators2.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/deepnlp/utils.py
+-rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/files/stop_en.txt
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/files/stop_es.txt
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.6.1/datawords/files/stop_pt.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/make.bat
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/source/api_reference.rst
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/source/conf.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/source/index.rst
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/source/introduction.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/source/api/deepnlp.rst
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/source/api/indexes.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/source/api/models.rst
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/source/api/parsers.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 datawords-0.6.1/docs/source/api/ranking.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 datawords-0.6.1/tests/shared.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 datawords-0.6.1/tests/test_indexes.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 datawords-0.6.1/tests/test_models.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 datawords-0.6.1/tests/test_parsers.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 datawords-0.6.1/tests/test_rankings.py
+-rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.6.1/tests/texts.txt
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.6.1/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.6.1/LICENSE
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.6.1/NOTICE.md
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.6.1/README.md
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 datawords-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 datawords-0.6.1/PKG-INFO
```

### Comparing `datawords-0.6.0/.pylintrc` & `datawords-0.6.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/Makefile` & `datawords-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/_utils.py` & `datawords-0.6.1/datawords/_utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/constants.py` & `datawords-0.6.1/datawords/constants.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/indexes.py` & `datawords-0.6.1/datawords/indexes.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/install_pytorch.py` & `datawords-0.6.1/datawords/install_pytorch.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/models.py` & `datawords-0.6.1/datawords/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,50 +36,30 @@
         epoch: int = 5,
         model: Word2Vec = None,
         using_kv=False,
         loaded_from=None,
         stopw: Optional[parsers.StopWords] = None,
     ):
         """
-
-        :param parser_conf: configuration of the parser
-        :type parser_conf: parsers.ParserConf
-        :param min_count: Ignore all words and bigrams with total collected
-            count lower than this value.
-        :type min_count: Optional[float]
-        :param threshold: Represent a score threshold for forming the phrases
-            (higher means fewer phrases). A phrase of words a followed by b is
-            accepted if the score of the phrase is greater than threshold.
-            Heavily depends on concrete scoring-function, see the scoring
-            parameter.
-        :param max_vocab_size: Maximum size (number of tokens) of the
-            vocabulary. Used to control pruning of less common words,
-            to keep memory under control. The default of 40M needs
-            about 3.6GB of RAM. Increase/decrease max_vocab_size
-            depending on how much available memory you have.
-        :type max_vocab_size: Optional[int] int
-        :param connector_words: Set of words that may be included within
-           a phrase, without affecting its scoring. If any is provided it
-           will use the lang value from the parser_conf. By default
-           datawords include CONNECTOR_WORDS for English, Portugues
-           an Spanish.
-        :type connector_words: Frozenset[str]
+        It's a wrapper around the original implementation of Word2Vec from the Gensim library.
+        It adds the option to store and track the training params of the model
+        including the parser used to do so. 
 
         """
 
         self._parser_conf = parser_conf
         self._phrases = phrases_model
         # self._models_path = models_path
         self._min_count = min_count
         self._size = size
         self._window = window
         self._min_count = min_count
         self._workers = workers
         self._epoch = epoch
-        self._parser = parsers.parser_from_conf(parser_conf, stopw=stopw)
+        self._parser = parsers.parser_from_conf(parser_conf, stopw=stopw, phrases=phrases_model)
         self.model: Union[Word2Vec, KeyedVectors] = model
         self._using_kv = using_kv
         self.loaded_from = loaded_from
         self._saved_path = loaded_from
 
     @property
     def vector_size(self) -> int:
```

### Comparing `datawords-0.6.0/datawords/parsers.py` & `datawords-0.6.1/datawords/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     strip_accents: bool = True
 
 
 def load_stop(lang="en", *, models_path=None, strip_accents=True) -> StopWords:
     """
     Open a list of stop words.
 
-    If `models_path` is ommited then it will look internally
-    for the list of words. Actually, it supports **en**, **pt** and **es**
+    If `models_path` is ommited then it will look internally in the
+    datawords package. Actually, it supports **en**, **pt** and **es**
 
     """
     if models_path:
         fp = f"{models_path}/stop_{lang}.txt"
     else:
         fp = f"{_utils.pkg_route()}/files/stop_{lang}.txt"
 
@@ -253,15 +253,16 @@
     final = _found
     if stopw:
         final = []
         for word in _found:
             if word not in stopw:
                 final.append(word)
     return final
-        
+
+
 def _apply_regex(reg_expr, word) -> str:
     _found = re.findall(reg_expr, word)
     if len(_found) > 0:
         if len(_found) > 1:
             word = "".join(_found)
         else:
             word = _found[0]
@@ -400,45 +401,65 @@
         self._emo_codes = emo_codes
         self._strip_accents = strip_accents
         self._numbers = numbers
         self._stopw = stop_words
         self._parse_urls = parse_urls
 
     def parse(self, txt: str) -> List[str]:
-        words = doc_parser(
-            txt,
-            self._stopw,
-            stemmer=self._stemmer,
-            emo_codes=self._emo_codes,
-            strip_accents=self._strip_accents,
-            lower=self._lower,
-            numbers=self._numbers,
-            parse_urls=self._parse_urls,
-        )
+        """
+        It gets a txt which could be a phrase, a doc, or anything
+        in between, and then parse it using the phraase model or
+        the parser.
+        """
+
         if self._phrases:
-            return self._phrases[words]
-        return words
+            parsed = self._phrases.parse(txt)
+        else:
+            parsed = doc_parser(
+                txt,
+                self._stopw,
+                stemmer=self._stemmer,
+                emo_codes=self._emo_codes,
+                strip_accents=self._strip_accents,
+                lower=self._lower,
+                numbers=self._numbers,
+                parse_urls=self._parse_urls,
+            )
+        return parsed
 
     def export_conf(self) -> ParserConf:
         """
         It exports the parser configuration but omits stopw path and stemmer path.
         """
+        phrases_model_path = None
+        if self._phrases:
+            conf = self._phrases.export_conf()
+            phrases_model_path = conf.path
         return ParserConf(
             lang=self._lang,
             emo_codes=self._emo_codes,
             strip_accents=self._strip_accents,
             lower=self._lower,
             numbers=self._numbers,
             parse_urls=self._parse_urls,
+            phrases_model_path=phrases_model_path,
         )
 
 
 def parser_from_conf(
-    conf: ParserConf, *, stopw: Optional[StopWords] = None, phrases=None
+    conf: ParserConf,
+    *,
+    stopw: Optional[StopWords] = None,
+    phrases: Optional[PhrasesModel] = None,
 ):
+    """
+    It loads :class:`SentencesParser` based on the :class:`ParserConf` configuration.
+    Also it's possible give an already intialized stop words and phrases objects,
+    to avoid multiple instances in a same process. 
+    """
     _stopw = stopw or load_stop(lang=conf.lang, models_path=conf.stopw_path)
     if not phrases and conf.phrases_model_path:
         phrases = PhrasesModel.load(conf.phrases_model_path)
     return SentencesParser(
         lang=conf.lang,
         phrases_model=phrases,
         lower=conf.lower,
```

### Comparing `datawords-0.6.0/datawords/ranking.py` & `datawords-0.6.1/datawords/ranking.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/utils.py` & `datawords-0.6.1/datawords/utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/deepnlp/core.py` & `datawords-0.6.1/datawords/deepnlp/core.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/deepnlp/translators.py` & `datawords-0.6.1/datawords/deepnlp/translators.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/deepnlp/translators2.py` & `datawords-0.6.1/datawords/deepnlp/translators2.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/files/stop_en.txt` & `datawords-0.6.1/datawords/files/stop_en.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/files/stop_es.txt` & `datawords-0.6.1/datawords/files/stop_es.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/datawords/files/stop_pt.txt` & `datawords-0.6.1/datawords/files/stop_pt.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/docs/Makefile` & `datawords-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/docs/make.bat` & `datawords-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/docs/source/conf.py` & `datawords-0.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/docs/source/index.rst` & `datawords-0.6.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/docs/source/introduction.rst` & `datawords-0.6.1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/docs/source/api/deepnlp.rst` & `datawords-0.6.1/docs/source/api/deepnlp.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/docs/source/api/indexes.rst` & `datawords-0.6.1/docs/source/api/indexes.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/docs/source/api/parsers.rst` & `datawords-0.6.1/docs/source/api/parsers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 
 
 
                   
 Other functions
 ^^^^^^^^^^^^^^^^
 
-.. autofunction:: datawords.parsers.load_stop2
+.. autofunction:: datawords.parsers.parser_from_conf
+
+.. autofunction:: datawords.parsers.load_stop
 
 .. autofunction:: datawords.parsers.generate_ngrams
 
 .. autofunction:: datawords.parsers.norm_token
 
 .. autofunction:: datawords.parsers.apply_regex
+
```

### Comparing `datawords-0.6.0/tests/test_indexes.py` & `datawords-0.6.1/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/tests/test_models.py` & `datawords-0.6.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/tests/test_parsers.py` & `datawords-0.6.1/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/tests/test_rankings.py` & `datawords-0.6.1/tests/test_rankings.py`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/tests/texts.txt` & `datawords-0.6.1/tests/texts.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/.gitignore` & `datawords-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/LICENSE` & `datawords-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/README.md` & `datawords-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/pyproject.toml` & `datawords-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datawords-0.6.0/PKG-INFO` & `datawords-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawords
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library to work with text data
 Project-URL: Documentation, https://github.com/unknown/datawords#readme
 Project-URL: Issues, https://github.com/unknown/datawords/issues
 Project-URL: Source, https://github.com/unknown/datawords
 Author-email: Xavier Petit <nuxion@gmail.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
```

