# Comparing `tmp/litestar-2.0.0b3.tar.gz` & `tmp/litestar-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar-2.0.0b3.tar", max compression
+gzip compressed data, was "litestar-2.0.0b4.tar", max compression
```

## Comparing `litestar-2.0.0b3.tar` & `litestar-2.0.0b4.tar`

### file list

```diff
@@ -1,312 +1,312 @@
--rw-r--r--   0        0        0     1092 2023-07-20 13:51:29.954681 litestar-2.0.0b3/LICENSE
--rw-r--r--   0        0        0    16756 2023-07-20 13:51:29.954681 litestar-2.0.0b3/docs/PYPI_README.md
--rw-r--r--   0        0        0      744 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/__init__.py
--rw-r--r--   0        0        0      228 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/__main__.py
--rw-r--r--   0        0        0       77 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     6395 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0      349 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7780 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5932 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1244 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1528 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_asgi/utils.py
--rw-r--r--   0        0        0       66 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3842 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4234 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    14983 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20484 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2808 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_layers/utils.py
--rw-r--r--   0        0        0     6165 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_multipart.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0     9202 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5536 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     1231 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0     9743 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/responses.py
--rw-r--r--   0        0        0       64 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     3250 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2250 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    24613 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0      524 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10909 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5220 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7664 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     1460 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_openapi/utils.py
--rw-r--r--   0        0        0     2396 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_parsers.py
--rw-r--r--   0        0        0      126 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_signature/__init__.py
--rw-r--r--   0        0        0    10095 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_signature/model.py
--rw-r--r--   0        0        0     2718 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/_signature/utils.py
--rw-r--r--   0        0        0    36944 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/app.py
--rw-r--r--   0        0        0     2200 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/background_tasks.py
--rw-r--r--   0        0        0      176 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     1300 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     2750 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     9395 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0    15702 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4647 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/channels/subscriber.py
--rw-r--r--   0        0        0      119 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/__init__.py
--rw-r--r--   0        0        0    12672 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/_utils.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0     6631 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2314 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2413 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0     2183 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    11706 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/app.py
--rw-r--r--   0        0        0     2742 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/compression.py
--rw-r--r--   0        0        0     5178 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/csrf.py
--rw-r--r--   0        0        0     2005 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/connection/__init__.py
--rw-r--r--   0        0        0    10791 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/connection/base.py
--rw-r--r--   0        0        0     7756 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/connection/request.py
--rw-r--r--   0        0        0    11530 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/connection/websocket.py
--rw-r--r--   0        0        0     1622 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/constants.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.982682 litestar-2.0.0b3/litestar/contrib/__init__.py
--rw-r--r--   0        0        0       85 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/attrs/__init__.py
--rw-r--r--   0        0        0     2096 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/attrs/attrs_schema_plugin.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4800 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4167 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     6408 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0     2557 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jinja.py
--rw-r--r--   0        0        0      521 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28722 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     4373 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     6953 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3983 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/mako.py
--rw-r--r--   0        0        0      683 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/msgspec.py
--rw-r--r--   0        0        0      180 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4235 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2214 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0     3168 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/piccolo.py
--rw-r--r--   0        0        0      207 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     2733 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/prometheus/config.py
--rw-r--r--   0        0        0     1646 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/prometheus/controller.py
--rw-r--r--   0        0        0     6873 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/prometheus/middleware.py
--rw-r--r--   0        0        0      808 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0     3011 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_dto_factory.py
--rw-r--r--   0        0        0     4571 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_init_plugin.py
--rw-r--r--   0        0        0     8802 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_schema_plugin.py
--rw-r--r--   0        0        0      364 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0      162 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/abc/__init__.py
--rw-r--r--   0        0        0     8889 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/abc/_async.py
--rw-r--r--   0        0        0     8907 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/abc/_sync.py
--rw-r--r--   0        0        0      328 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0     2064 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      641 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/testing/__init__.py
--rw-r--r--   0        0        0    25918 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5668 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0    11318 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      941 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      319 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/_slots_base.py
--rw-r--r--   0        0        0      504 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      458 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0     4541 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0    11423 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0    11483 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0     3753 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0     1647 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0     1505 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0      288 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/__init__.py
--rw-r--r--   0        0        0    28708 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_async.py
--rw-r--r--   0        0        0    28402 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_sync.py
--rw-r--r--   0        0        0     1033 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_util.py
--rw-r--r--   0        0        0      754 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/types.py
--rw-r--r--   0        0        0     6327 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0     9762 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/controller.py
--rw-r--r--   0        0        0    16456 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/data_extractors.py
--rw-r--r--   0        0        0      883 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3770 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    18809 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     2977 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9646 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/state.py
--rw-r--r--   0        0        0     2695 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7285 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/datastructures/url.py
--rw-r--r--   0        0        0     3117 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/di.py
--rw-r--r--   0        0        0      645 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/__init__.py
--rw-r--r--   0        0        0    21671 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/_backend.py
--rw-r--r--   0        0        0     4261 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/_types.py
--rw-r--r--   0        0        0    20517 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/_utils.py
--rw-r--r--   0        0        0     7288 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/base_factory.py
--rw-r--r--   0        0        0     2501 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/config.py
--rw-r--r--   0        0        0     4858 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/data_structures.py
--rw-r--r--   0        0        0     2507 2023-07-20 13:51:29.986682 litestar-2.0.0b3/litestar/dto/dataclass_dto_factory.py
--rw-r--r--   0        0        0     1325 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/factory/__init__.py
--rw-r--r--   0        0        0      701 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/factory/stdlib/dataclass.py
--rw-r--r--   0        0        0     1388 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/field.py
--rw-r--r--   0        0        0     4948 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/interface.py
--rw-r--r--   0        0        0     2113 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/msgspec_dto_factory.py
--rw-r--r--   0        0        0      516 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/dto/types.py
--rw-r--r--   0        0        0     1728 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/enums.py
--rw-r--r--   0        0        0      201 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/events/__init__.py
--rw-r--r--   0        0        0     4371 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/events/emitter.py
--rw-r--r--   0        0        0     1313 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/events/listener.py
--rw-r--r--   0        0        0     1302 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1721 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0      331 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/dto_exceptions.py
--rw-r--r--   0        0        0     4629 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5344 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/file_system.py
--rw-r--r--   0        0        0      559 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3868 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    21575 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     6450 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    26309 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    62224 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      340 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     7217 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    19092 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     3605 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/_utils.py
--rw-r--r--   0        0        0    12215 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/picologging.py
--rw-r--r--   0        0        0      860 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2079 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     3021 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3430 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5284 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/base.py
--rw-r--r--   0        0        0     8454 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/compression.py
--rw-r--r--   0        0        0     2554 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6438 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7141 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0     9435 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13307 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10817 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0       70 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     7941 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10352 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     8540 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      183 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5600 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/config.py
--rw-r--r--   0        0        0    15653 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/controller.py
--rw-r--r--   0        0        0      724 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1885 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2936 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      974 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      752 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4028 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6242 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2023-07-20 13:51:29.990682 litestar-2.0.0b3/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    34581 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0    11029 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/pagination.py
--rw-r--r--   0        0        0    15113 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/params.py
--rw-r--r--   0        0        0     7433 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/partial.py
--rw-r--r--   0        0        0     3923 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/plugins.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/py.typed
--rw-r--r--   0        0        0      208 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/__init__.py
--rw-r--r--   0        0        0    15238 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/base.py
--rw-r--r--   0        0        0    14298 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/file.py
--rw-r--r--   0        0        0     5440 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/redirect.py
--rw-r--r--   0        0        0     7956 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/streaming.py
--rw-r--r--   0        0        0     5229 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/response/template.py
--rw-r--r--   0        0        0    15308 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/router.py
--rw-r--r--   0        0        0      191 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1719 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6788 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/base.py
--rw-r--r--   0        0        0    13224 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/http.py
--rw-r--r--   0        0        0     3002 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/__init__.py
--rw-r--r--   0        0        0     7165 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/base.py
--rw-r--r--   0        0        0      188 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5602 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     4956 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0      348 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/serialization/__init__.py
--rw-r--r--   0        0        0      277 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/serialization/_msgspec_utils.py
--rw-r--r--   0        0        0     7755 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/serialization/msgspec_hooks.py
--rw-r--r--   0        0        0      158 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5046 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/static_files/base.py
--rw-r--r--   0        0        0     3598 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/static_files/config.py
--rw-r--r--   0        0        0     9536 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/status_codes.py
--rw-r--r--   0        0        0        0 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4396 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/base.py
--rw-r--r--   0        0        0     5430 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/file.py
--rw-r--r--   0        0        0     3625 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/memory.py
--rw-r--r--   0        0        0     6208 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/redis.py
--rw-r--r--   0        0        0     2216 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/template/__init__.py
--rw-r--r--   0        0        0     4083 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/template/base.py
--rw-r--r--   0        0        0     1894 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/template/config.py
--rw-r--r--   0        0        0      581 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17562 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     5145 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19671 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0    29713 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2540 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    22456 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     8056 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/transport.py
--rw-r--r--   0        0        0     8564 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4171 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/__init__.py
--rw-r--r--   0        0        0     8937 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      566 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2962 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1782 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/composite_types.py
--rw-r--r--   0        0        0      286 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/empty.py
--rw-r--r--   0        0        0     2635 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/file_types.py
--rw-r--r--   0        0        0      918 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1751 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2984 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/protocols.py
--rw-r--r--   0        0        0     2039 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/types/serialization.py
--rw-r--r--   0        0        0    20917 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/typing.py
--rw-r--r--   0        0        0     2167 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/compat.py
--rw-r--r--   0        0        0     3763 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3553 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/deprecation.py
--rw-r--r--   0        0        0     3334 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/helpers.py
--rw-r--r--   0        0        0      723 2023-07-20 13:51:29.994682 litestar-2.0.0b3/litestar/utils/path.py
--rw-r--r--   0        0        0    12498 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/predicates.py
--rw-r--r--   0        0        0     2789 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/scope.py
--rw-r--r--   0        0        0      983 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/sequence.py
--rw-r--r--   0        0        0     5521 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/signature.py
--rw-r--r--   0        0        0     4374 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/sync.py
--rw-r--r--   0        0        0     8299 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/typing.py
--rw-r--r--   0        0        0     1921 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/version.py
--rw-r--r--   0        0        0     1992 2023-07-20 13:51:29.998682 litestar-2.0.0b3/litestar/utils/warnings.py
--rw-r--r--   0        0        0    14275 2023-07-20 13:51:29.998682 litestar-2.0.0b3/pyproject.toml
--rw-r--r--   0        0        0    21325 1970-01-01 00:00:00.000000 litestar-2.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-21 15:49:23.812703 litestar-2.0.0b4/LICENSE
+-rw-r--r--   0        0        0    16790 2023-07-21 15:49:23.816703 litestar-2.0.0b4/docs/PYPI_README.md
+-rw-r--r--   0        0        0      744 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/__main__.py
+-rw-r--r--   0        0        0       77 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     6395 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7780 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5932 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1244 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3842 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4234 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    14983 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20484 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2808 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_layers/utils.py
+-rw-r--r--   0        0        0     6165 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_multipart.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0     9202 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     5536 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     1231 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0     9743 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     3250 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2250 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    24613 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0      524 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10909 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5220 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7664 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1460 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0     2396 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_parsers.py
+-rw-r--r--   0        0        0      126 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0    10095 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_signature/model.py
+-rw-r--r--   0        0        0     2718 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/_signature/utils.py
+-rw-r--r--   0        0        0    36944 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/app.py
+-rw-r--r--   0        0        0     2200 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/background_tasks.py
+-rw-r--r--   0        0        0      176 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     1300 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     2750 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     9395 2023-07-21 15:49:23.840704 litestar-2.0.0b4/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0    15702 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4647 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0      119 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    12672 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6631 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2314 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2413 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0     2183 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    11706 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/app.py
+-rw-r--r--   0        0        0     2742 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/compression.py
+-rw-r--r--   0        0        0     5178 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/csrf.py
+-rw-r--r--   0        0        0     2005 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    10791 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/connection/base.py
+-rw-r--r--   0        0        0     7756 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/connection/request.py
+-rw-r--r--   0        0        0    11530 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/connection/websocket.py
+-rw-r--r--   0        0        0     1622 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/constants.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/attrs/__init__.py
+-rw-r--r--   0        0        0     2096 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/attrs/attrs_schema_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4800 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4167 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     6408 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2557 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28722 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     4373 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6953 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3983 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/mako.py
+-rw-r--r--   0        0        0      683 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/msgspec.py
+-rw-r--r--   0        0        0      180 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4235 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2214 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     3168 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/piccolo.py
+-rw-r--r--   0        0        0      207 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     2733 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/prometheus/config.py
+-rw-r--r--   0        0        0     1646 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/prometheus/controller.py
+-rw-r--r--   0        0        0     6873 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/prometheus/middleware.py
+-rw-r--r--   0        0        0      808 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0     3011 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_dto_factory.py
+-rw-r--r--   0        0        0     4571 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_init_plugin.py
+-rw-r--r--   0        0        0     8802 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_schema_plugin.py
+-rw-r--r--   0        0        0      364 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0      162 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/abc/__init__.py
+-rw-r--r--   0        0        0     8889 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/abc/_async.py
+-rw-r--r--   0        0        0     8907 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/abc/_sync.py
+-rw-r--r--   0        0        0      328 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     2064 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      641 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    25918 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5668 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0    11308 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      941 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      319 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/_slots_base.py
+-rw-r--r--   0        0        0      504 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      458 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     4541 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0    11418 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0    11483 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     3753 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0     1647 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0     1505 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0      288 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/__init__.py
+-rw-r--r--   0        0        0    28708 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_async.py
+-rw-r--r--   0        0        0    28402 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_sync.py
+-rw-r--r--   0        0        0     1033 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_util.py
+-rw-r--r--   0        0        0      754 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/types.py
+-rw-r--r--   0        0        0     6327 2023-07-21 15:49:23.844704 litestar-2.0.0b4/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0     9762 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/controller.py
+-rw-r--r--   0        0        0    16456 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/data_extractors.py
+-rw-r--r--   0        0        0      883 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3770 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    18809 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9646 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     2695 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7285 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/datastructures/url.py
+-rw-r--r--   0        0        0     3117 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/di.py
+-rw-r--r--   0        0        0      645 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/__init__.py
+-rw-r--r--   0        0        0    21671 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/_backend.py
+-rw-r--r--   0        0        0     4261 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/_types.py
+-rw-r--r--   0        0        0    20517 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/_utils.py
+-rw-r--r--   0        0        0     7288 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/base_factory.py
+-rw-r--r--   0        0        0     2501 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/config.py
+-rw-r--r--   0        0        0     4858 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/data_structures.py
+-rw-r--r--   0        0        0     2507 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/dataclass_dto_factory.py
+-rw-r--r--   0        0        0     1325 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/factory/__init__.py
+-rw-r--r--   0        0        0      701 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/factory/stdlib/dataclass.py
+-rw-r--r--   0        0        0     1388 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/field.py
+-rw-r--r--   0        0        0     4948 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/interface.py
+-rw-r--r--   0        0        0     2113 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/msgspec_dto_factory.py
+-rw-r--r--   0        0        0      516 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/dto/types.py
+-rw-r--r--   0        0        0     1728 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/enums.py
+-rw-r--r--   0        0        0      201 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4371 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/events/emitter.py
+-rw-r--r--   0        0        0     1313 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/events/listener.py
+-rw-r--r--   0        0        0     1302 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1721 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0      331 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/dto_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5344 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/file_system.py
+-rw-r--r--   0        0        0      559 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3868 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    21575 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     6450 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    26309 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    62224 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      340 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     7217 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    19092 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     3605 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    12215 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2079 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     3021 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3430 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5284 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/base.py
+-rw-r--r--   0        0        0     8454 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/compression.py
+-rw-r--r--   0        0        0     2554 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6438 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7141 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     9435 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13307 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10817 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7941 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10352 2023-07-21 15:49:23.848704 litestar-2.0.0b4/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8540 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      183 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0     5600 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/config.py
+-rw-r--r--   0        0        0    15653 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      724 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1885 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4028 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34581 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0    11029 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/pagination.py
+-rw-r--r--   0        0        0    15113 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/params.py
+-rw-r--r--   0        0        0     7433 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/partial.py
+-rw-r--r--   0        0        0     3923 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/plugins.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/py.typed
+-rw-r--r--   0        0        0      208 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/__init__.py
+-rw-r--r--   0        0        0    15238 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/base.py
+-rw-r--r--   0        0        0    14298 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/file.py
+-rw-r--r--   0        0        0     5440 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/redirect.py
+-rw-r--r--   0        0        0     7956 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/streaming.py
+-rw-r--r--   0        0        0     5229 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/response/template.py
+-rw-r--r--   0        0        0    15308 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/router.py
+-rw-r--r--   0        0        0      191 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1719 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6788 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/base.py
+-rw-r--r--   0        0        0    13224 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/http.py
+-rw-r--r--   0        0        0     3002 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/base.py
+-rw-r--r--   0        0        0      188 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4956 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0      348 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/serialization/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/serialization/_msgspec_utils.py
+-rw-r--r--   0        0        0     7755 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/serialization/msgspec_hooks.py
+-rw-r--r--   0        0        0      158 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5046 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/static_files/base.py
+-rw-r--r--   0        0        0     3598 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/static_files/config.py
+-rw-r--r--   0        0        0     9536 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/status_codes.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4396 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/base.py
+-rw-r--r--   0        0        0     5430 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/memory.py
+-rw-r--r--   0        0        0     6208 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2216 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/template/__init__.py
+-rw-r--r--   0        0        0     4083 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/template/base.py
+-rw-r--r--   0        0        0     1894 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17562 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     5145 2023-07-21 15:49:23.852704 litestar-2.0.0b4/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19671 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0    29713 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2540 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    22456 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     8056 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8564 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4171 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8937 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      566 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2962 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1782 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      286 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/empty.py
+-rw-r--r--   0        0        0     2635 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/file_types.py
+-rw-r--r--   0        0        0      918 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1751 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2984 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/protocols.py
+-rw-r--r--   0        0        0     2039 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/types/serialization.py
+-rw-r--r--   0        0        0    20917 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/typing.py
+-rw-r--r--   0        0        0     2167 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3763 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3553 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     3334 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/path.py
+-rw-r--r--   0        0        0    12498 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/predicates.py
+-rw-r--r--   0        0        0     2789 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/scope.py
+-rw-r--r--   0        0        0      983 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/sequence.py
+-rw-r--r--   0        0        0     5521 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/signature.py
+-rw-r--r--   0        0        0     4374 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/sync.py
+-rw-r--r--   0        0        0     8299 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1921 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/version.py
+-rw-r--r--   0        0        0     1992 2023-07-21 15:49:23.856704 litestar-2.0.0b4/litestar/utils/warnings.py
+-rw-r--r--   0        0        0    13677 2023-07-21 15:49:23.856704 litestar-2.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0    21540 1970-01-01 00:00:00.000000 litestar-2.0.0b4/PKG-INFO
```

### Comparing `litestar-2.0.0b3/LICENSE` & `litestar-2.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/docs/PYPI_README.md` & `litestar-2.0.0b4/docs/PYPI_README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the latest pre-release version by instead running
 
 ```shell
-pip install litestar==2.0.0beta2
+pip install litestar==2.0.0beta3
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
 
@@ -174,15 +174,15 @@
 
 Litestar also supports the programmatic creation of DTOs with a `DTOFactory` class, which also supports the use of
 plugins.
 
 ### OpenAPI
 
 Litestar has custom logic to generate OpenAPI 3.1.0 schema, include optional generation of examples using the
-`pydantic-factories` library.
+[`polyfactory`](https://pypi.org/project/polyfactory/) library.
 
 #### ReDoc, Swagger-UI and Stoplight Elements API Documentation
 
 Litestar serves the documentation from the generated OpenAPI schema with:
 
 - [ReDoc](https://redoc.ly/)
 - [Swagger-UI](https://swagger.io/tools/swagger-ui/)
```

### Comparing `litestar-2.0.0b3/litestar/__init__.py` & `litestar-2.0.0b4/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_asgi/asgi_router.py` & `litestar-2.0.0b4/litestar/_asgi/asgi_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.0.0b4/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.0.0b4/litestar/_asgi/routing_trie/traversal.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_asgi/routing_trie/types.py` & `litestar-2.0.0b4/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_asgi/routing_trie/validate.py` & `litestar-2.0.0b4/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_asgi/utils.py` & `litestar-2.0.0b4/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_kwargs/cleanup.py` & `litestar-2.0.0b4/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_kwargs/dependencies.py` & `litestar-2.0.0b4/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_kwargs/extractors.py` & `litestar-2.0.0b4/litestar/_kwargs/extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_kwargs/kwargs_model.py` & `litestar-2.0.0b4/litestar/_kwargs/kwargs_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_kwargs/parameter_definition.py` & `litestar-2.0.0b4/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_layers/utils.py` & `litestar-2.0.0b4/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_multipart.py` & `litestar-2.0.0b4/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/parameters.py` & `litestar-2.0.0b4/litestar/_openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/path_item.py` & `litestar-2.0.0b4/litestar/_openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/request_body.py` & `litestar-2.0.0b4/litestar/_openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/responses.py` & `litestar-2.0.0b4/litestar/_openapi/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.0.0b4/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/schema_generation/examples.py` & `litestar-2.0.0b4/litestar/_openapi/schema_generation/examples.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/schema_generation/schema.py` & `litestar-2.0.0b4/litestar/_openapi/schema_generation/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/schema_generation/utils.py` & `litestar-2.0.0b4/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.0.0b4/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.0.0b4/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/typescript_converter/types.py` & `litestar-2.0.0b4/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_openapi/utils.py` & `litestar-2.0.0b4/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_parsers.py` & `litestar-2.0.0b4/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_signature/model.py` & `litestar-2.0.0b4/litestar/_signature/model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/_signature/utils.py` & `litestar-2.0.0b4/litestar/_signature/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/app.py` & `litestar-2.0.0b4/litestar/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/background_tasks.py` & `litestar-2.0.0b4/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/channels/backends/base.py` & `litestar-2.0.0b4/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/channels/backends/memory.py` & `litestar-2.0.0b4/litestar/channels/backends/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/channels/backends/redis.py` & `litestar-2.0.0b4/litestar/channels/backends/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/channels/plugin.py` & `litestar-2.0.0b4/litestar/channels/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/channels/subscriber.py` & `litestar-2.0.0b4/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/cli/_utils.py` & `litestar-2.0.0b4/litestar/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/cli/commands/core.py` & `litestar-2.0.0b4/litestar/cli/commands/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/cli/commands/schema.py` & `litestar-2.0.0b4/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/cli/commands/sessions.py` & `litestar-2.0.0b4/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/cli/main.py` & `litestar-2.0.0b4/litestar/cli/main.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/config/allowed_hosts.py` & `litestar-2.0.0b4/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/config/app.py` & `litestar-2.0.0b4/litestar/config/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/config/compression.py` & `litestar-2.0.0b4/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/config/cors.py` & `litestar-2.0.0b4/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/config/csrf.py` & `litestar-2.0.0b4/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/config/response_cache.py` & `litestar-2.0.0b4/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/connection/__init__.py` & `litestar-2.0.0b4/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/connection/base.py` & `litestar-2.0.0b4/litestar/connection/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/connection/request.py` & `litestar-2.0.0b4/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/connection/websocket.py` & `litestar-2.0.0b4/litestar/connection/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/constants.py` & `litestar-2.0.0b4/litestar/constants.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/attrs/attrs_schema_plugin.py` & `litestar-2.0.0b4/litestar/contrib/attrs/attrs_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/htmx/_utils.py` & `litestar-2.0.0b4/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/htmx/request.py` & `litestar-2.0.0b4/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/htmx/response.py` & `litestar-2.0.0b4/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/htmx/types.py` & `litestar-2.0.0b4/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/jinja.py` & `litestar-2.0.0b4/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/jwt/__init__.py` & `litestar-2.0.0b4/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/jwt/jwt_auth.py` & `litestar-2.0.0b4/litestar/contrib/jwt/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/jwt/jwt_token.py` & `litestar-2.0.0b4/litestar/contrib/jwt/jwt_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/jwt/middleware.py` & `litestar-2.0.0b4/litestar/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/mako.py` & `litestar-2.0.0b4/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/msgspec.py` & `litestar-2.0.0b4/litestar/contrib/msgspec.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.0.0b4/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/opentelemetry/config.py` & `litestar-2.0.0b4/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.0.0b4/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/piccolo.py` & `litestar-2.0.0b4/litestar/contrib/piccolo.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/prometheus/config.py` & `litestar-2.0.0b4/litestar/contrib/prometheus/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/prometheus/controller.py` & `litestar-2.0.0b4/litestar/contrib/prometheus/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/prometheus/middleware.py` & `litestar-2.0.0b4/litestar/contrib/prometheus/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/pydantic/__init__.py` & `litestar-2.0.0b4/litestar/contrib/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_dto_factory.py` & `litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_dto_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_init_plugin.py` & `litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_init_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/pydantic/pydantic_schema_plugin.py` & `litestar-2.0.0b4/litestar/contrib/pydantic/pydantic_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/repository/abc/_async.py` & `litestar-2.0.0b4/litestar/contrib/repository/abc/_async.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/repository/abc/_sync.py` & `litestar-2.0.0b4/litestar/contrib/repository/abc/_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/repository/filters.py` & `litestar-2.0.0b4/litestar/contrib/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/repository/handlers.py` & `litestar-2.0.0b4/litestar/contrib/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/repository/testing/generic_mock_repository.py` & `litestar-2.0.0b4/litestar/contrib/repository/testing/generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/base.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/dto.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     from typing_extensions import TypeAlias
 
 __all__ = ("SQLAlchemyDTO",)
 
 T = TypeVar("T", bound="DeclarativeBase | Collection[DeclarativeBase]")
 
-ElementType: TypeAlias = "Column[Any] | RelationshipProperty[Any]"
+ElementType: TypeAlias = "Column | RelationshipProperty"
 SQLA_NS = {**vars(orm), **vars(sql)}
 
 
 class SQLAlchemyDTO(AbstractDTOFactory[T], Generic[T]):
     """Support for domain modelling with SQLAlchemy."""
 
     __slots__ = ()
```

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/common.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """Automatically start transactions when database access is requested by an operation."""
     autoflush: bool | EmptyType = Empty
     """When ``True``, all query operations will issue a flush call to this :class:`Session <sqlalchemy.orm.Session>`
     before proceeding"""
     bind: EngineT | ConnectionT | None | EmptyType = Empty
     """The :class:`Engine <sqlalchemy.engine.Engine>` or :class:`Connection <sqlalchemy.engine.Connection>` that new
     :class:`Session <sqlalchemy.orm.Session>` objects will be bound to."""
-    binds: dict[type[Any] | Mapper[Any] | TableClause | str, EngineT | ConnectionT] | None | EmptyType = Empty
+    binds: dict[type[Any] | Mapper | TableClause | str, EngineT | ConnectionT] | None | EmptyType = Empty
     """A dictionary which may specify any number of :class:`Engine <sqlalchemy.engine.Engine>` or :class:`Connection
     <sqlalchemy.engine.Connection>` objects as the source of connectivity for SQL operations on a per-entity basis. The
     keys of the dictionary consist of any series of mapped classes, arbitrary Python classes that are bases for mapped
     classes, :class:`Table <sqlalchemy.schema.Table>` objects and :class:`Mapper <sqlalchemy.orm.Mapper>` objects. The
     values of the dictionary are then instances of :class:`Engine <sqlalchemy.engine.Engine>` or less commonly
     :class:`Connection <sqlalchemy.engine.Connection>` objects."""
     class_: type[SessionT] | EmptyType = Empty
```

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/engine.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/engine.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/init/plugin.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/init/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/plugins/serialization.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/plugins/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_async.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_async.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_sync.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/_util.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/_util.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/repository/types.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/repository/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/contrib/sqlalchemy/types.py` & `litestar-2.0.0b4/litestar/contrib/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/controller.py` & `litestar-2.0.0b4/litestar/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/data_extractors.py` & `litestar-2.0.0b4/litestar/data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/datastructures/__init__.py` & `litestar-2.0.0b4/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/datastructures/cookie.py` & `litestar-2.0.0b4/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/datastructures/headers.py` & `litestar-2.0.0b4/litestar/datastructures/headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/datastructures/multi_dicts.py` & `litestar-2.0.0b4/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/datastructures/response_header.py` & `litestar-2.0.0b4/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/datastructures/state.py` & `litestar-2.0.0b4/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/datastructures/upload_file.py` & `litestar-2.0.0b4/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/datastructures/url.py` & `litestar-2.0.0b4/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/di.py` & `litestar-2.0.0b4/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/__init__.py` & `litestar-2.0.0b4/litestar/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/_backend.py` & `litestar-2.0.0b4/litestar/dto/_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/_types.py` & `litestar-2.0.0b4/litestar/dto/_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/_utils.py` & `litestar-2.0.0b4/litestar/dto/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/base_factory.py` & `litestar-2.0.0b4/litestar/dto/base_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/config.py` & `litestar-2.0.0b4/litestar/dto/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/data_structures.py` & `litestar-2.0.0b4/litestar/dto/data_structures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/dataclass_dto_factory.py` & `litestar-2.0.0b4/litestar/dto/dataclass_dto_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/factory/__init__.py` & `litestar-2.0.0b4/litestar/dto/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/factory/stdlib/dataclass.py` & `litestar-2.0.0b4/litestar/dto/factory/stdlib/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/field.py` & `litestar-2.0.0b4/litestar/dto/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/interface.py` & `litestar-2.0.0b4/litestar/dto/interface.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/msgspec_dto_factory.py` & `litestar-2.0.0b4/litestar/dto/msgspec_dto_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/dto/types.py` & `litestar-2.0.0b4/litestar/dto/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/enums.py` & `litestar-2.0.0b4/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/events/emitter.py` & `litestar-2.0.0b4/litestar/events/emitter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/events/listener.py` & `litestar-2.0.0b4/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/exceptions/__init__.py` & `litestar-2.0.0b4/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/exceptions/base_exceptions.py` & `litestar-2.0.0b4/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/exceptions/http_exceptions.py` & `litestar-2.0.0b4/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/exceptions/websocket_exceptions.py` & `litestar-2.0.0b4/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/file_system.py` & `litestar-2.0.0b4/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/handlers/__init__.py` & `litestar-2.0.0b4/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/handlers/asgi_handlers.py` & `litestar-2.0.0b4/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/handlers/base.py` & `litestar-2.0.0b4/litestar/handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/handlers/http_handlers/_utils.py` & `litestar-2.0.0b4/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/handlers/http_handlers/base.py` & `litestar-2.0.0b4/litestar/handlers/http_handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/handlers/http_handlers/decorators.py` & `litestar-2.0.0b4/litestar/handlers/http_handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.0.0b4/litestar/handlers/websocket_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.0.0b4/litestar/handlers/websocket_handlers/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.0.0b4/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/logging/_utils.py` & `litestar-2.0.0b4/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/logging/config.py` & `litestar-2.0.0b4/litestar/logging/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/logging/picologging.py` & `litestar-2.0.0b4/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/logging/standard.py` & `litestar-2.0.0b4/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/_utils.py` & `litestar-2.0.0b4/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/allowed_hosts.py` & `litestar-2.0.0b4/litestar/middleware/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/authentication.py` & `litestar-2.0.0b4/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/base.py` & `litestar-2.0.0b4/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/compression.py` & `litestar-2.0.0b4/litestar/middleware/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/cors.py` & `litestar-2.0.0b4/litestar/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/csrf.py` & `litestar-2.0.0b4/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.0.0b4/litestar/middleware/exceptions/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/exceptions/middleware.py` & `litestar-2.0.0b4/litestar/middleware/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.0.0b4/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.0.0b4/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/logging.py` & `litestar-2.0.0b4/litestar/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/rate_limit.py` & `litestar-2.0.0b4/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/session/base.py` & `litestar-2.0.0b4/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/session/client_side.py` & `litestar-2.0.0b4/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/middleware/session/server_side.py` & `litestar-2.0.0b4/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/config.py` & `litestar-2.0.0b4/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/controller.py` & `litestar-2.0.0b4/litestar/openapi/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/datastructures.py` & `litestar-2.0.0b4/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/__init__.py` & `litestar-2.0.0b4/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/base.py` & `litestar-2.0.0b4/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/callback.py` & `litestar-2.0.0b4/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/components.py` & `litestar-2.0.0b4/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/contact.py` & `litestar-2.0.0b4/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/discriminator.py` & `litestar-2.0.0b4/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/encoding.py` & `litestar-2.0.0b4/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/enums.py` & `litestar-2.0.0b4/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/example.py` & `litestar-2.0.0b4/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/external_documentation.py` & `litestar-2.0.0b4/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/header.py` & `litestar-2.0.0b4/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/info.py` & `litestar-2.0.0b4/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/license.py` & `litestar-2.0.0b4/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/link.py` & `litestar-2.0.0b4/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/media_type.py` & `litestar-2.0.0b4/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/oauth_flow.py` & `litestar-2.0.0b4/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/oauth_flows.py` & `litestar-2.0.0b4/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/open_api.py` & `litestar-2.0.0b4/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/operation.py` & `litestar-2.0.0b4/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/parameter.py` & `litestar-2.0.0b4/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/path_item.py` & `litestar-2.0.0b4/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/paths.py` & `litestar-2.0.0b4/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/reference.py` & `litestar-2.0.0b4/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/request_body.py` & `litestar-2.0.0b4/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/response.py` & `litestar-2.0.0b4/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/responses.py` & `litestar-2.0.0b4/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/schema.py` & `litestar-2.0.0b4/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/security_requirement.py` & `litestar-2.0.0b4/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/security_scheme.py` & `litestar-2.0.0b4/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/server.py` & `litestar-2.0.0b4/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/server_variable.py` & `litestar-2.0.0b4/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/tag.py` & `litestar-2.0.0b4/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/openapi/spec/xml.py` & `litestar-2.0.0b4/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/pagination.py` & `litestar-2.0.0b4/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/params.py` & `litestar-2.0.0b4/litestar/params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/partial.py` & `litestar-2.0.0b4/litestar/partial.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/plugins.py` & `litestar-2.0.0b4/litestar/plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/response/base.py` & `litestar-2.0.0b4/litestar/response/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/response/file.py` & `litestar-2.0.0b4/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/response/redirect.py` & `litestar-2.0.0b4/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/response/streaming.py` & `litestar-2.0.0b4/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/response/template.py` & `litestar-2.0.0b4/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/router.py` & `litestar-2.0.0b4/litestar/router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/routes/asgi.py` & `litestar-2.0.0b4/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/routes/base.py` & `litestar-2.0.0b4/litestar/routes/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/routes/http.py` & `litestar-2.0.0b4/litestar/routes/http.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/routes/websocket.py` & `litestar-2.0.0b4/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/security/base.py` & `litestar-2.0.0b4/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/security/session_auth/auth.py` & `litestar-2.0.0b4/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/security/session_auth/middleware.py` & `litestar-2.0.0b4/litestar/security/session_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/serialization/msgspec_hooks.py` & `litestar-2.0.0b4/litestar/serialization/msgspec_hooks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/static_files/base.py` & `litestar-2.0.0b4/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/static_files/config.py` & `litestar-2.0.0b4/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/status_codes.py` & `litestar-2.0.0b4/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/stores/base.py` & `litestar-2.0.0b4/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/stores/file.py` & `litestar-2.0.0b4/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/stores/memory.py` & `litestar-2.0.0b4/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/stores/redis.py` & `litestar-2.0.0b4/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/stores/registry.py` & `litestar-2.0.0b4/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/template/base.py` & `litestar-2.0.0b4/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/template/config.py` & `litestar-2.0.0b4/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/__init__.py` & `litestar-2.0.0b4/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/client/__init__.py` & `litestar-2.0.0b4/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/client/async_client.py` & `litestar-2.0.0b4/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/client/base.py` & `litestar-2.0.0b4/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/client/sync_client.py` & `litestar-2.0.0b4/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/helpers.py` & `litestar-2.0.0b4/litestar/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/life_span_handler.py` & `litestar-2.0.0b4/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/request_factory.py` & `litestar-2.0.0b4/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/transport.py` & `litestar-2.0.0b4/litestar/testing/transport.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/testing/websocket_test_session.py` & `litestar-2.0.0b4/litestar/testing/websocket_test_session.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/__init__.py` & `litestar-2.0.0b4/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/asgi_types.py` & `litestar-2.0.0b4/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/builtin_types.py` & `litestar-2.0.0b4/litestar/types/builtin_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/callable_types.py` & `litestar-2.0.0b4/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/composite_types.py` & `litestar-2.0.0b4/litestar/types/composite_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/file_types.py` & `litestar-2.0.0b4/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/helper_types.py` & `litestar-2.0.0b4/litestar/types/helper_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/internal_types.py` & `litestar-2.0.0b4/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/protocols.py` & `litestar-2.0.0b4/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/types/serialization.py` & `litestar-2.0.0b4/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/typing.py` & `litestar-2.0.0b4/litestar/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/__init__.py` & `litestar-2.0.0b4/litestar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/compat.py` & `litestar-2.0.0b4/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/dataclass.py` & `litestar-2.0.0b4/litestar/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/deprecation.py` & `litestar-2.0.0b4/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/helpers.py` & `litestar-2.0.0b4/litestar/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/path.py` & `litestar-2.0.0b4/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/predicates.py` & `litestar-2.0.0b4/litestar/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/scope.py` & `litestar-2.0.0b4/litestar/utils/scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/sequence.py` & `litestar-2.0.0b4/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/signature.py` & `litestar-2.0.0b4/litestar/utils/signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/sync.py` & `litestar-2.0.0b4/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/typing.py` & `litestar-2.0.0b4/litestar/utils/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/version.py` & `litestar-2.0.0b4/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/litestar/utils/warnings.py` & `litestar-2.0.0b4/litestar/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b3/pyproject.toml` & `litestar-2.0.0b4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litestar"
-version = "2.0.0beta3"
+version = "2.0.0beta4"
 description = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
@@ -89,140 +89,122 @@
 jsbeautifier = { version = "*", optional = true }
 mako = { version = ">=1.2.4", optional = true }
 msgspec = ">=0.17.0"
 multidict = ">=6.0.2"
 opentelemetry-instrumentation-asgi = { version = "*", optional = true }
 piccolo = { version = "*", optional = true }
 picologging = { version = "*", optional = true }
-polyfactory = ">=2.3.2"
+polyfactory = ">=2.6.3"
 prometheus-client = { version = "*", optional = true }
 pydantic = { version = "*", optional = true, extras = ["email"] }
+pydantic-extra-types = { version = "*", optional = true }
 python-jose = { version = "*", optional = true }
 pyyaml = "*"
 redis = { version = ">=4.4.4, <4.5.0", optional = true, extras = ["hiredis"] }
 rich = { version = ">=13.0.0", optional = true }
 rich-click = { version = "*", optional = true }
 sqlalchemy = { version = ">=2.0.12", optional = true }
 structlog = { version = "*", optional = true }
-tortoise-orm = { version = ">=0.17.0", optional = true }
 typing-extensions = "*"
 uvicorn = { extras = ["standard"], version = ">=0.22.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 aiosqlite = "*"
-alembic = "*"
-annotated-types = "*"
 asyncmy = "*"
 asyncpg = "*"
-attrs = "*"
 beautifulsoup4 = "*"
-brotli = "*"
-click = "*"
-cryptography = "*"
 duckdb-engine = "*"
 fakeredis = { extras = ["lua"], version = "<2.17.0" }
 freezegun = "*"
 fsspec = "*"
 greenlet = "*"
 hypothesis = "*"
-jinja2 = "*"
-jsbeautifier = "*"
-mako = "*"
-mongomock-motor = { version = "*", markers = "sys_platform != 'win32'" }
-opentelemetry-instrumentation-asgi = "*"
 opentelemetry-sdk = "*"
 oracledb = "*"
-picologging = "*"
-pre-commit = "*"
-prometheus-client = "*"
 psycopg = "*"
-pydantic = "*"
-pydantic-extra-types = "*"
-email_validator = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-lazy-fixture = "*"
 pytest-mock = "*"
 pytest-rerunfailures = "*"
 python-dotenv = "*"
-python-jose = "*"
-redis = ">=4.4.4, <4.5.0"
-rich = "*"
-rich-click = "*"
-sqlalchemy = ">=2.0"
 sqlalchemy-spanner = "*"
 starlette = "*"
-structlog = "*"
 trio = "*"
-uvicorn = "*"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 auto-pytabs = { extras = ["sphinx"], version = "*" }
 black = "*"
-httpx = "*"
 sphinx = ">=5.3.0,<=6"
 sphinx-autobuild = "*"
 sphinx-copybutton = ">=0.5.1"
 sphinx-design = ">=0.3.0,<1"
 sphinxcontrib-mermaid = ">=0.8.1,<1"
 litestar-sphinx-theme = { git = "https://github.com/litestar-org/litestar-sphinx-theme.git" }
-uvicorn = "*"
-sphinx-click = "^4.4.0"
-piccolo = "*"                                                                                 # temporarily moved here because it depends on Pydantic <2 but we need it to generate the docs
+sphinx-click = ">=4.4.0"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 asyncpg-stubs = "*"
 black = "*"
 blacken-docs = "*"
 mypy = "*"
+pre-commit = "*"
 pyright = "*"
 ruff = '*'
 slotscheck = "*"
 sourcery = "*"
 types-beautifulsoup4 = "*"
 types-freezegun = "*"
 types-python-jose = "*"
 types-pyyaml = "*"
 types-redis = "*"
 
 [tool.poetry.extras]
 annotated-types = ["annotated-types"]
 attrs = ["attrs"]
-pydantic = ["pydantic"]
 brotli = ["brotli"]
 cli = ["click", "rich", "rich-click", "jsbeautifier", "uvicorn"]
 cryptography = ["cryptography"]
 jinja = ["jinja2"]
 jwt = ["python-jose", "cryptography"]
+mako = ["mako"]
 opentelemetry = ["opentelemetry-instrumentation-asgi"]
+piccolo = ["piccolo"]
 picologging = ["picologging"]
 prometheus = ["prometheus-client"]
+pydantic = ["pydantic", "pydantic-extra-types"]
 redis = ["redis"]
 sqlalchemy = ["sqlalchemy", "alembic"]
 standard = ["click", "jinja2", "jsbeautifier", "rich", "uvicorn", "rich-click"]
 structlog = ["structlog"]
-tortoise-orm = ["tortoise-orm"]
 
 full = [
     "alembic",
+    "annotated-types",
     "attrs",
     "brotli",
     "click",
+    "rich-click",
     "cryptography",
     "jinja2",
     "jsbeautifier",
+    "mako",
     "opentelemetry-instrumentation-asgi",
+    "piccolo",
+    "picologging",
     "prometheus-client",
+    "pydantic",
+    "pydantic-extra-types",
     "python-jose",
     "redis",
     "rich",
     "sqlalchemy",
     "structlog",
     "uvicorn",
 ]
@@ -328,67 +310,67 @@
 ]
 
 [tool.slotscheck]
 strict-imports = false
 
 [tool.ruff]
 select = [
-    "A",   # flake8-builtins
-    "B",   # flake8-bugbear
+    "A", # flake8-builtins
+    "B", # flake8-bugbear
     "BLE", # flake8-blind-except
-    "C4",  # flake8-comprehensions
+    "C4", # flake8-comprehensions
     "C90", # mccabe
-    "D",   # pydocstyle
-    "DJ",  # flake8-django
+    "D", # pydocstyle
+    "DJ", # flake8-django
     "DTZ", # flake8-datetimez
-    "E",   # pycodestyle errors
+    "E", # pycodestyle errors
     "ERA", # eradicate
     "EXE", # flake8-executable
-    "F",   # pyflakes
-    "G",   # flake8-logging-format
-    "I",   # isort
+    "F", # pyflakes
+    "G", # flake8-logging-format
+    "I", # isort
     "ICN", # flake8-import-conventions
     "ISC", # flake8-implicit-str-concat
-    "N",   # pep8-naming
+    "N", # pep8-naming
     "PIE", # flake8-pie
     "PLC", # pylint - convention
     "PLE", # pylint - error
     "PLW", # pylint - warning
     "PTH", # flake8-use-pathlib
-    "Q",   # flake8-quotes
+    "Q", # flake8-quotes
     "RET", # flake8-return
     "RUF", # Ruff-specific rules
-    "S",   # flake8-bandit
+    "S", # flake8-bandit
     "SIM", # flake8-simplify
     "T10", # flake8-debugger
     "T20", # flake8-print
     "TCH", # flake8-type-checking
     "TID", # flake8-tidy-imports
-    "UP",  # pyupgrade
-    "W",   # pycodestyle - warning
+    "UP", # pyupgrade
+    "W", # pycodestyle - warning
     "YTT", # flake8-2020
 ]
 
 ignore = [
-    "A003",    # flake8-builtins - class attribute {name} is shadowing a python builtin
-    "B010",    # flake8-bugbear - do not call setattr with a constant attribute value
-    "D100",    # pydocstyle - missing docstring in public module
-    "D101",    # pydocstyle - missing docstring in public class
-    "D102",    # pydocstyle - missing docstring in public method
-    "D103",    # pydocstyle - missing docstring in public function
-    "D104",    # pydocstyle - missing docstring in public package
-    "D105",    # pydocstyle - missing docstring in magic method
-    "D106",    # pydocstyle - missing docstring in public nested class
-    "D107",    # pydocstyle - missing docstring in __init__
-    "D202",    # pydocstyle - no blank lines allowed after function docstring
-    "D205",    # pydocstyle - 1 blank line required between summary line and description
-    "D415",    # pydocstyle - first line should end with a period, question mark, or exclamation point
-    "E501",    # pycodestyle line too long, handled by black
+    "A003", # flake8-builtins - class attribute {name} is shadowing a python builtin
+    "B010", # flake8-bugbear - do not call setattr with a constant attribute value
+    "D100", # pydocstyle - missing docstring in public module
+    "D101", # pydocstyle - missing docstring in public class
+    "D102", # pydocstyle - missing docstring in public method
+    "D103", # pydocstyle - missing docstring in public function
+    "D104", # pydocstyle - missing docstring in public package
+    "D105", # pydocstyle - missing docstring in magic method
+    "D106", # pydocstyle - missing docstring in public nested class
+    "D107", # pydocstyle - missing docstring in __init__
+    "D202", # pydocstyle - no blank lines allowed after function docstring
+    "D205", # pydocstyle - 1 blank line required between summary line and description
+    "D415", # pydocstyle - first line should end with a period, question mark, or exclamation point
+    "E501", # pycodestyle line too long, handled by black
     "PLW2901", # pylint - for loop variable overwritten by assignment target
-    "RUF012",  # Ruff-specific rule - annotated with classvar
+    "RUF012", # Ruff-specific rule - annotated with classvar
 ]
 line-length = 120
 src = ["litestar", "tests", "docs/examples"]
 target-version = "py38"
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `litestar-2.0.0b3/PKG-INFO` & `litestar-2.0.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litestar
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: Litestar - A production-ready, highly performant, extensible ASGI API Framework
 Home-page: https://litestar.dev/
 License: MIT
 Keywords: api,rest,http,asgi,pydantic,litestar,starlite,framework,websocket,litestar
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -39,53 +39,54 @@
 Provides-Extra: attrs
 Provides-Extra: brotli
 Provides-Extra: cli
 Provides-Extra: cryptography
 Provides-Extra: full
 Provides-Extra: jinja
 Provides-Extra: jwt
+Provides-Extra: mako
 Provides-Extra: opentelemetry
+Provides-Extra: piccolo
 Provides-Extra: picologging
 Provides-Extra: prometheus
 Provides-Extra: pydantic
 Provides-Extra: redis
 Provides-Extra: sqlalchemy
 Provides-Extra: standard
 Provides-Extra: structlog
-Provides-Extra: tortoise-orm
 Requires-Dist: alembic ; extra == "sqlalchemy" or extra == "full"
-Requires-Dist: annotated-types ; extra == "annotated-types"
+Requires-Dist: annotated-types ; extra == "annotated-types" or extra == "full"
 Requires-Dist: anyio (>=3)
 Requires-Dist: attrs ; extra == "attrs" or extra == "full"
 Requires-Dist: brotli ; extra == "brotli" or extra == "full"
 Requires-Dist: click ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: cryptography ; extra == "cryptography" or extra == "jwt" or extra == "full"
 Requires-Dist: fast-query-parsers (>=1.0.2)
 Requires-Dist: httpx (>=0.22)
 Requires-Dist: importlib-metadata ; python_version < "3.10"
 Requires-Dist: importlib-resources (>=5.12.0) ; python_version < "3.9"
 Requires-Dist: jinja2 (>=3.1.2) ; extra == "jinja" or extra == "standard" or extra == "full"
 Requires-Dist: jsbeautifier ; extra == "cli" or extra == "standard" or extra == "full"
-Requires-Dist: mako (>=1.2.4)
+Requires-Dist: mako (>=1.2.4) ; extra == "mako" or extra == "full"
 Requires-Dist: msgspec (>=0.17.0)
 Requires-Dist: multidict (>=6.0.2)
 Requires-Dist: opentelemetry-instrumentation-asgi ; extra == "opentelemetry" or extra == "full"
-Requires-Dist: piccolo
-Requires-Dist: picologging ; extra == "picologging"
-Requires-Dist: polyfactory (>=2.3.2)
+Requires-Dist: piccolo ; extra == "piccolo" or extra == "full"
+Requires-Dist: picologging ; extra == "picologging" or extra == "full"
+Requires-Dist: polyfactory (>=2.6.3)
 Requires-Dist: prometheus-client ; extra == "prometheus" or extra == "full"
-Requires-Dist: pydantic[email] ; extra == "pydantic"
+Requires-Dist: pydantic-extra-types ; extra == "pydantic" or extra == "full"
+Requires-Dist: pydantic[email] ; extra == "pydantic" or extra == "full"
 Requires-Dist: python-jose ; extra == "jwt" or extra == "full"
 Requires-Dist: pyyaml
 Requires-Dist: redis[hiredis] (>=4.4.4,<4.5.0) ; extra == "redis" or extra == "full"
 Requires-Dist: rich (>=13.0.0) ; extra == "cli" or extra == "standard" or extra == "full"
-Requires-Dist: rich-click ; extra == "cli" or extra == "standard"
+Requires-Dist: rich-click ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: sqlalchemy (>=2.0.12) ; extra == "sqlalchemy" or extra == "full"
 Requires-Dist: structlog ; extra == "structlog" or extra == "full"
-Requires-Dist: tortoise-orm (>=0.17.0) ; extra == "tortoise-orm"
 Requires-Dist: typing-extensions
 Requires-Dist: uvicorn[standard] (>=0.22.0) ; extra == "cli" or extra == "standard" or extra == "full"
 Project-URL: Blog, https://blog.litestar.dev
 Project-URL: Changelog, https://github.com/litestar-org/litestar/releases/
 Project-URL: Documentation, https://docs.litestar.dev/
 Project-URL: Discord, https://discord.gg/MmcwxztmQb
 Project-URL: Issue Tracker, https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
@@ -132,15 +133,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the latest pre-release version by instead running
 
 ```shell
-pip install litestar==2.0.0beta2
+pip install litestar==2.0.0beta3
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
 
@@ -270,15 +271,15 @@
 
 Litestar also supports the programmatic creation of DTOs with a `DTOFactory` class, which also supports the use of
 plugins.
 
 ### OpenAPI
 
 Litestar has custom logic to generate OpenAPI 3.1.0 schema, include optional generation of examples using the
-`pydantic-factories` library.
+[`polyfactory`](https://pypi.org/project/polyfactory/) library.
 
 #### ReDoc, Swagger-UI and Stoplight Elements API Documentation
 
 Litestar serves the documentation from the generated OpenAPI schema with:
 
 - [ReDoc](https://redoc.ly/)
 - [Swagger-UI](https://swagger.io/tools/swagger-ui/)
```

