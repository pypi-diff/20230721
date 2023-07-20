# Comparing `tmp/getpaper-0.2.6.tar.gz` & `tmp/getpaper-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.2.6.tar", last modified: Wed Jul 19 00:26:23 2023, max compression
+gzip compressed data, was "getpaper-0.2.8.tar", last modified: Thu Jul 20 22:44:38 2023, max compression
```

## Comparing `getpaper-0.2.6.tar` & `getpaper-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-07-19 00:26:23.989173 getpaper-0.2.6/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.2.6/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5937 2023-07-19 00:26:23.989173 getpaper-0.2.6/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5322 2023-07-19 00:22:38.000000 getpaper-0.2.6/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-07-19 00:26:23.989173 getpaper-0.2.6/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.2.6/getpaper/__init__.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5288 2023-06-26 00:35:31.000000 getpaper-0.2.6/getpaper/clean.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1020 2023-06-29 07:49:25.000000 getpaper-0.2.6/getpaper/config.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12926 2023-06-29 13:16:29.000000 getpaper-0.2.6/getpaper/download.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12234 2023-07-19 00:25:52.000000 getpaper-0.2.6/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12854 2023-06-29 07:52:58.000000 getpaper-0.2.6/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5052 2023-06-29 10:54:05.000000 getpaper-0.2.6/getpaper/splitting.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-07-19 00:26:23.989173 getpaper-0.2.6/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5937 2023-07-19 00:26:23.000000 getpaper-0.2.6/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      357 2023-07-19 00:26:23.000000 getpaper-0.2.6/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-07-19 00:26:23.000000 getpaper-0.2.6/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-07-19 00:26:23.000000 getpaper-0.2.6/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      247 2023-07-19 00:26:23.000000 getpaper-0.2.6/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-07-19 00:26:23.000000 getpaper-0.2.6/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-07-19 00:26:23.989173 getpaper-0.2.6/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1666 2023-07-19 00:12:59.000000 getpaper-0.2.6/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-07-20 22:44:38.733813 getpaper-0.2.8/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.2.8/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6804 2023-07-20 22:44:38.733813 getpaper-0.2.8/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6189 2023-07-20 22:28:24.000000 getpaper-0.2.8/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-07-20 22:44:38.733813 getpaper-0.2.8/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.2.8/getpaper/__init__.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5288 2023-06-26 00:35:31.000000 getpaper-0.2.8/getpaper/clean.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1083 2023-07-20 21:39:22.000000 getpaper-0.2.8/getpaper/config.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12926 2023-07-20 21:47:12.000000 getpaper-0.2.8/getpaper/download.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    13065 2023-07-20 22:40:31.000000 getpaper-0.2.8/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)    12854 2023-07-20 21:48:35.000000 getpaper-0.2.8/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5052 2023-07-20 21:41:58.000000 getpaper-0.2.8/getpaper/splitting.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-07-20 22:44:38.733813 getpaper-0.2.8/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     6804 2023-07-20 22:44:38.000000 getpaper-0.2.8/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      357 2023-07-20 22:44:38.000000 getpaper-0.2.8/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-07-20 22:44:38.000000 getpaper-0.2.8/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-07-20 22:44:38.000000 getpaper-0.2.8/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      268 2023-07-20 22:44:38.000000 getpaper-0.2.8/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-07-20 22:44:38.000000 getpaper-0.2.8/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-07-20 22:44:38.733813 getpaper-0.2.8/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1690 2023-07-20 22:34:22.000000 getpaper-0.2.8/setup.py
```

### Comparing `getpaper-0.2.6/LICENSE` & `getpaper-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.6/PKG-INFO` & `getpaper-0.2.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.2.6
+Version: 0.2.8
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -40,19 +40,19 @@
 ## Downloading papers
 
 After the installation you can either import the library into your python code or you can use the console scripts.
 
 If you install from pip calling _download_ will mean calling getpaper/download.py , for _parse_ - getpaper/parse.py , for _index_ - getpaper/index.py
 
 ```bash
-download download download_pubmed --pubmed 22266545 --folder papers --name pmid
+download download_pubmed --pubmed 22266545 --folder papers --name pmid
 ```
 Downloads the paper with pubmed id into the folder 'papers' and uses the pubmed id as name
 ```bash
-download download download_doi --doi 10.1519/JSC.0b013e318225bbae --folder papers
+download download_doi --doi 10.1519/JSC.0b013e318225bbae --folder papers
 ```
 Downloads the paper with DOI into the folder papers, as --name is not specified doi is used as name
 
 It is also possible to download many papers in parallel with download_papers(dois: List[str], destination: Path, threads: int) function, for example:
 ```python
 from pathlib import Path
 from typing import List
@@ -102,15 +102,15 @@
 
 ```bash
 getpaper/parse.py count_tokens --path /home/antonkulaga/sources/non-animal-models/data/inputs/datasets
 ```
 
 ## Indexing papers
 
-We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
+We also provide features to index the papers with openai or llama embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
@@ -119,18 +119,30 @@
 cd services
 docker compose -f docker-compose.yaml up
 ```
 then you can run the indexing of the paper with Qdrant:
 ```
 getpaper/index.py index_papers --papers data/output/test/papers --url http://localhost:6333 --collection mypapers --chunk_size 6000 --database Qdrant
 ```
+You can also take a look if things were added to the collection with qdrant web UI by checking http://localhost:6333/dashboard
+
+### Indexing with Llama-2 embeddings ###
+You can also use llama-2 embeddings if you install llama-cpp-python and pass a path to the model, for example for https://huggingface.co/TheBloke/Llama-2-13B-GGML model:
+```
+getpaper/index.py index_papers --papers data/output/test/papers --url http://localhost:6333 --collection papers_llama2_2000 --chunk_size 2000 --database Qdrant --embeddings llama --model /home/antonkulaga/sources/getpaper/data/models/llama-2-13b-chat.ggmlv3.q2_K.bin
+```
+Instead of explicitly pathing the model path you can also include the path to LLAMA_MODEL to the .env file as:
+```
+LLAMA_MODEL="/home/antonkulaga/sources/getpaper/data/models/llama-2-13b-chat.ggmlv3.q2_K.bin"
+```
 Note: if you want to use Qdrant cloud you do not need docker-compose, but you need to provide a key and look at qdrant cloud setting for the url to give.
 ```
 getpaper/index.py index_papers --papers data/output/test/papers --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io:6333 --key put_your_key_here --collection mypapers --chunk_size 6000 --database Qdrant
 ```
+Note: there are temporal issues with embeddings for llama.
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
```

### Comparing `getpaper-0.2.6/README.md` & `getpaper-0.2.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 ## Downloading papers
 
 After the installation you can either import the library into your python code or you can use the console scripts.
 
 If you install from pip calling _download_ will mean calling getpaper/download.py , for _parse_ - getpaper/parse.py , for _index_ - getpaper/index.py
 
 ```bash
-download download download_pubmed --pubmed 22266545 --folder papers --name pmid
+download download_pubmed --pubmed 22266545 --folder papers --name pmid
 ```
 Downloads the paper with pubmed id into the folder 'papers' and uses the pubmed id as name
 ```bash
-download download download_doi --doi 10.1519/JSC.0b013e318225bbae --folder papers
+download download_doi --doi 10.1519/JSC.0b013e318225bbae --folder papers
 ```
 Downloads the paper with DOI into the folder papers, as --name is not specified doi is used as name
 
 It is also possible to download many papers in parallel with download_papers(dois: List[str], destination: Path, threads: int) function, for example:
 ```python
 from pathlib import Path
 from typing import List
@@ -84,15 +84,15 @@
 
 ```bash
 getpaper/parse.py count_tokens --path /home/antonkulaga/sources/non-animal-models/data/inputs/datasets
 ```
 
 ## Indexing papers
 
-We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
+We also provide features to index the papers with openai or llama embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
@@ -101,18 +101,30 @@
 cd services
 docker compose -f docker-compose.yaml up
 ```
 then you can run the indexing of the paper with Qdrant:
 ```
 getpaper/index.py index_papers --papers data/output/test/papers --url http://localhost:6333 --collection mypapers --chunk_size 6000 --database Qdrant
 ```
+You can also take a look if things were added to the collection with qdrant web UI by checking http://localhost:6333/dashboard
+
+### Indexing with Llama-2 embeddings ###
+You can also use llama-2 embeddings if you install llama-cpp-python and pass a path to the model, for example for https://huggingface.co/TheBloke/Llama-2-13B-GGML model:
+```
+getpaper/index.py index_papers --papers data/output/test/papers --url http://localhost:6333 --collection papers_llama2_2000 --chunk_size 2000 --database Qdrant --embeddings llama --model /home/antonkulaga/sources/getpaper/data/models/llama-2-13b-chat.ggmlv3.q2_K.bin
+```
+Instead of explicitly pathing the model path you can also include the path to LLAMA_MODEL to the .env file as:
+```
+LLAMA_MODEL="/home/antonkulaga/sources/getpaper/data/models/llama-2-13b-chat.ggmlv3.q2_K.bin"
+```
 Note: if you want to use Qdrant cloud you do not need docker-compose, but you need to provide a key and look at qdrant cloud setting for the url to give.
 ```
 getpaper/index.py index_papers --papers data/output/test/papers --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io:6333 --key put_your_key_here --collection mypapers --chunk_size 6000 --database Qdrant
 ```
+Note: there are temporal issues with embeddings for llama.
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
```

### Comparing `getpaper-0.2.6/getpaper/clean.py` & `getpaper-0.2.8/getpaper/clean.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.6/getpaper/config.py` & `getpaper-0.2.8/getpaper/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,18 +20,21 @@
 LOG_LEVELS = [loader.value for loader in LogLevel]
 
 
 def configure_logger(log_level: Union[str, LogLevel]):
     level = log_level.value if isinstance(log_level, LogLevel) else log_level
     # yes, it is duplicate but it is nice to avoid cross-module dependencies here
     if level.upper() != LogLevel.NONE.value:
+        logger
         logger.add(sys.stdout, level=level.upper())
 
-def load_environment_keys(debug: bool = True):
-    e = dotenv.find_dotenv()
+
+def load_environment_keys(debug: bool = True, usecwd:bool = False):
+    e = dotenv.find_dotenv(usecwd=usecwd)
+    print(e)
     if debug:
         print(f"environment found at {e}")
     has_env: bool = load_dotenv(e, verbose=True, override=True)
     if not has_env:
         print("Did not found environment file, using system OpenAI key (if exists)")
     openai_key = os.getenv('OPENAI_API_KEY')
     return openai_key
```

### Comparing `getpaper-0.2.6/getpaper/download.py` & `getpaper-0.2.8/getpaper/download.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.6/getpaper/index.py` & `getpaper-0.2.8/getpaper/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import os
 from enum import Enum
 from pathlib import Path
 
 import click
 from click import Context
 from langchain.embeddings import OpenAIEmbeddings, LlamaCppEmbeddings, VertexAIEmbeddings
 from langchain.embeddings.base import Embeddings
@@ -20,19 +21,21 @@
     Chroma = "Chroma"
     Qdrant = "Qdrant"
 
 
 VECTOR_DATABASES: list[str] = [db.value for db in VectorDatabase]
 
 
-def resolve_embeddings(embeddings_name: str) -> Embeddings:
+def resolve_embeddings(embeddings_name: str, model_path: Optional[Union[Path, str]] = None) -> Embeddings:
     if embeddings_name == "openai":
         return OpenAIEmbeddings()
-    elif embeddings_name == "lambda":
-        return LlamaCppEmbeddings()
+    elif embeddings_name == "llama":
+        if model_path is None:
+            logger.error(f"for llama embeddings for {model_path} model")
+        return LlamaCppEmbeddings(model_path = str(model_path))
     elif embeddings_name == "vertexai":
         return VertexAIEmbeddings()
     else:
         logger.warning(f"{embeddings_name} is not yet supported by CLI, using default openai embeddings instead")
         return OpenAIEmbeddings()
 
 
@@ -86,24 +89,24 @@
     for doc in documents:
         logger.trace(f"ADD TEXT: {doc.page_content}")
         logger.trace(f"ADD METADATA {doc.metadata}")
     db.add_texts(texts=texts, metadatas=metadatas, ids=ids)
     return db
 
 
-def init_qdrant(collection_name: str, path_or_url: str,  embedding_function: Optional[Embeddings], api_key: Optional[str] = None, distance_func: str = "Cosine"):
+def init_qdrant(collection_name: str, path_or_url: str,  embedding_function: Optional[Embeddings], api_key: Optional[str] = None, distance_func: str = "Cosine", prefer_grpc: bool = False):
     is_url = "ttp:" in path_or_url or "ttps:" in path_or_url
     path: Optional[str] = None if is_url else path_or_url
     url: Optional[str] = path_or_url if is_url else None
     logger.info(f"initializing quadrant database at {path_or_url}")
     client: QdrantClient = QdrantClient(
         url=url,
         port=6333,
         grpc_port=6334,
-        prefer_grpc=is_url,
+        prefer_grpc=is_url if prefer_grpc is None else prefer_grpc,
         api_key=api_key,
         path=path
     )
     from qdrant_client.http import models as rest
     #client.recreate_collection(collection_name)
     # Just do a single quick embedding to get vector size
     partial_embeddings = embedding_function.embed_documents("probe")
@@ -114,47 +117,41 @@
         vectors_config=rest.VectorParams(
             size=vector_size,
             distance=rest.Distance[distance_func],
         )
     )
     return Qdrant(client, collection_name=collection_name, embeddings=embedding_function)
 
-"""
-def init_db(database: VectorDatabase, collection_name: str, path_or_url: Optional[Union[Path, str]], embeddings: Optional[Embeddings]):
-    if database == VectorDatabase.Chroma:
-        return Chroma(collection_name=collection_name, persist_directory=str(where), embedding_function=embeddings)
-    elif database == VectorDatabase.Qdrant:
-        return init_qdrant(collection_name=collection_name, path_or_url=path_or_url, embedding_function=embeddings)
-"""
 
 def write_remote_db(url: str,
                     collection_name: str,
                     documents: list[Document],
                     splitter: TextSplitter,
                     id_field: Optional[str] = None,
                     embeddings: Optional[Embeddings] = None,
                     database: VectorDatabase = VectorDatabase.Qdrant,
-                    key: Optional[str] = None):
+                    key: Optional[str] = None, prefer_grpc: bool = False):
     if database == VectorDatabase.Qdrant:
         logger.info(f"writing a collection {collection_name} of {len(documents)} documents to quadrant db at {url}")
-        db = init_qdrant(collection_name, path_or_url=url, embedding_function=embeddings, api_key=key)
+        db = init_qdrant(collection_name, path_or_url=url, embedding_function=embeddings, api_key=key, prefer_grpc=prefer_grpc)
         db_updated = db_with_documents(db, documents, splitter,  id_field)
         return db_updated
     else:
         raise Exception(f"Remote Chroma is not yet supported by this script!")
     pass
 
 
 def write_local_db(persist_directory: Path,
                    collection_name: str,
                    documents: list[Document],
                    splitter: TextSplitter,
                    id_field: Optional[str] = None,
                    embeddings: Optional[Embeddings] = None,
-                   database: VectorDatabase = VectorDatabase.Qdrant
+                   database: VectorDatabase = VectorDatabase.Chroma,
+                   prefer_grpc: bool = False
                    ):
     """
     Writes the provided documents to a database.
 
     Args:
         persist_directory (Path): The directory where the database should be saved.
         collection_name (str): The name of the collection in the database.
@@ -175,15 +172,15 @@
 
     # If no embeddings were provided, default to OpenAIEmbeddings
     if embeddings is None:
         embeddings = OpenAIEmbeddings()
 
     # Create a Chroma database with the specified collection name and embeddings, and save it in the specified directory
     if database == VectorDatabase.Qdrant:
-        db = init_qdrant(collection_name, str(where), embedding_function=embeddings)
+        db = init_qdrant(collection_name, str(where), embedding_function=embeddings,  prefer_grpc = prefer_grpc)
     else:
         db = Chroma(collection_name=collection_name, persist_directory=str(where), embedding_function=embeddings)
     #db = init_db(database, collection_name=collection_name, path_or_url=str(where), embedding_function=embeddings)
     # Add the documents to the database
     db_updated = db_with_documents(db, documents, splitter,  id_field)
 
     # Persist the changes to the database
@@ -198,66 +195,78 @@
 def app(ctx: Context):
     # if ctx.invoked_subcommand is None:
     #    click.echo('Running the default command...')
     #    test_index()
     pass
 
 
-@logger.catch
-def index_papers(papers_folder: Path,
-                 collection: str,
-                 splitter: SourceTextSplitter,
-                 embeddings: str,
-                 include_meta: bool,
-                 folder: Optional[str] = None,
-                 url: Optional[str] = None,
-                 key: Optional[str] = None,
-                 database: VectorDatabase = VectorDatabase.Chroma.value
-                 ):
-    load_environment_keys() # for openai key
-    embeddings_function = resolve_embeddings(embeddings)
+def index_selected_papers(papers_folder: Path,
+                          collection: str,
+                          splitter: SourceTextSplitter,
+                          embeddings: str,
+                          include_meta: bool,
+                          folder: Optional[Union[Path,str]] = None,
+                          url: Optional[str] = None,
+                          key: Optional[str] = None,
+                          database: VectorDatabase = VectorDatabase.Chroma.value,
+                          model: Optional[Union[Path, str]] = None,
+                          prefer_grpc: Optional[bool] = None
+                          ):
+    openai_key = load_environment_keys() #for openai key
+    embeddings_function = resolve_embeddings(embeddings, model)
     logger.info(f"embeddings are {embeddings}")
     documents = papers_to_documents(papers_folder, include_meta=include_meta)
     if folder is not None:
-        index = Path(folder)
+        index = Path(folder) if isinstance(folder, str) else folder
         index.mkdir(exist_ok=True)
         where = index / f"{embeddings}_{splitter.chunk_size}_chunk"
         where.mkdir(exist_ok=True, parents=True)
         logger.info(f"writing index of papers to {where}")
-        return write_local_db(where, collection, documents, splitter, embeddings=embeddings_function)
+        return write_local_db(where, collection, documents, splitter, embeddings=embeddings_function, prefer_grpc = prefer_grpc, database=database)
     elif url is not None:
-        return write_remote_db(url, collection, documents, splitter, embeddings=embeddings_function, database=database, key=key)
+        return write_remote_db(url, collection, documents, splitter, embeddings=embeddings_function, database=database, key=key, prefer_grpc = prefer_grpc)
     else:
         raise Exception("neither folder nor url are set")
         pass
 
 
 @app.command("index_papers")
 @click.option('--papers', type=click.Path(exists=True), help="papers folder to index")
 @click.option('--collection', default='papers', help='papers collection name')
 @click.option('--folder', type=click.Path(), default=None, help="folder to put chroma indexes to")
 @click.option('--url', type=click.STRING, default=None, help="alternatively you can provide url, for example http://localhost:6333 for qdrant")
 @click.option('--key', type=click.STRING, default=None, help="your api key if you are using cloud vector store")
 @click.option('--splitter_name', type=click.Choice(["openai", "recursive"]), default="openai", help='which splitter to choose for the text splitting')
 @click.option('--chunk_size', type=click.INT, default=3000, help='size of the chunk for splitting (characters for recursive spliiter and tokens for openai one)')
-@click.option('--embeddings', type=click.Choice(["openai", "lambda", "vertexai"]), default="openai",
+@click.option('--embeddings', type=click.Choice(["openai", "llama", "vertexai"]), default="openai",
               help='size of the chunk for splitting')
+@click.option("--model", type=click.Path(), default=None, help="path to the model (required for embeddings)")
 @click.option('--include_meta', type=click.BOOL, default=True, help="if metadata is included")
 @click.option('--database', type=click.Choice(VECTOR_DATABASES, case_sensitive=False), default=VectorDatabase.Chroma.value, help = "which store to take")
+@click.option('--prefer_grpc', type=click.BOOL, default = None)
 @click.option('--log_level', type=click.Choice(LOG_LEVELS, case_sensitive=False), default=LogLevel.DEBUG.value, help="logging level")
-def index_papers_command(papers: str, collection: str, folder: str, url: str, key: str, splitter_name: str, chunk_size: int, embeddings: str, include_meta: bool, database: str, log_level: str) -> Path:
+def index_papers_command(papers: str, collection: str, folder: str, url: str, key: str, splitter_name: str, chunk_size: int, embeddings: str, model: Optional[str], include_meta: bool, database: str, prefer_grpc: Optional[bool], log_level: str) -> Path:
     configure_logger(log_level)
+    load_environment_keys(usecwd=True)
     papers_folder = Path(papers)
     assert not (folder is None and url is None and key is None), "either database folder or database url or api_key should be provided!"
-    if splitter_name == "recursive":
+    if splitter_name == "openai":
         # Create a RecursiveSplitterWithSource to split the documents into chunks of the specified size
         splitter = SourceTextSplitter(chunk_size=chunk_size)
     elif splitter_name == "recursive":
         splitter = OpenAISplitter(tokens=chunk_size)
     else:
         logger.warning(f"{splitter_name} is not supported, using openai tiktoken based splitter instead")
         splitter = OpenAISplitter(tokens=chunk_size)
-    return index_papers(papers_folder, collection, splitter, embeddings, include_meta, folder, url, database=VectorDatabase[database], key=key)
+    if embeddings == "llama" and model is None:
+        model = os.getenv("LLAMA_MODEL")
+
+    return index_selected_papers(papers_folder, collection, splitter, embeddings, include_meta, folder, url,
+                                 database=VectorDatabase[database],
+                                 key=key,
+                                 model=model,
+                                 prefer_grpc=prefer_grpc
+                                 )
 
 
 if __name__ == '__main__':
     app()
```

### Comparing `getpaper-0.2.6/getpaper/parse.py` & `getpaper-0.2.8/getpaper/parse.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.6/getpaper/splitting.py` & `getpaper-0.2.8/getpaper/splitting.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.2.6/getpaper.egg-info/PKG-INFO` & `getpaper-0.2.8/getpaper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.2.6
+Version: 0.2.8
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
@@ -40,19 +40,19 @@
 ## Downloading papers
 
 After the installation you can either import the library into your python code or you can use the console scripts.
 
 If you install from pip calling _download_ will mean calling getpaper/download.py , for _parse_ - getpaper/parse.py , for _index_ - getpaper/index.py
 
 ```bash
-download download download_pubmed --pubmed 22266545 --folder papers --name pmid
+download download_pubmed --pubmed 22266545 --folder papers --name pmid
 ```
 Downloads the paper with pubmed id into the folder 'papers' and uses the pubmed id as name
 ```bash
-download download download_doi --doi 10.1519/JSC.0b013e318225bbae --folder papers
+download download_doi --doi 10.1519/JSC.0b013e318225bbae --folder papers
 ```
 Downloads the paper with DOI into the folder papers, as --name is not specified doi is used as name
 
 It is also possible to download many papers in parallel with download_papers(dois: List[str], destination: Path, threads: int) function, for example:
 ```python
 from pathlib import Path
 from typing import List
@@ -102,15 +102,15 @@
 
 ```bash
 getpaper/parse.py count_tokens --path /home/antonkulaga/sources/non-animal-models/data/inputs/datasets
 ```
 
 ## Indexing papers
 
-We also provide features to index the papers with openai or lambda embeddings and save them in chromadb vector store.
+We also provide features to index the papers with openai or llama embeddings and save them in chromadb vector store.
 For openai embeddings to work you have to create .env file and specify your openai key there, see .env.template as example
 
 For example if you have your papers inside data/output/test/papers folder, and you want to make a ChromaDB index at data/output/test/index you can do it by:
 ```bash
 getpaper/index.py index_papers --papers data/output/test/papers --folder data/output/test/index --collection mypapers --chunk_size 6000
 ```
 
@@ -119,18 +119,30 @@
 cd services
 docker compose -f docker-compose.yaml up
 ```
 then you can run the indexing of the paper with Qdrant:
 ```
 getpaper/index.py index_papers --papers data/output/test/papers --url http://localhost:6333 --collection mypapers --chunk_size 6000 --database Qdrant
 ```
+You can also take a look if things were added to the collection with qdrant web UI by checking http://localhost:6333/dashboard
+
+### Indexing with Llama-2 embeddings ###
+You can also use llama-2 embeddings if you install llama-cpp-python and pass a path to the model, for example for https://huggingface.co/TheBloke/Llama-2-13B-GGML model:
+```
+getpaper/index.py index_papers --papers data/output/test/papers --url http://localhost:6333 --collection papers_llama2_2000 --chunk_size 2000 --database Qdrant --embeddings llama --model /home/antonkulaga/sources/getpaper/data/models/llama-2-13b-chat.ggmlv3.q2_K.bin
+```
+Instead of explicitly pathing the model path you can also include the path to LLAMA_MODEL to the .env file as:
+```
+LLAMA_MODEL="/home/antonkulaga/sources/getpaper/data/models/llama-2-13b-chat.ggmlv3.q2_K.bin"
+```
 Note: if you want to use Qdrant cloud you do not need docker-compose, but you need to provide a key and look at qdrant cloud setting for the url to give.
 ```
 getpaper/index.py index_papers --papers data/output/test/papers --url https://5bea7502-97d4-4876-98af-0cdf8af4bd18.us-east-1-0.aws.cloud.qdrant.io:6333 --key put_your_key_here --collection mypapers --chunk_size 6000 --database Qdrant
 ```
+Note: there are temporal issues with embeddings for llama.
 
 # Examples
 
 You can run examples.py to see usage examples
 
 # Additional requirements
```

### Comparing `getpaper-0.2.6/setup.py` & `getpaper-0.2.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.6'
+VERSION = '0.2.8'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
@@ -19,16 +19,16 @@
     author_email="<antonkulaga@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['pyfunctional', 'more-itertools', 'click', 'python-dotenv', 'tiktoken', 'pynction',
                       'unstructured', 'unstructured-inference', 'unstructured[local-inference]', 'unstructured.PaddleOCR',
-                      'scidownl', 'langchain', 'openai', 'Deprecated', 'semanticscholar', 'pdfminer', 'loguru',
-                      'qdrant-client', 'chromadb'],
+                      'scidownl', 'langchain', 'openai', 'Deprecated', 'semanticscholar', 'pdfminer.six', 'loguru',
+                      'qdrant-client', 'chromadb', 'llama-cpp-python'],
     keywords=['python', 'utils', 'files', 'papers', 'download'],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         "Operating System :: Unix",
```

