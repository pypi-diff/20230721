# Comparing `tmp/fastapi-serve-0.0.6.dev5.tar.gz` & `tmp/fastapi-serve-0.0.7.dev45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.6.dev5.tar", last modified: Thu Jul 20 14:42:41 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.7.dev45.tar", last modified: Fri Jul 21 10:21:34 2023, max compression
```

## Comparing `fastapi-serve-0.0.6.dev5.tar` & `fastapi-serve-0.0.7.dev45.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.985055 fastapi-serve-0.0.6.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-20 14:42:41.985055 fastapi-serve-0.0.6.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.985055 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/blob/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/blob/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/fastapi_serve/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:41.981055 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 14:42:41.000000 fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:42:41.985055 fastapi-serve-0.0.6.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-20 14:42:37.000000 fastapi-serve-0.0.6.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.251269 fastapi-serve-0.0.7.dev45/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-21 10:21:33.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.251269 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/blob/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/fastapi_serve/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:34.251269 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 10:21:34.000000 fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:21:34.255269 fastapi-serve-0.0.7.dev45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-21 10:21:29.000000 fastapi-serve-0.0.7.dev45/setup.py
```

### Comparing `fastapi-serve-0.0.6.dev5/LICENSE` & `fastapi-serve-0.0.7.dev45/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/PKG-INFO` & `fastapi-serve-0.0.7.dev45/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.6.dev5
+Version: 0.0.7.dev45
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -35,32 +35,32 @@
 <p align=center>
 <a href="https://pypi.org/project/fastapi-serve/"><img alt="PyPI" src="https://img.shields.io/pypi/v/fastapi-serve?label=Release&style=flat-square"></a>
 <a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
 <a href="https://pypistats.org/packages/fastapi-serve"><img alt="PyPI - Downloads from official pypistats" src="https://img.shields.io/pypi/dm/fastapi-serve?style=flat-square"></a>
 <a href="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml"><img alt="Github CD status" src="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml/badge.svg"></a>
 </p>
 
-Welcome to **fastapi-serve**, your one-stop solution to seamless FastAPI application deployments. Powered by our open-source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve` provides an effortless transition from your local setup to [cloud.jina.ai](https://cloud.jina.ai/), our robust and scalable cloud platform. 🌩️
+Welcome to **fastapi-serve**, your one-stop solution for seamless FastAPI application deployments. Powered by our open-source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve` provides an effortless transition from your local setup to [cloud.jina.ai](https://cloud.jina.ai/), our robust and scalable cloud platform. 🌩️
 
 Designed with developers in mind, `fastapi-serve` simplifies the deployment process by packing robust functionality, ease-of-use, and automated procedures into one comprehensive package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI application development, allowing you to focus on what truly matters - writing great code!
 
 
 ## 😍 Features 
 
 - 🌎 **HTTPS**: Auto-provisioned DNS and TLS certificates for your app.
 - 🔗 **Protocols**: Full compatibility with HTTP, WebSocket, and GraphQL.
 - ↕️ **Scaling**: Scale your app manually or let it auto-scale based on RPS, CPU, and Memory.
 - 🗝️ **Secrets**: Secure handling of secrets and environment variables.
 - 🎛️ **Hardware**: Choose the right compute resources for your app's needs with ease.
-- 🔒 **Authorization**: Built-in OAuth2.0 token-based security to secure your endpoints. 
+- 🔒 **Authorization**: Built-in `OAuth2.0` token-based security to secure your endpoints. 
 - 💾 **App Storage**: Persistent and secure network storage for your app data.
 - 🔄 **Blob Storage**: Built-in support for seamless user file uploads and downloads.
 - 🔎 **Observability**: Integrated access to logs, metrics, and traces. (Alerting coming soon!)
 - 📦 **Containerization**: Effortless containerization of your Python codebase with our integrated registry.
-- 🛠️ **Self-Hosting**: Export your app for self-hosting with ease, including docker-compose and Kubernetes yamls.
+- 🛠️ **Self-Hosting**: Export your app for self-hosting with ease, including docker-compose and Kubernetes YAMLs.
 
 ## 💡 Getting Started
 
 First, install the `fastapi-serve` package using pip:
 
 ```bash
 pip install fastapi-serve
@@ -75,45 +75,45 @@
 You'll get a URL to access your newly deployed application along with the Swagger UI.
 
 ## 📚 Documentation
 
 Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
 - 🚀 **Getting Started**
-    - 🧱 [Deploy a Simple FastAPI Application](docs/simple/)
+    - 🧱 [Deploy a simple FastAPI application](docs/simple/)
     - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
-    - ⚙️ [Understanding Configuration and Pricing](docs/CONFIG.MD)
+    - ⚙️ [Understanding configuration and pricing on Jina AI Cloud](docs/CONFIG.MD)
     - 🔄 [Upgrade your FastAPI applications with zero downtime](docs/upgrades/)
-    - 🏢 Managing Larger Applications with Complex Directory Structure (Example TBD!)
+    - 🏢 Managing Larger Applications with Complex Directory Structure (Documentation in progress 🚧)
 - ↕️ **Scaling**
     - 💹 [Auto-scaling endpoints based on CPU usage](docs/autoscaling/cpu/)
     - 📉 [Serverless (scale-to-zero) deployments based on RPS](docs/autoscaling/serverless/) 
 - 🧩 **Config & Credentials**
-    - 🌍 [Leverage Environment Variables for app configuration](docs/envs/)
-    - 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
+    - 🌍 [Leverage environment variables for app configuration](docs/envs/)
+    - 🗝️ [Use secrets for Redis-powered rate limiting](docs/rate_limit/)
 - 💾 **Storage**
-    - 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
-    - 🌐 Network Storage for persisting and securely accessing app data (Example TBD!)
+    - 📁 [Manage file uploads and downloads with built-in blob storage](docs/file_handling/)
+    - 🌐 Network storage for persisting and securely accessing app data (Documentation in progress 🚧)
 - 🔒 **Security**
-    - 👮‍♂️ [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
+    - 👮‍♂️ [Secure your endpoints with built-in OAuth2.0 authorization](docs/authorization/)
 - 🐳 **Deployment Options**
-    - 🚢 Deployment with Custom Dockerfile (Coming Soon!)
-    - ☸️ [Export Your App for Self-Hosting with docker-compose / Kubernetes](docs/export/)
+    - 🚢 Deployment with custom dockerfile (Documentation in progress 🚧)
+    - ☸️ [Export your app for self-hosting with docker-compose / Kubernetes](docs/export/)
 - 📈 **Observability**
-    - 📊 Access Logs, Metrics, and Traces for your app (Example TBD!)
-    - 🚨 Set up Alerts for your app (Coming Soon!)
+    - 📊 Access logs, metrics, and traces for your app (Documentation in progress 🚧)
+    - 🚨 Set up alerts for your app (Documentation in progress 🚧)
 
 
 ## 💪 Support
 
 If you encounter any problems or have questions, feel free to open an issue on the GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to get help from our community members and the Jina team.
 
 
 ## 🌐 Our Cloud Platform  
 
-`cloud.jina.ai` is our robust and scalable cloud platform designed to run your FastAPI applications with minimum hassle and maximum efficiency. With features like auto-scaling, integrated observability, and automated containerization, it provides a seamless and worry-free deployment experience.
+Our robust and scalable cloud platform `cloud.jina.ai` is designed to run your FastAPI applications with minimum hassle and maximum efficiency. With features like auto-scaling, integrated observability, and automated containerization, it provides a seamless and worry-free deployment experience.
 
 ---
 
 `fastapi-serve` is more than just a deployment tool, it's a bridge that connects your local development environment with our powerful cloud infrastructure. Start using `fastapi-serve` today, and experience the joy of effortless deployments! 🎊
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.6.dev5 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.7.dev45 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -16,65 +16,66 @@
 Engineering :: Artificial Intelligence Description-Content-Type: text/markdown
 Provides-Extra: test License-File: LICENSE
  ***** FastAPI-Serve: FastAPI to the Cloud, Batteries Included! âï¸ðð
                                      *****
                     [PyPI] [https://img.shields.io/discord/
   1106542220112302130?logo=discord&logoColor=white&style=flat-square] [PyPI_-
              Downloads_from_official_pypistats] [Github_CD_status]
-Welcome to **fastapi-serve**, your one-stop solution to seamless FastAPI
+Welcome to **fastapi-serve**, your one-stop solution for seamless FastAPI
 application deployments. Powered by our open-source framework [Jina](https://
 github.com/jina-ai/jina), `fastapi-serve` provides an effortless transition
 from your local setup to [cloud.jina.ai](https://cloud.jina.ai/), our robust
 and scalable cloud platform. ð©ï¸ Designed with developers in mind,
 `fastapi-serve` simplifies the deployment process by packing robust
 functionality, ease-of-use, and automated procedures into one comprehensive
 package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI
 application development, allowing you to focus on what truly matters - writing
 great code! ## ð Features - ð **HTTPS**: Auto-provisioned DNS and TLS
 certificates for your app. - ð **Protocols**: Full compatibility with HTTP,
 WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app manually or let it
 auto-scale based on RPS, CPU, and Memory. - ðï¸ **Secrets**: Secure
 handling of secrets and environment variables. - ðï¸ **Hardware**: Choose
 the right compute resources for your app's needs with ease. - ð
-**Authorization**: Built-in OAuth2.0 token-based security to secure your
+**Authorization**: Built-in `OAuth2.0` token-based security to secure your
 endpoints. - ð¾ **App Storage**: Persistent and secure network storage for
 your app data. - ð **Blob Storage**: Built-in support for seamless user file
 uploads and downloads. - ð **Observability**: Integrated access to logs,
 metrics, and traces. (Alerting coming soon!) - ð¦ **Containerization**:
 Effortless containerization of your Python codebase with our integrated
 registry. - ð ï¸ **Self-Hosting**: Export your app for self-hosting with
-ease, including docker-compose and Kubernetes yamls. ## ð¡ Getting Started
+ease, including docker-compose and Kubernetes YAMLs. ## ð¡ Getting Started
 First, install the `fastapi-serve` package using pip: ```bash pip install
 fastapi-serve ``` Then, simply use the `fastapi-serve` command to deploy your
 FastAPI application: ```bash fastapi-serve deploy jcloud main:app ``` You'll
 get a URL to access your newly deployed application along with the Swagger UI.
 ## ð Documentation Dive into understanding `fastapi-serve` through our
 comprehensive documentation and examples: - ð **Getting Started** - ð§±
-[Deploy a Simple FastAPI Application](docs/simple/) - ð¥ï¸ [Dig deep into
-the `fastapi-serve` CLI](docs/CLI.md) - âï¸ [Understanding Configuration and
-Pricing](docs/CONFIG.MD) - ð [Upgrade your FastAPI applications with zero
-downtime](docs/upgrades/) - ð¢ Managing Larger Applications with Complex
-Directory Structure (Example TBD!) - âï¸ **Scaling** - ð¹ [Auto-scaling
-endpoints based on CPU usage](docs/autoscaling/cpu/) - ð [Serverless (scale-
-to-zero) deployments based on RPS](docs/autoscaling/serverless/) - ð§©
-**Config & Credentials** - ð [Leverage Environment Variables for app
-configuration](docs/envs/) - ðï¸ [Use Secrets for Redis-Powered Rate
-Limiting](docs/rate_limit/) - ð¾ **Storage** - ð [Handle File Uploads and
-Downloads with built-in Blob Storage](docs/file_handling/) - ð Network
-Storage for persisting and securely accessing app data (Example TBD!) - ð
-**Security** - ð®ââï¸ [Secure Your Endpoints with built-in OAuth2.0
-Authorization](docs/authorization/) - ð³ **Deployment Options** - ð¢
-Deployment with Custom Dockerfile (Coming Soon!) - â¸ï¸ [Export Your App for
-Self-Hosting with docker-compose / Kubernetes](docs/export/) - ð
-**Observability** - ð Access Logs, Metrics, and Traces for your app (Example
-TBD!) - ð¨ Set up Alerts for your app (Coming Soon!) ## ðª Support If you
-encounter any problems or have questions, feel free to open an issue on the
-GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
-get help from our community members and the Jina team. ## ð Our Cloud
-Platform `cloud.jina.ai` is our robust and scalable cloud platform designed to
-run your FastAPI applications with minimum hassle and maximum efficiency. With
-features like auto-scaling, integrated observability, and automated
-containerization, it provides a seamless and worry-free deployment experience.
---- `fastapi-serve` is more than just a deployment tool, it's a bridge that
-connects your local development environment with our powerful cloud
-infrastructure. Start using `fastapi-serve` today, and experience the joy of
-effortless deployments! ð
+[Deploy a simple FastAPI application](docs/simple/) - ð¥ï¸ [Dig deep into
+the `fastapi-serve` CLI](docs/CLI.md) - âï¸ [Understanding configuration and
+pricing on Jina AI Cloud](docs/CONFIG.MD) - ð [Upgrade your FastAPI
+applications with zero downtime](docs/upgrades/) - ð¢ Managing Larger
+Applications with Complex Directory Structure (Documentation in progress ð§)
+- âï¸ **Scaling** - ð¹ [Auto-scaling endpoints based on CPU usage](docs/
+autoscaling/cpu/) - ð [Serverless (scale-to-zero) deployments based on RPS]
+(docs/autoscaling/serverless/) - ð§© **Config & Credentials** - ð [Leverage
+environment variables for app configuration](docs/envs/) - ðï¸ [Use secrets
+for Redis-powered rate limiting](docs/rate_limit/) - ð¾ **Storage** - ð
+[Manage file uploads and downloads with built-in blob storage](docs/
+file_handling/) - ð Network storage for persisting and securely accessing
+app data (Documentation in progress ð§) - ð **Security** - ð®ââï¸
+[Secure your endpoints with built-in OAuth2.0 authorization](docs/
+authorization/) - ð³ **Deployment Options** - ð¢ Deployment with custom
+dockerfile (Documentation in progress ð§) - â¸ï¸ [Export your app for self-
+hosting with docker-compose / Kubernetes](docs/export/) - ð
+**Observability** - ð Access logs, metrics, and traces for your app
+(Documentation in progress ð§) - ð¨ Set up alerts for your app
+(Documentation in progress ð§) ## ðª Support If you encounter any problems
+or have questions, feel free to open an issue on the GitHub repository. You can
+also join our [Discord](https://discord.jina.ai/) to get help from our
+community members and the Jina team. ## ð Our Cloud Platform Our robust and
+scalable cloud platform `cloud.jina.ai` is designed to run your FastAPI
+applications with minimum hassle and maximum efficiency. With features like
+auto-scaling, integrated observability, and automated containerization, it
+provides a seamless and worry-free deployment experience. --- `fastapi-serve`
+is more than just a deployment tool, it's a bridge that connects your local
+development environment with our powerful cloud infrastructure. Start using
+`fastapi-serve` today, and experience the joy of effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.6.dev5/README.md` & `fastapi-serve-0.0.7.dev45/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 <p align=center>
 <a href="https://pypi.org/project/fastapi-serve/"><img alt="PyPI" src="https://img.shields.io/pypi/v/fastapi-serve?label=Release&style=flat-square"></a>
 <a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
 <a href="https://pypistats.org/packages/fastapi-serve"><img alt="PyPI - Downloads from official pypistats" src="https://img.shields.io/pypi/dm/fastapi-serve?style=flat-square"></a>
 <a href="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml"><img alt="Github CD status" src="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml/badge.svg"></a>
 </p>
 
-Welcome to **fastapi-serve**, your one-stop solution to seamless FastAPI application deployments. Powered by our open-source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve` provides an effortless transition from your local setup to [cloud.jina.ai](https://cloud.jina.ai/), our robust and scalable cloud platform. 🌩️
+Welcome to **fastapi-serve**, your one-stop solution for seamless FastAPI application deployments. Powered by our open-source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve` provides an effortless transition from your local setup to [cloud.jina.ai](https://cloud.jina.ai/), our robust and scalable cloud platform. 🌩️
 
 Designed with developers in mind, `fastapi-serve` simplifies the deployment process by packing robust functionality, ease-of-use, and automated procedures into one comprehensive package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI application development, allowing you to focus on what truly matters - writing great code!
 
 
 ## 😍 Features 
 
 - 🌎 **HTTPS**: Auto-provisioned DNS and TLS certificates for your app.
 - 🔗 **Protocols**: Full compatibility with HTTP, WebSocket, and GraphQL.
 - ↕️ **Scaling**: Scale your app manually or let it auto-scale based on RPS, CPU, and Memory.
 - 🗝️ **Secrets**: Secure handling of secrets and environment variables.
 - 🎛️ **Hardware**: Choose the right compute resources for your app's needs with ease.
-- 🔒 **Authorization**: Built-in OAuth2.0 token-based security to secure your endpoints. 
+- 🔒 **Authorization**: Built-in `OAuth2.0` token-based security to secure your endpoints. 
 - 💾 **App Storage**: Persistent and secure network storage for your app data.
 - 🔄 **Blob Storage**: Built-in support for seamless user file uploads and downloads.
 - 🔎 **Observability**: Integrated access to logs, metrics, and traces. (Alerting coming soon!)
 - 📦 **Containerization**: Effortless containerization of your Python codebase with our integrated registry.
-- 🛠️ **Self-Hosting**: Export your app for self-hosting with ease, including docker-compose and Kubernetes yamls.
+- 🛠️ **Self-Hosting**: Export your app for self-hosting with ease, including docker-compose and Kubernetes YAMLs.
 
 ## 💡 Getting Started
 
 First, install the `fastapi-serve` package using pip:
 
 ```bash
 pip install fastapi-serve
@@ -45,43 +45,43 @@
 You'll get a URL to access your newly deployed application along with the Swagger UI.
 
 ## 📚 Documentation
 
 Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
 - 🚀 **Getting Started**
-    - 🧱 [Deploy a Simple FastAPI Application](docs/simple/)
+    - 🧱 [Deploy a simple FastAPI application](docs/simple/)
     - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
-    - ⚙️ [Understanding Configuration and Pricing](docs/CONFIG.MD)
+    - ⚙️ [Understanding configuration and pricing on Jina AI Cloud](docs/CONFIG.MD)
     - 🔄 [Upgrade your FastAPI applications with zero downtime](docs/upgrades/)
-    - 🏢 Managing Larger Applications with Complex Directory Structure (Example TBD!)
+    - 🏢 Managing Larger Applications with Complex Directory Structure (Documentation in progress 🚧)
 - ↕️ **Scaling**
     - 💹 [Auto-scaling endpoints based on CPU usage](docs/autoscaling/cpu/)
     - 📉 [Serverless (scale-to-zero) deployments based on RPS](docs/autoscaling/serverless/) 
 - 🧩 **Config & Credentials**
-    - 🌍 [Leverage Environment Variables for app configuration](docs/envs/)
-    - 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
+    - 🌍 [Leverage environment variables for app configuration](docs/envs/)
+    - 🗝️ [Use secrets for Redis-powered rate limiting](docs/rate_limit/)
 - 💾 **Storage**
-    - 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
-    - 🌐 Network Storage for persisting and securely accessing app data (Example TBD!)
+    - 📁 [Manage file uploads and downloads with built-in blob storage](docs/file_handling/)
+    - 🌐 Network storage for persisting and securely accessing app data (Documentation in progress 🚧)
 - 🔒 **Security**
-    - 👮‍♂️ [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
+    - 👮‍♂️ [Secure your endpoints with built-in OAuth2.0 authorization](docs/authorization/)
 - 🐳 **Deployment Options**
-    - 🚢 Deployment with Custom Dockerfile (Coming Soon!)
-    - ☸️ [Export Your App for Self-Hosting with docker-compose / Kubernetes](docs/export/)
+    - 🚢 Deployment with custom dockerfile (Documentation in progress 🚧)
+    - ☸️ [Export your app for self-hosting with docker-compose / Kubernetes](docs/export/)
 - 📈 **Observability**
-    - 📊 Access Logs, Metrics, and Traces for your app (Example TBD!)
-    - 🚨 Set up Alerts for your app (Coming Soon!)
+    - 📊 Access logs, metrics, and traces for your app (Documentation in progress 🚧)
+    - 🚨 Set up alerts for your app (Documentation in progress 🚧)
 
 
 ## 💪 Support
 
 If you encounter any problems or have questions, feel free to open an issue on the GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to get help from our community members and the Jina team.
 
 
 ## 🌐 Our Cloud Platform  
 
-`cloud.jina.ai` is our robust and scalable cloud platform designed to run your FastAPI applications with minimum hassle and maximum efficiency. With features like auto-scaling, integrated observability, and automated containerization, it provides a seamless and worry-free deployment experience.
+Our robust and scalable cloud platform `cloud.jina.ai` is designed to run your FastAPI applications with minimum hassle and maximum efficiency. With features like auto-scaling, integrated observability, and automated containerization, it provides a seamless and worry-free deployment experience.
 
 ---
 
 `fastapi-serve` is more than just a deployment tool, it's a bridge that connects your local development environment with our powerful cloud infrastructure. Start using `fastapi-serve` today, and experience the joy of effortless deployments! 🎊
```

#### html2text {}

```diff
@@ -1,63 +1,64 @@
  ***** FastAPI-Serve: FastAPI to the Cloud, Batteries Included! âï¸ðð
                                      *****
                     [PyPI] [https://img.shields.io/discord/
   1106542220112302130?logo=discord&logoColor=white&style=flat-square] [PyPI_-
              Downloads_from_official_pypistats] [Github_CD_status]
-Welcome to **fastapi-serve**, your one-stop solution to seamless FastAPI
+Welcome to **fastapi-serve**, your one-stop solution for seamless FastAPI
 application deployments. Powered by our open-source framework [Jina](https://
 github.com/jina-ai/jina), `fastapi-serve` provides an effortless transition
 from your local setup to [cloud.jina.ai](https://cloud.jina.ai/), our robust
 and scalable cloud platform. ð©ï¸ Designed with developers in mind,
 `fastapi-serve` simplifies the deployment process by packing robust
 functionality, ease-of-use, and automated procedures into one comprehensive
 package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI
 application development, allowing you to focus on what truly matters - writing
 great code! ## ð Features - ð **HTTPS**: Auto-provisioned DNS and TLS
 certificates for your app. - ð **Protocols**: Full compatibility with HTTP,
 WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app manually or let it
 auto-scale based on RPS, CPU, and Memory. - ðï¸ **Secrets**: Secure
 handling of secrets and environment variables. - ðï¸ **Hardware**: Choose
 the right compute resources for your app's needs with ease. - ð
-**Authorization**: Built-in OAuth2.0 token-based security to secure your
+**Authorization**: Built-in `OAuth2.0` token-based security to secure your
 endpoints. - ð¾ **App Storage**: Persistent and secure network storage for
 your app data. - ð **Blob Storage**: Built-in support for seamless user file
 uploads and downloads. - ð **Observability**: Integrated access to logs,
 metrics, and traces. (Alerting coming soon!) - ð¦ **Containerization**:
 Effortless containerization of your Python codebase with our integrated
 registry. - ð ï¸ **Self-Hosting**: Export your app for self-hosting with
-ease, including docker-compose and Kubernetes yamls. ## ð¡ Getting Started
+ease, including docker-compose and Kubernetes YAMLs. ## ð¡ Getting Started
 First, install the `fastapi-serve` package using pip: ```bash pip install
 fastapi-serve ``` Then, simply use the `fastapi-serve` command to deploy your
 FastAPI application: ```bash fastapi-serve deploy jcloud main:app ``` You'll
 get a URL to access your newly deployed application along with the Swagger UI.
 ## ð Documentation Dive into understanding `fastapi-serve` through our
 comprehensive documentation and examples: - ð **Getting Started** - ð§±
-[Deploy a Simple FastAPI Application](docs/simple/) - ð¥ï¸ [Dig deep into
-the `fastapi-serve` CLI](docs/CLI.md) - âï¸ [Understanding Configuration and
-Pricing](docs/CONFIG.MD) - ð [Upgrade your FastAPI applications with zero
-downtime](docs/upgrades/) - ð¢ Managing Larger Applications with Complex
-Directory Structure (Example TBD!) - âï¸ **Scaling** - ð¹ [Auto-scaling
-endpoints based on CPU usage](docs/autoscaling/cpu/) - ð [Serverless (scale-
-to-zero) deployments based on RPS](docs/autoscaling/serverless/) - ð§©
-**Config & Credentials** - ð [Leverage Environment Variables for app
-configuration](docs/envs/) - ðï¸ [Use Secrets for Redis-Powered Rate
-Limiting](docs/rate_limit/) - ð¾ **Storage** - ð [Handle File Uploads and
-Downloads with built-in Blob Storage](docs/file_handling/) - ð Network
-Storage for persisting and securely accessing app data (Example TBD!) - ð
-**Security** - ð®ââï¸ [Secure Your Endpoints with built-in OAuth2.0
-Authorization](docs/authorization/) - ð³ **Deployment Options** - ð¢
-Deployment with Custom Dockerfile (Coming Soon!) - â¸ï¸ [Export Your App for
-Self-Hosting with docker-compose / Kubernetes](docs/export/) - ð
-**Observability** - ð Access Logs, Metrics, and Traces for your app (Example
-TBD!) - ð¨ Set up Alerts for your app (Coming Soon!) ## ðª Support If you
-encounter any problems or have questions, feel free to open an issue on the
-GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
-get help from our community members and the Jina team. ## ð Our Cloud
-Platform `cloud.jina.ai` is our robust and scalable cloud platform designed to
-run your FastAPI applications with minimum hassle and maximum efficiency. With
-features like auto-scaling, integrated observability, and automated
-containerization, it provides a seamless and worry-free deployment experience.
---- `fastapi-serve` is more than just a deployment tool, it's a bridge that
-connects your local development environment with our powerful cloud
-infrastructure. Start using `fastapi-serve` today, and experience the joy of
-effortless deployments! ð
+[Deploy a simple FastAPI application](docs/simple/) - ð¥ï¸ [Dig deep into
+the `fastapi-serve` CLI](docs/CLI.md) - âï¸ [Understanding configuration and
+pricing on Jina AI Cloud](docs/CONFIG.MD) - ð [Upgrade your FastAPI
+applications with zero downtime](docs/upgrades/) - ð¢ Managing Larger
+Applications with Complex Directory Structure (Documentation in progress ð§)
+- âï¸ **Scaling** - ð¹ [Auto-scaling endpoints based on CPU usage](docs/
+autoscaling/cpu/) - ð [Serverless (scale-to-zero) deployments based on RPS]
+(docs/autoscaling/serverless/) - ð§© **Config & Credentials** - ð [Leverage
+environment variables for app configuration](docs/envs/) - ðï¸ [Use secrets
+for Redis-powered rate limiting](docs/rate_limit/) - ð¾ **Storage** - ð
+[Manage file uploads and downloads with built-in blob storage](docs/
+file_handling/) - ð Network storage for persisting and securely accessing
+app data (Documentation in progress ð§) - ð **Security** - ð®ââï¸
+[Secure your endpoints with built-in OAuth2.0 authorization](docs/
+authorization/) - ð³ **Deployment Options** - ð¢ Deployment with custom
+dockerfile (Documentation in progress ð§) - â¸ï¸ [Export your app for self-
+hosting with docker-compose / Kubernetes](docs/export/) - ð
+**Observability** - ð Access logs, metrics, and traces for your app
+(Documentation in progress ð§) - ð¨ Set up alerts for your app
+(Documentation in progress ð§) ## ðª Support If you encounter any problems
+or have questions, feel free to open an issue on the GitHub repository. You can
+also join our [Discord](https://discord.jina.ai/) to get help from our
+community members and the Jina team. ## ð Our Cloud Platform Our robust and
+scalable cloud platform `cloud.jina.ai` is designed to run your FastAPI
+applications with minimum hassle and maximum efficiency. With features like
+auto-scaling, integrated observability, and automated containerization, it
+provides a seamless and worry-free deployment experience. --- `fastapi-serve`
+is more than just a deployment tool, it's a bridge that connects your local
+development environment with our powerful cloud infrastructure. Start using
+`fastapi-serve` today, and experience the joy of effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/__main__.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/config.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/export.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/export.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/cloud/options.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/helper.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/utils/auth.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/utils/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/utils/blob/storage.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/utils/blob/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve/utils/helper.py` & `fastapi-serve-0.0.7.dev45/fastapi_serve/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.6.dev5
+Version: 0.0.7.dev45
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -35,32 +35,32 @@
 <p align=center>
 <a href="https://pypi.org/project/fastapi-serve/"><img alt="PyPI" src="https://img.shields.io/pypi/v/fastapi-serve?label=Release&style=flat-square"></a>
 <a href="https://discord.jina.ai"><img src="https://img.shields.io/discord/1106542220112302130?logo=discord&logoColor=white&style=flat-square"></a>
 <a href="https://pypistats.org/packages/fastapi-serve"><img alt="PyPI - Downloads from official pypistats" src="https://img.shields.io/pypi/dm/fastapi-serve?style=flat-square"></a>
 <a href="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml"><img alt="Github CD status" src="https://github.com/jina-ai/fastapi-serve/actions/workflows/cd.yml/badge.svg"></a>
 </p>
 
-Welcome to **fastapi-serve**, your one-stop solution to seamless FastAPI application deployments. Powered by our open-source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve` provides an effortless transition from your local setup to [cloud.jina.ai](https://cloud.jina.ai/), our robust and scalable cloud platform. 🌩️
+Welcome to **fastapi-serve**, your one-stop solution for seamless FastAPI application deployments. Powered by our open-source framework [Jina](https://github.com/jina-ai/jina), `fastapi-serve` provides an effortless transition from your local setup to [cloud.jina.ai](https://cloud.jina.ai/), our robust and scalable cloud platform. 🌩️
 
 Designed with developers in mind, `fastapi-serve` simplifies the deployment process by packing robust functionality, ease-of-use, and automated procedures into one comprehensive package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI application development, allowing you to focus on what truly matters - writing great code!
 
 
 ## 😍 Features 
 
 - 🌎 **HTTPS**: Auto-provisioned DNS and TLS certificates for your app.
 - 🔗 **Protocols**: Full compatibility with HTTP, WebSocket, and GraphQL.
 - ↕️ **Scaling**: Scale your app manually or let it auto-scale based on RPS, CPU, and Memory.
 - 🗝️ **Secrets**: Secure handling of secrets and environment variables.
 - 🎛️ **Hardware**: Choose the right compute resources for your app's needs with ease.
-- 🔒 **Authorization**: Built-in OAuth2.0 token-based security to secure your endpoints. 
+- 🔒 **Authorization**: Built-in `OAuth2.0` token-based security to secure your endpoints. 
 - 💾 **App Storage**: Persistent and secure network storage for your app data.
 - 🔄 **Blob Storage**: Built-in support for seamless user file uploads and downloads.
 - 🔎 **Observability**: Integrated access to logs, metrics, and traces. (Alerting coming soon!)
 - 📦 **Containerization**: Effortless containerization of your Python codebase with our integrated registry.
-- 🛠️ **Self-Hosting**: Export your app for self-hosting with ease, including docker-compose and Kubernetes yamls.
+- 🛠️ **Self-Hosting**: Export your app for self-hosting with ease, including docker-compose and Kubernetes YAMLs.
 
 ## 💡 Getting Started
 
 First, install the `fastapi-serve` package using pip:
 
 ```bash
 pip install fastapi-serve
@@ -75,45 +75,45 @@
 You'll get a URL to access your newly deployed application along with the Swagger UI.
 
 ## 📚 Documentation
 
 Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
 - 🚀 **Getting Started**
-    - 🧱 [Deploy a Simple FastAPI Application](docs/simple/)
+    - 🧱 [Deploy a simple FastAPI application](docs/simple/)
     - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
-    - ⚙️ [Understanding Configuration and Pricing](docs/CONFIG.MD)
+    - ⚙️ [Understanding configuration and pricing on Jina AI Cloud](docs/CONFIG.MD)
     - 🔄 [Upgrade your FastAPI applications with zero downtime](docs/upgrades/)
-    - 🏢 Managing Larger Applications with Complex Directory Structure (Example TBD!)
+    - 🏢 Managing Larger Applications with Complex Directory Structure (Documentation in progress 🚧)
 - ↕️ **Scaling**
     - 💹 [Auto-scaling endpoints based on CPU usage](docs/autoscaling/cpu/)
     - 📉 [Serverless (scale-to-zero) deployments based on RPS](docs/autoscaling/serverless/) 
 - 🧩 **Config & Credentials**
-    - 🌍 [Leverage Environment Variables for app configuration](docs/envs/)
-    - 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
+    - 🌍 [Leverage environment variables for app configuration](docs/envs/)
+    - 🗝️ [Use secrets for Redis-powered rate limiting](docs/rate_limit/)
 - 💾 **Storage**
-    - 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
-    - 🌐 Network Storage for persisting and securely accessing app data (Example TBD!)
+    - 📁 [Manage file uploads and downloads with built-in blob storage](docs/file_handling/)
+    - 🌐 Network storage for persisting and securely accessing app data (Documentation in progress 🚧)
 - 🔒 **Security**
-    - 👮‍♂️ [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
+    - 👮‍♂️ [Secure your endpoints with built-in OAuth2.0 authorization](docs/authorization/)
 - 🐳 **Deployment Options**
-    - 🚢 Deployment with Custom Dockerfile (Coming Soon!)
-    - ☸️ [Export Your App for Self-Hosting with docker-compose / Kubernetes](docs/export/)
+    - 🚢 Deployment with custom dockerfile (Documentation in progress 🚧)
+    - ☸️ [Export your app for self-hosting with docker-compose / Kubernetes](docs/export/)
 - 📈 **Observability**
-    - 📊 Access Logs, Metrics, and Traces for your app (Example TBD!)
-    - 🚨 Set up Alerts for your app (Coming Soon!)
+    - 📊 Access logs, metrics, and traces for your app (Documentation in progress 🚧)
+    - 🚨 Set up alerts for your app (Documentation in progress 🚧)
 
 
 ## 💪 Support
 
 If you encounter any problems or have questions, feel free to open an issue on the GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to get help from our community members and the Jina team.
 
 
 ## 🌐 Our Cloud Platform  
 
-`cloud.jina.ai` is our robust and scalable cloud platform designed to run your FastAPI applications with minimum hassle and maximum efficiency. With features like auto-scaling, integrated observability, and automated containerization, it provides a seamless and worry-free deployment experience.
+Our robust and scalable cloud platform `cloud.jina.ai` is designed to run your FastAPI applications with minimum hassle and maximum efficiency. With features like auto-scaling, integrated observability, and automated containerization, it provides a seamless and worry-free deployment experience.
 
 ---
 
 `fastapi-serve` is more than just a deployment tool, it's a bridge that connects your local development environment with our powerful cloud infrastructure. Start using `fastapi-serve` today, and experience the joy of effortless deployments! 🎊
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.6.dev5 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.7.dev45 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -16,65 +16,66 @@
 Engineering :: Artificial Intelligence Description-Content-Type: text/markdown
 Provides-Extra: test License-File: LICENSE
  ***** FastAPI-Serve: FastAPI to the Cloud, Batteries Included! âï¸ðð
                                      *****
                     [PyPI] [https://img.shields.io/discord/
   1106542220112302130?logo=discord&logoColor=white&style=flat-square] [PyPI_-
              Downloads_from_official_pypistats] [Github_CD_status]
-Welcome to **fastapi-serve**, your one-stop solution to seamless FastAPI
+Welcome to **fastapi-serve**, your one-stop solution for seamless FastAPI
 application deployments. Powered by our open-source framework [Jina](https://
 github.com/jina-ai/jina), `fastapi-serve` provides an effortless transition
 from your local setup to [cloud.jina.ai](https://cloud.jina.ai/), our robust
 and scalable cloud platform. ð©ï¸ Designed with developers in mind,
 `fastapi-serve` simplifies the deployment process by packing robust
 functionality, ease-of-use, and automated procedures into one comprehensive
 package. With `fastapi-serve`, we aim to streamline the "last mile" of FastAPI
 application development, allowing you to focus on what truly matters - writing
 great code! ## ð Features - ð **HTTPS**: Auto-provisioned DNS and TLS
 certificates for your app. - ð **Protocols**: Full compatibility with HTTP,
 WebSocket, and GraphQL. - âï¸ **Scaling**: Scale your app manually or let it
 auto-scale based on RPS, CPU, and Memory. - ðï¸ **Secrets**: Secure
 handling of secrets and environment variables. - ðï¸ **Hardware**: Choose
 the right compute resources for your app's needs with ease. - ð
-**Authorization**: Built-in OAuth2.0 token-based security to secure your
+**Authorization**: Built-in `OAuth2.0` token-based security to secure your
 endpoints. - ð¾ **App Storage**: Persistent and secure network storage for
 your app data. - ð **Blob Storage**: Built-in support for seamless user file
 uploads and downloads. - ð **Observability**: Integrated access to logs,
 metrics, and traces. (Alerting coming soon!) - ð¦ **Containerization**:
 Effortless containerization of your Python codebase with our integrated
 registry. - ð ï¸ **Self-Hosting**: Export your app for self-hosting with
-ease, including docker-compose and Kubernetes yamls. ## ð¡ Getting Started
+ease, including docker-compose and Kubernetes YAMLs. ## ð¡ Getting Started
 First, install the `fastapi-serve` package using pip: ```bash pip install
 fastapi-serve ``` Then, simply use the `fastapi-serve` command to deploy your
 FastAPI application: ```bash fastapi-serve deploy jcloud main:app ``` You'll
 get a URL to access your newly deployed application along with the Swagger UI.
 ## ð Documentation Dive into understanding `fastapi-serve` through our
 comprehensive documentation and examples: - ð **Getting Started** - ð§±
-[Deploy a Simple FastAPI Application](docs/simple/) - ð¥ï¸ [Dig deep into
-the `fastapi-serve` CLI](docs/CLI.md) - âï¸ [Understanding Configuration and
-Pricing](docs/CONFIG.MD) - ð [Upgrade your FastAPI applications with zero
-downtime](docs/upgrades/) - ð¢ Managing Larger Applications with Complex
-Directory Structure (Example TBD!) - âï¸ **Scaling** - ð¹ [Auto-scaling
-endpoints based on CPU usage](docs/autoscaling/cpu/) - ð [Serverless (scale-
-to-zero) deployments based on RPS](docs/autoscaling/serverless/) - ð§©
-**Config & Credentials** - ð [Leverage Environment Variables for app
-configuration](docs/envs/) - ðï¸ [Use Secrets for Redis-Powered Rate
-Limiting](docs/rate_limit/) - ð¾ **Storage** - ð [Handle File Uploads and
-Downloads with built-in Blob Storage](docs/file_handling/) - ð Network
-Storage for persisting and securely accessing app data (Example TBD!) - ð
-**Security** - ð®ââï¸ [Secure Your Endpoints with built-in OAuth2.0
-Authorization](docs/authorization/) - ð³ **Deployment Options** - ð¢
-Deployment with Custom Dockerfile (Coming Soon!) - â¸ï¸ [Export Your App for
-Self-Hosting with docker-compose / Kubernetes](docs/export/) - ð
-**Observability** - ð Access Logs, Metrics, and Traces for your app (Example
-TBD!) - ð¨ Set up Alerts for your app (Coming Soon!) ## ðª Support If you
-encounter any problems or have questions, feel free to open an issue on the
-GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
-get help from our community members and the Jina team. ## ð Our Cloud
-Platform `cloud.jina.ai` is our robust and scalable cloud platform designed to
-run your FastAPI applications with minimum hassle and maximum efficiency. With
-features like auto-scaling, integrated observability, and automated
-containerization, it provides a seamless and worry-free deployment experience.
---- `fastapi-serve` is more than just a deployment tool, it's a bridge that
-connects your local development environment with our powerful cloud
-infrastructure. Start using `fastapi-serve` today, and experience the joy of
-effortless deployments! ð
+[Deploy a simple FastAPI application](docs/simple/) - ð¥ï¸ [Dig deep into
+the `fastapi-serve` CLI](docs/CLI.md) - âï¸ [Understanding configuration and
+pricing on Jina AI Cloud](docs/CONFIG.MD) - ð [Upgrade your FastAPI
+applications with zero downtime](docs/upgrades/) - ð¢ Managing Larger
+Applications with Complex Directory Structure (Documentation in progress ð§)
+- âï¸ **Scaling** - ð¹ [Auto-scaling endpoints based on CPU usage](docs/
+autoscaling/cpu/) - ð [Serverless (scale-to-zero) deployments based on RPS]
+(docs/autoscaling/serverless/) - ð§© **Config & Credentials** - ð [Leverage
+environment variables for app configuration](docs/envs/) - ðï¸ [Use secrets
+for Redis-powered rate limiting](docs/rate_limit/) - ð¾ **Storage** - ð
+[Manage file uploads and downloads with built-in blob storage](docs/
+file_handling/) - ð Network storage for persisting and securely accessing
+app data (Documentation in progress ð§) - ð **Security** - ð®ââï¸
+[Secure your endpoints with built-in OAuth2.0 authorization](docs/
+authorization/) - ð³ **Deployment Options** - ð¢ Deployment with custom
+dockerfile (Documentation in progress ð§) - â¸ï¸ [Export your app for self-
+hosting with docker-compose / Kubernetes](docs/export/) - ð
+**Observability** - ð Access logs, metrics, and traces for your app
+(Documentation in progress ð§) - ð¨ Set up alerts for your app
+(Documentation in progress ð§) ## ðª Support If you encounter any problems
+or have questions, feel free to open an issue on the GitHub repository. You can
+also join our [Discord](https://discord.jina.ai/) to get help from our
+community members and the Jina team. ## ð Our Cloud Platform Our robust and
+scalable cloud platform `cloud.jina.ai` is designed to run your FastAPI
+applications with minimum hassle and maximum efficiency. With features like
+auto-scaling, integrated observability, and automated containerization, it
+provides a seamless and worry-free deployment experience. --- `fastapi-serve`
+is more than just a deployment tool, it's a bridge that connects your local
+development environment with our powerful cloud infrastructure. Start using
+`fastapi-serve` today, and experience the joy of effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.6.dev5/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.7.dev45/fastapi_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.6.dev5/setup.py` & `fastapi-serve-0.0.7.dev45/setup.py`

 * *Files identical despite different names*

