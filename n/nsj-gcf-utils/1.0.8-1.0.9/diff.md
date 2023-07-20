# Comparing `tmp/nsj_gcf_utils-1.0.8.tar.gz` & `tmp/nsj_gcf_utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Trabalho\nsj_gcf_utils\dist\tmpww8taslb\nsj_gcf_utils-1.0.8.tar", last modified: Fri Aug 26 15:01:05 2022, max compression
+gzip compressed data, was "nsj_gcf_utils-1.0.9.tar", last modified: Thu Sep  8 22:10:23 2022, max compression
```

## Comparing `nsj_gcf_utils-1.0.8.tar` & `nsj_gcf_utils-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-08-26 15:01:05.000000 nsj_gcf_utils-1.0.8/
--rw-rw-rw-   0        0        0       14 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     2086 2022-08-26 15:01:05.000000 nsj_gcf_utils-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1487 2022-08-05 17:54:52.000000 nsj_gcf_utils-1.0.8/README.md
--rw-rw-rw-   0        0        0      108 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      804 2022-08-26 15:01:05.000000 nsj_gcf_utils-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-26 15:01:04.000000 nsj_gcf_utils-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-08-26 15:01:05.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/
--rw-rw-rw-   0        0        0        0 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/__init__.py
--rw-rw-rw-   0        0        0     2285 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/abstract_repository.py
--rw-rw-rw-   0        0        0      445 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/app_logger.py
--rw-rw-rw-   0        0        0     1553 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/authentication_service.py
--rw-rw-rw-   0        0        0     7000 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/db_adapter.py
--rw-rw-rw-   0        0        0     6543 2022-08-26 14:59:48.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/db_adapter2.py
--rw-rw-rw-   0        0        0     1167 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/dto_util.py
--rw-rw-rw-   0        0        0      508 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/exception.py
--rw-rw-rw-   0        0        0     1237 2022-06-03 20:46:45.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/hash_util.py
--rw-rw-rw-   0        0        0    10049 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/http_util.py
--rw-rw-rw-   0        0        0     3057 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/iban.py
--rw-rw-rw-   0        0        0     5625 2022-08-05 17:40:36.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/json_util.py
--rw-rw-rw-   0        0        0     1583 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/keycloak_service.py
--rw-rw-rw-   0        0        0     1845 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/nsj_authentication_service.py
--rw-rw-rw-   0        0        0     4034 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/pagination_util.py
--rw-rw-rw-   0        0        0     2870 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/rest_error_util.py
--rw-rw-rw-   0        0        0     6666 2022-05-27 14:55:35.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/router.py
-drwxrwxrwx   0        0        0        0 2022-08-26 15:01:05.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils.egg-info/
--rw-rw-rw-   0        0        0     2086 2022-08-26 15:01:04.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2022-08-26 15:01:04.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-26 15:01:04.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-08-26 15:01:04.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-08-26 15:01:04.000000 nsj_gcf_utils-1.0.8/src/nsj_gcf_utils.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2022-09-08 22:10:23.946760 nsj_gcf_utils-1.0.9/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2022-03-23 22:20:57.000000 nsj_gcf_utils-1.0.9/LICENSE
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2048 2022-09-08 22:10:23.946760 nsj_gcf_utils-1.0.9/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1465 2022-09-08 22:05:52.000000 nsj_gcf_utils-1.0.9/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-03-25 14:56:36.000000 nsj_gcf_utils-1.0.9/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      770 2022-09-08 22:10:23.946760 nsj_gcf_utils-1.0.9/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2022-09-08 22:10:23.938760 nsj_gcf_utils-1.0.9/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2022-09-08 22:10:23.942760 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-03-23 22:20:57.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2220 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/abstract_repository.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      430 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/app_logger.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1503 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/authentication_service.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6780 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/db_adapter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6340 2022-09-08 22:08:25.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/db_adapter2.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1134 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/dto_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      490 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1205 2022-09-08 22:05:52.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/hash_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9774 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/http_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2962 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/iban.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5867 2022-09-08 22:09:20.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/json_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1533 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/keycloak_service.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1785 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/nsj_authentication_service.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3875 2022-09-06 23:16:26.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/pagination_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2765 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/rest_error_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6484 2022-08-30 00:49:27.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/router.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2022-09-08 22:10:23.942760 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2048 2022-09-08 22:10:23.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      826 2022-09-08 22:10:23.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2022-09-08 22:10:23.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       50 2022-09-08 22:10:23.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2022-09-08 22:10:23.000000 nsj_gcf_utils-1.0.9/src/nsj_gcf_utils.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nsj_gcf_utils-1.0.8/PKG-INFO` & `nsj_gcf_utils-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: nsj_gcf_utils
-Version: 1.0.8
-Summary: Utilitários para construção de Google Cloud Functions.
-Home-page: https://github.com/Nasajon/nsj_gcf_utils
-Author: Nasajon Sistemas
-Author-email: contact.dev@nasajon.com.br
-Project-URL: Source, https://github.com/Nasajon/nsj_gcf_utils
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# nsj_gcf_utils
-Utilitários para construção de Google Cloud Functions.
-
-## Features disponíveis
-
-Segue breve descrição das features disponiveis, identificando os respectivos módulos:
-
-* ```nsj_gcf_utils.app_logger```: Configuração padrão de logger para aplicações GCF.
-* ```nsj_gcf_utils.authentication_service```: Validação de chaves recebidas no cabeçalho X-API-Key.
-* ```nsj_gcf_utils.db_adapter```: Adapter de comunicação com o banco.
-* ```nsj_gcf_utils.http_util```: Realiza requisições HTTP, com suporte a tentativas seguidas em caso de falha.
-* ```nsj_gcf_utils.iban```: Utilitário para manipulação de International Bank Account Number (IBAN)
-* ```nsj_gcf_utils.json_util```: Serialização e desserialização em JSON, com manipulação nativa de datas no formato "yyyy-mm-ddThh:mm:ss". Decimal é traduzido para string ao serializar para JSON.
-* ```nsj_gcf_utils.keycloak_service```: Autenticação para aplicação enquanto cliente Oauth.
-* ```nsj_gcf_utils.nsj_authentication_service```: Validação de access_token recebido no cabeçalho Authorization (Bearer token), por meio do padrão Token Instrospection (RFC 7662).
-* ```nsj_gcf_utils.router```: Utilitário para controler de rotas por meio decorators, fazendo com que uma fucntion-framework se comporte de modo similar a outros frameworks web como Spring ou Symfony.
-
-## Testes Automatizados
-
-Sempre rode o comando abaixo, antes de dar push neste repositório:
-
-> make tests
+Metadata-Version: 2.1
+Name: nsj_gcf_utils
+Version: 1.0.9
+Summary: Utilitários para construção de Google Cloud Functions.
+Home-page: https://github.com/Nasajon/nsj_gcf_utils
+Author: Nasajon Sistemas
+Author-email: contact.dev@nasajon.com.br
+Project-URL: Source, https://github.com/Nasajon/nsj_gcf_utils
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# nsj_gcf_utils
+Utilitários para construção de Google Cloud Functions.
+
+## Features disponíveis
+
+Segue breve descrição das features disponiveis, identificando os respectivos módulos:
+
+* ```nsj_gcf_utils.app_logger```: Configuração padrão de logger para aplicações GCF.
+* ```nsj_gcf_utils.authentication_service```: Validação de chaves recebidas no cabeçalho X-API-Key.
+* ```nsj_gcf_utils.db_adapter```: Adapter de comunicação com o banco.
+* ```nsj_gcf_utils.http_util```: Realiza requisições HTTP, com suporte a tentativas seguidas em caso de falha.
+* ```nsj_gcf_utils.iban```: Utilitário para manipulação de International Bank Account Number (IBAN)
+* ```nsj_gcf_utils.json_util```: Serialização e desserialização em JSON, com manipulação nativa de datas no formato "yyyy-mm-ddThh:mm:ss". Decimal é traduzido para string ao serializar para JSON.
+* ```nsj_gcf_utils.keycloak_service```: Autenticação para aplicação enquanto cliente Oauth.
+* ```nsj_gcf_utils.nsj_authentication_service```: Validação de access_token recebido no cabeçalho Authorization (Bearer token), por meio do padrão Token Instrospection (RFC 7662).
+* ```nsj_gcf_utils.router```: Utilitário para controler de rotas por meio decorators, fazendo com que uma fucntion-framework se comporte de modo similar a outros frameworks web como Spring ou Symfony.
+
+## Testes Automatizados
+
+Sempre rode o comando abaixo, antes de dar push neste repositório:
+
+> make tests
```

### Comparing `nsj_gcf_utils-1.0.8/README.md` & `nsj_gcf_utils-1.0.9/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# nsj_gcf_utils
-Utilitários para construção de Google Cloud Functions.
-
-## Features disponíveis
-
-Segue breve descrição das features disponiveis, identificando os respectivos módulos:
-
-* ```nsj_gcf_utils.app_logger```: Configuração padrão de logger para aplicações GCF.
-* ```nsj_gcf_utils.authentication_service```: Validação de chaves recebidas no cabeçalho X-API-Key.
-* ```nsj_gcf_utils.db_adapter```: Adapter de comunicação com o banco.
-* ```nsj_gcf_utils.http_util```: Realiza requisições HTTP, com suporte a tentativas seguidas em caso de falha.
-* ```nsj_gcf_utils.iban```: Utilitário para manipulação de International Bank Account Number (IBAN)
-* ```nsj_gcf_utils.json_util```: Serialização e desserialização em JSON, com manipulação nativa de datas no formato "yyyy-mm-ddThh:mm:ss". Decimal é traduzido para string ao serializar para JSON.
-* ```nsj_gcf_utils.keycloak_service```: Autenticação para aplicação enquanto cliente Oauth.
-* ```nsj_gcf_utils.nsj_authentication_service```: Validação de access_token recebido no cabeçalho Authorization (Bearer token), por meio do padrão Token Instrospection (RFC 7662).
-* ```nsj_gcf_utils.router```: Utilitário para controler de rotas por meio decorators, fazendo com que uma fucntion-framework se comporte de modo similar a outros frameworks web como Spring ou Symfony.
-
-## Testes Automatizados
-
-Sempre rode o comando abaixo, antes de dar push neste repositório:
-
-> make tests
+# nsj_gcf_utils
+Utilitários para construção de Google Cloud Functions.
+
+## Features disponíveis
+
+Segue breve descrição das features disponiveis, identificando os respectivos módulos:
+
+* ```nsj_gcf_utils.app_logger```: Configuração padrão de logger para aplicações GCF.
+* ```nsj_gcf_utils.authentication_service```: Validação de chaves recebidas no cabeçalho X-API-Key.
+* ```nsj_gcf_utils.db_adapter```: Adapter de comunicação com o banco.
+* ```nsj_gcf_utils.http_util```: Realiza requisições HTTP, com suporte a tentativas seguidas em caso de falha.
+* ```nsj_gcf_utils.iban```: Utilitário para manipulação de International Bank Account Number (IBAN)
+* ```nsj_gcf_utils.json_util```: Serialização e desserialização em JSON, com manipulação nativa de datas no formato "yyyy-mm-ddThh:mm:ss". Decimal é traduzido para string ao serializar para JSON.
+* ```nsj_gcf_utils.keycloak_service```: Autenticação para aplicação enquanto cliente Oauth.
+* ```nsj_gcf_utils.nsj_authentication_service```: Validação de access_token recebido no cabeçalho Authorization (Bearer token), por meio do padrão Token Instrospection (RFC 7662).
+* ```nsj_gcf_utils.router```: Utilitário para controler de rotas por meio decorators, fazendo com que uma fucntion-framework se comporte de modo similar a outros frameworks web como Spring ou Symfony.
+
+## Testes Automatizados
+
+Sempre rode o comando abaixo, antes de dar push neste repositório:
+
+> make tests
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/db_adapter.py` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/db_adapter.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-# import sqlalchemy
-import uuid
-
-
-class DBAdapter:
-
-    # TODO Refatorar para uso de parâmetros nomeados
-
-    def __init__(self, db_connection):
-        self._db = db_connection
-        self._transaction = None
-
-    def begin(self):
-        if self._transaction is None:
-            self._transaction = self._db.begin()
-
-    def commit(self):
-        if self._transaction is not None:
-            self._transaction.commit()
-            self._transaction = None
-
-    def rollback(self):
-        if self._transaction is not None:
-            self._transaction.rollback()
-            self._transaction = None
-
-    def in_transaction(self):
-        return self._transaction is not None
-
-    def execute(self, sql: str, parameters=None) -> int:
-        """
-        Executando uma instrução sql sem retorno.
-        É obrigatório a passagem de uma conexão de banco no argumento self._db.
-
-        Retorna o número de linhas afetadas pela instrução.
-        """
-        cur = None
-        try:
-            cur = self._execute(sql, parameters)
-
-            return cur.rowcount
-        finally:
-            if cur is not None:
-                cur.close()
-
-    def execute_query_to_model(self, sql: str, model_class: object, parameters=None) -> list:
-        """
-        Executando uma instrução sql com retorno.
-        O retorno é feito em forma de uma lista (list), com elementos do tipo passado pelo parâmetro
-        "model_class".
-        É importante destacar que para cada coluna do retorno, será procurado um atributo no model_class
-        com mesmo nome, para setar o valor. Se este não for encontrado, a coluna do retorno é ignorada.
-        """
-
-        result = []
-        cur = None
-        try:
-            cur = self._execute(sql, parameters)
-            rs = cur.fetchall()
-
-            for rec in rs:
-                model = model_class()
-
-                i = 0
-                for column in cur.keys():
-                    if (hasattr(model, column)):
-                        setattr(model, column, rec[i])
-
-                    i += 1
-
-                result.append(model)
-
-        finally:
-            if cur is not None:
-                cur.close()
-
-        return result
-
-    def execute_query(self, sql: str, parameters=None) -> list:
-        """
-        Executando uma instrução sql com retorno.
-        O retorno é feito em forma de uma lista (list), com elementos do tipo dict (onde cada chave é igual ao
-        nome do campo correspondente).
-        """
-        cur = None
-        try:
-            cur = self._execute(sql, parameters)
-            rs = cur.fetchall()
-
-            return [dict(rec.items()) for rec in rs]
-        finally:
-            if cur is not None:
-                cur.close()
-
-    def execute_query_first_result(self, sql: str, model_class: object, parameters=None) -> "model_class":
-        """
-        Executando uma instrução sql com retorno.
-        O retorno é feito em forma de um objeto do tipo passado pelo parâmetro "model_class".
-        É importante destacar que para cada coluna do retorno, será procurado um atributo no model_class
-        com mesmo nome, para setar o valor. Se este não for encontrado, a coluna do retorno é ignorada.
-        """
-
-        result = None
-        cur = None
-        try:
-            cur = self._execute(sql, parameters)
-            rs = cur.fetchone()
-
-            if (len(rs) > 0):
-                model = model_class()
-
-                i = 0
-                for column in cur.keys():
-                    if (hasattr(model, column)):
-                        setattr(model, column, rs[i])
-
-                    i += 1
-
-                result = model
-
-        finally:
-            if cur is not None:
-                cur.close()
-
-        return result
-
-    def get_single_result(self, sql: str, parameters=None):
-        """
-        Executa uma instrução SQL para a qual se espera um único retorno (com tipo primitivo). Exemplo:
-        select 1+1
-        Se não houver retorno, retorna None.
-        """
-        cur = None
-        try:
-            cur = self._execute(sql, parameters)
-            return cur.scalar()
-        finally:
-            if cur is not None:
-                cur.close()
-
-    def _check_type(self, parameter):
-        if (isinstance(parameter, uuid.UUID)):
-            return str(parameter)
-        else:
-            return parameter
-
-    def _execute(self, sql: str, parameters: list):
-        new_transaction = not self.in_transaction()
-
-        try:
-            if new_transaction:
-                self.begin()
-
-            if (parameters != None):
-                pars = [self._check_type(par) for par in parameters]
-                return self._db.execute(sql, pars)
-            else:
-                return self._db.execute(sql)
-        except:
-            if new_transaction:
-                self.rollback()
-            raise
-        finally:
-            if new_transaction:
-                self.commit()
-
-    def execute_query_from_file(self, query_file_path, *parameters):
-        with open(query_file_path) as f:
-            sql = f.read()
-        return self.execute_query(sql, parameters)
-
-
-# class AlchemyDBAdapter:
-#     def __init__(self, db_connection):
-#         self._db = db_connection
-
-#     def execute_query(self, sql: str, **kwargs) -> list:
-#         """
-#         Executando uma instrução sql com retorno.
-#         O retorno é feito em forma de uma lista (list), com elementos do tipo dict (onde cada chave é igual ao
-#         nome do campo correspondente).
-#         """
-#         cur = None
-#         sql = sqlalchemy.text(sql)
-#         try:
-#             cur = self._db.execute(sql, **kwargs)
-#             rs = cur.fetchall()
-
-#             return [dict(rec.items()) for rec in rs]
-#         finally:
-#             if cur is not None:
-#                 cur.close()
-
-#     def execute(self, sql: str, **kwargs) -> int:
-#         """
-#         Executando uma instrução sql sem retorno.
-#         É obrigatório a passagem de uma conexão de banco no argumento self._db.
-
-#         Retorna o número de linhas afetadas pela instrução.
-#         """
-#         cur = None
-#         sql = sqlalchemy.text(sql)
-#         try:
-#             with self._db.begin():
-#                 cur = self._db.execute(sql, **kwargs)
-
-#             return cur.rowcount
-#         finally:
-#             if cur is not None:
-#                 cur.close()
-
-#     def execute_query_from_file(self, query_file_path, **kwargs):
-#         with open(query_file_path) as f:
-#             sql = f.read()
-#         return self.execute_query(sql, **kwargs)
-
-#     def execute_from_file(self, sql_file_path, **kwargs):
-#         with open(sql_file_path) as f:
-#             sql = f.read()
-#         return self.execute(sql, **kwargs)
+# import sqlalchemy
+import uuid
+
+
+class DBAdapter:
+
+    # TODO Refatorar para uso de parâmetros nomeados
+
+    def __init__(self, db_connection):
+        self._db = db_connection
+        self._transaction = None
+
+    def begin(self):
+        if self._transaction is None:
+            self._transaction = self._db.begin()
+
+    def commit(self):
+        if self._transaction is not None:
+            self._transaction.commit()
+            self._transaction = None
+
+    def rollback(self):
+        if self._transaction is not None:
+            self._transaction.rollback()
+            self._transaction = None
+
+    def in_transaction(self):
+        return self._transaction is not None
+
+    def execute(self, sql: str, parameters=None) -> int:
+        """
+        Executando uma instrução sql sem retorno.
+        É obrigatório a passagem de uma conexão de banco no argumento self._db.
+
+        Retorna o número de linhas afetadas pela instrução.
+        """
+        cur = None
+        try:
+            cur = self._execute(sql, parameters)
+
+            return cur.rowcount
+        finally:
+            if cur is not None:
+                cur.close()
+
+    def execute_query_to_model(self, sql: str, model_class: object, parameters=None) -> list:
+        """
+        Executando uma instrução sql com retorno.
+        O retorno é feito em forma de uma lista (list), com elementos do tipo passado pelo parâmetro
+        "model_class".
+        É importante destacar que para cada coluna do retorno, será procurado um atributo no model_class
+        com mesmo nome, para setar o valor. Se este não for encontrado, a coluna do retorno é ignorada.
+        """
+
+        result = []
+        cur = None
+        try:
+            cur = self._execute(sql, parameters)
+            rs = cur.fetchall()
+
+            for rec in rs:
+                model = model_class()
+
+                i = 0
+                for column in cur.keys():
+                    if (hasattr(model, column)):
+                        setattr(model, column, rec[i])
+
+                    i += 1
+
+                result.append(model)
+
+        finally:
+            if cur is not None:
+                cur.close()
+
+        return result
+
+    def execute_query(self, sql: str, parameters=None) -> list:
+        """
+        Executando uma instrução sql com retorno.
+        O retorno é feito em forma de uma lista (list), com elementos do tipo dict (onde cada chave é igual ao
+        nome do campo correspondente).
+        """
+        cur = None
+        try:
+            cur = self._execute(sql, parameters)
+            rs = cur.fetchall()
+
+            return [dict(rec.items()) for rec in rs]
+        finally:
+            if cur is not None:
+                cur.close()
+
+    def execute_query_first_result(self, sql: str, model_class: object, parameters=None) -> "model_class":
+        """
+        Executando uma instrução sql com retorno.
+        O retorno é feito em forma de um objeto do tipo passado pelo parâmetro "model_class".
+        É importante destacar que para cada coluna do retorno, será procurado um atributo no model_class
+        com mesmo nome, para setar o valor. Se este não for encontrado, a coluna do retorno é ignorada.
+        """
+
+        result = None
+        cur = None
+        try:
+            cur = self._execute(sql, parameters)
+            rs = cur.fetchone()
+
+            if (len(rs) > 0):
+                model = model_class()
+
+                i = 0
+                for column in cur.keys():
+                    if (hasattr(model, column)):
+                        setattr(model, column, rs[i])
+
+                    i += 1
+
+                result = model
+
+        finally:
+            if cur is not None:
+                cur.close()
+
+        return result
+
+    def get_single_result(self, sql: str, parameters=None):
+        """
+        Executa uma instrução SQL para a qual se espera um único retorno (com tipo primitivo). Exemplo:
+        select 1+1
+        Se não houver retorno, retorna None.
+        """
+        cur = None
+        try:
+            cur = self._execute(sql, parameters)
+            return cur.scalar()
+        finally:
+            if cur is not None:
+                cur.close()
+
+    def _check_type(self, parameter):
+        if (isinstance(parameter, uuid.UUID)):
+            return str(parameter)
+        else:
+            return parameter
+
+    def _execute(self, sql: str, parameters: list):
+        new_transaction = not self.in_transaction()
+
+        try:
+            if new_transaction:
+                self.begin()
+
+            if (parameters != None):
+                pars = [self._check_type(par) for par in parameters]
+                return self._db.execute(sql, pars)
+            else:
+                return self._db.execute(sql)
+        except:
+            if new_transaction:
+                self.rollback()
+            raise
+        finally:
+            if new_transaction:
+                self.commit()
+
+    def execute_query_from_file(self, query_file_path, *parameters):
+        with open(query_file_path) as f:
+            sql = f.read()
+        return self.execute_query(sql, parameters)
+
+
+# class AlchemyDBAdapter:
+#     def __init__(self, db_connection):
+#         self._db = db_connection
+
+#     def execute_query(self, sql: str, **kwargs) -> list:
+#         """
+#         Executando uma instrução sql com retorno.
+#         O retorno é feito em forma de uma lista (list), com elementos do tipo dict (onde cada chave é igual ao
+#         nome do campo correspondente).
+#         """
+#         cur = None
+#         sql = sqlalchemy.text(sql)
+#         try:
+#             cur = self._db.execute(sql, **kwargs)
+#             rs = cur.fetchall()
+
+#             return [dict(rec.items()) for rec in rs]
+#         finally:
+#             if cur is not None:
+#                 cur.close()
+
+#     def execute(self, sql: str, **kwargs) -> int:
+#         """
+#         Executando uma instrução sql sem retorno.
+#         É obrigatório a passagem de uma conexão de banco no argumento self._db.
+
+#         Retorna o número de linhas afetadas pela instrução.
+#         """
+#         cur = None
+#         sql = sqlalchemy.text(sql)
+#         try:
+#             with self._db.begin():
+#                 cur = self._db.execute(sql, **kwargs)
+
+#             return cur.rowcount
+#         finally:
+#             if cur is not None:
+#                 cur.close()
+
+#     def execute_query_from_file(self, query_file_path, **kwargs):
+#         with open(query_file_path) as f:
+#             sql = f.read()
+#         return self.execute_query(sql, **kwargs)
+
+#     def execute_from_file(self, sql_file_path, **kwargs):
+#         with open(sql_file_path) as f:
+#             sql = f.read()
+#         return self.execute(sql, **kwargs)
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/db_adapter2.py` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/db_adapter2.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-import uuid
-
-from sqlparams import SQLParams
-
-
-class DBAdapter2:
-
-    def __init__(self, db_connection):
-        self._db = db_connection
-        self._transaction = None
-
-    def begin(self):
-        if self._transaction is None:
-            self._transaction = self._db.begin()
-
-    def commit(self):
-        if self._transaction is not None:
-            self._transaction.commit()
-            self._transaction = None
-
-    def rollback(self):
-        if self._transaction is not None:
-            self._transaction.rollback()
-            self._transaction = None
-
-    def in_transaction(self):
-        return self._transaction is not None
-
-    def execute(self, sql: str, **kwargs) -> int:
-        """
-        Executando uma instrução sql, com ou sem retorno.
-        É obrigatório a passagem de uma conexão de banco no argumento self._db.
-
-        Retorna o número de linhas afetadas pela instrução e o retorno esperado se houver, como uma tupla.
-        O retorno é feito em forma de uma lista (list), com elementos do tipo dict (onde cada chave é igual ao
-        nome do campo correspondente).
-        """
-        cur = None
-        try:
-            cur = self._execute(sql, **kwargs)
-
-            if 'returning' in sql.lower():
-                rs = cur.fetchall()
-                returning = [dict(rec.items()) for rec in rs]
-            else:
-                returning = None
-
-            return (cur.rowcount, returning)
-        finally:
-            if cur is not None:
-                cur.close()
-
-    def execute_query_to_model(self, sql: str, model_class: object, **kwargs) -> list:
-        """
-        Executando uma instrução sql com retorno.
-        O retorno é feito em forma de uma lista (list), com elementos do tipo passado pelo parâmetro
-        "model_class".
-        É importante destacar que para cada coluna do retorno, será procurado um atributo no model_class
-        com mesmo nome, para setar o valor. Se este não for encontrado, a coluna do retorno é ignorada.
-        """
-
-        result = []
-        cur = None
-        try:
-            cur = self._execute(sql, **kwargs)
-            rs = cur.fetchall()
-
-            for rec in rs:
-                model = model_class()
-
-                i = 0
-                for column in cur.keys():
-                    if (hasattr(model, column)):
-                        setattr(model, column, rec[i])
-
-                    i += 1
-
-                result.append(model)
-
-        finally:
-            if cur is not None:
-                cur.close()
-
-        return result
-
-    def execute_query(self, sql: str, **kwargs) -> list:
-        """
-        Executando uma instrução sql com retorno.
-        O retorno é feito em forma de uma lista (list), com elementos do tipo dict (onde cada chave é igual ao
-        nome do campo correspondente).
-        """
-        cur = None
-        try:
-            cur = self._execute(sql, **kwargs)
-            rs = cur.fetchall()
-
-            return [dict(rec.items()) for rec in rs]
-        finally:
-            if cur is not None:
-                cur.close()
-
-    def execute_query_first_result(self, sql: str, **kwargs) -> list:
-        """
-        Executando uma instrução sql com retorno.
-        O retorno é feito em forma de um dict (onde cada chave é igual ao nome do campo correspondente).
-
-        Apenas o primeiro registro é retornado (os demais serão descartados, se houverem).
-        Caso não haja registros correspondentes a query, retorna None.
-        """
-        cur = None
-        try:
-            cur = self._execute(sql, **kwargs)
-            rs = cur.fetchall()
-
-            results = [dict(rec.items()) for rec in rs]
-
-            if len(results) <= 0:
-                return None
-            else:
-                return results[0]
-        finally:
-            if cur is not None:
-                cur.close()
-
-    def execute_query_first_result_to_model(self, sql: str, model_class: object, **kwargs) -> "model_class":
-        """
-        Executando uma instrução sql com retorno.
-        O retorno é feito em forma de um objeto do tipo passado pelo parâmetro "model_class".
-        É importante destacar que para cada coluna do retorno, será procurado um atributo no model_class
-        com mesmo nome, para setar o valor. Se este não for encontrado, a coluna do retorno é ignorada.
-        """
-
-        result = None
-        cur = None
-        try:
-            cur = self._execute(sql, **kwargs)
-            rs = cur.fetchone()
-
-            if (len(rs) > 0):
-                model = model_class()
-
-                i = 0
-                for column in cur.keys():
-                    if (hasattr(model, column)):
-                        setattr(model, column, rs[i])
-
-                    i += 1
-
-                result = model
-
-        finally:
-            if cur is not None:
-                cur.close()
-
-        return result
-
-    def get_single_result(self, sql: str, **kwargs):
-        """
-        Executa uma instrução SQL para a qual se espera um único retorno (com tipo primitivo). Exemplo:
-        select 1+1
-        Se não houver retorno, retorna None.
-        """
-        cur = None
-        try:
-            cur = self._execute(sql, **kwargs)
-            return cur.scalar()
-        finally:
-            if cur is not None:
-                cur.close()
-
-    def _check_type(self, parameter):
-        if (isinstance(parameter, uuid.UUID)):
-            return str(parameter)
-        else:
-            return parameter
-
-    def _execute(self, sql: str, **kwargs):
-
-        new_transaction = not self.in_transaction()
-
-        try:
-            if new_transaction:
-                self.begin()
-
-            if (kwargs is not None):
-                pars = {key: self._check_type(kwargs[key]) for key in kwargs}
-                sql2, pars2 = SQLParams('named', 'format').format(sql, pars)
-                return self._db.execute(sql2, pars2)
-            else:
-                return self._db.execute(sql)
-        except:
-            if new_transaction:
-                self.rollback()
-            raise
-
-        finally:
-            if new_transaction:
-                self.commit()
-
-    def execute_query_from_file(self, query_file_path, **kwargs):
-        with open(query_file_path, 'r') as f:
-            sql = f.read()
-        return self.execute_query(sql, **kwargs)
+import uuid
+
+from sqlparams import SQLParams
+
+
+class DBAdapter2:
+
+    def __init__(self, db_connection):
+        self._db = db_connection
+        self._transaction = None
+
+    def begin(self):
+        if self._transaction is None:
+            self._transaction = self._db.begin()
+
+    def commit(self):
+        if self._transaction is not None:
+            self._transaction.commit()
+            self._transaction = None
+
+    def rollback(self):
+        if self._transaction is not None:
+            self._transaction.rollback()
+            self._transaction = None
+
+    def in_transaction(self):
+        return self._transaction is not None
+
+    def execute(self, sql: str, **kwargs) -> int:
+        """
+        Executando uma instrução sql, com ou sem retorno.
+        É obrigatório a passagem de uma conexão de banco no argumento self._db.
+
+        Retorna o número de linhas afetadas pela instrução e o retorno esperado se houver, como uma tupla.
+        O retorno é feito em forma de uma lista (list), com elementos do tipo dict (onde cada chave é igual ao
+        nome do campo correspondente).
+        """
+        cur = None
+        try:
+            cur = self._execute(sql, **kwargs)
+
+            if 'returning' in sql.lower():
+                rs = cur.fetchall()
+                returning = [dict(rec.items()) for rec in rs]
+            else:
+                returning = None
+
+            return (cur.rowcount, returning)
+        finally:
+            if cur is not None:
+                cur.close()
+
+    def execute_query_to_model(self, sql: str, model_class: object, **kwargs) -> list:
+        """
+        Executando uma instrução sql com retorno.
+        O retorno é feito em forma de uma lista (list), com elementos do tipo passado pelo parâmetro
+        "model_class".
+        É importante destacar que para cada coluna do retorno, será procurado um atributo no model_class
+        com mesmo nome, para setar o valor. Se este não for encontrado, a coluna do retorno é ignorada.
+        """
+
+        result = []
+        cur = None
+        try:
+            cur = self._execute(sql, **kwargs)
+            rs = cur.fetchall()
+
+            for rec in rs:
+                model = model_class()
+
+                i = 0
+                for column in cur.keys():
+                    if (hasattr(model, column)):
+                        setattr(model, column, rec[i])
+
+                    i += 1
+
+                result.append(model)
+
+        finally:
+            if cur is not None:
+                cur.close()
+
+        return result
+
+    def execute_query(self, sql: str, **kwargs) -> list:
+        """
+        Executando uma instrução sql com retorno.
+        O retorno é feito em forma de uma lista (list), com elementos do tipo dict (onde cada chave é igual ao
+        nome do campo correspondente).
+        """
+        cur = None
+        try:
+            cur = self._execute(sql, **kwargs)
+            rs = cur.fetchall()
+
+            return [dict(rec.items()) for rec in rs]
+        finally:
+            if cur is not None:
+                cur.close()
+
+    def execute_query_first_result(self, sql: str, **kwargs) -> list:
+        """
+        Executando uma instrução sql com retorno.
+        O retorno é feito em forma de um dict (onde cada chave é igual ao nome do campo correspondente).
+
+        Apenas o primeiro registro é retornado (os demais serão descartados, se houverem).
+        Caso não haja registros correspondentes a query, retorna None.
+        """
+        cur = None
+        try:
+            cur = self._execute(sql, **kwargs)
+            rs = cur.fetchall()
+
+            results = [dict(rec.items()) for rec in rs]
+
+            if len(results) <= 0:
+                return None
+            else:
+                return results[0]
+        finally:
+            if cur is not None:
+                cur.close()
+
+    def execute_query_first_result_to_model(self, sql: str, model_class: object, **kwargs) -> "model_class":
+        """
+        Executando uma instrução sql com retorno.
+        O retorno é feito em forma de um objeto do tipo passado pelo parâmetro "model_class".
+        É importante destacar que para cada coluna do retorno, será procurado um atributo no model_class
+        com mesmo nome, para setar o valor. Se este não for encontrado, a coluna do retorno é ignorada.
+        """
+
+        result = None
+        cur = None
+        try:
+            cur = self._execute(sql, **kwargs)
+            rs = cur.fetchone()
+
+            if (len(rs) > 0):
+                model = model_class()
+
+                i = 0
+                for column in cur.keys():
+                    if (hasattr(model, column)):
+                        setattr(model, column, rs[i])
+
+                    i += 1
+
+                result = model
+
+        finally:
+            if cur is not None:
+                cur.close()
+
+        return result
+
+    def get_single_result(self, sql: str, **kwargs):
+        """
+        Executa uma instrução SQL para a qual se espera um único retorno (com tipo primitivo). Exemplo:
+        select 1+1
+        Se não houver retorno, retorna None.
+        """
+        cur = None
+        try:
+            cur = self._execute(sql, **kwargs)
+            return cur.scalar()
+        finally:
+            if cur is not None:
+                cur.close()
+
+    def _check_type(self, parameter):
+        if (isinstance(parameter, uuid.UUID)):
+            return str(parameter)
+        else:
+            return parameter
+
+    def _execute(self, sql: str, **kwargs):
+
+        new_transaction = not self.in_transaction()
+
+        try:
+            if new_transaction:
+                self.begin()
+
+            if (kwargs is not None):
+                pars = {key: self._check_type(kwargs[key]) for key in kwargs}
+                sql2, pars2 = SQLParams('named', 'format').format(sql, pars)
+                return self._db.execute(sql2, pars2)
+            else:
+                return self._db.execute(sql)
+        except:
+            if new_transaction:
+                self.rollback()
+            raise
+
+        finally:
+            if new_transaction:
+                self.commit()
+
+    def execute_query_from_file(self, query_file_path, **kwargs):
+        with open(query_file_path, 'r') as f:
+            sql = f.read()
+        return self.execute_query(sql, **kwargs)
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/hash_util.py` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/hash_util.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from hashlib import sha256
-from nsj_gcf_utils.json_util import json_dumps
-
-"""Cria um hash usando SHA256 para ser usado para autenticação pelo webhook.
-   Ele recebe a url, o body e o metodo da requisição junto com uma chave especial.
-   Depois junta todos os dados e usa SHA256 para criar o hash.
-"""
-def hash_webhook(url, body, method, key):
-    # Converte o body para string caso o body seja um dict(json)
-    if isinstance(body, dict):
-        body = json_dumps(body)
-
-    # tipagem para ajudar o autocomplete de IDEs
-    # str na key caso ela seja um número ou um uuid
-    hash: str = url + body + method + str(key) 
-
-    return sha256(hash.encode()).hexdigest()
-
-# Teste para o integrador vmpay
-if __name__ == '__main__':
-    print(hash_webhook("http://localhost/produtos",{
-        "esquema": "estoque",
-        "tabela": "produtos",
-        "operacao": "I",
-        "dados": {
-            "especificacao": "teste14",
-            "codigo": "1234",
-            "codigodebarras": "",
-            "estabelecimento":"5e5a86b7-d494-4c31-806a-a5e74862403a",
-            "grupoempresarial": "0ef4df5d-9881-4c3c-b8ea-a09149f799a5",
-            "grupodeinventario": 0
-        }
+from hashlib import sha256
+from nsj_gcf_utils.json_util import json_dumps
+
+"""Cria um hash usando SHA256 para ser usado para autenticação pelo webhook.
+   Ele recebe a url, o body e o metodo da requisição junto com uma chave especial.
+   Depois junta todos os dados e usa SHA256 para criar o hash.
+"""
+def hash_webhook(url, body, method, key):
+    # Converte o body para string caso o body seja um dict(json)
+    if isinstance(body, dict):
+        body = json_dumps(body)
+
+    # tipagem para ajudar o autocomplete de IDEs
+    # str na key caso ela seja um número ou um uuid
+    hash: str = url + body + method + str(key) 
+
+    return sha256(hash.encode()).hexdigest()
+
+# Teste para o integrador vmpay
+if __name__ == '__main__':
+    print(hash_webhook("http://localhost/produtos",{
+        "esquema": "estoque",
+        "tabela": "produtos",
+        "operacao": "I",
+        "dados": {
+            "especificacao": "teste14",
+            "codigo": "1234",
+            "codigodebarras": "",
+            "estabelecimento":"5e5a86b7-d494-4c31-806a-a5e74862403a",
+            "grupoempresarial": "0ef4df5d-9881-4c3c-b8ea-a09149f799a5",
+            "grupodeinventario": 0
+        }
     }, "POST","124325"))
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/http_util.py` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/http_util.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,276 +1,276 @@
-import json
-import urllib
-
-import requests
-import time
-
-from nsj_gcf_utils.app_logger import logger
-from typing import Dict, Any
-
-
-class HttpUtilGetException(Exception):
-    pass
-
-
-class HttpUtilPostException(Exception):
-    pass
-
-class HttpUtilPutException(Exception):
-    pass
-
-class HttpUtilDeleteException(Exception):
-    pass
-
-
-class ResourceNotFound(Exception):
-    pass
-
-
-class HttpUtil:
-    @staticmethod
-    def post_retry(url: str, data: str, headers: Dict[str, str] = None, timeout: int = 20, tries: int = 3, interval: int = 3, format_data: bool = True, raise_for_status: bool = True, resouce_description: str = '', verify :bool = True, query_params: Dict[str, Any] = None):
-        # Encoding query params
-        if query_params is not None:
-            q_params = urllib.parse.urlencode(query_params, doseq=True)
-
-            if '?' in url:
-                url += '&' + q_params
-            else:
-                url += '?' + q_params
-                
-        logger.info(f'Post URL: {url}')
-        
-        # Formatting data
-        if format_data:
-            if isinstance(data, dict) or isinstance(data, list):
-                logger.info(
-                    'Converting data from "dict" or "list" to json string')
-                data = json.dumps(data)
-
-                # adding content-type: application/json in headers
-                if headers:
-                    if not ('content-type' in [k.lower() for k in headers.keys()]):
-                        headers['content-type'] = 'application/json'
-                else:
-                    headers = {'content-type': 'application/json'}
-            elif not isinstance(data, str):
-                logger.info('Converting data from non string to string')
-                data = str(data)
-
-        logger.info(f'Posting data (bellow) to URL: {url}')
-        if not('password' in data) and not('client_secret' in data) and not('pass' in data):
-            logger.info(f'Sending data: {data}')
-
-        # Making tries
-        exception_obj = None
-        resp = None
-        for i in range(tries):
-            resp = None
-            try:
-                resp = requests.post(
-                    url=url,
-                    data=data,
-                    headers=headers,
-                    timeout=timeout,
-                    verify=verify
-                )
-
-                if resp.status_code >= 200 and resp.status_code < 400:
-                    return resp
-                else:
-                    logger.warning(
-                        f'HTTP POST FAIL - URL: {url} - STATUS CODE {resp.status_code} - CONTENT {resp.text}')
-            except Exception as e:
-                logger.warning(
-                    f'HTTP POST FAIL - URL: {url} - EXCEPTION {e}')
-                exception_obj = e
-
-            time.sleep(interval)
-            logger.warning('Retring HTTP POST')
-
-        # If there was no success
-        if resp:
-            # Checking response status
-            if raise_for_status:
-                if resp.status_code == 404:
-                    raise ResourceNotFound(
-                        f'{resouce_description} - {resp.text}')
-                resp.raise_for_status()
-
-            return resp
-            # raise Exception(
-            #     f'Error posting data. Status code: {resp.status_code}. Content: {resp.text}')
-        else:
-            raise HttpUtilPostException(
-                f'Error posting data.\nMessage {exception_obj}')
-
-    @staticmethod
-    def get_retry(url: str, headers: Dict[str, str] = None, timeout: int = 20, tries: int = 3, interval: int = 3, raise_for_status: bool = True, resouce_description: str = '', data: str = None, verify :bool = True, query_params: Dict[str, Any] = None):
-        logger.info(f'Get URL: {url}')
-        
-        # Encoding query params
-        if query_params is not None:
-            q_params = urllib.parse.urlencode(query_params, doseq=True)
-
-            if '?' in url:
-                url += '&' + q_params
-            else:
-                url += '?' + q_params
-                
-        logger.info(f'Get URL: {url}')
-
-        # Making tries
-        exception_obj = None
-        resp = None
-        for i in range(tries):
-            resp = None
-            try:
-                resp = requests.get(
-                    url=url,
-                    headers=headers,
-                    timeout=timeout,
-                    data=data,
-                    verify=verify
-                )
-
-                if resp.status_code >= 200 and resp.status_code < 400:
-                    return resp
-                else:
-                    logger.warning(
-                        f'HTTP GET FAIL - URL: {url} - STATUS CODE {resp.status_code} - CONTENT {resp.text}')
-            except Exception as e:
-                logger.warning(
-                    f'HTTP GET FAIL - URL: {url} - EXCEPTION {e}')
-                exception_obj = e
-
-            time.sleep(interval)
-            logger.warning('Retring HTTP GET')
-
-        # If there was no success
-        if resp:
-            # Checking response status
-            if raise_for_status:
-                if resp.status_code == 404:
-                    raise ResourceNotFound(
-                        f'{resouce_description} - {resp.text}')
-                resp.raise_for_status()
-
-            return resp
-            # raise Exception(
-            #     f'Error getting data. Status code: {resp.status_code}. Content: {resp.text}')
-        else:
-            raise HttpUtilGetException(
-                f'Error getting data.\nMessage {exception_obj}')
-
-    @staticmethod
-    def put_retry(url: str, data: str, headers: Dict[str, str] = None, timeout: int = 20, tries: int = 3,
-                   interval: int = 3, format_data: bool = True, raise_for_status: bool = True,
-                   resouce_description: str = '', verify :bool = True):
-        # Formatting data
-        if format_data:
-            if isinstance(data, dict) or isinstance(data, list):
-                logger.info(
-                    'Converting data from "dict" or "list" to json string')
-                data = json.dumps(data)
-
-                # adding content-type: application/json in headers
-                if headers:
-                    if not ('content-type' in [k.lower() for k in headers.keys()]):
-                        headers['content-type'] = 'application/json'
-                else:
-                    headers = {'content-type': 'application/json'}
-            elif not isinstance(data, str):
-                logger.info('Converting data from non string to string')
-                data = str(data)
-
-        logger.info(f'Puting data (bellow) to URL: {url}')
-        if not ('password' in data) and not ('client_secret' in data) and not ('pass' in data):
-            logger.info(f'Sending data: {data}')
-
-        # Making tries
-        exception_obj = None
-        resp = None
-        for i in range(tries):
-            resp = None
-            try:
-                resp = requests.put(
-                    url=url,
-                    data=data,
-                    headers=headers,
-                    timeout=timeout,
-                    verify=verify
-                )
-
-                if resp.status_code >= 200 and resp.status_code < 400:
-                    return resp
-                else:
-                    logger.warning(
-                        f'HTTP PUT FAIL - URL: {url} - STATUS CODE {resp.status_code} - CONTENT {resp.text}')
-            except Exception as e:
-                logger.warning(
-                    f'HTTP PUT FAIL - URL: {url} - EXCEPTION {e}')
-                exception_obj = e
-
-            time.sleep(interval)
-            logger.warning('Retring HTTP PUT')
-
-        # If there was no success
-        if resp:
-            # Checking response status
-            if raise_for_status:
-                if resp.status_code == 404:
-                    raise ResourceNotFound(
-                        f'{resouce_description} - {resp.text}')
-                resp.raise_for_status()
-
-            return resp
-        else:
-            raise HttpUtilPutException(
-                f'Error puting data.\nMessage {exception_obj}')
-
-    @staticmethod
-    def delete_retry(url: str, headers: Dict[str, str] = None, timeout: int = 20, tries: int = 3,
-                   interval: int = 3, format_data: bool = True, raise_for_status: bool = True,
-                   resouce_description: str = '', verify :bool = True):
-
-
-
-        # Making tries
-        exception_obj = None
-        resp = None
-        for i in range(tries):
-            resp = None
-            try:
-                resp = requests.delete(
-                    url=url,
-                    headers=headers,
-                    timeout=timeout,
-                    verify=verify
-                )
-
-                if resp.status_code >= 200 and resp.status_code < 400:
-                    return resp
-                else:
-                    logger.warning(
-                        f'HTTP DELETE FAIL - URL: {url} - STATUS CODE {resp.status_code} - CONTENT {resp.text}')
-            except Exception as e:
-                logger.warning(
-                    f'HTTP DELETE FAIL - URL: {url} - EXCEPTION {e}')
-                exception_obj = e
-
-            time.sleep(interval)
-            logger.warning('Retring HTTP DELETE')
-
-        # If there was no success
-        if resp:
-            # Checking response status
-            if raise_for_status:
-                if resp.status_code == 404:
-                    raise ResourceNotFound(
-                        f'{resouce_description} - {resp.text}')
-                resp.raise_for_status()
-
-            return resp
-        else:
-            raise HttpUtilDeleteException(
+import json
+import urllib
+
+import requests
+import time
+
+from nsj_gcf_utils.app_logger import logger
+from typing import Dict, Any
+
+
+class HttpUtilGetException(Exception):
+    pass
+
+
+class HttpUtilPostException(Exception):
+    pass
+
+class HttpUtilPutException(Exception):
+    pass
+
+class HttpUtilDeleteException(Exception):
+    pass
+
+
+class ResourceNotFound(Exception):
+    pass
+
+
+class HttpUtil:
+    @staticmethod
+    def post_retry(url: str, data: str, headers: Dict[str, str] = None, timeout: int = 20, tries: int = 3, interval: int = 3, format_data: bool = True, raise_for_status: bool = True, resouce_description: str = '', verify :bool = True, query_params: Dict[str, Any] = None):
+        # Encoding query params
+        if query_params is not None:
+            q_params = urllib.parse.urlencode(query_params, doseq=True)
+
+            if '?' in url:
+                url += '&' + q_params
+            else:
+                url += '?' + q_params
+                
+        logger.info(f'Post URL: {url}')
+        
+        # Formatting data
+        if format_data:
+            if isinstance(data, dict) or isinstance(data, list):
+                logger.info(
+                    'Converting data from "dict" or "list" to json string')
+                data = json.dumps(data)
+
+                # adding content-type: application/json in headers
+                if headers:
+                    if not ('content-type' in [k.lower() for k in headers.keys()]):
+                        headers['content-type'] = 'application/json'
+                else:
+                    headers = {'content-type': 'application/json'}
+            elif not isinstance(data, str):
+                logger.info('Converting data from non string to string')
+                data = str(data)
+
+        logger.info(f'Posting data (bellow) to URL: {url}')
+        if not('password' in data) and not('client_secret' in data) and not('pass' in data):
+            logger.info(f'Sending data: {data}')
+
+        # Making tries
+        exception_obj = None
+        resp = None
+        for i in range(tries):
+            resp = None
+            try:
+                resp = requests.post(
+                    url=url,
+                    data=data,
+                    headers=headers,
+                    timeout=timeout,
+                    verify=verify
+                )
+
+                if resp.status_code >= 200 and resp.status_code < 400:
+                    return resp
+                else:
+                    logger.warning(
+                        f'HTTP POST FAIL - URL: {url} - STATUS CODE {resp.status_code} - CONTENT {resp.text}')
+            except Exception as e:
+                logger.warning(
+                    f'HTTP POST FAIL - URL: {url} - EXCEPTION {e}')
+                exception_obj = e
+
+            time.sleep(interval)
+            logger.warning('Retring HTTP POST')
+
+        # If there was no success
+        if resp:
+            # Checking response status
+            if raise_for_status:
+                if resp.status_code == 404:
+                    raise ResourceNotFound(
+                        f'{resouce_description} - {resp.text}')
+                resp.raise_for_status()
+
+            return resp
+            # raise Exception(
+            #     f'Error posting data. Status code: {resp.status_code}. Content: {resp.text}')
+        else:
+            raise HttpUtilPostException(
+                f'Error posting data.\nMessage {exception_obj}')
+
+    @staticmethod
+    def get_retry(url: str, headers: Dict[str, str] = None, timeout: int = 20, tries: int = 3, interval: int = 3, raise_for_status: bool = True, resouce_description: str = '', data: str = None, verify :bool = True, query_params: Dict[str, Any] = None):
+        logger.info(f'Get URL: {url}')
+        
+        # Encoding query params
+        if query_params is not None:
+            q_params = urllib.parse.urlencode(query_params, doseq=True)
+
+            if '?' in url:
+                url += '&' + q_params
+            else:
+                url += '?' + q_params
+                
+        logger.info(f'Get URL: {url}')
+
+        # Making tries
+        exception_obj = None
+        resp = None
+        for i in range(tries):
+            resp = None
+            try:
+                resp = requests.get(
+                    url=url,
+                    headers=headers,
+                    timeout=timeout,
+                    data=data,
+                    verify=verify
+                )
+
+                if resp.status_code >= 200 and resp.status_code < 400:
+                    return resp
+                else:
+                    logger.warning(
+                        f'HTTP GET FAIL - URL: {url} - STATUS CODE {resp.status_code} - CONTENT {resp.text}')
+            except Exception as e:
+                logger.warning(
+                    f'HTTP GET FAIL - URL: {url} - EXCEPTION {e}')
+                exception_obj = e
+
+            time.sleep(interval)
+            logger.warning('Retring HTTP GET')
+
+        # If there was no success
+        if resp:
+            # Checking response status
+            if raise_for_status:
+                if resp.status_code == 404:
+                    raise ResourceNotFound(
+                        f'{resouce_description} - {resp.text}')
+                resp.raise_for_status()
+
+            return resp
+            # raise Exception(
+            #     f'Error getting data. Status code: {resp.status_code}. Content: {resp.text}')
+        else:
+            raise HttpUtilGetException(
+                f'Error getting data.\nMessage {exception_obj}')
+
+    @staticmethod
+    def put_retry(url: str, data: str, headers: Dict[str, str] = None, timeout: int = 20, tries: int = 3,
+                   interval: int = 3, format_data: bool = True, raise_for_status: bool = True,
+                   resouce_description: str = '', verify :bool = True):
+        # Formatting data
+        if format_data:
+            if isinstance(data, dict) or isinstance(data, list):
+                logger.info(
+                    'Converting data from "dict" or "list" to json string')
+                data = json.dumps(data)
+
+                # adding content-type: application/json in headers
+                if headers:
+                    if not ('content-type' in [k.lower() for k in headers.keys()]):
+                        headers['content-type'] = 'application/json'
+                else:
+                    headers = {'content-type': 'application/json'}
+            elif not isinstance(data, str):
+                logger.info('Converting data from non string to string')
+                data = str(data)
+
+        logger.info(f'Puting data (bellow) to URL: {url}')
+        if not ('password' in data) and not ('client_secret' in data) and not ('pass' in data):
+            logger.info(f'Sending data: {data}')
+
+        # Making tries
+        exception_obj = None
+        resp = None
+        for i in range(tries):
+            resp = None
+            try:
+                resp = requests.put(
+                    url=url,
+                    data=data,
+                    headers=headers,
+                    timeout=timeout,
+                    verify=verify
+                )
+
+                if resp.status_code >= 200 and resp.status_code < 400:
+                    return resp
+                else:
+                    logger.warning(
+                        f'HTTP PUT FAIL - URL: {url} - STATUS CODE {resp.status_code} - CONTENT {resp.text}')
+            except Exception as e:
+                logger.warning(
+                    f'HTTP PUT FAIL - URL: {url} - EXCEPTION {e}')
+                exception_obj = e
+
+            time.sleep(interval)
+            logger.warning('Retring HTTP PUT')
+
+        # If there was no success
+        if resp:
+            # Checking response status
+            if raise_for_status:
+                if resp.status_code == 404:
+                    raise ResourceNotFound(
+                        f'{resouce_description} - {resp.text}')
+                resp.raise_for_status()
+
+            return resp
+        else:
+            raise HttpUtilPutException(
+                f'Error puting data.\nMessage {exception_obj}')
+
+    @staticmethod
+    def delete_retry(url: str, headers: Dict[str, str] = None, timeout: int = 20, tries: int = 3,
+                   interval: int = 3, format_data: bool = True, raise_for_status: bool = True,
+                   resouce_description: str = '', verify :bool = True):
+
+
+
+        # Making tries
+        exception_obj = None
+        resp = None
+        for i in range(tries):
+            resp = None
+            try:
+                resp = requests.delete(
+                    url=url,
+                    headers=headers,
+                    timeout=timeout,
+                    verify=verify
+                )
+
+                if resp.status_code >= 200 and resp.status_code < 400:
+                    return resp
+                else:
+                    logger.warning(
+                        f'HTTP DELETE FAIL - URL: {url} - STATUS CODE {resp.status_code} - CONTENT {resp.text}')
+            except Exception as e:
+                logger.warning(
+                    f'HTTP DELETE FAIL - URL: {url} - EXCEPTION {e}')
+                exception_obj = e
+
+            time.sleep(interval)
+            logger.warning('Retring HTTP DELETE')
+
+        # If there was no success
+        if resp:
+            # Checking response status
+            if raise_for_status:
+                if resp.status_code == 404:
+                    raise ResourceNotFound(
+                        f'{resouce_description} - {resp.text}')
+                resp.raise_for_status()
+
+            return resp
+        else:
+            raise HttpUtilDeleteException(
                 f'Error deleting data.\nMessage {exception_obj}')
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/json_util.py` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/json_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,162 +1,175 @@
-import copy
-import datetime
-import json
-import re
-import uuid
-import decimal
-
-# JSON DUMPS
-
-
-def convert_to_dumps(data):
-    if data == None:
-        return None
-
-    data_copy = copy.copy(data)
-
-    if isinstance(data_copy, datetime.datetime):
-        return data_copy.strftime('%Y-%m-%dT%H:%M:%S')
-    elif isinstance(data_copy, datetime.date):
-        return data_copy.strftime('%Y-%m-%d')
-    elif isinstance(data_copy, uuid.UUID):
-        return str(data_copy)
-    elif isinstance(data_copy, decimal.Decimal):
-        return str(data_copy)
-    elif isinstance(data_copy, dict):
-        for key in data_copy.keys():
-            data_copy[key] = convert_to_dumps(data_copy[key])
-        return data_copy
-    elif isinstance(data_copy, list):
-        for idx in range(0, len(data_copy)):
-            data_copy[idx] = convert_to_dumps(data_copy[idx])
-
-        return data_copy
-    elif isinstance(data_copy, str) or isinstance(data_copy, int) or isinstance(data_copy, float) or isinstance(data_copy, bool):
-        return data_copy
-    elif isinstance(data_copy, object):
-        to_dict_method = getattr(data_copy, 'to_dict', None)
-        if to_dict_method is not None and callable(to_dict_method):
-            dict_attrs = data_copy.to_dict()
-        else:
-            attrs_fields = [k for k in data_copy.__dict__ if not callable(
-                getattr(data_copy, k, None))]
-            dict_attrs = {k: data_copy.__dict__[k] for k in attrs_fields}
-
-        return convert_to_dumps(dict_attrs)
-    else:
-        return data_copy
-
-
-def json_dumps(data, ensure_ascii=True, convert_before_dump=True):
-    """
-    Retorna a representação em json (string) do objeto recebido no parâmetro "data".
-
-    É importante destacar que este método está preparado para as seguintes transformações:
-    - datetime.datetime => '%Y-%m-%dT%H:%M:%S'
-    - datetime.date => '%Y-%m-%d'
-    - uuid.UUID => str(uuid.UUID)
-    - Decimal => float
-
-    Além disso, objetos (que não sejam de tipos primitivos, como str, float e bool), são
-    tratados como dicionários, tendo todos os seus atributos considerados como chaves do json.
-
-    Adicionalmente, se um objeto implementar um método "to_dict", a representação, em dicionário,
-    desse objeto será obtida por meio da invocação deste método, antes da transformação do mesmo
-    em json (permitindo customizar o modo como um objeto é serializado em json).
-    """
-    if convert_before_dump:
-        data_copy = convert_to_dumps(data)
-    else:
-        data_copy = data
-
-    return json.dumps(data_copy, ensure_ascii=ensure_ascii)
-
-
-# JSON LOADS
-def _loads_datetime_uuid(value):
-    if not isinstance(value, str):
-        return value
-
-    matcher_datetime = re.compile(
-        '^(\d\d\d\d)-(\d\d)-(\d\d)T(\d\d):(\d\d):(\d\d)$')
-    matcher_date = re.compile('^(\d\d\d\d)-(\d\d)-(\d\d)$')
-    matcher_uuid = re.compile(
-        '^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$')
-
-    match_datetime = matcher_datetime.search(value)
-    match_date = matcher_date.search(value)
-    match_uuid = matcher_uuid.search(value)
-
-    if match_datetime:
-        ano = int(match_datetime.group(1))
-        mes = int(match_datetime.group(2))
-        dia = int(match_datetime.group(3))
-        hora = int(match_datetime.group(4))
-        minuto = int(match_datetime.group(5))
-        segundo = int(match_datetime.group(6))
-
-        return datetime.datetime(year=ano, month=mes, day=dia, hour=hora, minute=minuto, second=segundo)
-    elif match_date:
-        ano = int(match_date.group(1))
-        mes = int(match_date.group(2))
-        dia = int(match_date.group(3))
-
-        return datetime.date(year=ano, month=mes, day=dia)
-    elif match_uuid:
-        return uuid.UUID(value)
-    else:
-        return value
-
-
-def _internal_loads(data):
-    if isinstance(data, dict):
-        for key in data.keys():
-            data[key] = _internal_loads(data[key])
-        return data
-
-    elif isinstance(data, list):
-        vector = []
-        for item in data:
-            vector.append(_internal_loads(item))
-        return vector
-
-    else:
-        return _loads_datetime_uuid(data)
-
-
-def _loads_to_class(load_data, model_class=None):
-    if isinstance(load_data, list):
-        return [_loads_to_class(item, model_class) for item in load_data]
-    elif isinstance(load_data, dict):
-        obj = model_class()
-        for k in load_data:
-            if hasattr(obj, k):
-                setattr(obj, k, load_data[k])
-        return obj
-    else:
-        return model_class()
-
-
-def json_loads(str_json: str, model_class=None):
-    """
-    Interpreta a string json recebida no parâmetro "str_json", retornando:
-    - Um dicionário ou uma lista de dicionários (se o parâmetro "model_class" for nulo)
-    - Um objeto do tipo model_class, ou uma lista desses objetos, atribuido o valor
-    das chaves correspondentes no json, para cada atributo com mesmo nome, no objeto.
-
-    É importante destacar que este método está preparado para as seguintes transformações:
-    - '%Y-%m-%dT%H:%M:%S' => datetime.datetime
-    - '%Y-%m-%d' => datetime.date
-    """
-
-    if isinstance(str_json, str):
-        data = json.loads(str_json)
-    else:
-        data = str_json
-
-    load_data = _internal_loads(data)
-
-    if model_class is None or (not isinstance(load_data, dict) and not isinstance(load_data, list)):
-        return load_data
-    else:
-        return _loads_to_class(load_data, model_class)
+import copy
+import datetime
+import decimal
+import enum
+import json
+import re
+import uuid
+
+# JSON DUMPS
+
+
+class JsonLoadException(Exception):
+    pass
+
+
+def convert_to_dumps(data):
+    if data == None:
+        return None
+
+    data_copy = copy.copy(data)
+
+    if isinstance(data_copy, datetime.datetime):
+        return data_copy.strftime('%Y-%m-%dT%H:%M:%S')
+    elif isinstance(data_copy, datetime.date):
+        return data_copy.strftime('%Y-%m-%d')
+    elif isinstance(data_copy, uuid.UUID):
+        return str(data_copy)
+    elif isinstance(data_copy, decimal.Decimal):
+        return str(data_copy)
+    elif isinstance(data_copy, dict):
+        for key in data_copy.keys():
+            data_copy[key] = convert_to_dumps(data_copy[key])
+        return data_copy
+    elif isinstance(data_copy, list):
+        for idx in range(0, len(data_copy)):
+            data_copy[idx] = convert_to_dumps(data_copy[idx])
+
+        return data_copy
+    elif isinstance(data_copy.__class__, enum.EnumMeta):
+        return data_copy.value
+    elif isinstance(data_copy, str) or isinstance(data_copy, int) or isinstance(data_copy, float) or isinstance(data_copy, bool):
+        return data_copy
+    elif isinstance(data_copy, object):
+        to_dict_method = getattr(data_copy, 'to_dict', None)
+        if to_dict_method is not None and callable(to_dict_method):
+            dict_attrs = data_copy.to_dict()
+        else:
+            attrs_fields = [k for k in data_copy.__dict__ if not callable(
+                getattr(data_copy, k, None))]
+            dict_attrs = {k: data_copy.__dict__[k] for k in attrs_fields}
+
+        return convert_to_dumps(dict_attrs)
+    else:
+        return data_copy
+
+
+def json_dumps(data, ensure_ascii=True, convert_before_dump=True):
+    """
+    Retorna a representação em json (string) do objeto recebido no parâmetro "data".
+
+    É importante destacar que este método está preparado para as seguintes transformações:
+    - datetime.datetime => '%Y-%m-%dT%H:%M:%S'
+    - datetime.date => '%Y-%m-%d'
+    - uuid.UUID => str(uuid.UUID)
+    - Decimal => float
+
+    Além disso, objetos (que não sejam de tipos primitivos, como str, float e bool), são
+    tratados como dicionários, tendo todos os seus atributos considerados como chaves do json.
+
+    Adicionalmente, se um objeto implementar um método "to_dict", a representação, em dicionário,
+    desse objeto será obtida por meio da invocação deste método, antes da transformação do mesmo
+    em json (permitindo customizar o modo como um objeto é serializado em json).
+    """
+    if convert_before_dump:
+        data_copy = convert_to_dumps(data)
+    else:
+        data_copy = data
+
+    return json.dumps(data_copy, ensure_ascii=ensure_ascii)
+
+
+# JSON LOADS
+def _loads_datetime_uuid(value):
+    if not isinstance(value, str):
+        return value
+
+    matcher_datetime = re.compile(
+        '^(\d\d\d\d)-(\d\d)-(\d\d)T(\d\d):(\d\d):(\d\d)$')
+    matcher_date = re.compile('^(\d\d\d\d)-(\d\d)-(\d\d)$')
+    matcher_uuid = re.compile(
+        '^[A-Fa-f0-9]{8}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{4}-[A-Fa-f0-9]{12}$')
+
+    match_datetime = matcher_datetime.search(value)
+    match_date = matcher_date.search(value)
+    match_uuid = matcher_uuid.search(value)
+
+    if match_datetime:
+        ano = int(match_datetime.group(1))
+        mes = int(match_datetime.group(2))
+        dia = int(match_datetime.group(3))
+        hora = int(match_datetime.group(4))
+        minuto = int(match_datetime.group(5))
+        segundo = int(match_datetime.group(6))
+
+        return datetime.datetime(year=ano, month=mes, day=dia, hour=hora, minute=minuto, second=segundo)
+    elif match_date:
+        ano = int(match_date.group(1))
+        mes = int(match_date.group(2))
+        dia = int(match_date.group(3))
+
+        return datetime.date(year=ano, month=mes, day=dia)
+    elif match_uuid:
+        return uuid.UUID(value)
+    else:
+        return value
+
+
+def _internal_loads(data):
+    if isinstance(data, dict):
+        for key in data.keys():
+            data[key] = _internal_loads(data[key])
+        return data
+
+    elif isinstance(data, list):
+        vector = []
+        for item in data:
+            vector.append(_internal_loads(item))
+        return vector
+
+    else:
+        return _loads_datetime_uuid(data)
+
+
+def _loads_to_class(load_data, model_class=None):
+    if isinstance(load_data, list):
+        return [_loads_to_class(item, model_class) for item in load_data]
+    elif isinstance(load_data, dict):
+        obj = model_class()
+        for k in load_data:
+            if hasattr(obj, k):
+                setattr(obj, k, load_data[k])
+        return obj
+    else:
+        return model_class()
+
+
+def json_loads(str_json: str, model_class=None):
+    """
+    Interpreta a string json recebida no parâmetro "str_json", retornando:
+    - Um dicionário ou uma lista de dicionários (se o parâmetro "model_class" for nulo)
+    - Um objeto do tipo model_class, ou uma lista desses objetos, atribuido o valor
+    das chaves correspondentes no json, para cada atributo com mesmo nome, no objeto.
+
+    É importante destacar que este método está preparado para as seguintes transformações:
+    - '%Y-%m-%dT%H:%M:%S' => datetime.datetime
+    - '%Y-%m-%d' => datetime.date
+    """
+    try:
+        if isinstance(str_json, str):
+            data = json.loads(str_json)
+        else:
+            data = str_json
+
+        load_data = _internal_loads(data)
+
+        if model_class is None or (not isinstance(load_data, dict) and not isinstance(load_data, list)):
+            return load_data
+        else:
+            return _loads_to_class(load_data, model_class)
+    except Exception as e:
+        msg = f"Erro interpretando json. Mensagem original do erro: {e}."
+        msg += '\nCorpo do json recebido:\n'
+        msg += f"{str_json}"
+
+        raise JsonLoadException(msg)
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/keycloak_service.py` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/keycloak_service.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from typing import Tuple
-
-from nsj_gcf_utils.http_util import HttpUtil
-
-
-class KeycloackService:
-    """
-    Class to authentication with KeyCloak.
-    """
-    _keycloack_token_url: str
-
-    def __init__(self, keycloack_token_url: str) -> None:
-        self._keycloack_token_url = keycloack_token_url
-
-    # TODO Melhorar controle de conexão, incluindo renovação do acess_token pelo refresh_token
-
-    def authenticate(self, client_id: str, username: str, password: str, scope: str, client_secret: str = None) -> Tuple[str, int, str, int]:
-        """
-        Authenticate with keycloak.
-
-        Returns a tuple, with:
-        [access_token: str, expires_in: int, refresh_token: str, refresh_expires_in: int]
-        """
-
-        # Making data
-        headers = {'Content-type': 'application/x-www-form-urlencoded'}
-        data = {
-            'client_id': client_id,
-            'scope': scope,
-            'grant_type': 'password',
-            'username': username,
-            'password': password
-        }
-
-        if client_secret is not None:
-            data['client_secret'] = client_secret
-
-        # Calling API
-        resp = HttpUtil.post_retry(self._keycloack_token_url,
-                                   headers=headers, data=data, format_data=False, resouce_description='get_access_token')
-
-        # Reading result
-        resp = resp.json()
-
-        return (
-            resp['access_token'],
-            resp['expires_in'],
-            resp['refresh_token'],
-            resp['refresh_expires_in']
-        )
+from typing import Tuple
+
+from nsj_gcf_utils.http_util import HttpUtil
+
+
+class KeycloackService:
+    """
+    Class to authentication with KeyCloak.
+    """
+    _keycloack_token_url: str
+
+    def __init__(self, keycloack_token_url: str) -> None:
+        self._keycloack_token_url = keycloack_token_url
+
+    # TODO Melhorar controle de conexão, incluindo renovação do acess_token pelo refresh_token
+
+    def authenticate(self, client_id: str, username: str, password: str, scope: str, client_secret: str = None) -> Tuple[str, int, str, int]:
+        """
+        Authenticate with keycloak.
+
+        Returns a tuple, with:
+        [access_token: str, expires_in: int, refresh_token: str, refresh_expires_in: int]
+        """
+
+        # Making data
+        headers = {'Content-type': 'application/x-www-form-urlencoded'}
+        data = {
+            'client_id': client_id,
+            'scope': scope,
+            'grant_type': 'password',
+            'username': username,
+            'password': password
+        }
+
+        if client_secret is not None:
+            data['client_secret'] = client_secret
+
+        # Calling API
+        resp = HttpUtil.post_retry(self._keycloack_token_url,
+                                   headers=headers, data=data, format_data=False, resouce_description='get_access_token')
+
+        # Reading result
+        resp = resp.json()
+
+        return (
+            resp['access_token'],
+            resp['expires_in'],
+            resp['refresh_token'],
+            resp['refresh_expires_in']
+        )
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/nsj_authentication_service.py` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/nsj_authentication_service.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import base64
-import re
-import requests
-
-
-class NsjAuthenticationService:
-
-    def __init__(self, client_id: str, client_secret: str, introspection_url: str) -> None:
-        self._client_id = client_id
-        self._client_secret = client_secret
-        self._introspection_url = introspection_url
-
-    def authenticate(self, access_token: str) -> str:
-        """
-        Check if access_token is valid (throught token introspection endpoint),
-        and returns access_token info, or None (is not valid).
-        """
-
-        # Checking heaaders
-        if not access_token:
-            return None
-
-        # Checking format (throught regex)
-        matcher = re.compile('^Bearer (.+)$')
-        match = matcher.match(access_token)
-        if not match:
-            return None
-        access_token = match.group(1)
-
-        # Calling Introspection Endpoint
-        basic = f'{self._client_id}:{self._client_secret}'
-        basic = base64.b64encode(basic.encode('utf-8')).decode('utf-8')
-        basic = f'Basic {basic}'
-
-        data = {
-            'token': access_token,
-            'token_type_hint': 'access_token'
-        }
-
-        headers = {
-            'Accept': 'application/json',
-            'Content-Type': 'application/x-www-form-urlencoded',
-            'Authorization': basic
-        }
-
-        resp = requests.post(url=self._introspection_url,
-                             data=data, headers=headers, timeout=60)
-
-        if resp.status_code == 401:
-            return Exception('Authentication error in token introspection. Check client_id and client_secret.')
-
-        resp.raise_for_status()
-        resp = resp.json()
-
-        # Testing result
-        if not ('username' in resp):
-            return None
-
-        # Returning token info
-        return resp
+import base64
+import re
+import requests
+
+
+class NsjAuthenticationService:
+
+    def __init__(self, client_id: str, client_secret: str, introspection_url: str) -> None:
+        self._client_id = client_id
+        self._client_secret = client_secret
+        self._introspection_url = introspection_url
+
+    def authenticate(self, access_token: str) -> str:
+        """
+        Check if access_token is valid (throught token introspection endpoint),
+        and returns access_token info, or None (is not valid).
+        """
+
+        # Checking heaaders
+        if not access_token:
+            return None
+
+        # Checking format (throught regex)
+        matcher = re.compile('^Bearer (.+)$')
+        match = matcher.match(access_token)
+        if not match:
+            return None
+        access_token = match.group(1)
+
+        # Calling Introspection Endpoint
+        basic = f'{self._client_id}:{self._client_secret}'
+        basic = base64.b64encode(basic.encode('utf-8')).decode('utf-8')
+        basic = f'Basic {basic}'
+
+        data = {
+            'token': access_token,
+            'token_type_hint': 'access_token'
+        }
+
+        headers = {
+            'Accept': 'application/json',
+            'Content-Type': 'application/x-www-form-urlencoded',
+            'Authorization': basic
+        }
+
+        resp = requests.post(url=self._introspection_url,
+                             data=data, headers=headers, timeout=60)
+
+        if resp.status_code == 401:
+            return Exception('Authentication error in token introspection. Check client_id and client_secret.')
+
+        resp.raise_for_status()
+        resp = resp.json()
+
+        # Testing result
+        if not ('username' in resp):
+            return None
+
+        # Returning token info
+        return resp
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/rest_error_util.py` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/rest_error_util.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-from nsj_gcf_utils  .exception import ERPException
-from nsj_gcf_utils.json_util import json_dumps, json_loads
-from pydantic import ValidationError
-from typing import Dict, List, Union, Tuple
-
-
-def _format_tuple_error(error: Tuple[str, str]):
-    return {
-        'code': error[0],
-        'message': error[1]
-    }
-
-
-def _format_erpexception_error(error: ERPException):
-    return {
-        'code': error.mope_code,
-        'message': error.message
-    }
-
-
-def _format_list_error(error: Union[List[Tuple[str, str]], List[ERPException]]):
-    result = []
-    for e in error:
-        if isinstance(e, tuple):
-            formated = _format_tuple_error(e)
-        elif isinstance(e, ERPException):
-            formated = _format_erpexception_error(e)
-        elif isinstance(e, str):
-            e = (None, e)
-            formated = _format_tuple_error(e)
-        elif isinstance(e, Exception):
-            e = (None, f'{e}')
-            formated = _format_tuple_error(e)
-        else:
-            formated = _format_unknow_error()
-
-        result.append(formated)
-
-    return result
-
-
-def _format_unknow_error():
-    return {
-        'code': None,
-        'message': 'Erro desconhecido'
-    }
-
-
-def _format_pydantic_validation_error(error: ValidationError):
-    result = []
-    errors = json_loads(error.json())
-    for e in errors:
-        msg = f"Erro de validando campo '{e['loc'][0]}' de entrada. Mensagem do erro: {e['msg']}."
-        e_tuple = (None, msg)
-        result.append(_format_tuple_error(e_tuple))
-
-    return result
-
-
-def format_error_body(
-    error: Union[
-        Tuple[str, str],
-        List[Tuple[str, str]],
-        ERPException,
-        List[ERPException],
-        str,
-        Exception,
-        List[str],
-        List[Exception],
-        ValidationError
-    ]
-) -> List[Dict[str, str]]:
-
-    if isinstance(error, tuple):
-        return [_format_tuple_error(error)]
-    elif isinstance(error, list):
-        return _format_list_error(error)
-    elif isinstance(error, ERPException):
-        return [_format_erpexception_error(error)]
-    elif isinstance(error, str):
-        error = (None, error)
-        return [_format_tuple_error(error)]
-    elif isinstance(error, ValidationError):
-        return _format_pydantic_validation_error(error)
-    elif isinstance(error, Exception):
-        error = (None, f'{error}')
-        return [_format_tuple_error(error)]
-    else:
-        return [_format_unknow_error()]
-
-
-def format_json_error(
-    error: Union[
-        Tuple[str, str],
-        List[Tuple[str, str]],
-        ERPException,
-        List[ERPException],
-        str,
-        Exception,
-        List[str],
-        List[Exception],
-        ValidationError
-    ]
-) -> List[Dict[str, str]]:
-    return json_dumps(format_error_body(error))
+from nsj_gcf_utils  .exception import ERPException
+from nsj_gcf_utils.json_util import json_dumps, json_loads
+from pydantic import ValidationError
+from typing import Dict, List, Union, Tuple
+
+
+def _format_tuple_error(error: Tuple[str, str]):
+    return {
+        'code': error[0],
+        'message': error[1]
+    }
+
+
+def _format_erpexception_error(error: ERPException):
+    return {
+        'code': error.mope_code,
+        'message': error.message
+    }
+
+
+def _format_list_error(error: Union[List[Tuple[str, str]], List[ERPException]]):
+    result = []
+    for e in error:
+        if isinstance(e, tuple):
+            formated = _format_tuple_error(e)
+        elif isinstance(e, ERPException):
+            formated = _format_erpexception_error(e)
+        elif isinstance(e, str):
+            e = (None, e)
+            formated = _format_tuple_error(e)
+        elif isinstance(e, Exception):
+            e = (None, f'{e}')
+            formated = _format_tuple_error(e)
+        else:
+            formated = _format_unknow_error()
+
+        result.append(formated)
+
+    return result
+
+
+def _format_unknow_error():
+    return {
+        'code': None,
+        'message': 'Erro desconhecido'
+    }
+
+
+def _format_pydantic_validation_error(error: ValidationError):
+    result = []
+    errors = json_loads(error.json())
+    for e in errors:
+        msg = f"Erro de validando campo '{e['loc'][0]}' de entrada. Mensagem do erro: {e['msg']}."
+        e_tuple = (None, msg)
+        result.append(_format_tuple_error(e_tuple))
+
+    return result
+
+
+def format_error_body(
+    error: Union[
+        Tuple[str, str],
+        List[Tuple[str, str]],
+        ERPException,
+        List[ERPException],
+        str,
+        Exception,
+        List[str],
+        List[Exception],
+        ValidationError
+    ]
+) -> List[Dict[str, str]]:
+
+    if isinstance(error, tuple):
+        return [_format_tuple_error(error)]
+    elif isinstance(error, list):
+        return _format_list_error(error)
+    elif isinstance(error, ERPException):
+        return [_format_erpexception_error(error)]
+    elif isinstance(error, str):
+        error = (None, error)
+        return [_format_tuple_error(error)]
+    elif isinstance(error, ValidationError):
+        return _format_pydantic_validation_error(error)
+    elif isinstance(error, Exception):
+        error = (None, f'{error}')
+        return [_format_tuple_error(error)]
+    else:
+        return [_format_unknow_error()]
+
+
+def format_json_error(
+    error: Union[
+        Tuple[str, str],
+        List[Tuple[str, str]],
+        ERPException,
+        List[ERPException],
+        str,
+        Exception,
+        List[str],
+        List[Exception],
+        ValidationError
+    ]
+) -> List[Dict[str, str]]:
+    return json_dumps(format_error_body(error))
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils/router.py` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils/router.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-import re
-
-from nsj_gcf_utils.app_logger import logger
-from typing import List
-
-
-class Router:
-    from functools import partialmethod
-
-    def __init__(self, authentication_service=None, nsj_authentication_service=None):
-        self.routes = []
-        self.authentication_service = authentication_service
-        self.nsj_authentication_service = nsj_authentication_service
-
-    def add(self, path, authentication_fn, methods=['GET', 'POST'], required_pars: List[str] = None, allowed_clients: List[str] = None, required_query_args: List[str] = None):
-        def route_function(function):
-            # Making a regex to path
-            regex_path = path.replace('/', '\/')
-            matcher = re.compile('(\{([\w-]+)\})')
-            args = matcher.findall(regex_path)
-            path_args = []
-            for arg in args:
-                regex_path = regex_path.replace(arg[0], '([\w-]+)')
-                path_args.append(arg[1])
-
-            regex_path = '^' + regex_path + '$'
-
-            # Registering path
-            route = {
-                'path': path,
-                'regex_path': regex_path,
-                'methods': methods,
-                'callable': function,
-                'authentication_fn': authentication_fn,
-                'required_pars': required_pars,
-                'path_args': path_args,
-                'allowed_clients': allowed_clients,
-                'required_query_args': required_query_args}
-            self.routes.append(route)
-            return function
-        return route_function
-
-    def verify_api_key(self, request) -> str:
-        """
-        Returns the app_client id, if api_key is valid, or None otherwise.
-        """
-
-        api_key = request.headers.get('X-API-Key')
-
-        if api_key is None or api_key == '':
-            logger.info("No API Key Provided.")
-            return None
-
-        if self.authentication_service is None:
-            return None
-
-        return self.authentication_service.verify_api_key(api_key)
-
-    def verify_access_token(self, request) -> str:
-        """
-        Returns a dict with token info, if access_token is valid, or None otherwise.
-        """
-
-        access_token = request.headers.get('Authorization')
-
-        if access_token is None or access_token == '':
-            logger.info("No access_token Provided.")
-            return None
-
-        if self.nsj_authentication_service is None:
-            return None
-
-        return self.nsj_authentication_service.authenticate(access_token)
-
-    def verify_api_key_or_access_token(self, request) -> str:
-        """
-        Returns api_key or access_token result
-        """
-
-        auth_info = self.verify_api_key(request)
-        if auth_info is None:
-            auth_info = self.verify_access_token(request)
-
-        if auth_info is None or auth_info == '':
-            logger.info("No API Key or access_token Provided.")
-            return None
-
-        return auth_info
-
-    __call__ = partialmethod(
-        add, authentication_fn=lambda self, request: 'not_auth_required')
-    auth_api_key = partialmethod(
-        add, authentication_fn=verify_api_key)
-    auth_access_token = partialmethod(
-        add, authentication_fn=verify_access_token)
-    auth_api_key_or_access_token = partialmethod(
-        add, authentication_fn=verify_api_key_or_access_token)
-
-    def route(self, request):
-        path = request.path
-        logger.info(f'Routing to {path}')
-
-        # Searching route using regex expression (each route is interpreted like a regex pattern)
-        route = None
-        path_args = []
-        for r in self.routes:
-            matcher = re.compile(r['regex_path'])
-            match = matcher.search(path)
-
-            if not match:
-                continue
-
-            if not request.method in r['methods']:
-                continue
-
-            route = r
-
-            # Making a dict of path args (where each regex group is an argument)
-            path_args = {}
-            for i in range(0, matcher.groups):
-                path_key = route['path_args'][i]
-                path_args[path_key] = match.group(i+1)
-
-            break
-
-        # Checking if route exists
-        if not route:
-            return ('{"code": 404, "message": "Resource not found"}', 404, {})
-
-        # Checking authentication
-        auth_info = route['authentication_fn'](self, request)
-        if not auth_info:
-            return ('{"code", "401", "message": "Unauthorized."', 401, {})
-
-        # Checking authorization
-        if (
-            auth_info != 'not_auth_required'
-            and isinstance(auth_info, str)
-            and route['allowed_clients']
-            and not (auth_info in route['allowed_clients'])
-        ):
-            return ('{"code", "403", "message": "Forbidden. Client of X-API-Key has no access to this resource."', 403, {})
-
-        # Checking if called HTTP method is acceptable
-        if not request.method in route['methods']:
-            return ('{"code": 405, "message": "Method not allowed"}', 405, {})
-
-        # Checking required pars
-        required_pars = route['required_pars']
-        if required_pars:
-            req_body = request.get_json()
-            if not req_body:
-                return ('{' + f'"code": 400, "message": "Missing parameters {required_pars}"' + '}', 400, {})
-
-            missing_pars = []
-            for par in required_pars:
-                if not(par in req_body):
-                    missing_pars.append(par)
-
-            if len(missing_pars) > 0:
-                return ('{' + f'"code": 400, "message": "Missing parameters: {missing_pars}"' + '}', 400, {})
-
-        # Checking required query args
-        required_query_args = route['required_query_args']
-        if required_query_args:
-            args = request.args
-            if not args or len(args) <= 0:
-                return ('{' + f'"code": 400, "message": "Missing query arguments {required_query_args}"' + '}', 400, {})
-
-            missing_args = []
-            for par in required_query_args:
-                if not(par in args):
-                    missing_args.append(par)
-
-            if len(missing_args) > 0:
-                return ('{' + f'"code": 400, "message": "Missing query arguments {missing_args}"' + '}', 400, {})
-
-        # Returning original function handler
-        if auth_info == 'not_auth_required':
-            return route['callable'](request, **path_args)
-        else:
-            return route['callable'](request, auth_info, **path_args)
+import re
+
+from nsj_gcf_utils.app_logger import logger
+from typing import List
+
+
+class Router:
+    from functools import partialmethod
+
+    def __init__(self, authentication_service=None, nsj_authentication_service=None):
+        self.routes = []
+        self.authentication_service = authentication_service
+        self.nsj_authentication_service = nsj_authentication_service
+
+    def add(self, path, authentication_fn, methods=['GET', 'POST'], required_pars: List[str] = None, allowed_clients: List[str] = None, required_query_args: List[str] = None):
+        def route_function(function):
+            # Making a regex to path
+            regex_path = path.replace('/', '\/')
+            matcher = re.compile('(\{([\w-]+)\})')
+            args = matcher.findall(regex_path)
+            path_args = []
+            for arg in args:
+                regex_path = regex_path.replace(arg[0], '([\w-]+)')
+                path_args.append(arg[1])
+
+            regex_path = '^' + regex_path + '$'
+
+            # Registering path
+            route = {
+                'path': path,
+                'regex_path': regex_path,
+                'methods': methods,
+                'callable': function,
+                'authentication_fn': authentication_fn,
+                'required_pars': required_pars,
+                'path_args': path_args,
+                'allowed_clients': allowed_clients,
+                'required_query_args': required_query_args}
+            self.routes.append(route)
+            return function
+        return route_function
+
+    def verify_api_key(self, request) -> str:
+        """
+        Returns the app_client id, if api_key is valid, or None otherwise.
+        """
+
+        api_key = request.headers.get('X-API-Key')
+
+        if api_key is None or api_key == '':
+            logger.info("No API Key Provided.")
+            return None
+
+        if self.authentication_service is None:
+            return None
+
+        return self.authentication_service.verify_api_key(api_key)
+
+    def verify_access_token(self, request) -> str:
+        """
+        Returns a dict with token info, if access_token is valid, or None otherwise.
+        """
+
+        access_token = request.headers.get('Authorization')
+
+        if access_token is None or access_token == '':
+            logger.info("No access_token Provided.")
+            return None
+
+        if self.nsj_authentication_service is None:
+            return None
+
+        return self.nsj_authentication_service.authenticate(access_token)
+
+    def verify_api_key_or_access_token(self, request) -> str:
+        """
+        Returns api_key or access_token result
+        """
+
+        auth_info = self.verify_api_key(request)
+        if auth_info is None:
+            auth_info = self.verify_access_token(request)
+
+        if auth_info is None or auth_info == '':
+            logger.info("No API Key or access_token Provided.")
+            return None
+
+        return auth_info
+
+    __call__ = partialmethod(
+        add, authentication_fn=lambda self, request: 'not_auth_required')
+    auth_api_key = partialmethod(
+        add, authentication_fn=verify_api_key)
+    auth_access_token = partialmethod(
+        add, authentication_fn=verify_access_token)
+    auth_api_key_or_access_token = partialmethod(
+        add, authentication_fn=verify_api_key_or_access_token)
+
+    def route(self, request):
+        path = request.path
+        logger.info(f'Routing to {path}')
+
+        # Searching route using regex expression (each route is interpreted like a regex pattern)
+        route = None
+        path_args = []
+        for r in self.routes:
+            matcher = re.compile(r['regex_path'])
+            match = matcher.search(path)
+
+            if not match:
+                continue
+
+            if not request.method in r['methods']:
+                continue
+
+            route = r
+
+            # Making a dict of path args (where each regex group is an argument)
+            path_args = {}
+            for i in range(0, matcher.groups):
+                path_key = route['path_args'][i]
+                path_args[path_key] = match.group(i+1)
+
+            break
+
+        # Checking if route exists
+        if not route:
+            return ('{"code": 404, "message": "Resource not found"}', 404, {})
+
+        # Checking authentication
+        auth_info = route['authentication_fn'](self, request)
+        if not auth_info:
+            return ('{"code", "401", "message": "Unauthorized."', 401, {})
+
+        # Checking authorization
+        if (
+            auth_info != 'not_auth_required'
+            and isinstance(auth_info, str)
+            and route['allowed_clients']
+            and not (auth_info in route['allowed_clients'])
+        ):
+            return ('{"code", "403", "message": "Forbidden. Client of X-API-Key has no access to this resource."', 403, {})
+
+        # Checking if called HTTP method is acceptable
+        if not request.method in route['methods']:
+            return ('{"code": 405, "message": "Method not allowed"}', 405, {})
+
+        # Checking required pars
+        required_pars = route['required_pars']
+        if required_pars:
+            req_body = request.get_json()
+            if not req_body:
+                return ('{' + f'"code": 400, "message": "Missing parameters {required_pars}"' + '}', 400, {})
+
+            missing_pars = []
+            for par in required_pars:
+                if not(par in req_body):
+                    missing_pars.append(par)
+
+            if len(missing_pars) > 0:
+                return ('{' + f'"code": 400, "message": "Missing parameters: {missing_pars}"' + '}', 400, {})
+
+        # Checking required query args
+        required_query_args = route['required_query_args']
+        if required_query_args:
+            args = request.args
+            if not args or len(args) <= 0:
+                return ('{' + f'"code": 400, "message": "Missing query arguments {required_query_args}"' + '}', 400, {})
+
+            missing_args = []
+            for par in required_query_args:
+                if not(par in args):
+                    missing_args.append(par)
+
+            if len(missing_args) > 0:
+                return ('{' + f'"code": 400, "message": "Missing query arguments {missing_args}"' + '}', 400, {})
+
+        # Returning original function handler
+        if auth_info == 'not_auth_required':
+            return route['callable'](request, **path_args)
+        else:
+            return route['callable'](request, auth_info, **path_args)
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils.egg-info/PKG-INFO` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: nsj-gcf-utils
-Version: 1.0.8
-Summary: Utilitários para construção de Google Cloud Functions.
-Home-page: https://github.com/Nasajon/nsj_gcf_utils
-Author: Nasajon Sistemas
-Author-email: contact.dev@nasajon.com.br
-Project-URL: Source, https://github.com/Nasajon/nsj_gcf_utils
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# nsj_gcf_utils
-Utilitários para construção de Google Cloud Functions.
-
-## Features disponíveis
-
-Segue breve descrição das features disponiveis, identificando os respectivos módulos:
-
-* ```nsj_gcf_utils.app_logger```: Configuração padrão de logger para aplicações GCF.
-* ```nsj_gcf_utils.authentication_service```: Validação de chaves recebidas no cabeçalho X-API-Key.
-* ```nsj_gcf_utils.db_adapter```: Adapter de comunicação com o banco.
-* ```nsj_gcf_utils.http_util```: Realiza requisições HTTP, com suporte a tentativas seguidas em caso de falha.
-* ```nsj_gcf_utils.iban```: Utilitário para manipulação de International Bank Account Number (IBAN)
-* ```nsj_gcf_utils.json_util```: Serialização e desserialização em JSON, com manipulação nativa de datas no formato "yyyy-mm-ddThh:mm:ss". Decimal é traduzido para string ao serializar para JSON.
-* ```nsj_gcf_utils.keycloak_service```: Autenticação para aplicação enquanto cliente Oauth.
-* ```nsj_gcf_utils.nsj_authentication_service```: Validação de access_token recebido no cabeçalho Authorization (Bearer token), por meio do padrão Token Instrospection (RFC 7662).
-* ```nsj_gcf_utils.router```: Utilitário para controler de rotas por meio decorators, fazendo com que uma fucntion-framework se comporte de modo similar a outros frameworks web como Spring ou Symfony.
-
-## Testes Automatizados
-
-Sempre rode o comando abaixo, antes de dar push neste repositório:
-
-> make tests
+Metadata-Version: 2.1
+Name: nsj-gcf-utils
+Version: 1.0.9
+Summary: Utilitários para construção de Google Cloud Functions.
+Home-page: https://github.com/Nasajon/nsj_gcf_utils
+Author: Nasajon Sistemas
+Author-email: contact.dev@nasajon.com.br
+Project-URL: Source, https://github.com/Nasajon/nsj_gcf_utils
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# nsj_gcf_utils
+Utilitários para construção de Google Cloud Functions.
+
+## Features disponíveis
+
+Segue breve descrição das features disponiveis, identificando os respectivos módulos:
+
+* ```nsj_gcf_utils.app_logger```: Configuração padrão de logger para aplicações GCF.
+* ```nsj_gcf_utils.authentication_service```: Validação de chaves recebidas no cabeçalho X-API-Key.
+* ```nsj_gcf_utils.db_adapter```: Adapter de comunicação com o banco.
+* ```nsj_gcf_utils.http_util```: Realiza requisições HTTP, com suporte a tentativas seguidas em caso de falha.
+* ```nsj_gcf_utils.iban```: Utilitário para manipulação de International Bank Account Number (IBAN)
+* ```nsj_gcf_utils.json_util```: Serialização e desserialização em JSON, com manipulação nativa de datas no formato "yyyy-mm-ddThh:mm:ss". Decimal é traduzido para string ao serializar para JSON.
+* ```nsj_gcf_utils.keycloak_service```: Autenticação para aplicação enquanto cliente Oauth.
+* ```nsj_gcf_utils.nsj_authentication_service```: Validação de access_token recebido no cabeçalho Authorization (Bearer token), por meio do padrão Token Instrospection (RFC 7662).
+* ```nsj_gcf_utils.router```: Utilitário para controler de rotas por meio decorators, fazendo com que uma fucntion-framework se comporte de modo similar a outros frameworks web como Spring ou Symfony.
+
+## Testes Automatizados
+
+Sempre rode o comando abaixo, antes de dar push neste repositório:
+
+> make tests
```

### Comparing `nsj_gcf_utils-1.0.8/src/nsj_gcf_utils.egg-info/SOURCES.txt` & `nsj_gcf_utils-1.0.9/src/nsj_gcf_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

