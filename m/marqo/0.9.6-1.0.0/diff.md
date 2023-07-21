# Comparing `tmp/marqo-0.9.6.tar.gz` & `tmp/marqo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-0.9.6.tar", last modified: Wed May 31 09:00:39 2023, max compression
+gzip compressed data, was "marqo-1.0.0.tar", last modified: Fri Jul 21 05:03:38 2023, max compression
```

## Comparing `marqo-0.9.6.tar` & `marqo-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:39.221007 marqo-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-05-31 09:00:23.000000 marqo-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-05-31 09:00:39.217007 marqo-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21052 2023-05-31 09:00:23.000000 marqo-0.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 09:00:23.000000 marqo-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:00:39.221007 marqo-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-31 09:00:23.000000 marqo-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:39.213007 marqo-0.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:39.217007 marqo-0.9.6/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/marqo_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 09:00:23.000000 marqo-0.9.6/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:39.217007 marqo-0.9.6/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21505 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 09:00:39.000000 marqo-0.9.6/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:03:38.649696 marqo-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-21 05:03:25.000000 marqo-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-21 05:03:38.649696 marqo-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-21 05:03:25.000000 marqo-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 05:03:25.000000 marqo-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:03:38.649696 marqo-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-21 05:03:25.000000 marqo-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:03:38.645696 marqo-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:03:38.649696 marqo-1.0.0/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25202 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/marqo_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/marqo_url_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 05:03:25.000000 marqo-1.0.0/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:03:38.649696 marqo-1.0.0/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21541 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 05:03:38.000000 marqo-1.0.0/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-0.9.6/LICENSE` & `marqo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-0.9.6/PKG-INFO` & `marqo-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 0.9.6
+Version: 1.0.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -116,25 +116,28 @@
 4. Start indexing and searching! Let's look at a simple example below:
 
 ```python
 import marqo
 
 mq = marqo.Client(url='http://localhost:8882')
 
-mq.index("my-first-index").add_documents([
-    {
-        "Title": "The Travels of Marco Polo",
-        "Description": "A 13th-century travelogue describing Polo's travels"
-    }, 
-    {
-        "Title": "Extravehicular Mobility Unit (EMU)",
-        "Description": "The EMU is a spacesuit that provides environmental protection, "
-                       "mobility, life support, and communications for astronauts",
-        "_id": "article_591"
-    }]
+mq.create_index("my-first-index")
+mq.index("my-first-index").add_documents(
+    [
+        {
+            "Title": "The Travels of Marco Polo",
+            "Description": "A 13th-century travelogue describing Polo's travels"},
+        {
+            "Title": "Extravehicular Mobility Unit (EMU)",
+            "Description": "The EMU is a spacesuit that provides environmental protection, "
+                           "mobility, life support, and communications for astronauts",
+            "_id": "article_591"
+        }
+    ], 
+    tensor_fields=["Title", "Description"]
 )
 
 results = mq.index("my-first-index").search(
     q="What is the best outfit to wear on the moon?", searchable_attributes=["Title", "Description"]
 )
 
 ```
@@ -286,16 +289,16 @@
 ```python
 
 import marqo
 import pprint
 
 mq = marqo.Client(url="http://localhost:8882")
 
-mq.index("my-weighted-query-index").add_documents(
-    [
+mq.create_index("my-weighted-query-index")
+mq.index("my-weighted-query-index").add_documents([
         {
             "Title": "Smartphone",
             "Description": "A smartphone is a portable computer device that combines mobile telephone "
             "functions and computing functions into one unit.",
         },
         {
             "Title": "Telephone",
@@ -304,15 +307,16 @@
         },
         {
             "Title": "Thylacine",
             "Description": "The thylacine, also commonly known as the Tasmanian tiger or Tasmanian wolf, "
             "is an extinct carnivorous marsupial."
             "The last known of its species died in 1936.",
         },
-    ]
+    ],
+    tensor_fields=["Title", "Description"]
 )
 
 # initially we ask for a type of communications device which is popular in the 21st century
 query = {
     # a weighting of 1.1 gives this query slightly more importance
     "I need to buy a communications device, what should I get?": 1.1,
     # a weighting of 1 gives this query a neutral importance
@@ -379,26 +383,24 @@
             "Title": "Horse Jumping",
             "captioned_image": {
                 "caption": "A person riding a horse over a jump in a competition.",
                 "image": "https://raw.githubusercontent.com/marqo-ai/marqo/mainline/examples/ImageSearchGuide/data/image1.jpg",
             },
         },
     ],
-    # Create the mappings, here we define our captioned_image mapping 
-    # which weights the image more heavily than the caption - these pairs 
-    # will be represented by a single vector in the index
     mappings={
         "captioned_image": {
             "type": "multimodal_combination",
             "weights": {
                 "caption": 0.3,
                 "image": 0.7,
             },
         }
     },
+    tensor_fields=["captioned_image"],
 )
 
 # Search this index with a simple text query
 results = mq.index("my-first-multimodal-index").search(
     q="Give me some images of vehicles and modes of transport. I am especially interested in air travel and commercial aeroplanes.",
     searchable_attributes=["captioned_image"],
 )
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 0.9.6 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 1.0.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
@@ -60,21 +60,22 @@
 (https://docs.docker.com/get-docker/). Ensure that docker has at least 8GB
 memory and 50GB storage. 2. Use docker to run Marqo (Mac users with M-series
 chips will need to [go here](#m-series-mac-users)): ```bash docker rm -f marqo
 docker pull marqoai/marqo:latest docker run --name marqo -it --privileged -
 p 8882:8882 --add-host host.docker.internal:host-gateway marqoai/marqo:latest
 ``` 3. Install the Marqo client: ```bash pip install marqo ``` 4. Start
 indexing and searching! Let's look at a simple example below: ```python import
-marqo mq = marqo.Client(url='http://localhost:8882') mq.index("my-first-
-index").add_documents([ { "Title": "The Travels of Marco Polo", "Description":
-"A 13th-century travelogue describing Polo's travels" }, { "Title":
-"Extravehicular Mobility Unit (EMU)", "Description": "The EMU is a spacesuit
-that provides environmental protection, " "mobility, life support, and
-communications for astronauts", "_id": "article_591" }] ) results = mq.index
-("my-first-index").search( q="What is the best outfit to wear on the moon?",
+marqo mq = marqo.Client(url='http://localhost:8882') mq.create_index("my-first-
+index") mq.index("my-first-index").add_documents( [ { "Title": "The Travels of
+Marco Polo", "Description": "A 13th-century travelogue describing Polo's
+travels"}, { "Title": "Extravehicular Mobility Unit (EMU)", "Description": "The
+EMU is a spacesuit that provides environmental protection, " "mobility, life
+support, and communications for astronauts", "_id": "article_591" } ],
+tensor_fields=["Title", "Description"] ) results = mq.index("my-first-
+index").search( q="What is the best outfit to wear on the moon?",
 searchable_attributes=["Title", "Description"] ) ``` - `mq` is the client that
 wraps the `marqo` API - `add_documents()` takes a list of documents,
 represented as python dicts for indexing. - `add_documents()` creates an index
 with default settings, if one does not already exist. - You can optionally set
 a document's ID with the special `_id` field. Otherwise, Marqo will generate
 one. - If the index doesn't exist, Marqo will create it. If it exists then
 Marqo will add the documents to the index. Let's have a look at the results:
@@ -128,62 +129,61 @@
 ai_hippo_statue.png') ``` ### Searching using weights in queries Queries can
 also be provided as dictionaries where each key is a query and their
 corresponding values are weights. This allows for more advanced queries
 consisting of multiple components with weightings towards or against them,
 queries can have negations via negative weighting. The example below shows the
 application of this to a scenario where a user may want to ask a question but
 also negate results that match a certain semantic criterion. ```python import
-marqo import pprint mq = marqo.Client(url="http://localhost:8882") mq.index
-("my-weighted-query-index").add_documents( [ { "Title": "Smartphone",
-"Description": "A smartphone is a portable computer device that combines mobile
-telephone " "functions and computing functions into one unit.", }, { "Title":
-"Telephone", "Description": "A telephone is a telecommunications device that
-permits two or more users to" "conduct a conversation when they are too far
-apart to be easily heard directly.", }, { "Title": "Thylacine", "Description":
-"The thylacine, also commonly known as the Tasmanian tiger or Tasmanian wolf, "
-"is an extinct carnivorous marsupial." "The last known of its species died in
-1936.", }, ] ) # initially we ask for a type of communications device which is
-popular in the 21st century query = { # a weighting of 1.1 gives this query
-slightly more importance "I need to buy a communications device, what should I
-get?": 1.1, # a weighting of 1 gives this query a neutral importance
-"Technology that became prevelant in the 21st century": 1.0, } results =
-mq.index("my-weighted-query-index").search( q=query, searchable_attributes=
-["Title", "Description"] ) print("Query 1:") pprint.pprint(results) # now we
-ask for a type of communications which predates the 21st century query = { # a
-weighting of 1 gives this query a neutral importance "I need to buy a
-communications device, what should I get?": 1.0, # a weighting of -1 gives this
-query a negation effect "Technology that became prevelant in the 21st century":
--1.0, } results = mq.index("my-weighted-query-index").search( q=query,
-searchable_attributes=["Title", "Description"] ) print("\nQuery 2:")
-pprint.pprint(results) ``` ### Creating and searching indexes with multimodal
-combination fields Marqo lets you have indexes with multimodal combination
-fields. Multimodal combination fields can combine text and images into one
-field. This allows scoring of documents across the combined text and image
-fields together. It also allows for a single vector representation instead of
-needing many which saves on storage. The relative weighting of each component
-can be set per document. The example below demonstrates this with retrival of
-caption and image pairs using multiple types of queries. ```python import marqo
-import pprint mq = marqo.Client(url="http://localhost:8882") settings =
-{"treat_urls_and_pointers_as_images": True, "model": "ViT-L/14"}
+marqo import pprint mq = marqo.Client(url="http://localhost:8882")
+mq.create_index("my-weighted-query-index") mq.index("my-weighted-query-
+index").add_documents([ { "Title": "Smartphone", "Description": "A smartphone
+is a portable computer device that combines mobile telephone " "functions and
+computing functions into one unit.", }, { "Title": "Telephone", "Description":
+"A telephone is a telecommunications device that permits two or more users to"
+"conduct a conversation when they are too far apart to be easily heard
+directly.", }, { "Title": "Thylacine", "Description": "The thylacine, also
+commonly known as the Tasmanian tiger or Tasmanian wolf, " "is an extinct
+carnivorous marsupial." "The last known of its species died in 1936.", }, ],
+tensor_fields=["Title", "Description"] ) # initially we ask for a type of
+communications device which is popular in the 21st century query = { # a
+weighting of 1.1 gives this query slightly more importance "I need to buy a
+communications device, what should I get?": 1.1, # a weighting of 1 gives this
+query a neutral importance "Technology that became prevelant in the 21st
+century": 1.0, } results = mq.index("my-weighted-query-index").search( q=query,
+searchable_attributes=["Title", "Description"] ) print("Query 1:")
+pprint.pprint(results) # now we ask for a type of communications which predates
+the 21st century query = { # a weighting of 1 gives this query a neutral
+importance "I need to buy a communications device, what should I get?": 1.0, #
+a weighting of -1 gives this query a negation effect "Technology that became
+prevelant in the 21st century": -1.0, } results = mq.index("my-weighted-query-
+index").search( q=query, searchable_attributes=["Title", "Description"] ) print
+("\nQuery 2:") pprint.pprint(results) ``` ### Creating and searching indexes
+with multimodal combination fields Marqo lets you have indexes with multimodal
+combination fields. Multimodal combination fields can combine text and images
+into one field. This allows scoring of documents across the combined text and
+image fields together. It also allows for a single vector representation
+instead of needing many which saves on storage. The relative weighting of each
+component can be set per document. The example below demonstrates this with
+retrival of caption and image pairs using multiple types of queries. ```python
+import marqo import pprint mq = marqo.Client(url="http://localhost:8882")
+settings = {"treat_urls_and_pointers_as_images": True, "model": "ViT-L/14"}
 mq.create_index("my-first-multimodal-index", **settings) mq.index("my-first-
 multimodal-index").add_documents( [ { "Title": "Flying Plane",
 "captioned_image": { "caption": "An image of a passenger plane flying in front
 of the moon.", "image": "https://raw.githubusercontent.com/marqo-ai/marqo/
 mainline/examples/ImageSearchGuide/data/image2.jpg", }, }, { "Title": "Red
 Bus", "captioned_image": { "caption": "A red double decker London bus traveling
 to Aldwych", "image": "https://raw.githubusercontent.com/marqo-ai/marqo/
 mainline/examples/ImageSearchGuide/data/image4.jpg", }, }, { "Title": "Horse
 Jumping", "captioned_image": { "caption": "A person riding a horse over a jump
 in a competition.", "image": "https://raw.githubusercontent.com/marqo-ai/marqo/
-mainline/examples/ImageSearchGuide/data/image1.jpg", }, }, ], # Create the
-mappings, here we define our captioned_image mapping # which weights the image
-more heavily than the caption - these pairs # will be represented by a single
-vector in the index mappings={ "captioned_image": { "type":
-"multimodal_combination", "weights": { "caption": 0.3, "image": 0.7, }, } }, )
-# Search this index with a simple text query results = mq.index("my-first-
+mainline/examples/ImageSearchGuide/data/image1.jpg", }, }, ], mappings=
+{ "captioned_image": { "type": "multimodal_combination", "weights":
+{ "caption": 0.3, "image": 0.7, }, } }, tensor_fields=["captioned_image"], ) #
+Search this index with a simple text query results = mq.index("my-first-
 multimodal-index").search( q="Give me some images of vehicles and modes of
 transport. I am especially interested in air travel and commercial
 aeroplanes.", searchable_attributes=["captioned_image"], ) print("Query 1:")
 pprint.pprint(results) # search the index with a query that uses weighted
 components results = mq.index("my-first-multimodal-index").search( q={ "What
 are some vehicles and modes of transport?": 1.0, "Aeroplanes and other things
 that fly": -1.0, }, searchable_attributes=["captioned_image"], ) print("\nQuery
```

### Comparing `marqo-0.9.6/README.md` & `marqo-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,25 +102,28 @@
 4. Start indexing and searching! Let's look at a simple example below:
 
 ```python
 import marqo
 
 mq = marqo.Client(url='http://localhost:8882')
 
-mq.index("my-first-index").add_documents([
-    {
-        "Title": "The Travels of Marco Polo",
-        "Description": "A 13th-century travelogue describing Polo's travels"
-    }, 
-    {
-        "Title": "Extravehicular Mobility Unit (EMU)",
-        "Description": "The EMU is a spacesuit that provides environmental protection, "
-                       "mobility, life support, and communications for astronauts",
-        "_id": "article_591"
-    }]
+mq.create_index("my-first-index")
+mq.index("my-first-index").add_documents(
+    [
+        {
+            "Title": "The Travels of Marco Polo",
+            "Description": "A 13th-century travelogue describing Polo's travels"},
+        {
+            "Title": "Extravehicular Mobility Unit (EMU)",
+            "Description": "The EMU is a spacesuit that provides environmental protection, "
+                           "mobility, life support, and communications for astronauts",
+            "_id": "article_591"
+        }
+    ], 
+    tensor_fields=["Title", "Description"]
 )
 
 results = mq.index("my-first-index").search(
     q="What is the best outfit to wear on the moon?", searchable_attributes=["Title", "Description"]
 )
 
 ```
@@ -272,16 +275,16 @@
 ```python
 
 import marqo
 import pprint
 
 mq = marqo.Client(url="http://localhost:8882")
 
-mq.index("my-weighted-query-index").add_documents(
-    [
+mq.create_index("my-weighted-query-index")
+mq.index("my-weighted-query-index").add_documents([
         {
             "Title": "Smartphone",
             "Description": "A smartphone is a portable computer device that combines mobile telephone "
             "functions and computing functions into one unit.",
         },
         {
             "Title": "Telephone",
@@ -290,15 +293,16 @@
         },
         {
             "Title": "Thylacine",
             "Description": "The thylacine, also commonly known as the Tasmanian tiger or Tasmanian wolf, "
             "is an extinct carnivorous marsupial."
             "The last known of its species died in 1936.",
         },
-    ]
+    ],
+    tensor_fields=["Title", "Description"]
 )
 
 # initially we ask for a type of communications device which is popular in the 21st century
 query = {
     # a weighting of 1.1 gives this query slightly more importance
     "I need to buy a communications device, what should I get?": 1.1,
     # a weighting of 1 gives this query a neutral importance
@@ -365,26 +369,24 @@
             "Title": "Horse Jumping",
             "captioned_image": {
                 "caption": "A person riding a horse over a jump in a competition.",
                 "image": "https://raw.githubusercontent.com/marqo-ai/marqo/mainline/examples/ImageSearchGuide/data/image1.jpg",
             },
         },
     ],
-    # Create the mappings, here we define our captioned_image mapping 
-    # which weights the image more heavily than the caption - these pairs 
-    # will be represented by a single vector in the index
     mappings={
         "captioned_image": {
             "type": "multimodal_combination",
             "weights": {
                 "caption": 0.3,
                 "image": 0.7,
             },
         }
     },
+    tensor_fields=["captioned_image"],
 )
 
 # Search this index with a simple text query
 results = mq.index("my-first-multimodal-index").search(
     q="Give me some images of vehicles and modes of transport. I am especially interested in air travel and commercial aeroplanes.",
     searchable_attributes=["captioned_image"],
 )
```

#### html2text {}

```diff
@@ -53,21 +53,22 @@
 (https://docs.docker.com/get-docker/). Ensure that docker has at least 8GB
 memory and 50GB storage. 2. Use docker to run Marqo (Mac users with M-series
 chips will need to [go here](#m-series-mac-users)): ```bash docker rm -f marqo
 docker pull marqoai/marqo:latest docker run --name marqo -it --privileged -
 p 8882:8882 --add-host host.docker.internal:host-gateway marqoai/marqo:latest
 ``` 3. Install the Marqo client: ```bash pip install marqo ``` 4. Start
 indexing and searching! Let's look at a simple example below: ```python import
-marqo mq = marqo.Client(url='http://localhost:8882') mq.index("my-first-
-index").add_documents([ { "Title": "The Travels of Marco Polo", "Description":
-"A 13th-century travelogue describing Polo's travels" }, { "Title":
-"Extravehicular Mobility Unit (EMU)", "Description": "The EMU is a spacesuit
-that provides environmental protection, " "mobility, life support, and
-communications for astronauts", "_id": "article_591" }] ) results = mq.index
-("my-first-index").search( q="What is the best outfit to wear on the moon?",
+marqo mq = marqo.Client(url='http://localhost:8882') mq.create_index("my-first-
+index") mq.index("my-first-index").add_documents( [ { "Title": "The Travels of
+Marco Polo", "Description": "A 13th-century travelogue describing Polo's
+travels"}, { "Title": "Extravehicular Mobility Unit (EMU)", "Description": "The
+EMU is a spacesuit that provides environmental protection, " "mobility, life
+support, and communications for astronauts", "_id": "article_591" } ],
+tensor_fields=["Title", "Description"] ) results = mq.index("my-first-
+index").search( q="What is the best outfit to wear on the moon?",
 searchable_attributes=["Title", "Description"] ) ``` - `mq` is the client that
 wraps the `marqo` API - `add_documents()` takes a list of documents,
 represented as python dicts for indexing. - `add_documents()` creates an index
 with default settings, if one does not already exist. - You can optionally set
 a document's ID with the special `_id` field. Otherwise, Marqo will generate
 one. - If the index doesn't exist, Marqo will create it. If it exists then
 Marqo will add the documents to the index. Let's have a look at the results:
@@ -121,62 +122,61 @@
 ai_hippo_statue.png') ``` ### Searching using weights in queries Queries can
 also be provided as dictionaries where each key is a query and their
 corresponding values are weights. This allows for more advanced queries
 consisting of multiple components with weightings towards or against them,
 queries can have negations via negative weighting. The example below shows the
 application of this to a scenario where a user may want to ask a question but
 also negate results that match a certain semantic criterion. ```python import
-marqo import pprint mq = marqo.Client(url="http://localhost:8882") mq.index
-("my-weighted-query-index").add_documents( [ { "Title": "Smartphone",
-"Description": "A smartphone is a portable computer device that combines mobile
-telephone " "functions and computing functions into one unit.", }, { "Title":
-"Telephone", "Description": "A telephone is a telecommunications device that
-permits two or more users to" "conduct a conversation when they are too far
-apart to be easily heard directly.", }, { "Title": "Thylacine", "Description":
-"The thylacine, also commonly known as the Tasmanian tiger or Tasmanian wolf, "
-"is an extinct carnivorous marsupial." "The last known of its species died in
-1936.", }, ] ) # initially we ask for a type of communications device which is
-popular in the 21st century query = { # a weighting of 1.1 gives this query
-slightly more importance "I need to buy a communications device, what should I
-get?": 1.1, # a weighting of 1 gives this query a neutral importance
-"Technology that became prevelant in the 21st century": 1.0, } results =
-mq.index("my-weighted-query-index").search( q=query, searchable_attributes=
-["Title", "Description"] ) print("Query 1:") pprint.pprint(results) # now we
-ask for a type of communications which predates the 21st century query = { # a
-weighting of 1 gives this query a neutral importance "I need to buy a
-communications device, what should I get?": 1.0, # a weighting of -1 gives this
-query a negation effect "Technology that became prevelant in the 21st century":
--1.0, } results = mq.index("my-weighted-query-index").search( q=query,
-searchable_attributes=["Title", "Description"] ) print("\nQuery 2:")
-pprint.pprint(results) ``` ### Creating and searching indexes with multimodal
-combination fields Marqo lets you have indexes with multimodal combination
-fields. Multimodal combination fields can combine text and images into one
-field. This allows scoring of documents across the combined text and image
-fields together. It also allows for a single vector representation instead of
-needing many which saves on storage. The relative weighting of each component
-can be set per document. The example below demonstrates this with retrival of
-caption and image pairs using multiple types of queries. ```python import marqo
-import pprint mq = marqo.Client(url="http://localhost:8882") settings =
-{"treat_urls_and_pointers_as_images": True, "model": "ViT-L/14"}
+marqo import pprint mq = marqo.Client(url="http://localhost:8882")
+mq.create_index("my-weighted-query-index") mq.index("my-weighted-query-
+index").add_documents([ { "Title": "Smartphone", "Description": "A smartphone
+is a portable computer device that combines mobile telephone " "functions and
+computing functions into one unit.", }, { "Title": "Telephone", "Description":
+"A telephone is a telecommunications device that permits two or more users to"
+"conduct a conversation when they are too far apart to be easily heard
+directly.", }, { "Title": "Thylacine", "Description": "The thylacine, also
+commonly known as the Tasmanian tiger or Tasmanian wolf, " "is an extinct
+carnivorous marsupial." "The last known of its species died in 1936.", }, ],
+tensor_fields=["Title", "Description"] ) # initially we ask for a type of
+communications device which is popular in the 21st century query = { # a
+weighting of 1.1 gives this query slightly more importance "I need to buy a
+communications device, what should I get?": 1.1, # a weighting of 1 gives this
+query a neutral importance "Technology that became prevelant in the 21st
+century": 1.0, } results = mq.index("my-weighted-query-index").search( q=query,
+searchable_attributes=["Title", "Description"] ) print("Query 1:")
+pprint.pprint(results) # now we ask for a type of communications which predates
+the 21st century query = { # a weighting of 1 gives this query a neutral
+importance "I need to buy a communications device, what should I get?": 1.0, #
+a weighting of -1 gives this query a negation effect "Technology that became
+prevelant in the 21st century": -1.0, } results = mq.index("my-weighted-query-
+index").search( q=query, searchable_attributes=["Title", "Description"] ) print
+("\nQuery 2:") pprint.pprint(results) ``` ### Creating and searching indexes
+with multimodal combination fields Marqo lets you have indexes with multimodal
+combination fields. Multimodal combination fields can combine text and images
+into one field. This allows scoring of documents across the combined text and
+image fields together. It also allows for a single vector representation
+instead of needing many which saves on storage. The relative weighting of each
+component can be set per document. The example below demonstrates this with
+retrival of caption and image pairs using multiple types of queries. ```python
+import marqo import pprint mq = marqo.Client(url="http://localhost:8882")
+settings = {"treat_urls_and_pointers_as_images": True, "model": "ViT-L/14"}
 mq.create_index("my-first-multimodal-index", **settings) mq.index("my-first-
 multimodal-index").add_documents( [ { "Title": "Flying Plane",
 "captioned_image": { "caption": "An image of a passenger plane flying in front
 of the moon.", "image": "https://raw.githubusercontent.com/marqo-ai/marqo/
 mainline/examples/ImageSearchGuide/data/image2.jpg", }, }, { "Title": "Red
 Bus", "captioned_image": { "caption": "A red double decker London bus traveling
 to Aldwych", "image": "https://raw.githubusercontent.com/marqo-ai/marqo/
 mainline/examples/ImageSearchGuide/data/image4.jpg", }, }, { "Title": "Horse
 Jumping", "captioned_image": { "caption": "A person riding a horse over a jump
 in a competition.", "image": "https://raw.githubusercontent.com/marqo-ai/marqo/
-mainline/examples/ImageSearchGuide/data/image1.jpg", }, }, ], # Create the
-mappings, here we define our captioned_image mapping # which weights the image
-more heavily than the caption - these pairs # will be represented by a single
-vector in the index mappings={ "captioned_image": { "type":
-"multimodal_combination", "weights": { "caption": 0.3, "image": 0.7, }, } }, )
-# Search this index with a simple text query results = mq.index("my-first-
+mainline/examples/ImageSearchGuide/data/image1.jpg", }, }, ], mappings=
+{ "captioned_image": { "type": "multimodal_combination", "weights":
+{ "caption": 0.3, "image": 0.7, }, } }, tensor_fields=["captioned_image"], ) #
+Search this index with a simple text query results = mq.index("my-first-
 multimodal-index").search( q="Give me some images of vehicles and modes of
 transport. I am especially interested in air travel and commercial
 aeroplanes.", searchable_attributes=["captioned_image"], ) print("Query 1:")
 pprint.pprint(results) # search the index with a query that uses weighted
 components results = mq.index("my-first-multimodal-index").search( q={ "What
 are some vehicles and modes of transport?": 1.0, "Aeroplanes and other things
 that fly": -1.0, }, searchable_attributes=["captioned_image"], ) print("\nQuery
```

### Comparing `marqo-0.9.6/setup.py` & `marqo-1.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,22 +5,23 @@
     long_description = fh.read()
 
 setup(
     install_requires=[
         # client:
         "requests",
         "urllib3",
-        "pydantic"
+        "pydantic<2.0.0",
+        "packaging"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="0.9.6",
+    version="1.0.0",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-0.9.6/src/marqo/_httprequests.py` & `marqo-1.0.0/src/marqo/_httprequests.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,88 +17,101 @@
 OPERATION_MAPPING = {
     'delete': session.delete,
     'get': session.get,
     'post': session.post,
     'put': session.put
 }
 
+
 class HttpRequests:
     def __init__(self, config: Config) -> None:
         self.config = config
         self.headers = {'x-api-key': config.api_key} if config.api_key else {}
 
     def _operation(self, method: HTTP_OPERATIONS) -> Callable:
         if method not in ALLOWED_OPERATIONS:
             raise ValueError("{} not an allowed operation {}".format(method, ALLOWED_OPERATIONS))
 
         return OPERATION_MAPPING[method]
 
+    def _construct_path(self, path: str, index_name="") -> str:
+        """Augment the URL request path based if telemetry is required."""
+        url = f"{self.config.get_url(index_name=index_name)}/{path}"
+        if self.config.use_telemetry:
+            delimeter= "?" if "?" not in f"{self.config.url}/{path}" else "&"
+            return url + f"{delimeter}telemetry=True"
+        return url
+
     def send_request(
         self,
         http_operation: HTTP_OPERATIONS,
         path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str], str]] = None,
         content_type: Optional[str] = None,
+        index_name: str = ""
     ) -> Any:
         req_headers = copy.deepcopy(self.headers)
 
         if content_type is not None and content_type:
             req_headers['Content-Type'] = content_type
 
         if not isinstance(body, (bytes, str)) and body is not None:
             body = json.dumps(body)
 
         try:
             response = self._operation(http_operation)(
-                url=f"{self.config.url}/{path}",
+                url=self._construct_path(path, index_name),
                 timeout=self.config.timeout,
                 headers=req_headers,
                 data=body,
                 verify=True
             )
             return self.__validate(response)
         except requests.exceptions.Timeout as err:
             raise BackendTimeoutError(str(err)) from err
         except requests.exceptions.ConnectionError as err:
             raise BackendCommunicationError(str(err)) from err
 
-
     def get(
         self, path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str], str]] = None,
+        index_name: str = ""
     ) -> Any:
         content_type = None
         if body is not None:
             content_type = 'application/json'
-        return self.send_request('get', path=path, body=body, content_type=content_type)
+        return self.send_request('get', path=path, body=body, content_type=content_type,index_name=index_name)
 
     def post(
         self,
         path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str], str]] = None,
         content_type: Optional[str] = 'application/json',
+        index_name: str = ""
     ) -> Any:
-        return self.send_request('post', path, body, content_type)
+        return self.send_request('post', path, body, content_type, index_name=index_name)
 
     def put(
         self,
         path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str], str]] = None,
         content_type: Optional[str] = None,
+        index_name: str = ""
     ) -> Any:
         if body is not None:
             content_type = 'application/json'
-        return self.send_request('put', path, body, content_type)
+        return self.send_request('put', path, body, content_type, index_name=index_name)
 
     def delete(
         self,
         path: str,
         body: Optional[Union[Dict[str, Any], List[Dict[str, Any]], List[str]]] = None,
+        index_name: str = ""
     ) -> Any:
-        return self.send_request('delete', path, body)
+        return self.send_request('delete', path, body, index_name=index_name)
 
     @staticmethod
     def __to_json(
         request: requests.Response
     ) -> Any:
         if request.content == b'':
             return request
```

### Comparing `marqo-0.9.6/src/marqo/client.py` & `marqo-1.0.0/src/marqo/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,99 @@
 import base64
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import error_wrappers
+from requests.exceptions import RequestException
 
 from marqo.index import Index
 from marqo.config import Config
 from marqo.models import BulkSearchBody, BulkSearchQuery
 from marqo._httprequests import HttpRequests
 from marqo import utils, enums
 from marqo import errors
+from marqo.version import minimum_supported_marqo_version
+from marqo.marqo_logging import mq_logger
+from marqo.errors import MarqoWebError
+# we want to avoid name conflicts with marqo.version
+from packaging import version as versioning_helpers
+from json import JSONDecodeError
+
+# A dictionary to cache the marqo url and version for compatibility check
+marqo_url_and_version_cache = {}
 
 
 class Client:
     """
     A client for the marqo API
 
     A client instance is needed for every marqo API method to know the location of
     marqo and its permissions.
     """
+
     def __init__(
-        self, url: str = "http://localhost:8882", main_user: str = None, main_password: str = None,
-        indexing_device: Optional[Union[enums.Devices, str]] = None,
-        search_device: Optional[Union[enums.Devices, str]] = None,
-        api_key: str = None
+            self, url: str = "http://localhost:8882",
+            main_user: str = None, main_password: str = None,
+            return_telemetry: bool = False,
+            api_key: str = None
     ) -> None:
         """
         Parameters
         ----------
         url:
             The url to the S2Search API (ex: http://localhost:8882)
         """
         self.main_user = main_user
         self.main_password = main_password
         if (main_user is not None) and (main_password is not None):
             self.url = utils.construct_authorized_url(url_base=url, username=main_user, password=main_password)
         else:
             self.url = url
-        self.config = Config(self.url, indexing_device=indexing_device, search_device=search_device, api_key=api_key)
+        self.config = Config(self.url, use_telemetry=return_telemetry, api_key=api_key)
         self.http = HttpRequests(self.config)
+        self._marqo_minimum_supported_version_check()
 
     def create_index(
         self, index_name: str,
         treat_urls_and_pointers_as_images=False, model=None,
         normalize_embeddings=True,
         sentences_per_chunk=2,
         sentence_overlap=0,
         image_preprocessing_method=None,
-        settings_dict=None
+        settings_dict=None,
+        inference_node_type=None,
+        storage_node_type=None,
+        inference_node_count=1,
     ) -> Dict[str, Any]:
-        """Create the index.
+        """Create the index. Please refer to the marqo cloud to see options for inference and storage node types.
 
         Args:
             index_name: name of the index.
             treat_urls_and_pointers_as_images:
             model:
             normalize_embeddings:
             sentences_per_chunk:
             sentence_overlap:
             image_preprocessing_method:
             settings_dict: if specified, overwrites all other setting
                 parameters, and is passed directly as the index's
                 index_settings
+            inference_node_type:
+            storage_node_type:
+            inference_node_count;
         Returns:
             Response body, containing information about index creation result
         """
         return Index.create(
             config=self.config, index_name=index_name,
             treat_urls_and_pointers_as_images=treat_urls_and_pointers_as_images,
             model=model, normalize_embeddings=normalize_embeddings,
             sentences_per_chunk=sentences_per_chunk, sentence_overlap=sentence_overlap,
             image_preprocessing_method=image_preprocessing_method,
-            settings_dict=settings_dict
+            settings_dict=settings_dict, inference_node_type=inference_node_type, storage_node_type=storage_node_type,
+            inference_node_count=inference_node_count
         )
 
     def delete_index(self, index_name: str) -> Dict[str, Any]:
         """Deletes an index
 
         Args:
             index_name: name of the index
@@ -97,15 +116,15 @@
         Returns:
             An Index instance containing the information of the fetched index.
 
         Raises:
         """
         ix = Index(self.config, index_name)
         # verify it exists:
-        self.http.get(path=f"indexes/{index_name}/stats")
+        self.http.get(path=f"indexes/{index_name}/stats", index_name=index_name)
         return ix
 
     def index(self, index_name: str) -> Index:
         """Create a local reference to an index identified by index_name,
         without doing an HTTP call.
 
         Calling this method doesn't create an index on the Marqo instance, but
@@ -135,58 +154,85 @@
             )
             for index_info in response["results"]
         ]
         return response
 
     def enrich(self, documents: List[Dict], enrichment: Dict, device: str = None, ):
         """Enrich documents"""
-        selected_device = device if device is not None else self.config.indexing_device
-        translated = utils.translate_device_string_for_url(selected_device)
+        translated = utils.translate_device_string_for_url(device)
         response = self.http.post(path=f'enrichment?device={translated}', body={
             "documents": documents,
             "enrichment": enrichment
         })
         return response
 
     def bulk_search(self, queries: List[Dict[str, Any]], device: Optional[str] = None) -> Dict[str, Any]:
         try:
             parsed_queries = [BulkSearchBody(**q) for q in queries]
         except error_wrappers.ValidationError as e:
             raise errors.InvalidArgError(f"some parameters in search query(s) are invalid. Errors are: {e.errors()}")
 
-        selected_device = device if device is not None else self.config.search_device
-        translated = utils.translate_device_string_for_url(selected_device)
-        
+        translated_device_param = f"{f'?&device={utils.translate_device_string_for_url(device)}' if device is not None else ''}"
         return self.http.post(
-            f"indexes/bulk/search?device={translated}",
+            f"indexes/bulk/search{translated_device_param}",
             body=BulkSearchQuery(queries=parsed_queries).json()
         )
 
     @staticmethod
     def _base64url_encode(
-        data: bytes
+            data: bytes
     ) -> str:
         return base64.urlsafe_b64encode(data).decode('utf-8').replace('=', '')
 
     def get_marqo(self):
         return self.http.get(path="")
 
     def health(self):
         return self.http.get(path="health")
 
-
-    def eject_model(self, model_name:str, model_device:str):
+    def eject_model(self, model_name: str, model_device: str):
         return self.http.delete(path=f"models?model_name={model_name}&model_device={model_device}")
 
-
     def get_loaded_models(self):
         return self.http.get(path="models")
 
-
     def get_cuda_info(self):
         return self.http.get(path="device/cuda")
 
-
     def get_cpu_info(self):
         return self.http.get(path="device/cpu")
 
+    def _marqo_minimum_supported_version_check(self):
+        min_ver = minimum_supported_marqo_version()
+        skip_warning_message = (
+            f"Marqo encountered a problem trying to check the Marqo version found at `{self.url}`. "
+            f"The minimum supported Marqo version for this client is {min_ver}. "
+            f"If you are sure your Marqo version is compatible with this client, you can ignore this message. ")
+
+        # Skip the check if the url is previously labelled as "_skipped"
+        if self.url in marqo_url_and_version_cache and marqo_url_and_version_cache[self.url] == "_skipped":
+            mq_logger.warning(skip_warning_message)
+            return
+
+        # Skip the check for Marqo CloudV2 APIs right now
+        skip_version_check_url = ["https://api.marqo.ai", "https://cloud.marqo.ai"]
+        if self.url in skip_version_check_url:
+            marqo_url_and_version_cache[self.url] = "_skipped"
+            mq_logger.warning(skip_warning_message)
+            return
+
+        # Do version check
+        try:
+            if self.url not in marqo_url_and_version_cache:
+                marqo_url_and_version_cache[self.url] = self.get_marqo()["version"]
+            marqo_version = marqo_url_and_version_cache[self.url]
+            if versioning_helpers.parse(marqo_version) < versioning_helpers.parse(min_ver):
+                mq_logger.warning(f"Your Marqo Python client requires a minimum Marqo version of "
+                                  f"{minimum_supported_marqo_version()} to function properly, but your Marqo version is {marqo_version}. "
+                                  f"Please upgrade your Marqo instance to avoid potential errors. "
+                                  f"If you have already changed your Marqo instance but still get this warning, please restart your Marqo client Python interpreter.")
+        except (MarqoWebError, RequestException, TypeError, KeyError) as e:
+            mq_logger.warning(skip_warning_message)
+            marqo_url_and_version_cache[self.url] = "_skipped"
+        return
+
```

### Comparing `marqo-0.9.6/src/marqo/defaults.py` & `marqo-1.0.0/src/marqo/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,10 +14,10 @@
                 "split_overlap": 0,
                 "split_method": "sentence"
             },
             "image_preprocessing": {
                 "patch_method": None
             }
         },
-        "number_of_shards": 2,
-        "number_of_replicas": 1,
+        "number_of_shards": 1,
+        "number_of_replicas": 0,
     }
```

### Comparing `marqo-0.9.6/src/marqo/index.py` & `marqo-1.0.0/src/marqo/index.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import functools
 import json
 import logging
 import pprint
+import time
+
 from marqo import defaults
 import typing
 from urllib import parse
 from datetime import datetime
 from timeit import default_timer as timer
 from typing import Any, Dict, Generator, List, Optional, Union
 from marqo._httprequests import HttpRequests
@@ -50,15 +52,18 @@
     def create(config: Config, index_name: str,
                treat_urls_and_pointers_as_images=False,
                model=None,
                normalize_embeddings=True,
                sentences_per_chunk=2,
                sentence_overlap=0,
                image_preprocessing_method=None,
-               settings_dict: dict = None
+               settings_dict: dict = None,
+               inference_node_type: str = None,
+               storage_node_type: str = None,
+               inference_node_count: int = 1,
                ) -> Dict[str, Any]:
         """Create the index.
 
         Args:
             config: config instance
             index_name: name of the index.
             treat_urls_and_pointers_as_images:
@@ -66,14 +71,17 @@
             normalize_embeddings:
             sentences_per_chunk:
             sentence_overlap:
             image_preprocessing_method:
             settings_dict: if specified, overwrites all other setting
                 parameters, and is passed directly as the index's
                 index_settings
+            inference_node_type: inference type for the index
+            storage_node_type: storage type for the index
+            inference_node_count: number of inference nodes for the index
         Returns:
             Response body, containing information about index creation result
         """
         req = HttpRequests(config)
 
         if settings_dict is not None and settings_dict:
             return req.post(f"indexes/{index_name}", body=settings_dict)
@@ -87,15 +95,27 @@
             cl_ix_defaults['model'] = model
             cl_ix_defaults['normalize_embeddings'] = normalize_embeddings
             cl_text_preprocessing = cl_ix_defaults['text_preprocessing']
             cl_text_preprocessing['split_overlap'] = sentence_overlap
             cl_text_preprocessing['split_length'] = sentences_per_chunk
             cl_img_preprocessing = cl_ix_defaults['image_preprocessing']
             cl_img_preprocessing['patch_method'] = image_preprocessing_method
-            return req.post(f"indexes/{index_name}", body=cl_settings)
+            if not config.cluster_is_marqo:
+                return req.post(f"indexes/{index_name}", body=cl_settings)
+            cl_settings['inference_type'] = inference_node_type
+            cl_settings['storage_class'] = storage_node_type
+            cl_settings['inference_node_count'] = inference_node_count
+            response = req.post(f"indexes/{index_name}", body=cl_settings)
+            index = Index(config, index_name)
+            creation = index.get_status()
+            while creation['index_status'] != 'READY':
+                time.sleep(10)
+                creation = index.get_status()
+                mq_logger.info(f"Index creation status: {creation['index_status']}")
+            return response
 
         return req.post(f"indexes/{index_name}", body={
             "index_defaults": {
                 "treat_urls_and_pointers_as_images": treat_urls_and_pointers_as_images,
                 "model": model,
                 "normalize_embeddings": normalize_embeddings,
                 "text_preprocessing": {
@@ -107,15 +127,19 @@
                     "patch_method": image_preprocessing_method
                 }
             }
         })
 
     def refresh(self):
         """refreshes the index"""
-        return self.http.post(path=F"indexes/{self.index_name}/refresh")
+        return self.http.post(path=F"indexes/{self.index_name}/refresh", index_name=self.index_name,)
+
+    def get_status(self):
+        """gets the status of the index"""
+        return self.http.get(path=F"indexes/{self.index_name}/status")
 
     def search(self, q: Union[str, dict], searchable_attributes: Optional[List[str]] = None,
                limit: int = 10, offset: int = 0, search_method: Union[SearchMethods.TENSOR, str] = SearchMethods.TENSOR,
                highlights=None, device: Optional[str] = None, filter_string: str = None,
                show_highlights=True, reranker=None, image_download_headers: Optional[Dict] = None,
                attributes_to_retrieve: Optional[List[str]] = None, boost: Optional[Dict[str,List[Union[float, int]]]] = None,
                context: Optional[dict] = None, score_modifiers: Optional[dict] = None, model_auth: Optional[dict] = None
@@ -133,37 +157,36 @@
             searchable_attributes:  attributes to search
             limit: The max number of documents to be returned
             offset: The number of search results to skip (for pagination)
             search_method: Indicates TENSOR or LEXICAL (keyword) search
             show_highlights: True if highlights are to be returned
             reranker:
             device: the device used to index the data. Examples include "cpu",
-                "cuda" and "cuda:2". Overrides the Client's default device.
+                "cuda" and "cuda:2".
             filter_string: a filter string, used to prefilter documents during the
                 search. For example: "car_colour:blue"
             attributes_to_retrieve: a list of document attributes to be
                 retrieved. If left as None, then all attributes will be
                 retrieved.
             context: a dictionary to allow you to bring your own vectors and more into search.
             score_modifiers: a dictionary to modify the score based on field values, for tensor search only
             model_auth: authorisation that lets Marqo download a private model, if required
         Returns:
             Dictionary with hits and other metadata
         """
 
         start_time_client_request = timer()
         if highlights is not None:
-            logging.warning("Deprecation warning for parameter 'highlights'. "
-                            "Please use the 'showHighlights' instead. ")
+            mq_logger.warning("Deprecation warning for parameter 'highlights'. "
+                              "Please use the 'showHighlights' instead. ")
             show_highlights = highlights if show_highlights is True else show_highlights
 
-        selected_device = device if device is not None else self.config.search_device
         path_with_query_str = (
-            f"indexes/{self.index_name}/search?"
-            f"&device={utils.translate_device_string_for_url(selected_device)}"
+            f"indexes/{self.index_name}/search"
+            f"{f'?&device={utils.translate_device_string_for_url(device)}' if device is not None else ''}"
         )
         body = {
             "q": q,
             "searchableAttributes": searchable_attributes,
             "limit": limit,
             "offset": offset,
             "searchMethod": search_method,
@@ -181,15 +204,16 @@
             body["context"] = context
         if score_modifiers is not None:
             body["scoreModifiers"] = score_modifiers
         if model_auth is not None:
             body["modelAuth"] = model_auth
         res = self.http.post(
             path=path_with_query_str,
-            body=body
+            body=body,
+            index_name=self.index_name,
         )
 
         num_results = len(res["hits"])
         end_time_client_request = timer()
         total_client_request_time = end_time_client_request - start_time_client_request
 
         search_time_log = (f"search ({search_method.lower()}): took {(total_client_request_time):.3f}s to send query "
@@ -211,15 +235,15 @@
 
         Returns:
             Dictionary containing the documents information.
         """
         url_string = f"indexes/{self.index_name}/documents/{document_id}"
         if expose_facets is not None:
             url_string += f"?expose_facets={expose_facets}"
-        return self.http.get(url_string)
+        return self.http.get(url_string, index_name=self.index_name,)
 
     def get_documents(self, document_ids: List[str], expose_facets=None) -> Dict[str, Any]:
         """Gets a selection of documents based on their IDs.
 
         Args:
             document_ids: IDs to be searched
             expose_facets: If True, tensor facets will be returned for the the
@@ -230,227 +254,159 @@
             Dictionary containing the documents information.
         """
         url_string = f"indexes/{self.index_name}/documents"
         if expose_facets is not None:
             url_string += f"?expose_facets={expose_facets}"
         return self.http.get(
             url_string,
-            body=document_ids
+            body=document_ids,
+            index_name=self.index_name,
         )
 
     def add_documents(
         self,
         documents: List[Dict[str, Any]],
-        auto_refresh=True,
-        server_batch_size: int = None,
+        auto_refresh: bool = True,
         client_batch_size: int = None,
-        processes: int = None,
         device: str = None,
+        tensor_fields: List[str] = None,
         non_tensor_fields: List[str] = None,
         use_existing_tensors: bool = False,
         image_download_headers: dict = None,
         mappings: dict = None,
         model_auth: dict = None
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
         """Add documents to this index. Does a partial update on existing documents,
         based on their ID. Adds unseen documents to the index.
 
         Args:
             documents: List of documents. Each document should be a dictionary.
             auto_refresh: Automatically refresh the index. If you are making
                 lots of requests, it is advised to set this to False to
                 increase performance.
-            server_batch_size: if it is set, documents will be indexed into batches
-                on the server as they are indexed. Otherwise documents are unbatched
-                server-side.
             client_batch_size: if it is set, documents will be indexed into batches
                 in the client, before being sent off. Otherwise documents are unbatched
                 client-side.
-            processes: number of processes for the server to use, to do indexing,
             device: the device used to index the data. Examples include "cpu",
                 "cuda" and "cuda:2"
-            non_tensor_fields: fields within documents to not create and store tensors against.
+            tensor_fields: fields within documents to create and store tensors against.
+            non_tensor_fields: fields within documents to not create and store tensors against. Cannot be used with
+                tensor_fields.
+                .. deprecated:: 2.0.0
+                    This parameter has been deprecated and will be removed in Marqo 2.0.0. User tensor_fields instead.
             use_existing_tensors: use vectors that already exist in the docs.
             image_download_headers: a dictionary of headers to be passed while downloading images,
                 for URLs found in documents
             mappings: a dictionary to help handle the object fields. e.g., multimodal_combination field
             model_auth: used to authorise a private model
         Returns:
             Response body outlining indexing result
         """
-        if non_tensor_fields is None:
-            non_tensor_fields = []
+        if tensor_fields is not None and non_tensor_fields is not None:
+            raise errors.InvalidArgError('Cannot define `non_tensor_fields` when `tensor_fields` is defined. '
+                                         '`non_tensor_fields` has been deprecated and will be removed in Marqo 2.0.0. '
+                                         'Its use is discouraged.')
+
+        if tensor_fields is None and non_tensor_fields is None:
+            raise errors.InvalidArgError('You must include the `tensor_fields` parameter. '
+                                         'Use `tensor_fields=[]` to index for lexical-only search.')
+
+        if non_tensor_fields is not None:
+            mq_logger.warning('The `non_tensor_fields` parameter has been deprecated and will be removed in '
+                              'Marqo 2.0.0. Use `tensor_fields` instead.')
+
         if image_download_headers is None:
             image_download_headers = dict()
-        return self._generic_add_update_docs(
-            update_method="replace",
-            documents=documents, auto_refresh=auto_refresh, server_batch_size=server_batch_size,
-            client_batch_size=client_batch_size, processes=processes, device=device, non_tensor_fields=non_tensor_fields,
-            use_existing_tensors=use_existing_tensors, image_download_headers=image_download_headers, mappings=mappings,
-            model_auth=model_auth
+        return self._add_docs_organiser(
+            documents=documents, auto_refresh=auto_refresh,
+            client_batch_size=client_batch_size, device=device, tensor_fields=tensor_fields,
+            non_tensor_fields=non_tensor_fields, use_existing_tensors=use_existing_tensors,
+            image_download_headers=image_download_headers, mappings=mappings, model_auth=model_auth
         )
 
-    def update_documents(
+    def _add_docs_organiser(
         self,
         documents: List[Dict[str, Any]],
         auto_refresh=True,
-        server_batch_size: int = None,
         client_batch_size: int = None,
-        processes: int = None,
-        device: str = None,
-        non_tensor_fields: List[str] = None,
-    ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
-        """
-        Will be deprecated soon.
-        Add documents to this index. Does a partial updates on existing documents,
-        based on their ID. Adds unseen documents to the index.
-
-        Args:
-            documents: List of documents. Each document should be a dictionary.
-            auto_refresh: Automatically refresh the index. If you are making
-                lots of requests, it is advised to turn this to false to
-                increase performance.
-            server_batch_size: if it is set, documents will be indexed into batches
-                on the server as they are indexed. Otherwise documents are unbatched
-                server-side.
-            client_batch_size: if it is set, documents will be indexed into batches
-                in the client, before being sent of. Otherwise documents are unbatched
-                client-side.
-            processes: number of processes for the server to use, to do indexing,
-            device: the device used to index the data. Examples include "cpu",
-                "cuda" and "cuda:2"
-            non_tensor_fields: fields within documents to not create and store tensors against.
-
-        Returns:
-            Response body outlining indexing result
-        """
-        mq_logger.warning(
-            "`update_documents()` is deprecated and will be removed in a future release. "
-            "To update documents with minimal inference operations, use `add_documents()` "
-            "with use_existing_tensors=True ")
-        if non_tensor_fields is None:
-            non_tensor_fields = []
-        return self._generic_add_update_docs(
-            update_method="update",
-            documents=documents, auto_refresh=auto_refresh, server_batch_size=server_batch_size,
-            client_batch_size=client_batch_size, processes=processes, device=device, non_tensor_fields=non_tensor_fields,
-        )
-
-    def _generic_add_update_docs(
-        self,
-        update_method: str,
-        documents: List[Dict[str, Any]],
-        auto_refresh=True,
-        server_batch_size: int = None,
-        client_batch_size: int = None,
-        processes: int = None,
         device: str = None,
+        tensor_fields: List = None,
         non_tensor_fields: List = None,
         use_existing_tensors: bool = False,
         image_download_headers: dict = None,
         mappings: dict = None,
         model_auth: dict = None
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
 
+        if (tensor_fields is None and non_tensor_fields is None) \
+                or (tensor_fields is not None and non_tensor_fields is not None):
+            raise ValueError("Exactly one of tensor_fields or non_tensor_fields must be provided.")
+
         error_detected_message = ('Errors detected in add documents call. '
                                   'Please examine the returned result object for more information.')
-        if non_tensor_fields is None:
-            non_tensor_fields = []
 
-        selected_device = device if device is not None else self.config.indexing_device
         num_docs = len(documents)
 
         # ADD DOCS TIMER-LOGGER (1)
         t0 = timer()
         start_time_client_process = timer()
         base_path = f"indexes/{self.index_name}/documents"
-        non_tensor_fields_query_param = utils.convert_list_to_query_params("non_tensor_fields", non_tensor_fields)
-        image_download_headers_param = (utils.convert_dict_to_url_params(image_download_headers)
-                                        if image_download_headers else '')
-        model_auth_param = (utils.convert_dict_to_url_params(model_auth) if model_auth else '')
-        mappings_param = (utils.convert_dict_to_url_params(mappings) if mappings else '')
         query_str_params = (
-            f"{f'&device={utils.translate_device_string_for_url(selected_device)}'}"
-            f"{f'&processes={processes}' if processes is not None else ''}"
-            f"{f'&batch_size={server_batch_size}' if server_batch_size is not None else ''}"
-            f"{f'&use_existing_tensors={str(use_existing_tensors).lower()}' if use_existing_tensors is not None else ''}"
-            f"{f'&{non_tensor_fields_query_param}' if len(non_tensor_fields) > 0 else ''}"
-            f"{f'&image_download_headers={image_download_headers_param}' if image_download_headers else ''}"
-            f"{f'&mappings={mappings_param}' if mappings else ''}"
-            f"{f'&model_auth={model_auth_param}' if model_auth_param else ''}"
+            f"{f'&device={utils.translate_device_string_for_url(device)}' if device is not None else ''}"
         )
+
+        base_body = {
+            "useExistingTensors" : use_existing_tensors,
+            "imageDownloadHeaders" : image_download_headers,
+            "mappings" : mappings,
+            "modelAuth": model_auth,
+        }
+        if tensor_fields is not None:
+            base_body['tensorFields'] = tensor_fields
+        else:
+            base_body['nonTensorFields'] = non_tensor_fields
+
         end_time_client_process = timer()
         total_client_process_time = end_time_client_process - start_time_client_process
         mq_logger.debug(f"add_documents pre-processing: took {(total_client_process_time):.3f}s for {num_docs} docs, "
                        f"for an average of {(total_client_process_time / num_docs):.3f}s per doc.")
 
         if client_batch_size is not None:
             if client_batch_size <= 0:
                 raise errors.InvalidArgError("Batch size can't be less than 1!")
             res = self._batch_request(
                 base_path=base_path, auto_refresh=auto_refresh,
-                update_method=update_method, docs=documents, verbose=False,
-                query_str_params=query_str_params, batch_size=client_batch_size
+                docs=documents, verbose=False,
+                query_str_params=query_str_params, batch_size=client_batch_size, base_body = base_body
             )
 
         else:
             # no Client Batching
             refresh_option = f"?refresh={str(auto_refresh).lower()}"
             path_with_query_str = f"{base_path}{refresh_option}{query_str_params}"
 
             # ADD DOCS TIMER-LOGGER (2)
             start_time_client_request = timer()
 
-            if update_method == 'update':
-                res = self.http.put(path=path_with_query_str, body=documents)
-            elif update_method == 'replace':
-                res = self.http.post(path=path_with_query_str, body=documents)
-            else:
-                raise ValueError(f'Received unknown update_method `{update_method}`. '
-                                 f'Allowed update_methods: ["replace", "update"] ')
-
-
+            body = {"documents": documents, **base_body}
+            res = self.http.post(
+                path=path_with_query_str, body=body, index_name=self.index_name,
+            )
             end_time_client_request = timer()
             total_client_request_time = end_time_client_request - start_time_client_request
 
             mq_logger.debug(f"add_documents roundtrip: took {(total_client_request_time):.3f}s to send {num_docs} "
                             f"docs to Marqo (roundtrip, unbatched), for an average of {(total_client_request_time / num_docs):.3f}s per doc.")
             errors_detected = False
-            if server_batch_size is not None:
-                # with Server Batching (show processing time for each batch)
-                mq_logger.debug(f"add_documents Marqo index (server-side batch reports): ")
-
-                if processes is not None and processes > 1:
-                    # for multiprocess, timing messages should be arranged by process, then batch
-                    for process in range(len(res)):
-                        mq_logger.debug(f"   process {process}:")
 
-                        for batch in range(len(res[process])):
-                            server_batch_result_count = len(res[process][batch]["items"])
-                            mq_logger.debug(f"       marqo server batch {batch}: "
-                                            f"processed {server_batch_result_count} docs in {(res[process][batch]['processingTimeMs'] / 1000):.3f}s, "
-                                            f"for an average of {(res[process][batch]['processingTimeMs'] / (1000 * server_batch_result_count)):.3f}s per doc.")
-                            if 'errors' in res[process][batch] and res[process][batch]['errors']:
-                                errors_detected = True
-                else:
-                    # for single process, timing messages should be arranged by batch ONLY
-                    for batch in range(len(res)):
-                        server_batch_result_count = len(res[batch]["items"])
-                        mq_logger.debug(f"   marqo server batch {batch}: "
-                                        f"processed {server_batch_result_count} docs in {(res[batch]['processingTimeMs'] / 1000):.3f}s, "
-                                        f"for an average of {(res[batch]['processingTimeMs'] / (1000 * server_batch_result_count)):.3f}s per doc.")
-                        if 'errors' in res[batch] and res[batch]['errors']:
-                            errors_detected = True
-            else:
-                # no Server Batching
-                if 'processingTimeMs' in res:       # Only outputs log if response is non-empty
-                    mq_logger.debug(f"add_documents Marqo index: took {(res['processingTimeMs'] / 1000):.3f}s for Marqo to process & index {num_docs} "
-                                    f"docs (server unbatched), for an average of {(res['processingTimeMs'] / (1000 * num_docs)):.3f}s per doc.")
-                if 'errors' in res and res['errors']:
-                    mq_logger.info(error_detected_message)
+            if 'processingTimeMs' in res:       # Only outputs log if response is non-empty
+                mq_logger.debug(f"add_documents Marqo index: took {(res['processingTimeMs'] / 1000):.3f}s for Marqo to process & index {num_docs} "
+                                f"docs (server unbatched), for an average of {(res['processingTimeMs'] / (1000 * num_docs)):.3f}s per doc.")
+            if 'errors' in res and res['errors']:
+                mq_logger.info(error_detected_message)
 
             if errors_detected:
                 mq_logger.info(error_detected_message)
         total_add_docs_time = timer() - t0
         mq_logger.debug(f"add_documents completed. total time taken: {(total_add_docs_time):.3f}s.")
         return res
 
@@ -463,21 +419,19 @@
 
         Returns:
             A dict with information about the delete operation.
         """
         base_path = f"indexes/{self.index_name}/documents/delete-batch"
         path_with_refresh = base_path if auto_refresh is None else base_path + f"?refresh={str(auto_refresh).lower()}"
 
-        return self.http.post(
-            path=path_with_refresh, body=ids
-        )
+        return self.http.post(path=path_with_refresh, body=ids, index_name=self.index_name,)
 
     def get_stats(self) -> Dict[str, Any]:
         """Get stats about the index"""
-        return self.http.get(path=f"indexes/{self.index_name}/stats")
+        return self.http.get(path=f"indexes/{self.index_name}/stats", index_name=self.index_name,)
 
     @staticmethod
     def _maybe_datetime(the_date: Optional[Union[datetime, str]]) -> Optional[datetime]:
         """This should handle incoming timestamps from Marqo, including
          parsing if necessary."""
         if the_date is None or not the_date:
             return None
@@ -486,17 +440,16 @@
             return the_date
         elif isinstance(the_date, str):
             parsed_date = datetime.strptime(the_date, "%Y-%m-%dT%H:%M:%S.%f")
             return parsed_date
 
     def _batch_request(
             self, docs: List[Dict],  base_path: str,
-            query_str_params: str,
-            update_method: str, verbose: bool = True,
-            auto_refresh: bool = True, batch_size: int = 50
+            query_str_params: str, base_body: dict, verbose: bool = True,
+            auto_refresh: bool = True, batch_size: int = 50,
     ) -> List[Dict[str, Any]]:
         """Batches a large chunk of documents to be sent as multiple
         add_documents invocations
 
         Args:
             docs: A list of documents
             batch_size: Size of a batch passed into a single add_documents
@@ -524,21 +477,17 @@
 
         batched = functools.reduce(lambda x, y: batch_requests(x, y), deeper, [])
 
         def verbosely_add_docs(i, docs):
             errors_detected = False
 
             t0 = timer()
-            if update_method == 'replace':
-                res = self.http.post(path=path_with_query_str, body=docs)
-            elif update_method == 'update':
-                res = self.http.put(path=path_with_query_str, body=docs)
-            else:
-                raise ValueError(f'Received unknown update_method `{update_method}`. '
-                                 f'Allowed update_methods: ["replace", "update"] ')
+            body = {"documents": docs, **base_body}
+            res = self.http.post(path=path_with_query_str, body=body, index_name=self.index_name)
+
             total_batch_time = timer() - t0
             num_docs = len(docs)
 
             if isinstance(res, list):
                 # with Server Batching (show processing time for each batch)
                 mq_logger.info(
                     f"    add_documents batch {i} roundtrip: took {(total_batch_time):.3f}s to add {num_docs} docs, "
@@ -586,8 +535,8 @@
         if auto_refresh:
             self.refresh()
         mq_logger.debug('completed batch ingestion.')
         return results
 
     def get_settings(self) -> dict:
         """Get all settings of the index"""
-        return self.http.get(path=f"indexes/{self.index_name}/settings")
+        return self.http.get(path=f"indexes/{self.index_name}/settings", index_name=self.index_name,)
```

### Comparing `marqo-0.9.6/src/marqo/models.py` & `marqo-1.0.0/src/marqo/models.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.6/src/marqo/utils.py` & `marqo-1.0.0/src/marqo/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         raise errors.MarqoError(f"Could not parse url: {url_base}")
     url_split = url_base.split(http_sep)
     if len(url_split) != 2:
         raise errors.MarqoError(f"Could not parse url: {url_base}")
     http_part, domain_part = url_split
     return f"{http_part}{http_sep}{username}:{password}@{domain_part}"
 
+
 def translate_device_string_for_url(device: Optional[str]) -> Optional[str]:
     """Translates a device string for use as a URL param
 
     Args:
         device: a string representing a device on the server. Examples include
             "cpu", "cuda", "cuda:2"
```

### Comparing `marqo-0.9.6/src/marqo.egg-info/PKG-INFO` & `marqo-1.0.0/src/marqo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 0.9.6
+Version: 1.0.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -116,25 +116,28 @@
 4. Start indexing and searching! Let's look at a simple example below:
 
 ```python
 import marqo
 
 mq = marqo.Client(url='http://localhost:8882')
 
-mq.index("my-first-index").add_documents([
-    {
-        "Title": "The Travels of Marco Polo",
-        "Description": "A 13th-century travelogue describing Polo's travels"
-    }, 
-    {
-        "Title": "Extravehicular Mobility Unit (EMU)",
-        "Description": "The EMU is a spacesuit that provides environmental protection, "
-                       "mobility, life support, and communications for astronauts",
-        "_id": "article_591"
-    }]
+mq.create_index("my-first-index")
+mq.index("my-first-index").add_documents(
+    [
+        {
+            "Title": "The Travels of Marco Polo",
+            "Description": "A 13th-century travelogue describing Polo's travels"},
+        {
+            "Title": "Extravehicular Mobility Unit (EMU)",
+            "Description": "The EMU is a spacesuit that provides environmental protection, "
+                           "mobility, life support, and communications for astronauts",
+            "_id": "article_591"
+        }
+    ], 
+    tensor_fields=["Title", "Description"]
 )
 
 results = mq.index("my-first-index").search(
     q="What is the best outfit to wear on the moon?", searchable_attributes=["Title", "Description"]
 )
 
 ```
@@ -286,16 +289,16 @@
 ```python
 
 import marqo
 import pprint
 
 mq = marqo.Client(url="http://localhost:8882")
 
-mq.index("my-weighted-query-index").add_documents(
-    [
+mq.create_index("my-weighted-query-index")
+mq.index("my-weighted-query-index").add_documents([
         {
             "Title": "Smartphone",
             "Description": "A smartphone is a portable computer device that combines mobile telephone "
             "functions and computing functions into one unit.",
         },
         {
             "Title": "Telephone",
@@ -304,15 +307,16 @@
         },
         {
             "Title": "Thylacine",
             "Description": "The thylacine, also commonly known as the Tasmanian tiger or Tasmanian wolf, "
             "is an extinct carnivorous marsupial."
             "The last known of its species died in 1936.",
         },
-    ]
+    ],
+    tensor_fields=["Title", "Description"]
 )
 
 # initially we ask for a type of communications device which is popular in the 21st century
 query = {
     # a weighting of 1.1 gives this query slightly more importance
     "I need to buy a communications device, what should I get?": 1.1,
     # a weighting of 1 gives this query a neutral importance
@@ -379,26 +383,24 @@
             "Title": "Horse Jumping",
             "captioned_image": {
                 "caption": "A person riding a horse over a jump in a competition.",
                 "image": "https://raw.githubusercontent.com/marqo-ai/marqo/mainline/examples/ImageSearchGuide/data/image1.jpg",
             },
         },
     ],
-    # Create the mappings, here we define our captioned_image mapping 
-    # which weights the image more heavily than the caption - these pairs 
-    # will be represented by a single vector in the index
     mappings={
         "captioned_image": {
             "type": "multimodal_combination",
             "weights": {
                 "caption": 0.3,
                 "image": 0.7,
             },
         }
     },
+    tensor_fields=["captioned_image"],
 )
 
 # Search this index with a simple text query
 results = mq.index("my-first-multimodal-index").search(
     q="Give me some images of vehicles and modes of transport. I am especially interested in air travel and commercial aeroplanes.",
     searchable_attributes=["captioned_image"],
 )
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 0.9.6 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 1.0.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
@@ -60,21 +60,22 @@
 (https://docs.docker.com/get-docker/). Ensure that docker has at least 8GB
 memory and 50GB storage. 2. Use docker to run Marqo (Mac users with M-series
 chips will need to [go here](#m-series-mac-users)): ```bash docker rm -f marqo
 docker pull marqoai/marqo:latest docker run --name marqo -it --privileged -
 p 8882:8882 --add-host host.docker.internal:host-gateway marqoai/marqo:latest
 ``` 3. Install the Marqo client: ```bash pip install marqo ``` 4. Start
 indexing and searching! Let's look at a simple example below: ```python import
-marqo mq = marqo.Client(url='http://localhost:8882') mq.index("my-first-
-index").add_documents([ { "Title": "The Travels of Marco Polo", "Description":
-"A 13th-century travelogue describing Polo's travels" }, { "Title":
-"Extravehicular Mobility Unit (EMU)", "Description": "The EMU is a spacesuit
-that provides environmental protection, " "mobility, life support, and
-communications for astronauts", "_id": "article_591" }] ) results = mq.index
-("my-first-index").search( q="What is the best outfit to wear on the moon?",
+marqo mq = marqo.Client(url='http://localhost:8882') mq.create_index("my-first-
+index") mq.index("my-first-index").add_documents( [ { "Title": "The Travels of
+Marco Polo", "Description": "A 13th-century travelogue describing Polo's
+travels"}, { "Title": "Extravehicular Mobility Unit (EMU)", "Description": "The
+EMU is a spacesuit that provides environmental protection, " "mobility, life
+support, and communications for astronauts", "_id": "article_591" } ],
+tensor_fields=["Title", "Description"] ) results = mq.index("my-first-
+index").search( q="What is the best outfit to wear on the moon?",
 searchable_attributes=["Title", "Description"] ) ``` - `mq` is the client that
 wraps the `marqo` API - `add_documents()` takes a list of documents,
 represented as python dicts for indexing. - `add_documents()` creates an index
 with default settings, if one does not already exist. - You can optionally set
 a document's ID with the special `_id` field. Otherwise, Marqo will generate
 one. - If the index doesn't exist, Marqo will create it. If it exists then
 Marqo will add the documents to the index. Let's have a look at the results:
@@ -128,62 +129,61 @@
 ai_hippo_statue.png') ``` ### Searching using weights in queries Queries can
 also be provided as dictionaries where each key is a query and their
 corresponding values are weights. This allows for more advanced queries
 consisting of multiple components with weightings towards or against them,
 queries can have negations via negative weighting. The example below shows the
 application of this to a scenario where a user may want to ask a question but
 also negate results that match a certain semantic criterion. ```python import
-marqo import pprint mq = marqo.Client(url="http://localhost:8882") mq.index
-("my-weighted-query-index").add_documents( [ { "Title": "Smartphone",
-"Description": "A smartphone is a portable computer device that combines mobile
-telephone " "functions and computing functions into one unit.", }, { "Title":
-"Telephone", "Description": "A telephone is a telecommunications device that
-permits two or more users to" "conduct a conversation when they are too far
-apart to be easily heard directly.", }, { "Title": "Thylacine", "Description":
-"The thylacine, also commonly known as the Tasmanian tiger or Tasmanian wolf, "
-"is an extinct carnivorous marsupial." "The last known of its species died in
-1936.", }, ] ) # initially we ask for a type of communications device which is
-popular in the 21st century query = { # a weighting of 1.1 gives this query
-slightly more importance "I need to buy a communications device, what should I
-get?": 1.1, # a weighting of 1 gives this query a neutral importance
-"Technology that became prevelant in the 21st century": 1.0, } results =
-mq.index("my-weighted-query-index").search( q=query, searchable_attributes=
-["Title", "Description"] ) print("Query 1:") pprint.pprint(results) # now we
-ask for a type of communications which predates the 21st century query = { # a
-weighting of 1 gives this query a neutral importance "I need to buy a
-communications device, what should I get?": 1.0, # a weighting of -1 gives this
-query a negation effect "Technology that became prevelant in the 21st century":
--1.0, } results = mq.index("my-weighted-query-index").search( q=query,
-searchable_attributes=["Title", "Description"] ) print("\nQuery 2:")
-pprint.pprint(results) ``` ### Creating and searching indexes with multimodal
-combination fields Marqo lets you have indexes with multimodal combination
-fields. Multimodal combination fields can combine text and images into one
-field. This allows scoring of documents across the combined text and image
-fields together. It also allows for a single vector representation instead of
-needing many which saves on storage. The relative weighting of each component
-can be set per document. The example below demonstrates this with retrival of
-caption and image pairs using multiple types of queries. ```python import marqo
-import pprint mq = marqo.Client(url="http://localhost:8882") settings =
-{"treat_urls_and_pointers_as_images": True, "model": "ViT-L/14"}
+marqo import pprint mq = marqo.Client(url="http://localhost:8882")
+mq.create_index("my-weighted-query-index") mq.index("my-weighted-query-
+index").add_documents([ { "Title": "Smartphone", "Description": "A smartphone
+is a portable computer device that combines mobile telephone " "functions and
+computing functions into one unit.", }, { "Title": "Telephone", "Description":
+"A telephone is a telecommunications device that permits two or more users to"
+"conduct a conversation when they are too far apart to be easily heard
+directly.", }, { "Title": "Thylacine", "Description": "The thylacine, also
+commonly known as the Tasmanian tiger or Tasmanian wolf, " "is an extinct
+carnivorous marsupial." "The last known of its species died in 1936.", }, ],
+tensor_fields=["Title", "Description"] ) # initially we ask for a type of
+communications device which is popular in the 21st century query = { # a
+weighting of 1.1 gives this query slightly more importance "I need to buy a
+communications device, what should I get?": 1.1, # a weighting of 1 gives this
+query a neutral importance "Technology that became prevelant in the 21st
+century": 1.0, } results = mq.index("my-weighted-query-index").search( q=query,
+searchable_attributes=["Title", "Description"] ) print("Query 1:")
+pprint.pprint(results) # now we ask for a type of communications which predates
+the 21st century query = { # a weighting of 1 gives this query a neutral
+importance "I need to buy a communications device, what should I get?": 1.0, #
+a weighting of -1 gives this query a negation effect "Technology that became
+prevelant in the 21st century": -1.0, } results = mq.index("my-weighted-query-
+index").search( q=query, searchable_attributes=["Title", "Description"] ) print
+("\nQuery 2:") pprint.pprint(results) ``` ### Creating and searching indexes
+with multimodal combination fields Marqo lets you have indexes with multimodal
+combination fields. Multimodal combination fields can combine text and images
+into one field. This allows scoring of documents across the combined text and
+image fields together. It also allows for a single vector representation
+instead of needing many which saves on storage. The relative weighting of each
+component can be set per document. The example below demonstrates this with
+retrival of caption and image pairs using multiple types of queries. ```python
+import marqo import pprint mq = marqo.Client(url="http://localhost:8882")
+settings = {"treat_urls_and_pointers_as_images": True, "model": "ViT-L/14"}
 mq.create_index("my-first-multimodal-index", **settings) mq.index("my-first-
 multimodal-index").add_documents( [ { "Title": "Flying Plane",
 "captioned_image": { "caption": "An image of a passenger plane flying in front
 of the moon.", "image": "https://raw.githubusercontent.com/marqo-ai/marqo/
 mainline/examples/ImageSearchGuide/data/image2.jpg", }, }, { "Title": "Red
 Bus", "captioned_image": { "caption": "A red double decker London bus traveling
 to Aldwych", "image": "https://raw.githubusercontent.com/marqo-ai/marqo/
 mainline/examples/ImageSearchGuide/data/image4.jpg", }, }, { "Title": "Horse
 Jumping", "captioned_image": { "caption": "A person riding a horse over a jump
 in a competition.", "image": "https://raw.githubusercontent.com/marqo-ai/marqo/
-mainline/examples/ImageSearchGuide/data/image1.jpg", }, }, ], # Create the
-mappings, here we define our captioned_image mapping # which weights the image
-more heavily than the caption - these pairs # will be represented by a single
-vector in the index mappings={ "captioned_image": { "type":
-"multimodal_combination", "weights": { "caption": 0.3, "image": 0.7, }, } }, )
-# Search this index with a simple text query results = mq.index("my-first-
+mainline/examples/ImageSearchGuide/data/image1.jpg", }, }, ], mappings=
+{ "captioned_image": { "type": "multimodal_combination", "weights":
+{ "caption": 0.3, "image": 0.7, }, } }, tensor_fields=["captioned_image"], ) #
+Search this index with a simple text query results = mq.index("my-first-
 multimodal-index").search( q="Give me some images of vehicles and modes of
 transport. I am especially interested in air travel and commercial
 aeroplanes.", searchable_attributes=["captioned_image"], ) print("Query 1:")
 pprint.pprint(results) # search the index with a query that uses weighted
 components results = mq.index("my-first-multimodal-index").search( q={ "What
 are some vehicles and modes of transport?": 1.0, "Aeroplanes and other things
 that fly": -1.0, }, searchable_attributes=["captioned_image"], ) print("\nQuery
```

