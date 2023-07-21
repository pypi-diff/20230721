# Comparing `tmp/gyver-2.3.4.tar.gz` & `tmp/gyver-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver-2.3.4.tar", max compression
+gzip compressed data, was "gyver-2.4.0.tar", max compression
```

## Comparing `gyver-2.3.4.tar` & `gyver-2.4.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1079 2023-06-20 21:41:14.557536 gyver-2.3.4/LICENSE
--rw-r--r--   0        0        0     1005 2023-06-20 21:41:14.557536 gyver-2.3.4/README.md
--rw-r--r--   0        0        0      158 2023-07-14 20:30:45.883837 gyver-2.3.4/gyver/__init__.py
--rw-r--r--   0        0        0      359 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/cache/__init__.py
--rw-r--r--   0        0        0     1201 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/cache/asyncio.py
--rw-r--r--   0        0        0      237 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/cache/config.py
--rw-r--r--   0        0        0     1776 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/cache/interface.py
--rw-r--r--   0        0        0     1395 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/cache/mapper.py
--rw-r--r--   0        0        0     5993 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/cache/mock.py
--rw-r--r--   0        0        0     4283 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/cache/redis.py
--rw-r--r--   0        0        0     1128 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/cache/sync.py
--rw-r--r--   0        0        0      558 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/cache/utils.py
--rw-r--r--   0        0        0      597 2023-07-14 20:26:34.305166 gyver-2.3.4/gyver/config/__init__.py
--rw-r--r--   0        0        0       78 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/config/adapter/__init__.py
--rw-r--r--   0        0        0     1320 2023-06-20 21:41:14.559536 gyver-2.3.4/gyver/config/adapter/attrs.py
--rw-r--r--   0        0        0     1078 2023-06-20 21:41:14.560536 gyver-2.3.4/gyver/config/adapter/dataclass.py
--rw-r--r--   0        0        0     5940 2023-06-27 06:41:36.152386 gyver-2.3.4/gyver/config/adapter/factory.py
--rw-r--r--   0        0        0     1056 2023-06-20 21:41:14.560536 gyver-2.3.4/gyver/config/adapter/gattrs.py
--rw-r--r--   0        0        0     2107 2023-06-20 21:41:14.560536 gyver-2.3.4/gyver/config/adapter/interface.py
--rw-r--r--   0        0        0     1701 2023-06-20 21:41:14.560536 gyver-2.3.4/gyver/config/adapter/mark.py
--rw-r--r--   0        0        0     1091 2023-06-20 21:41:14.560536 gyver-2.3.4/gyver/config/adapter/pydantic.py
--rw-r--r--   0        0        0     3459 2023-06-27 06:41:36.152386 gyver-2.3.4/gyver/config/config.py
--rw-r--r--   0        0        0     2815 2023-07-14 20:29:04.452357 gyver-2.3.4/gyver/config/envconfig.py
--rw-r--r--   0        0        0     1016 2023-06-27 06:41:36.152386 gyver-2.3.4/gyver/config/interface.py
--rw-r--r--   0        0        0     5534 2023-06-27 06:41:36.152386 gyver-2.3.4/gyver/config/lazy.py
--rw-r--r--   0        0        0      627 2023-06-27 06:41:36.152386 gyver-2.3.4/gyver/config/typedef.py
--rw-r--r--   0        0        0      473 2023-06-20 21:41:14.560536 gyver-2.3.4/gyver/config/utils.py
--rw-r--r--   0        0        0      419 2023-06-20 21:41:14.560536 gyver-2.3.4/gyver/context/__init__.py
--rw-r--r--   0        0        0      288 2023-06-20 21:41:14.560536 gyver-2.3.4/gyver/context/atomic_/__init__.py
--rw-r--r--   0        0        0     2317 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/context/atomic_/bound.py
--rw-r--r--   0        0        0     2493 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/context/atomic_/core.py
--rw-r--r--   0        0        0     1332 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/context/atomic_/resolver.py
--rw-r--r--   0        0        0     5659 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/context/context.py
--rw-r--r--   0        0        0      102 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/context/interfaces/__init__.py
--rw-r--r--   0        0        0     1525 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/context/interfaces/adapter.py
--rw-r--r--   0        0        0       39 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/context/typedef.py
--rw-r--r--   0        0        0      253 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/crypto/__init__.py
--rw-r--r--   0        0        0      133 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/crypto/config.py
--rw-r--r--   0        0        0      909 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/crypto/fernet.py
--rw-r--r--   0        0        0     1856 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/crypto/rsa.py
--rw-r--r--   0        0        0      749 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/database/__init__.py
--rw-r--r--   0        0        0     2136 2023-06-20 21:41:14.561536 gyver-2.3.4/gyver/database/adapter.py
--rw-r--r--   0        0        0     1233 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/config.py
--rw-r--r--   0        0        0      360 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/context/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/context/asyncio.py
--rw-r--r--   0        0        0     3349 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/context/sync.py
--rw-r--r--   0        0        0      170 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/drivers/__init__.py
--rw-r--r--   0        0        0      229 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/drivers/dialect.py
--rw-r--r--   0        0        0      224 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/drivers/interface.py
--rw-r--r--   0        0        0     1493 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/drivers/utils.py
--rw-r--r--   0        0        0     1076 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/entity.py
--rw-r--r--   0        0        0      498 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/entity.pyi
--rw-r--r--   0        0        0       50 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/metadata.py
--rw-r--r--   0        0        0     1012 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/query/__init__.py
--rw-r--r--   0        0        0     1692 2023-06-20 21:41:14.562536 gyver-2.3.4/gyver/database/query/_helpers.py
--rw-r--r--   0        0        0     2935 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/database/query/comp.py
--rw-r--r--   0        0        0      294 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/database/query/exc.py
--rw-r--r--   0        0        0     1220 2023-06-29 13:49:12.116121 gyver-2.3.4/gyver/database/query/interface.py
--rw-r--r--   0        0        0      279 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/database/query/null.py
--rw-r--r--   0        0        0     1270 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/database/query/order_by.py
--rw-r--r--   0        0        0     1239 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/database/query/paginate.py
--rw-r--r--   0        0        0      697 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/database/query/utils.py
--rw-r--r--   0        0        0     4613 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/database/query/where.py
--rw-r--r--   0        0        0      327 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/database/typedef.py
--rw-r--r--   0        0        0     4243 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/database/utils.py
--rw-r--r--   0        0        0     2272 2023-06-27 06:41:36.152386 gyver-2.3.4/gyver/exc.py
--rw-r--r--   0        0        0      225 2023-06-20 21:52:51.019089 gyver-2.3.4/gyver/filetree/__init__.py
--rw-r--r--   0        0        0     1749 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/filetree/filetree.py
--rw-r--r--   0        0        0      348 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/filetree/helpers.py
--rw-r--r--   0        0        0     3248 2023-07-05 16:03:52.217431 gyver-2.3.4/gyver/filetree/interface.py
--rw-r--r--   0        0        0     2502 2023-07-14 20:26:34.416168 gyver-2.3.4/gyver/filetree/typedef.py
--rw-r--r--   0        0        0     2808 2023-06-27 06:41:36.153386 gyver-2.3.4/gyver/filetree/virtual.py
--rw-r--r--   0        0        0      857 2023-06-20 21:41:14.563536 gyver-2.3.4/gyver/model.py
--rw-r--r--   0        0        0      101 2023-06-20 21:41:14.564536 gyver-2.3.4/gyver/pools/__init__.py
--rw-r--r--   0        0        0     5764 2023-06-20 21:41:14.564536 gyver-2.3.4/gyver/pools/asyncio.py
--rw-r--r--   0        0        0     2225 2023-06-20 21:41:14.564536 gyver-2.3.4/gyver/pools/resource.py
--rw-r--r--   0        0        0     3855 2023-06-20 21:41:14.564536 gyver-2.3.4/gyver/pools/thread.py
--rw-r--r--   0        0        0        0 2023-06-20 21:41:14.564536 gyver-2.3.4/gyver/py.typed
--rw-r--r--   0        0        0      186 2023-06-20 21:41:14.564536 gyver-2.3.4/gyver/url/__init__.py
--rw-r--r--   0        0        0     4639 2023-07-14 20:26:33.599156 gyver-2.3.4/gyver/url/core.py
--rw-r--r--   0        0        0      423 2023-06-20 21:41:14.564536 gyver-2.3.4/gyver/url/encode.py
--rw-r--r--   0        0        0     1285 2023-06-27 06:41:36.153386 gyver-2.3.4/gyver/url/fragment.py
--rw-r--r--   0        0        0     5566 2023-06-27 06:41:36.153386 gyver-2.3.4/gyver/url/netloc.py
--rw-r--r--   0        0        0     4307 2023-06-27 06:41:36.153386 gyver-2.3.4/gyver/url/path.py
--rw-r--r--   0        0        0     3636 2023-07-14 20:26:34.443168 gyver-2.3.4/gyver/url/query.py
--rw-r--r--   0        0        0     1186 2023-06-27 06:41:36.153386 gyver-2.3.4/gyver/url/utils.py
--rw-r--r--   0        0        0      726 2023-06-20 21:41:14.565536 gyver-2.3.4/gyver/utils/__init__.py
--rw-r--r--   0        0        0      156 2023-06-20 21:41:14.565536 gyver-2.3.4/gyver/utils/exc.py
--rw-r--r--   0        0        0     7836 2023-06-20 21:41:14.565536 gyver-2.3.4/gyver/utils/finder.py
--rw-r--r--   0        0        0     4262 2023-06-27 06:41:36.153386 gyver-2.3.4/gyver/utils/helpers.py
--rw-r--r--   0        0        0      174 2023-06-20 21:41:14.565536 gyver-2.3.4/gyver/utils/json.py
--rw-r--r--   0        0        0     2574 2023-06-27 06:41:36.154386 gyver-2.3.4/gyver/utils/lazy.py
--rw-r--r--   0        0        0     1319 2023-06-20 21:41:14.565536 gyver-2.3.4/gyver/utils/singleton.py
--rw-r--r--   0        0        0     2582 2023-07-11 14:06:07.748075 gyver-2.3.4/gyver/utils/strings.py
--rw-r--r--   0        0        0      134 2023-06-27 06:41:36.154386 gyver-2.3.4/gyver/utils/timezone.py
--rw-r--r--   0        0        0     2456 2023-07-14 20:30:45.881837 gyver-2.3.4/pyproject.toml
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 gyver-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-18 19:49:51.064698 gyver-2.4.0/LICENSE
+-rw-r--r--   0        0        0     1005 2023-07-18 19:49:51.064698 gyver-2.4.0/README.md
+-rw-r--r--   0        0        0      158 2023-07-21 13:13:04.112911 gyver-2.4.0/gyver/__init__.py
+-rw-r--r--   0        0        0      359 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/cache/__init__.py
+-rw-r--r--   0        0        0     1201 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/cache/asyncio.py
+-rw-r--r--   0        0        0      237 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/cache/config.py
+-rw-r--r--   0        0        0     1776 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/cache/interface.py
+-rw-r--r--   0        0        0     1395 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/cache/mapper.py
+-rw-r--r--   0        0        0     5993 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/cache/mock.py
+-rw-r--r--   0        0        0     4283 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/cache/redis.py
+-rw-r--r--   0        0        0     1128 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/cache/sync.py
+-rw-r--r--   0        0        0      558 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/cache/utils.py
+-rw-r--r--   0        0        0      597 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/config/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/config/adapter/__init__.py
+-rw-r--r--   0        0        0     1320 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/config/adapter/attrs.py
+-rw-r--r--   0        0        0     1078 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/config/adapter/dataclass.py
+-rw-r--r--   0        0        0     5940 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/config/adapter/factory.py
+-rw-r--r--   0        0        0     1056 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/config/adapter/gattrs.py
+-rw-r--r--   0        0        0     2107 2023-07-18 19:49:51.064698 gyver-2.4.0/gyver/config/adapter/interface.py
+-rw-r--r--   0        0        0     1701 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/config/adapter/mark.py
+-rw-r--r--   0        0        0     1091 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/config/adapter/pydantic.py
+-rw-r--r--   0        0        0     3459 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/config/config.py
+-rw-r--r--   0        0        0     2933 2023-07-21 13:09:14.825356 gyver-2.4.0/gyver/config/envconfig.py
+-rw-r--r--   0        0        0     1016 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/config/interface.py
+-rw-r--r--   0        0        0     5534 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/config/lazy.py
+-rw-r--r--   0        0        0      627 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/config/typedef.py
+-rw-r--r--   0        0        0      473 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/config/utils.py
+-rw-r--r--   0        0        0      419 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/context/__init__.py
+-rw-r--r--   0        0        0      288 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/context/atomic_/__init__.py
+-rw-r--r--   0        0        0     2317 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/context/atomic_/bound.py
+-rw-r--r--   0        0        0     2493 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/context/atomic_/core.py
+-rw-r--r--   0        0        0     1332 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/context/atomic_/resolver.py
+-rw-r--r--   0        0        0     5659 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/context/context.py
+-rw-r--r--   0        0        0      102 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/context/interfaces/__init__.py
+-rw-r--r--   0        0        0     1525 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/context/interfaces/adapter.py
+-rw-r--r--   0        0        0       39 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/context/typedef.py
+-rw-r--r--   0        0        0      253 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/crypto/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/crypto/config.py
+-rw-r--r--   0        0        0      909 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/crypto/fernet.py
+-rw-r--r--   0        0        0     1856 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/crypto/rsa.py
+-rw-r--r--   0        0        0      749 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/__init__.py
+-rw-r--r--   0        0        0     2136 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/adapter.py
+-rw-r--r--   0        0        0     1233 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/config.py
+-rw-r--r--   0        0        0      360 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/context/__init__.py
+-rw-r--r--   0        0        0     3542 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/context/asyncio.py
+-rw-r--r--   0        0        0     3349 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/context/sync.py
+-rw-r--r--   0        0        0      170 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/drivers/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/drivers/dialect.py
+-rw-r--r--   0        0        0      224 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/drivers/interface.py
+-rw-r--r--   0        0        0     1493 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/drivers/utils.py
+-rw-r--r--   0        0        0     1076 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/entity.py
+-rw-r--r--   0        0        0      498 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/entity.pyi
+-rw-r--r--   0        0        0       50 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/metadata.py
+-rw-r--r--   0        0        0     1012 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/__init__.py
+-rw-r--r--   0        0        0     1692 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/_helpers.py
+-rw-r--r--   0        0        0     2935 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/comp.py
+-rw-r--r--   0        0        0      294 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/exc.py
+-rw-r--r--   0        0        0     1220 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/interface.py
+-rw-r--r--   0        0        0      279 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/null.py
+-rw-r--r--   0        0        0     1270 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/order_by.py
+-rw-r--r--   0        0        0     1239 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/paginate.py
+-rw-r--r--   0        0        0      697 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/utils.py
+-rw-r--r--   0        0        0     4613 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/query/where.py
+-rw-r--r--   0        0        0      327 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/typedef.py
+-rw-r--r--   0        0        0     4243 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/database/utils.py
+-rw-r--r--   0        0        0     2285 2023-07-21 13:16:39.102411 gyver-2.4.0/gyver/exc.py
+-rw-r--r--   0        0        0      225 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/filetree/__init__.py
+-rw-r--r--   0        0        0     1749 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/filetree/filetree.py
+-rw-r--r--   0        0        0      348 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/filetree/helpers.py
+-rw-r--r--   0        0        0     3248 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/filetree/interface.py
+-rw-r--r--   0        0        0     2502 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/filetree/typedef.py
+-rw-r--r--   0        0        0     2808 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/filetree/virtual.py
+-rw-r--r--   0        0        0      857 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/model.py
+-rw-r--r--   0        0        0      101 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/pools/__init__.py
+-rw-r--r--   0        0        0     5764 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/pools/asyncio.py
+-rw-r--r--   0        0        0     2225 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/pools/resource.py
+-rw-r--r--   0        0        0     3855 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/pools/thread.py
+-rw-r--r--   0        0        0        0 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/py.typed
+-rw-r--r--   0        0        0      186 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/url/__init__.py
+-rw-r--r--   0        0        0     4639 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/url/core.py
+-rw-r--r--   0        0        0      423 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/url/encode.py
+-rw-r--r--   0        0        0     1285 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/url/fragment.py
+-rw-r--r--   0        0        0     5566 2023-07-18 19:49:51.068698 gyver-2.4.0/gyver/url/netloc.py
+-rw-r--r--   0        0        0     4307 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/url/path.py
+-rw-r--r--   0        0        0     3636 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/url/query.py
+-rw-r--r--   0        0        0     1186 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/url/utils.py
+-rw-r--r--   0        0        0      726 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/utils/__init__.py
+-rw-r--r--   0        0        0      156 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/utils/exc.py
+-rw-r--r--   0        0        0     7836 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/utils/finder.py
+-rw-r--r--   0        0        0     4262 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/utils/helpers.py
+-rw-r--r--   0        0        0      174 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/utils/json.py
+-rw-r--r--   0        0        0     2574 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/utils/lazy.py
+-rw-r--r--   0        0        0     1319 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/utils/singleton.py
+-rw-r--r--   0        0        0     2582 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/utils/strings.py
+-rw-r--r--   0        0        0      134 2023-07-18 19:49:51.072698 gyver-2.4.0/gyver/utils/timezone.py
+-rw-r--r--   0        0        0     2456 2023-07-21 13:13:04.108911 gyver-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 gyver-2.4.0/PKG-INFO
```

### Comparing `gyver-2.3.4/LICENSE` & `gyver-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/README.md` & `gyver-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/cache/asyncio.py` & `gyver-2.4.0/gyver/cache/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/cache/interface.py` & `gyver-2.4.0/gyver/cache/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/cache/mapper.py` & `gyver-2.4.0/gyver/cache/mapper.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/cache/mock.py` & `gyver-2.4.0/gyver/cache/mock.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/cache/redis.py` & `gyver-2.4.0/gyver/cache/redis.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/cache/sync.py` & `gyver-2.4.0/gyver/cache/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/cache/utils.py` & `gyver-2.4.0/gyver/cache/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/__init__.py` & `gyver-2.4.0/gyver/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/adapter/attrs.py` & `gyver-2.4.0/gyver/config/adapter/attrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/adapter/dataclass.py` & `gyver-2.4.0/gyver/config/adapter/dataclass.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/adapter/factory.py` & `gyver-2.4.0/gyver/config/adapter/factory.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/adapter/gattrs.py` & `gyver-2.4.0/gyver/config/adapter/gattrs.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/adapter/interface.py` & `gyver-2.4.0/gyver/config/adapter/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/adapter/mark.py` & `gyver-2.4.0/gyver/config/adapter/mark.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/adapter/pydantic.py` & `gyver-2.4.0/gyver/config/adapter/pydantic.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/config.py` & `gyver-2.4.0/gyver/config/config.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/envconfig.py` & `gyver-2.4.0/gyver/config/envconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,30 +32,33 @@
     return False
 
 
 @define
 class EnvConfig(Config):
     mapping: EnvMapping = default_mapping
     env_var: str = "CONFIG_ENV"
+    env_cast: Callable[[str], Env] = Env
     dotfiles: Sequence[DotFile] = ()
     ignore_default_rule: Callable[[Env], bool] = default_rule
 
     def __init__(
         self,
         *dotfiles: DotFile,
         env_var: str = "CONFIG_ENV",
         mapping: EnvMapping = default_mapping,
-        ignore_default_rule: Callable[[Env], bool] = default_rule
+        ignore_default_rule: Callable[[Env], bool] = default_rule,
+        env_cast: Callable[[str], Env] = Env
     ) -> None:
         call_init(
             self,
             env_var=env_var,
             mapping=mapping,
             dotfiles=dotfiles,
             ignore_default_rule=ignore_default_rule,
+            env_cast=env_cast,
         )
 
     def __post_init__(self):
         if self.dotfile:
             EnvConfig.file_values.manual_set(
                 self, dict(self._read_file(self.dotfile.filename))
             )
```

### Comparing `gyver-2.3.4/gyver/config/interface.py` & `gyver-2.4.0/gyver/config/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/lazy.py` & `gyver-2.4.0/gyver/config/lazy.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/config/typedef.py` & `gyver-2.4.0/gyver/config/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/context/atomic_/bound.py` & `gyver-2.4.0/gyver/context/atomic_/bound.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/context/atomic_/core.py` & `gyver-2.4.0/gyver/context/atomic_/core.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/context/atomic_/resolver.py` & `gyver-2.4.0/gyver/context/atomic_/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/context/context.py` & `gyver-2.4.0/gyver/context/context.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/context/interfaces/adapter.py` & `gyver-2.4.0/gyver/context/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/crypto/fernet.py` & `gyver-2.4.0/gyver/crypto/fernet.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/crypto/rsa.py` & `gyver-2.4.0/gyver/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/__init__.py` & `gyver-2.4.0/gyver/database/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/adapter.py` & `gyver-2.4.0/gyver/database/adapter.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/config.py` & `gyver-2.4.0/gyver/database/config.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/context/asyncio.py` & `gyver-2.4.0/gyver/database/context/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/context/sync.py` & `gyver-2.4.0/gyver/database/context/sync.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/drivers/utils.py` & `gyver-2.4.0/gyver/database/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/entity.py` & `gyver-2.4.0/gyver/database/entity.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/query/__init__.py` & `gyver-2.4.0/gyver/database/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/query/_helpers.py` & `gyver-2.4.0/gyver/database/query/_helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/query/comp.py` & `gyver-2.4.0/gyver/database/query/comp.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/query/interface.py` & `gyver-2.4.0/gyver/database/query/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/query/order_by.py` & `gyver-2.4.0/gyver/database/query/order_by.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/query/paginate.py` & `gyver-2.4.0/gyver/database/query/paginate.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/query/utils.py` & `gyver-2.4.0/gyver/database/query/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/query/where.py` & `gyver-2.4.0/gyver/database/query/where.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/database/utils.py` & `gyver-2.4.0/gyver/database/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/exc.py` & `gyver-2.4.0/gyver/exc.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             return f"{self.message} ({len(self.exceptions)} sub-exception{suffix})"
 
         def __repr__(self) -> str:
             return f"{self.__class__.__name__}({self.message!r}, {self.exceptions!r})"
 
 else:
 
-    class ErrorGroup(GyverError, ExceptionGroup):
+    class ErrorGroup(GyverError, ExceptionGroup): # noqa: F821
         pass
 
 
 class FailedFileOperation(GyverError):
     """Exception raised when an error happened while interacting with a file"""
```

### Comparing `gyver-2.3.4/gyver/filetree/filetree.py` & `gyver-2.4.0/gyver/filetree/filetree.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/filetree/interface.py` & `gyver-2.4.0/gyver/filetree/interface.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/filetree/typedef.py` & `gyver-2.4.0/gyver/filetree/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/filetree/virtual.py` & `gyver-2.4.0/gyver/filetree/virtual.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/model.py` & `gyver-2.4.0/gyver/model.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/pools/asyncio.py` & `gyver-2.4.0/gyver/pools/asyncio.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/pools/resource.py` & `gyver-2.4.0/gyver/pools/resource.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/pools/thread.py` & `gyver-2.4.0/gyver/pools/thread.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/url/core.py` & `gyver-2.4.0/gyver/url/core.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/url/fragment.py` & `gyver-2.4.0/gyver/url/fragment.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/url/netloc.py` & `gyver-2.4.0/gyver/url/netloc.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/url/path.py` & `gyver-2.4.0/gyver/url/path.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/url/query.py` & `gyver-2.4.0/gyver/url/query.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/url/utils.py` & `gyver-2.4.0/gyver/url/utils.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/utils/__init__.py` & `gyver-2.4.0/gyver/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/utils/finder.py` & `gyver-2.4.0/gyver/utils/finder.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/utils/helpers.py` & `gyver-2.4.0/gyver/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/utils/lazy.py` & `gyver-2.4.0/gyver/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/utils/singleton.py` & `gyver-2.4.0/gyver/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/gyver/utils/strings.py` & `gyver-2.4.0/gyver/utils/strings.py`

 * *Files identical despite different names*

### Comparing `gyver-2.3.4/pyproject.toml` & `gyver-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver"
-version = "2.3.4"
+version = "2.4.0"
 description = "Toolbox for web development"
 authors = ["Gustavo Correa <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guscardvs/gyver"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gyver-2.3.4/PKG-INFO` & `gyver-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver
-Version: 2.3.4
+Version: 2.4.0
 Summary: Toolbox for web development
 Home-page: https://github.com/guscardvs/gyver
 Author: Gustavo Correa
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

