# Comparing `tmp/litestar-2.0.0b1.tar.gz` & `tmp/litestar-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar-2.0.0b1.tar", max compression
+gzip compressed data, was "litestar-2.0.0b2.tar", max compression
```

## Comparing `litestar-2.0.0b1.tar` & `litestar-2.0.0b2.tar`

### file list

```diff
@@ -1,313 +1,317 @@
--rw-r--r--   0        0        0     1092 2023-06-16 11:23:18.734701 litestar-2.0.0b1/LICENSE
--rw-r--r--   0        0        0    51150 2023-06-16 11:23:18.734701 litestar-2.0.0b1/docs/PYPI_README.md
--rw-r--r--   0        0        0      744 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/__init__.py
--rw-r--r--   0        0        0      228 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/__main__.py
--rw-r--r--   0        0        0       77 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     6380 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0      349 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7823 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5938 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1267 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1528 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_asgi/utils.py
--rw-r--r--   0        0        0       66 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3868 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4239 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    14894 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20450 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2759 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_layers/utils.py
--rw-r--r--   0        0        0     5922 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_multipart.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0    10215 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5491 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     1523 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    10471 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/responses.py
--rw-r--r--   0        0        0       64 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     7191 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2104 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    35844 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0      524 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10970 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5240 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7685 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     1464 2023-06-16 11:23:18.770701 litestar-2.0.0b1/litestar/_openapi/utils.py
--rw-r--r--   0        0        0     2338 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_parsers.py
--rw-r--r--   0        0        0      182 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/__init__.py
--rw-r--r--   0        0        0     7023 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/field.py
--rw-r--r--   0        0        0     4334 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/metadata.py
--rw-r--r--   0        0        0       64 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/models/__init__.py
--rw-r--r--   0        0        0    13948 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/models/attrs_signature_model.py
--rw-r--r--   0        0        0     3736 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/models/base.py
--rw-r--r--   0        0        0     6689 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/models/pydantic_signature_model.py
--rw-r--r--   0        0        0     5639 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/_signature/utils.py
--rw-r--r--   0        0        0    36313 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/app.py
--rw-r--r--   0        0        0     2200 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/background_tasks.py
--rw-r--r--   0        0        0      176 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     1300 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     2768 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     9364 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0    15726 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4647 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/channels/subscriber.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/__init__.py
--rw-r--r--   0        0        0    12595 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/_utils.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0     6630 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2568 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2381 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0     2125 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    11442 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/app.py
--rw-r--r--   0        0        0     2742 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/compression.py
--rw-r--r--   0        0        0     5177 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/csrf.py
--rw-r--r--   0        0        0     1991 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/connection/__init__.py
--rw-r--r--   0        0        0    10821 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/connection/base.py
--rw-r--r--   0        0        0     7698 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/connection/request.py
--rw-r--r--   0        0        0    11274 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/connection/websocket.py
--rw-r--r--   0        0        0     1363 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/constants.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4917 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4051 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     6401 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0     2557 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jinja.py
--rw-r--r--   0        0        0      521 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28722 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     4463 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     6970 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3961 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/mako.py
--rw-r--r--   0        0        0     2167 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/msgspec.py
--rw-r--r--   0        0        0      180 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4206 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2206 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0     2341 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/pydantic.py
--rw-r--r--   0        0        0      364 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0      162 2023-06-16 11:23:18.774701 litestar-2.0.0b1/litestar/contrib/repository/abc/__init__.py
--rw-r--r--   0        0        0     8889 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/abc/_async.py
--rw-r--r--   0        0        0     8907 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/abc/_sync.py
--rw-r--r--   0        0        0      328 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0     2064 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      641 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/testing/__init__.py
--rw-r--r--   0        0        0    26054 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5571 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0     8465 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      941 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      319 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/_slots_base.py
--rw-r--r--   0        0        0      504 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      458 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0     4575 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0    11408 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0    11500 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0     3787 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0     1647 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0     1426 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0      288 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/__init__.py
--rw-r--r--   0        0        0    23050 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_async.py
--rw-r--r--   0        0        0    22806 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_sync.py
--rw-r--r--   0        0        0     1033 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_util.py
--rw-r--r--   0        0        0      754 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/types.py
--rw-r--r--   0        0        0     6349 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0     9546 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/controller.py
--rw-r--r--   0        0        0    16508 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/data_extractors.py
--rw-r--r--   0        0        0      883 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3757 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    17316 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     2977 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9646 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/state.py
--rw-r--r--   0        0        0     3310 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7273 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/datastructures/url.py
--rw-r--r--   0        0        0     3117 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/di.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/__init__.py
--rw-r--r--   0        0        0      240 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/__init__.py
--rw-r--r--   0        0        0      245 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/__init__.py
--rw-r--r--   0        0        0    18470 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/abc.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/__init__.py
--rw-r--r--   0        0        0     1339 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/backend.py
--rw-r--r--   0        0        0     1691 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/utils.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/backend.py
--rw-r--r--   0        0        0     1936 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/utils.py
--rw-r--r--   0        0        0     3704 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/types.py
--rw-r--r--   0        0        0    14227 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/_backends/utils.py
--rw-r--r--   0        0        0     7720 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/abc.py
--rw-r--r--   0        0        0     1405 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/config.py
--rw-r--r--   0        0        0     3276 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/data_structures.py
--rw-r--r--   0        0        0      313 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/exc.py
--rw-r--r--   0        0        0     1388 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/field.py
--rw-r--r--   0        0        0       65 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/stdlib/__init__.py
--rw-r--r--   0        0        0     2144 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/stdlib/dataclass.py
--rw-r--r--   0        0        0      363 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/types.py
--rw-r--r--   0        0        0     4457 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/factory/utils.py
--rw-r--r--   0        0        0     4474 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/interface.py
--rw-r--r--   0        0        0      309 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/dto/types.py
--rw-r--r--   0        0        0     1728 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/enums.py
--rw-r--r--   0        0        0      201 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/events/__init__.py
--rw-r--r--   0        0        0     4355 2023-06-16 11:23:18.778701 litestar-2.0.0b1/litestar/events/emitter.py
--rw-r--r--   0        0        0     1305 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/events/listener.py
--rw-r--r--   0        0        0     1165 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1702 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0     4629 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5336 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/file_system.py
--rw-r--r--   0        0        0      559 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3868 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    20477 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     6658 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    26422 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    62224 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      340 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     7151 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    18876 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     3605 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/_utils.py
--rw-r--r--   0        0        0    12050 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/picologging.py
--rw-r--r--   0        0        0      860 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2081 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     3086 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3430 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5284 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/base.py
--rw-r--r--   0        0        0     8395 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/compression.py
--rw-r--r--   0        0        0     2565 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6466 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7210 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0     9275 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13330 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10811 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0       70 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     7935 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10365 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     8558 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      183 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5226 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/config.py
--rw-r--r--   0        0        0    15696 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/controller.py
--rw-r--r--   0        0        0      898 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1915 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2936 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      974 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      752 2023-06-16 11:23:18.782701 litestar-2.0.0b1/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4218 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6242 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    34574 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0    11029 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/pagination.py
--rw-r--r--   0        0        0    14871 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/params.py
--rw-r--r--   0        0        0     7100 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/partial.py
--rw-r--r--   0        0        0     3905 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/plugins.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/py.typed
--rw-r--r--   0        0        0      208 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/__init__.py
--rw-r--r--   0        0        0    15231 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/base.py
--rw-r--r--   0        0        0    14298 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/file.py
--rw-r--r--   0        0        0     5440 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/redirect.py
--rw-r--r--   0        0        0     7943 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/streaming.py
--rw-r--r--   0        0        0     5229 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/response/template.py
--rw-r--r--   0        0        0    14998 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/router.py
--rw-r--r--   0        0        0      191 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1719 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6437 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/base.py
--rw-r--r--   0        0        0    13244 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/http.py
--rw-r--r--   0        0        0     3002 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/__init__.py
--rw-r--r--   0        0        0     7165 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/base.py
--rw-r--r--   0        0        0      188 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5602 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     4952 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0     7714 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/serialization.py
--rw-r--r--   0        0        0      158 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5046 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/static_files/base.py
--rw-r--r--   0        0        0     3598 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/static_files/config.py
--rw-r--r--   0        0        0     9536 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/status_codes.py
--rw-r--r--   0        0        0        0 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4396 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/base.py
--rw-r--r--   0        0        0     5425 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/file.py
--rw-r--r--   0        0        0     3625 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/memory.py
--rw-r--r--   0        0        0     6231 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/redis.py
--rw-r--r--   0        0        0     2233 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/template/__init__.py
--rw-r--r--   0        0        0     4083 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/template/base.py
--rw-r--r--   0        0        0     1894 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/template/config.py
--rw-r--r--   0        0        0      581 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17445 2023-06-16 11:23:18.786701 litestar-2.0.0b1/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     5132 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19555 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0    29657 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2532 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    21927 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     8057 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/transport.py
--rw-r--r--   0        0        0     8559 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4047 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/__init__.py
--rw-r--r--   0        0        0     8671 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      453 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2222 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1705 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/composite_types.py
--rw-r--r--   0        0        0      183 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/empty.py
--rw-r--r--   0        0        0     2666 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/file_types.py
--rw-r--r--   0        0        0      344 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1720 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2965 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/protocols.py
--rw-r--r--   0        0        0     1820 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/types/serialization.py
--rw-r--r--   0        0        0     6483 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/typing.py
--rw-r--r--   0        0        0     1953 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/compat.py
--rw-r--r--   0        0        0     3635 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3520 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/deprecation.py
--rw-r--r--   0        0        0     3334 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/helpers.py
--rw-r--r--   0        0        0      723 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/path.py
--rw-r--r--   0        0        0    11750 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/predicates.py
--rw-r--r--   0        0        0     2823 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/scope.py
--rw-r--r--   0        0        0     1003 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/sequence.py
--rw-r--r--   0        0        0     8410 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/signature.py
--rw-r--r--   0        0        0     4374 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/sync.py
--rw-r--r--   0        0        0     8302 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/typing.py
--rw-r--r--   0        0        0     1921 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/version.py
--rw-r--r--   0        0        0     1992 2023-06-16 11:23:18.790701 litestar-2.0.0b1/litestar/utils/warnings.py
--rw-r--r--   0        0        0    12666 2023-06-16 11:23:18.794701 litestar-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    55082 1970-01-01 00:00:00.000000 litestar-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-24 19:32:57.844417 litestar-2.0.0b2/LICENSE
+-rw-r--r--   0        0        0    51236 2023-06-24 19:32:57.848417 litestar-2.0.0b2/docs/PYPI_README.md
+-rw-r--r--   0        0        0      744 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/__init__.py
+-rw-r--r--   0        0        0      228 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/__main__.py
+-rw-r--r--   0        0        0       77 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     6395 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7823 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5977 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1267 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3842 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4239 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    14894 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20450 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2759 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_layers/utils.py
+-rw-r--r--   0        0        0     5922 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_multipart.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0     9429 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     5536 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     1213 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0     9629 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     3190 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2254 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    30936 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0      524 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    11000 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5240 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7685 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1464 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0     2338 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_parsers.py
+-rw-r--r--   0        0        0      182 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0     7121 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/field.py
+-rw-r--r--   0        0        0     4516 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/metadata.py
+-rw-r--r--   0        0        0       64 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/models/__init__.py
+-rw-r--r--   0        0        0    17165 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/models/attrs_signature_model.py
+-rw-r--r--   0        0        0     5585 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/models/base.py
+-rw-r--r--   0        0        0     7300 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/models/pydantic_signature_model.py
+-rw-r--r--   0        0        0     5556 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/_signature/utils.py
+-rw-r--r--   0        0        0    36404 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/app.py
+-rw-r--r--   0        0        0     2200 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/background_tasks.py
+-rw-r--r--   0        0        0      176 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     1300 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     2768 2023-06-24 19:32:57.880416 litestar-2.0.0b2/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     9422 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0    15726 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4647 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    12711 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6630 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2568 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2381 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0     2125 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    11442 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/app.py
+-rw-r--r--   0        0        0     2742 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/compression.py
+-rw-r--r--   0        0        0     5182 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/csrf.py
+-rw-r--r--   0        0        0     1991 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    10826 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/connection/base.py
+-rw-r--r--   0        0        0     7698 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/connection/request.py
+-rw-r--r--   0        0        0    11274 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/connection/websocket.py
+-rw-r--r--   0        0        0     1363 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/constants.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4916 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4059 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     6408 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2557 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28722 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     4463 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6986 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3983 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/mako.py
+-rw-r--r--   0        0        0     2167 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/msgspec.py
+-rw-r--r--   0        0        0      180 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4235 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2214 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0      207 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     2733 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/prometheus/config.py
+-rw-r--r--   0        0        0     1646 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/prometheus/controller.py
+-rw-r--r--   0        0        0     6766 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/prometheus/middleware.py
+-rw-r--r--   0        0        0     2341 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/pydantic.py
+-rw-r--r--   0        0        0      364 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/abc/__init__.py
+-rw-r--r--   0        0        0     8889 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/abc/_async.py
+-rw-r--r--   0        0        0     8907 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/abc/_sync.py
+-rw-r--r--   0        0        0      328 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     2064 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      641 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    26054 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5535 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0     8773 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      941 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/_slots_base.py
+-rw-r--r--   0        0        0      504 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      458 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     4575 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0    11423 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0    11500 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     3787 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0     1647 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0     1441 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0      288 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/__init__.py
+-rw-r--r--   0        0        0    22904 2023-06-24 19:32:57.884416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_async.py
+-rw-r--r--   0        0        0    22646 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_sync.py
+-rw-r--r--   0        0        0     1033 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_util.py
+-rw-r--r--   0        0        0      754 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/types.py
+-rw-r--r--   0        0        0     6359 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0     9545 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/controller.py
+-rw-r--r--   0        0        0    16539 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/data_extractors.py
+-rw-r--r--   0        0        0      883 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3762 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    17352 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9646 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     3310 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7273 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/datastructures/url.py
+-rw-r--r--   0        0        0     3117 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/di.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/__init__.py
+-rw-r--r--   0        0        0      240 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/__init__.py
+-rw-r--r--   0        0        0    18286 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/abc.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/msgspec/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/msgspec/backend.py
+-rw-r--r--   0        0        0     1691 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/msgspec/utils.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/pydantic/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/pydantic/backend.py
+-rw-r--r--   0        0        0     1936 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/pydantic/utils.py
+-rw-r--r--   0        0        0     3704 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/types.py
+-rw-r--r--   0        0        0    14227 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/_backends/utils.py
+-rw-r--r--   0        0        0     7692 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/abc.py
+-rw-r--r--   0        0        0     1405 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/config.py
+-rw-r--r--   0        0        0     3291 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/data_structures.py
+-rw-r--r--   0        0        0      313 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/exc.py
+-rw-r--r--   0        0        0     1388 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/field.py
+-rw-r--r--   0        0        0       65 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/stdlib/__init__.py
+-rw-r--r--   0        0        0     2144 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/stdlib/dataclass.py
+-rw-r--r--   0        0        0      363 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/types.py
+-rw-r--r--   0        0        0     4457 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/factory/utils.py
+-rw-r--r--   0        0        0     4442 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/interface.py
+-rw-r--r--   0        0        0      309 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/dto/types.py
+-rw-r--r--   0        0        0     1728 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/enums.py
+-rw-r--r--   0        0        0      201 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4371 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/events/emitter.py
+-rw-r--r--   0        0        0     1313 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/events/listener.py
+-rw-r--r--   0        0        0     1165 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1702 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5344 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/file_system.py
+-rw-r--r--   0        0        0      559 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3868 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    20199 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     6450 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    26346 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    62224 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      340 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     7151 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    19091 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     3605 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    12050 2023-06-24 19:32:57.888416 litestar-2.0.0b2/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2081 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     3094 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3430 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5284 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/base.py
+-rw-r--r--   0        0        0     8454 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/compression.py
+-rw-r--r--   0        0        0     2573 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6466 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7210 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     9435 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13330 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10811 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7935 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10365 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8558 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      183 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0     5226 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/config.py
+-rw-r--r--   0        0        0    15866 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      898 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1915 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4028 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34574 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0    11029 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/pagination.py
+-rw-r--r--   0        0        0    14893 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/params.py
+-rw-r--r--   0        0        0     7097 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/partial.py
+-rw-r--r--   0        0        0     3905 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/plugins.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/py.typed
+-rw-r--r--   0        0        0      208 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/__init__.py
+-rw-r--r--   0        0        0    15236 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/base.py
+-rw-r--r--   0        0        0    14298 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/file.py
+-rw-r--r--   0        0        0     5440 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/redirect.py
+-rw-r--r--   0        0        0     7956 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/streaming.py
+-rw-r--r--   0        0        0     5229 2023-06-24 19:32:57.892416 litestar-2.0.0b2/litestar/response/template.py
+-rw-r--r--   0        0        0    15001 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/router.py
+-rw-r--r--   0        0        0      191 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1719 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6437 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/base.py
+-rw-r--r--   0        0        0    13244 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/http.py
+-rw-r--r--   0        0        0     3002 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/base.py
+-rw-r--r--   0        0        0      188 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4978 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0     7714 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/serialization.py
+-rw-r--r--   0        0        0      158 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5046 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/static_files/base.py
+-rw-r--r--   0        0        0     3598 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/static_files/config.py
+-rw-r--r--   0        0        0     9536 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/status_codes.py
+-rw-r--r--   0        0        0        0 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4396 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/base.py
+-rw-r--r--   0        0        0     5430 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/memory.py
+-rw-r--r--   0        0        0     6231 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2233 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/template/__init__.py
+-rw-r--r--   0        0        0     4083 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/template/base.py
+-rw-r--r--   0        0        0     1894 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17562 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     5145 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19671 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0    30009 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2540 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    21927 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     8056 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8564 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4073 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8930 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      566 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2962 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1872 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      272 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/empty.py
+-rw-r--r--   0        0        0     2635 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/file_types.py
+-rw-r--r--   0        0        0      781 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1924 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2984 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/protocols.py
+-rw-r--r--   0        0        0     2005 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/types/serialization.py
+-rw-r--r--   0        0        0     6479 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/typing.py
+-rw-r--r--   0        0        0     2001 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3645 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3520 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     3351 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/path.py
+-rw-r--r--   0        0        0    12066 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/predicates.py
+-rw-r--r--   0        0        0     2823 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/scope.py
+-rw-r--r--   0        0        0     1003 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/sequence.py
+-rw-r--r--   0        0        0     8410 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/signature.py
+-rw-r--r--   0        0        0     4374 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/sync.py
+-rw-r--r--   0        0        0     8279 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1921 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/version.py
+-rw-r--r--   0        0        0     1992 2023-06-24 19:32:57.896416 litestar-2.0.0b2/litestar/utils/warnings.py
+-rw-r--r--   0        0        0    12929 2023-06-24 19:32:57.900416 litestar-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0    55447 1970-01-01 00:00:00.000000 litestar-2.0.0b2/PKG-INFO
```

### Comparing `litestar-2.0.0b1/LICENSE` & `litestar-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/docs/PYPI_README.md` & `litestar-2.0.0b2/docs/PYPI_README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!-- markdownlint-disable -->
 <p align="center">
-  <img src="artwork/banner-light.svg" alt="Litestar Logo - Light" width="100%" height="auto" />
+  <img src="https://github.com/litestar-org/litestar/blob/ecb4412055710f78124710990584aa24fc6c9a55/artwork/banner-light.svg" alt="Litestar Logo - Light" width="100%" height="auto" />
 </p>
 <!-- markdownlint-restore -->
 
 <div align="center">
 
 [![ci](https://github.com/litestar-org/litestar/actions/workflows/ci.yaml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/ci.yaml)
 [![PyPI - Version](https://badge.fury.io/py/litestar.svg)](https://badge.fury.io/py/litestar)
@@ -48,15 +48,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the alpha version by instead running
 
 ```shell
-pip install litestar==2.0.0alpha7
+pip install litestar==2.0.0beta1
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
```

### Comparing `litestar-2.0.0b1/litestar/__init__.py` & `litestar-2.0.0b2/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_asgi/asgi_router.py` & `litestar-2.0.0b2/litestar/_asgi/asgi_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import re
 from collections import defaultdict
 from functools import lru_cache
 from traceback import format_exc
-from typing import TYPE_CHECKING, Pattern
+from typing import TYPE_CHECKING, Any, Pattern
 
 from litestar._asgi.routing_trie import validate_node
 from litestar._asgi.routing_trie.mapping import add_route_to_trie
 from litestar._asgi.routing_trie.traversal import parse_path_to_route
 from litestar._asgi.routing_trie.types import create_node
 from litestar._asgi.utils import get_route_handlers
 from litestar.exceptions import ImproperlyConfiguredException
@@ -80,15 +80,15 @@
         normalized_path = normalize_path(scope["path"])
         asgi_app, scope["route_handler"], scope["path"], scope["path_params"] = self.handle_routing(
             path=normalized_path, method=scope.get("method")
         )
         await asgi_app(scope, receive, send)
 
     @lru_cache(1024)  # noqa: B019
-    def handle_routing(self, path: str, method: Method | None) -> tuple[ASGIApp, RouteHandlerType, str, dict]:
+    def handle_routing(self, path: str, method: Method | None) -> tuple[ASGIApp, RouteHandlerType, str, dict[str, Any]]:
         """Handle routing for a given path / method combo. This method is meant to allow easy caching.
 
         Args:
             path: The path of the request.
             method: The scope's method, if any.
 
         Returns:
```

### Comparing `litestar-2.0.0b1/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.0.0b2/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.0.0b2/litestar/_asgi/routing_trie/traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             if current_node.is_path_type:
                 path_params.append(normalize_path("/".join(path_components[i:])))
                 break
 
             path_params.append(component)
             continue
 
-        if i != len(path_components) - 1:
+        if i != len(path_components) - 1 or not current_node.children:
             raise NotFoundException()
 
     if not current_node.asgi_handlers:
         raise NotFoundException()
 
     return current_node, path_params, path
 
@@ -109,15 +109,15 @@
 def parse_path_to_route(
     method: Method | None,
     mount_paths_regex: Pattern | None,
     mount_routes: dict[str, RouteTrieNode],
     path: str,
     plain_routes: set[str],
     root_node: RouteTrieNode,
-) -> tuple[ASGIApp, RouteHandlerType, str, dict]:
+) -> tuple[ASGIApp, RouteHandlerType, str, dict[str, Any]]:
     """Given a scope object, retrieve the asgi_handlers and is_mount boolean values from correct trie node.
 
     Args:
         method: The scope's method, if any.
         root_node: The root trie node.
         path: The path to resolve scope instance.
         plain_routes: The set of plain routes.
```

### Comparing `litestar-2.0.0b1/litestar/_asgi/routing_trie/types.py` & `litestar-2.0.0b2/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_asgi/routing_trie/validate.py` & `litestar-2.0.0b2/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_asgi/utils.py` & `litestar-2.0.0b2/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_kwargs/cleanup.py` & `litestar-2.0.0b2/litestar/_kwargs/cleanup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self._generators.append(generator)
 
     @staticmethod
     def _wrap_next(generator: AnyGenerator) -> Callable[[], Coroutine[None, None, None]]:
         if isasyncgen(generator):
 
             async def wrapped_async() -> None:
-                await async_next(generator, None)  # type: ignore[arg-type]
+                await async_next(generator, None)
 
             return wrapped_async
 
         def wrapped() -> None:
             next(generator, None)  # type: ignore[arg-type]
 
         return AsyncCallable(wrapped)
```

### Comparing `litestar-2.0.0b1/litestar/_kwargs/dependencies.py` & `litestar-2.0.0b2/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_kwargs/extractors.py` & `litestar-2.0.0b2/litestar/_kwargs/extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_kwargs/kwargs_model.py` & `litestar-2.0.0b2/litestar/_kwargs/kwargs_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_kwargs/parameter_definition.py` & `litestar-2.0.0b2/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_layers/utils.py` & `litestar-2.0.0b2/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_multipart.py` & `litestar-2.0.0b2/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_openapi/parameters.py` & `litestar-2.0.0b2/litestar/_openapi/parameters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,31 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from litestar._openapi.schema_generation import create_schema
-from litestar._signature.field import SignatureField
 from litestar.constants import RESERVED_KWARGS
 from litestar.enums import ParamType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.openapi.spec.parameter import Parameter
 from litestar.openapi.spec.schema import Schema
 from litestar.params import DependencyKwarg, ParameterKwarg
 from litestar.types import Empty
 
-__all__ = (
-    "ParameterCollection",
-    "create_parameter",
-    "create_parameter_for_handler",
-    "create_path_parameter_schema",
-    "get_layered_parameter",
-    "get_recursive_handler_parameters",
-)
+__all__ = ("create_parameter_for_handler",)
 
 
 if TYPE_CHECKING:
+    from litestar._openapi.schema_generation import SchemaCreator
+    from litestar._signature.field import SignatureField
     from litestar.di import Provide
     from litestar.handlers.base import BaseRouteHandler
     from litestar.openapi.spec import Reference
     from litestar.types.internal_types import PathParameterDefinition
 
 
-def create_path_parameter_schema(
-    path_parameter: PathParameterDefinition,
-    field: SignatureField,
-    generate_examples: bool,
-    schemas: dict[str, Schema],
-) -> Schema | Reference:
-    """Create a path parameter from the given path_param definition."""
-    return create_schema(
-        field=SignatureField(
-            children=None,
-            default_value=field.default_value,
-            extra=field.extra,
-            field_type=path_parameter.type,
-            kwarg_model=field.kwarg_model,
-            name=field.name,
-        ),
-        generate_examples=generate_examples,
-        plugins=[],
-        schemas=schemas,
-        prefer_alias=True,
-    )
-
-
 class ParameterCollection:
     """Facilitates conditional deduplication of parameters.
 
     If multiple parameters with the same name are produced for a handler, the condition is ignored if the two
     ``Parameter`` instances are the same (the first is retained and any duplicates are ignored). If the ``Parameter``
     instances are not the same, an exception is raised.
     """
@@ -96,48 +66,53 @@
         return list(self._parameters.values())
 
 
 def create_parameter(
     signature_field: SignatureField,
     parameter_name: str,
     path_parameters: tuple[PathParameterDefinition, ...],
-    generate_examples: bool,
-    schemas: dict[str, Schema],
+    schema_creator: SchemaCreator,
 ) -> Parameter:
     """Create an OpenAPI Parameter instance."""
+    from litestar._signature.field import SignatureField
+
     result: Schema | Reference | None = None
     kwargs_model = signature_field.kwarg_model if isinstance(signature_field.kwarg_model, ParameterKwarg) else None
 
     if any(path_param.name == parameter_name for path_param in path_parameters):
         param_in = ParamType.PATH
         is_required = True
         path_parameter = [p for p in path_parameters if parameter_name in p.name][0]
-        result = create_path_parameter_schema(
-            field=signature_field, generate_examples=generate_examples, path_parameter=path_parameter, schemas=schemas
+        result = schema_creator.for_field(
+            SignatureField(
+                children=None,
+                default_value=signature_field.default_value,
+                extra=signature_field.extra,
+                field_type=path_parameter.type,
+                kwarg_model=signature_field.kwarg_model,
+                name=signature_field.name,
+            )
         )
-
     elif kwargs_model and kwargs_model.header:
         parameter_name = kwargs_model.header
         param_in = ParamType.HEADER
         is_required = signature_field.is_required
     elif kwargs_model and kwargs_model.cookie:
         parameter_name = kwargs_model.cookie
         param_in = ParamType.COOKIE
         is_required = signature_field.is_required
     else:
         is_required = signature_field.is_required
         param_in = ParamType.QUERY
         parameter_name = kwargs_model.query if kwargs_model and kwargs_model.query else parameter_name
 
     if not result:
-        result = create_schema(
-            field=signature_field, generate_examples=generate_examples, plugins=[], schemas=schemas, prefer_alias=True
-        )
+        result = schema_creator.for_field(signature_field)
 
-    schema = result if isinstance(result, Schema) else schemas[result.value]
+    schema = result if isinstance(result, Schema) else schema_creator.schemas[result.value]
 
     return Parameter(
         description=schema.description,
         name=parameter_name,
         param_in=param_in,
         required=is_required,
         schema=result,
@@ -146,46 +121,47 @@
 
 def get_recursive_handler_parameters(
     field_name: str,
     signature_field: SignatureField,
     dependency_providers: dict[str, Provide],
     route_handler: BaseRouteHandler,
     path_parameters: tuple[PathParameterDefinition, ...],
-    generate_examples: bool,
-    schemas: dict[str, Schema],
+    schema_creator: SchemaCreator,
 ) -> list[Parameter]:
     """Create and return parameters for a handler.
 
     If the provided field is not a dependency, a normal parameter is created and returned as a list, otherwise
     `create_parameter_for_handler()` is called to generate parameters for the dependency.
     """
 
     if field_name not in dependency_providers:
         return [
             create_parameter(
-                generate_examples=generate_examples,
+                signature_field=signature_field,
                 parameter_name=field_name,
                 path_parameters=path_parameters,
-                schemas=schemas,
-                signature_field=signature_field,
+                schema_creator=schema_creator,
             )
         ]
+
     dependency_fields = dependency_providers[field_name].signature_model.fields
     return create_parameter_for_handler(
-        route_handler, dependency_fields, path_parameters, generate_examples, schemas=schemas
+        route_handler=route_handler,
+        handler_fields=dependency_fields,
+        path_parameters=path_parameters,
+        schema_creator=schema_creator,
     )
 
 
 def get_layered_parameter(
     field_name: str,
     signature_field: SignatureField,
     layered_parameters: dict[str, SignatureField],
     path_parameters: tuple[PathParameterDefinition, ...],
-    generate_examples: bool,
-    schemas: dict[str, Schema],
+    schema_creator: SchemaCreator,
 ) -> Parameter:
     """Create a layered parameter for a given signature model field.
 
     Layer info is extracted from the provided ``layered_parameters`` dict and set as the field's ``field_info`` attribute.
     """
     layer_field = layered_parameters[field_name]
 
@@ -193,86 +169,84 @@
     default_value = signature_field.default_value if not signature_field.is_empty else layer_field.default_value
     field_type = signature_field.field_type if signature_field is not Empty else layer_field.field_type  # type: ignore
 
     parameter_name = field_name
     if isinstance(field.kwarg_model, ParameterKwarg):
         parameter_name = field.kwarg_model.query or field.kwarg_model.header or field.kwarg_model.cookie or field_name
 
+    from litestar._signature.field import SignatureField
+
+    signature_field = SignatureField.create(
+        children=field.children,
+        default_value=default_value,
+        extra=field.extra,
+        field_type=field_type,
+        kwarg_model=field.kwarg_model,
+        name=field_name,
+    )
     return create_parameter(
-        signature_field=SignatureField.create(
-            children=field.children,
-            default_value=default_value,
-            extra=field.extra,
-            field_type=field_type,
-            kwarg_model=field.kwarg_model,
-            name=field_name,
-        ),
-        generate_examples=generate_examples,
+        signature_field=signature_field,
         parameter_name=parameter_name,
         path_parameters=path_parameters,
-        schemas=schemas,
+        schema_creator=schema_creator,
     )
 
 
 def create_parameter_for_handler(
     route_handler: BaseRouteHandler,
     handler_fields: dict[str, SignatureField],
     path_parameters: tuple[PathParameterDefinition, ...],
-    generate_examples: bool,
-    schemas: dict[str, Schema],
+    schema_creator: SchemaCreator,
 ) -> list[Parameter]:
     """Create a list of path/query/header Parameter models for the given PathHandler."""
     parameters = ParameterCollection(route_handler=route_handler)
-    dependencies = route_handler.resolve_dependencies()
+    dependency_providers = route_handler.resolve_dependencies()
 
     layered_parameters = route_handler.resolve_layered_parameters()
 
     unique_handler_fields = tuple(
         (k, v) for k, v in handler_fields.items() if k not in RESERVED_KWARGS and k not in layered_parameters
     )
     unique_layered_fields = tuple(
         (k, v) for k, v in layered_parameters.items() if k not in RESERVED_KWARGS and k not in handler_fields
     )
     intersection_fields = tuple(
         (k, v) for k, v in handler_fields.items() if k not in RESERVED_KWARGS and k in layered_parameters
     )
 
     for field_name, signature_field in unique_handler_fields:
-        if isinstance(signature_field.kwarg_model, DependencyKwarg) and field_name not in dependencies:
+        if isinstance(signature_field.kwarg_model, DependencyKwarg) and field_name not in dependency_providers:
             # never document explicit dependencies
             continue
 
         for parameter in get_recursive_handler_parameters(
-            dependency_providers=dependencies,
             field_name=field_name,
-            generate_examples=generate_examples,
-            path_parameters=path_parameters,
-            route_handler=route_handler,
-            schemas=schemas,
             signature_field=signature_field,
+            dependency_providers=dependency_providers,
+            route_handler=route_handler,
+            path_parameters=path_parameters,
+            schema_creator=schema_creator,
         ):
             parameters.add(parameter)
 
     for field_name, signature_field in unique_layered_fields:
         parameters.add(
             create_parameter(
-                generate_examples=generate_examples,
+                signature_field=signature_field,
                 parameter_name=field_name,
                 path_parameters=path_parameters,
-                schemas=schemas,
-                signature_field=signature_field,
+                schema_creator=schema_creator,
             )
         )
 
     for field_name, signature_field in intersection_fields:
         parameters.add(
             get_layered_parameter(
                 field_name=field_name,
-                generate_examples=generate_examples,
+                signature_field=signature_field,
                 layered_parameters=layered_parameters,
                 path_parameters=path_parameters,
-                schemas=schemas,
-                signature_field=signature_field,
+                schema_creator=schema_creator,
             )
         )
 
     return parameters.list()
```

### Comparing `litestar-2.0.0b1/litestar/_openapi/path_item.py` & `litestar-2.0.0b2/litestar/_openapi/path_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from inspect import cleandoc
 from typing import TYPE_CHECKING
 
 from litestar._openapi.parameters import create_parameter_for_handler
 from litestar._openapi.request_body import create_request_body
 from litestar._openapi.responses import create_responses
+from litestar._openapi.schema_generation import SchemaCreator
 from litestar._openapi.utils import SEPARATORS_CLEANUP_PATTERN
 from litestar.openapi.spec.path_item import PathItem
 from litestar.utils.helpers import unwrap_partial
 
 __all__ = ("create_path_item", "extract_layered_values", "get_description_for_handler")
 
 
@@ -82,56 +83,51 @@
 
     Returns:
         A tuple containing the path item and a list of operation ids.
     """
     path_item = PathItem()
     operation_ids: list[str] = []
 
+    request_schema_creator = SchemaCreator(create_examples, plugins, schemas, prefer_alias=True)
+    response_schema_creator = SchemaCreator(create_examples, plugins, schemas, prefer_alias=False)
     for http_method, handler_tuple in route.route_handler_map.items():
         route_handler, _ = handler_tuple
 
         if route_handler.include_in_schema:
             handler_fields = route_handler.signature_model.fields if route_handler.signature_model else {}
             parameters = (
                 create_parameter_for_handler(
                     route_handler=route_handler,
                     handler_fields=handler_fields,
                     path_parameters=route.path_parameters,
-                    generate_examples=create_examples,
-                    schemas=schemas,
+                    schema_creator=request_schema_creator,
                 )
                 or None
             )
             raises_validation_error = bool("data" in handler_fields or path_item.parameters or parameters)
 
             request_body = None
             if "data" in handler_fields:
                 request_body = create_request_body(
-                    route_handler=route_handler,
-                    field=handler_fields["data"],
-                    generate_examples=create_examples,
-                    plugins=plugins,
-                    schemas=schemas,
+                    route_handler=route_handler, field=handler_fields["data"], schema_creator=request_schema_creator
                 )
             operation_id = route_handler.operation_id or operation_id_creator(
                 route_handler, http_method, route.path_components
             )
             tags, security = extract_layered_values(route_handler)
             operation = route_handler.operation_class(
                 operation_id=operation_id,
                 tags=tags,
                 summary=route_handler.summary or SEPARATORS_CLEANUP_PATTERN.sub("", route_handler.handler_name.title()),
                 description=get_description_for_handler(route_handler, use_handler_docstrings),
                 deprecated=route_handler.deprecated,
                 responses=create_responses(
                     route_handler=route_handler,
                     raises_validation_error=raises_validation_error,
-                    generate_examples=create_examples,
-                    plugins=plugins,
-                    schemas=schemas,
+                    schema_creator=response_schema_creator,
                 ),
                 request_body=request_body,
                 parameters=parameters,  # type: ignore[arg-type]
                 security=security,
             )
             operation_ids.append(operation_id)
             setattr(path_item, http_method.lower(), operation)
```

### Comparing `litestar-2.0.0b1/litestar/_openapi/request_body.py` & `litestar-2.0.0b2/litestar/_openapi/request_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from litestar._openapi.schema_generation import create_schema
 from litestar.enums import RequestEncodingType
 from litestar.openapi.spec.media_type import OpenAPIMediaType
 from litestar.openapi.spec.request_body import RequestBody
 from litestar.params import BodyKwarg
 
 __all__ = ("create_request_body",)
 
 
 if TYPE_CHECKING:
+    from litestar._openapi.schema_generation import SchemaCreator
     from litestar._signature.field import SignatureField
     from litestar.handlers import BaseRouteHandler
-    from litestar.openapi.spec import Schema
-    from litestar.plugins import OpenAPISchemaPluginProtocol
 
 
 def create_request_body(
-    route_handler: BaseRouteHandler,
-    field: SignatureField,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
+    route_handler: BaseRouteHandler, field: SignatureField, schema_creator: SchemaCreator
 ) -> RequestBody | None:
     """Create a RequestBody model for the given RouteHandler or return None."""
     media_type: RequestEncodingType | str = RequestEncodingType.JSON
     if isinstance(field.kwarg_model, BodyKwarg) and field.kwarg_model.media_type:
         media_type = field.kwarg_model.media_type
 
     if dto := route_handler.resolve_dto():
-        schema = dto.create_openapi_schema("data", str(route_handler), generate_examples, schemas, True)
+        schema = dto.create_openapi_schema("data", str(route_handler), schema_creator)
     else:
-        schema = create_schema(
-            field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas, prefer_alias=True
-        )
+        schema = schema_creator.for_field(field)
 
     return RequestBody(required=True, content={media_type: OpenAPIMediaType(schema=schema)})
```

### Comparing `litestar-2.0.0b1/litestar/_openapi/responses.py` & `litestar-2.0.0b2/litestar/_openapi/responses.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from copy import copy
 from dataclasses import asdict
 from http import HTTPStatus
 from inspect import Signature
 from operator import attrgetter
 from typing import TYPE_CHECKING, Any, Iterator
 
-from litestar._openapi.schema_generation import create_schema
 from litestar._signature.field import SignatureField
 from litestar.enums import MediaType
 from litestar.exceptions import HTTPException, ValidationException
 from litestar.openapi.spec import OpenAPIResponse
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.header import OpenAPIHeader
 from litestar.openapi.spec.media_type import OpenAPIMediaType
@@ -27,18 +26,18 @@
     Response as LitestarResponse,
 )
 from litestar.response.base import ASGIResponse
 from litestar.types.builtin_types import NoneType
 from litestar.utils import get_enum_string_value, get_name
 
 if TYPE_CHECKING:
+    from litestar._openapi.schema_generation import SchemaCreator
     from litestar.datastructures.cookie import Cookie
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.openapi.spec.responses import Responses
-    from litestar.plugins import OpenAPISchemaPluginProtocol
 
 
 __all__ = (
     "create_additional_responses",
     "create_cookie_schema",
     "create_error_responses",
     "create_responses",
@@ -65,18 +64,15 @@
     cookie_copy = copy(cookie)
     cookie_copy.value = "<string>"
     value = cookie_copy.to_header(header="")
     return Schema(description=cookie.description or "", example=value)
 
 
 def create_success_response(  # noqa: C901
-    route_handler: HTTPRouteHandler,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
+    route_handler: HTTPRouteHandler, schema_creator: SchemaCreator
 ) -> OpenAPIResponse:
     """Create the schema for a success response."""
     return_type = route_handler.parsed_fn_signature.return_type
     return_annotation = return_type.annotation
     default_descriptions: dict[Any, str] = {
         Stream: "Stream Response",
         Redirect: "Redirect Response",
@@ -87,41 +83,34 @@
         or default_descriptions.get(return_annotation)
         or HTTPStatus(route_handler.status_code).description
     )
 
     if return_annotation is not Signature.empty and not return_type.is_subclass_of(
         (NoneType, File, Redirect, Stream, ASGIResponse)
     ):
+        media_type = route_handler.media_type
         if return_annotation is Template:
             return_annotation = str
-            route_handler.media_type = get_enum_string_value(MediaType.HTML)
+            media_type = media_type or MediaType.HTML
         elif return_type.is_subclass_of(LitestarResponse):
             return_annotation = return_type.inner_types[0].annotation if return_type.inner_types else Any
-            if not route_handler.media_type:
-                route_handler.media_type = get_enum_string_value(MediaType.JSON)
+            media_type = media_type or MediaType.JSON
 
         if dto := route_handler.resolve_return_dto():
-            result = dto.create_openapi_schema("return", str(route_handler), generate_examples, schemas, False)
+            result = dto.create_openapi_schema("return", str(route_handler), schema_creator)
         else:
-            result = create_schema(
-                field=SignatureField.create(field_type=return_annotation),
-                generate_examples=generate_examples,
-                plugins=plugins,
-                schemas=schemas,
-                prefer_alias=False,
-            )
+            result = schema_creator.for_field(SignatureField.create(return_annotation))
 
-        schema = result if isinstance(result, Schema) else schemas[result.value]
+        schema = result if isinstance(result, Schema) else schema_creator.schemas[result.value]
 
         schema.content_encoding = route_handler.content_encoding
         schema.content_media_type = route_handler.content_media_type
 
         response = OpenAPIResponse(
-            content={route_handler.media_type: OpenAPIMediaType(schema=result)},
-            description=description,
+            content={get_enum_string_value(media_type): OpenAPIMediaType(schema=result)}, description=description
         )
 
     elif return_type.is_subclass_of(Redirect):
         response = OpenAPIResponse(
             content=None,
             description=description,
             headers={
@@ -160,26 +149,20 @@
             content=None,
             description=description,
         )
 
     if response.headers is None:
         response.headers = {}
 
+    no_examples_schema_creator = schema_creator.not_generating_examples
     for response_header in route_handler.resolve_response_headers():
         header = OpenAPIHeader()
         for attribute_name, attribute_value in ((k, v) for k, v in asdict(response_header).items() if v is not None):
             if attribute_name == "value":
-                header.schema = create_schema(
-                    field=SignatureField.create(field_type=type(attribute_value)),
-                    generate_examples=False,
-                    plugins=plugins,
-                    schemas=schemas,
-                    prefer_alias=False,
-                )
-
+                header.schema = no_examples_schema_creator.for_field(SignatureField.create(type(attribute_value)))
             elif attribute_name != "documentation_only":
                 setattr(header, attribute_name, attribute_value)
 
         response.headers[response_header.name] = header
 
     if cookies := route_handler.resolve_response_cookies():
         response.headers["Set-Cookie"] = OpenAPIHeader(
@@ -222,56 +205,41 @@
         yield str(status_code), OpenAPIResponse(
             description=HTTPStatus(status_code).description,
             content={MediaType.JSON: OpenAPIMediaType(schema=schema)},
         )
 
 
 def create_additional_responses(
-    route_handler: HTTPRouteHandler,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
+    route_handler: HTTPRouteHandler, schema_creator: SchemaCreator
 ) -> Iterator[tuple[str, OpenAPIResponse]]:
     """Create the schema for additional responses, if any."""
     if not route_handler.responses:
         return
 
+    schema_creator = copy(schema_creator)
     for status_code, additional_response in route_handler.responses.items():
-        schema = create_schema(
-            field=SignatureField.create(field_type=additional_response.data_container),
-            generate_examples=additional_response.generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=False,
-        )
+        schema_creator.generate_examples = additional_response.generate_examples
+        schema = schema_creator.for_field(SignatureField.create(additional_response.data_container))
         yield str(status_code), OpenAPIResponse(
             description=additional_response.description,
             content={additional_response.media_type: OpenAPIMediaType(schema=schema)},
         )
 
 
 def create_responses(
-    route_handler: HTTPRouteHandler,
-    raises_validation_error: bool,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
+    route_handler: HTTPRouteHandler, raises_validation_error: bool, schema_creator: SchemaCreator
 ) -> Responses | None:
     """Create a Response model embedded in a `Responses` dictionary for the given RouteHandler or return None."""
-
     responses: Responses = {
-        str(route_handler.status_code): create_success_response(
-            generate_examples=generate_examples, plugins=plugins, route_handler=route_handler, schemas=schemas
-        ),
+        str(route_handler.status_code): create_success_response(route_handler, schema_creator),
     }
 
     exceptions = list(route_handler.raises or [])
     if raises_validation_error and ValidationException not in exceptions:
         exceptions.append(ValidationException)
     for status_code, response in create_error_responses(exceptions=exceptions):
         responses[status_code] = response
 
-    for status_code, response in create_additional_responses(
-        route_handler=route_handler, plugins=plugins, schemas=schemas
-    ):
+    for status_code, response in create_additional_responses(route_handler, schema_creator):
         responses[status_code] = response
 
     return responses or None
```

### Comparing `litestar-2.0.0b1/litestar/_openapi/schema_generation/examples.py` & `litestar-2.0.0b2/litestar/_openapi/schema_generation/examples.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
+from dataclasses import replace
 from enum import Enum
 from typing import TYPE_CHECKING, Any
 
 from _decimal import Decimal
 from polyfactory.exceptions import ParameterException
 from polyfactory.field_meta import FieldMeta, Null
+from polyfactory.utils.helpers import unwrap_annotation
 
 from litestar.openapi.spec import Example
 from litestar.types import Empty
 from litestar.utils import is_pydantic_model_instance
 
 try:
     from polyfactory.factories.pydantic_factory import ModelFactory as Factory
@@ -17,16 +19,20 @@
     from polyfactory.factories import DataclassFactory as Factory  # type: ignore[assignment]
 
 
 if TYPE_CHECKING:
     from litestar._signature.field import SignatureField
 
 
+Factory.seed_random(10)
+
+
 def _normalize_example_value(value: Any) -> Any:
     """Normalize the example value to make it look a bit prettier."""
+    value = unwrap_annotation(annotation=value, random=Factory.__random__)
     if isinstance(value, (Decimal, float)):
         value = round(float(value), 2)
     if isinstance(value, Enum):
         value = value.value
     if is_pydantic_model_instance(value):
         value = value.dict()
     if isinstance(value, (list, set)):
@@ -34,31 +40,31 @@
     if isinstance(value, dict):
         for k, v in value.items():
             value[k] = _normalize_example_value(v)
     return value
 
 
 def _create_field_meta(field: SignatureField) -> FieldMeta:
-    return FieldMeta(
-        name=field.name,
+    return FieldMeta.from_type(
         annotation=field.field_type,
         constraints={"constant": field.is_const},
         default=field.default_value if field.default_value is not Empty else Null,
-        children=[_create_field_meta(child) for child in field.children] if field.children else None,
+        name=field.name,
+        random=Factory.__random__,
     )
 
 
 def create_examples_for_field(field: SignatureField) -> list[Example]:
     """Create an OpenAPI Example instance.
 
     Args:
         field: A signature field.
 
     Returns:
         A list including a single example.
     """
     try:
-        field_meta = _create_field_meta(field)
-        value = _normalize_example_value(Factory.get_field_value(field_meta))
+        field_meta = _create_field_meta(replace(field, field_type=_normalize_example_value(field.field_type)))
+        value = Factory.get_field_value(field_meta)
         return [Example(description=f"Example {field.name} value", value=value)]
-    except ParameterException:  # pragma: no cover
+    except ParameterException:
         return []
```

### Comparing `litestar-2.0.0b1/litestar/_openapi/schema_generation/schema.py` & `litestar-2.0.0b2/litestar/_openapi/schema_generation/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,24 +22,29 @@
     MutableMapping,
     MutableSequence,
     OrderedDict,
     Pattern,
     Sequence,
     Set,
     Tuple,
+    Union,
     cast,
+    get_origin,
 )
 from uuid import UUID
 
 from _decimal import Decimal
 from msgspec.structs import fields as msgspec_struct_fields
-from typing_extensions import get_args, get_type_hints
+from polyfactory.utils.predicates import is_safe_subclass
+from typing_extensions import NotRequired, Required, get_args, get_type_hints
 
 from litestar._openapi.schema_generation.constrained_fields import (
-    create_constrained_field_schema,
+    create_date_constrained_field_schema,
+    create_numerical_constrained_field_schema,
+    create_string_constrained_field_schema,
 )
 from litestar._openapi.schema_generation.examples import create_examples_for_field
 from litestar._openapi.schema_generation.utils import sort_schemas_and_references
 from litestar._signature.field import SignatureField
 from litestar.constants import UNDEFINED_SENTINELS
 from litestar.datastructures import UploadFile
 from litestar.exceptions import ImproperlyConfiguredException
@@ -199,15 +204,14 @@
         pydantic.StrictFloat: Schema(type=OpenAPIType.NUMBER),
         pydantic.StrictInt: Schema(type=OpenAPIType.INTEGER),
         pydantic.StrictStr: Schema(type=OpenAPIType.STRING),
     }
 except ImportError:
     PYDANTIC_TYPE_MAP = {}
 
-__all__ = ("create_schema",)
 
 KWARG_MODEL_ATTRIBUTE_TO_OPENAPI_PROPERTY_MAP: dict[str, str] = {
     "default": "default",
     "multiple_of": "multipleOf",
     "ge": "minimum",
     "le": "maximum",
     "lt": "exclusiveMaximum",
@@ -296,49 +300,49 @@
         A schema instance.
     """
     enum_values: list[str | int] = [v.value for v in annotation]  # type: ignore
     openapi_type = OpenAPIType.STRING if isinstance(enum_values[0], str) else OpenAPIType.INTEGER
     return Schema(type=openapi_type, enum=enum_values)
 
 
-def iter_flat_literal_args(annotation: Any) -> Iterable[Any]:
+def _iter_flat_literal_args(annotation: Any) -> Iterable[Any]:
     """Iterate over the flattened arguments of a Literal.
 
     Args:
         annotation: An Literal annotation.
 
     Yields:
         The flattened arguments of the Literal.
     """
     for arg in get_args(annotation):
         if get_origin_or_inner_type(arg) is Literal:
-            yield from iter_flat_literal_args(arg)
+            yield from _iter_flat_literal_args(arg)
         else:
             yield arg
 
 
 def create_literal_schema(annotation: Any) -> Schema:
     """Create a schema instance for a Literal.
 
     Args:
         annotation: An Literal annotation.
 
     Returns:
         A schema instance.
     """
-    args = tuple(iter_flat_literal_args(annotation))
+    args = tuple(_iter_flat_literal_args(annotation))
     schema = copy(TYPE_MAP[type(args[0])])
     if len(args) > 1:
         schema.enum = args
     else:
         schema.const = args[0]
     return schema
 
 
-def create_schema_for_annotation(annotation: Any) -> Schema | None:
+def create_schema_for_annotation(annotation: Any) -> Schema:
     """Get a schema from the type mapping - if possible.
 
     Args:
         annotation: A type annotation.
 
     Returns:
         A schema instance or None.
@@ -346,666 +350,450 @@
 
     if annotation in TYPE_MAP:
         return copy(TYPE_MAP[annotation])
 
     if isinstance(annotation, EnumMeta):
         return create_enum_schema(annotation)
 
-    return None
+    return Schema()
 
 
-def create_schema_for_optional_field(
-    field: SignatureField,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema:
-    """Create a Schema for an optional SignatureField.
+class SchemaCreator:
+    __slots__ = ("generate_examples", "plugins", "schemas", "prefer_alias")
 
-    Args:
-        field: A signature field instance.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
-
-    Returns:
-        A schema instance.
-    """
-    schema_or_reference = create_schema(
-        field=SignatureField.create(
-            field_type=make_non_optional_union(field.field_type),
-            name=field.name,
-            default_value=field.default_value,
-        ),
-        generate_examples=generate_examples,
-        plugins=plugins,
-        schemas=schemas,
-        prefer_alias=prefer_alias,
-    )
-
-    if isinstance(schema_or_reference, Schema) and isinstance(schema_or_reference.one_of, list):
-        result: list[Schema | Reference] = schema_or_reference.one_of
-    else:
-        result = [schema_or_reference]
+    def __init__(
+        self,
+        generate_examples: bool = False,
+        plugins: list[OpenAPISchemaPluginProtocol] | None = None,
+        schemas: dict[str, Schema] | None = None,
+        prefer_alias: bool = True,
+    ) -> None:
+        """Instantiate a SchemaCreator.
+
+        Args:
+            generate_examples: Whether to generate examples if none are given.
+            plugins: A list of plugins.
+            schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+            prefer_alias: Whether to prefer the alias name for the schema.
+        """
+        self.generate_examples = generate_examples
+        self.plugins = plugins if plugins is not None else []
+        self.schemas = schemas if schemas is not None else {}
+        self.prefer_alias = prefer_alias
+
+    @property
+    def not_generating_examples(self) -> SchemaCreator:
+        """Return a SchemaCreator with generate_examples set to False."""
+        if not self.generate_examples:
+            return self
+        new = copy(self)
+        new.generate_examples = False
+        return new
+
+    def for_field(self, field: SignatureField) -> Schema | Reference:
+        """Create a Schema for a given SignatureField.
+
+        Args:
+            field: A signature field instance.
+
+        Returns:
+            A schema instance.
+        """
+        result: Schema | Reference
+        if field.is_optional:
+            result = self.for_optional_field(field)
+        elif field.is_union:
+            result = self.for_union_field(field)
+        elif is_pydantic_model_class(field.field_type):
+            result = self.for_pydantic_model(field.field_type)
+        elif is_attrs_class(field.field_type):
+            result = self.for_attrs_class(field.field_type)
+        elif is_struct_class(field.field_type):
+            result = self.for_struct_class(field.field_type)
+        elif is_dataclass_class(field.field_type):
+            result = self.for_dataclass(field.field_type)
+        elif is_typed_dict(field.field_type):
+            result = self.for_typed_dict(field.field_type)
+        elif plugins_for_annotation := [
+            plugin for plugin in self.plugins if plugin.is_plugin_supported_type(field.field_type)
+        ]:
+            result = self.for_plugin(field, plugins_for_annotation[0])
+        elif is_pydantic_constrained_field(field.field_type) or (
+            isinstance(field.kwarg_model, (ParameterKwarg, BodyKwarg)) and field.kwarg_model.is_constrained
+        ):
+            result = self.for_constrained_field(field)
+        elif field.children and not field.is_generic:
+            result = self.for_object_type(field)
+        elif field.is_generic and (
+            get_origin_or_inner_type(field.field_type) in (ClassicPagination, CursorPagination, OffsetPagination)
+        ):
+            result = self.for_builtin_generics(field)
+        else:
+            result = create_schema_for_annotation(field.field_type)
 
-    return Schema(
-        one_of=[
-            Schema(type=OpenAPIType.NULL),
-            *result,
-        ]
-    )
-
-
-def create_schema_for_union_field(
-    field: SignatureField,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema:
-    """Create a Schema for a union SignatureField.
+        return self.process_schema_result(field, result) if isinstance(result, Schema) else result
 
-    Args:
-        field: A signature field instance.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
+    def for_optional_field(self, field: SignatureField) -> Schema:
+        """Create a Schema for an optional SignatureField.
 
-    Returns:
-        A schema instance.
-    """
-    return Schema(
-        one_of=sort_schemas_and_references(
-            [
-                create_schema(
-                    field=sub_field,
-                    generate_examples=generate_examples,
-                    plugins=plugins,
-                    schemas=schemas,
-                    prefer_alias=prefer_alias,
-                )
-                for sub_field in field.children or []
-            ]
+        Args:
+            field: A signature field instance.
+
+        Returns:
+            A schema instance.
+        """
+        schema_or_reference = self.for_field(
+            SignatureField.create(
+                field_type=make_non_optional_union(field.field_type),
+                name=field.name,
+                default_value=field.default_value,
+            )
         )
-    )
-
+        if isinstance(schema_or_reference, Schema) and isinstance(schema_or_reference.one_of, list):
+            result = schema_or_reference.one_of
+        else:
+            result = [schema_or_reference]
 
-def create_schema_for_object_type(
-    field: SignatureField,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema:
-    """Create schema for object types (dict, Mapping, list, Sequence etc.) types.
+        return Schema(one_of=[Schema(type=OpenAPIType.NULL), *result])
 
-    Args:
-        field: A signature field instance.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
+    def for_union_field(self, field: SignatureField) -> Schema:
+        """Create a Schema for a union SignatureField.
 
-    Returns:
-        A schema instance.
-    """
-    if field.is_mapping:
-        return Schema(
-            type=OpenAPIType.OBJECT,
-            additional_properties=(
-                create_schema(
-                    field=field.children[1],
-                    generate_examples=generate_examples,
-                    plugins=plugins,
-                    schemas=schemas,
-                    prefer_alias=prefer_alias,
-                )
-                if field.children and len(field.children) == 2
-                else None
-            ),
-        )
-
-    if field.is_non_string_sequence or field.is_non_string_iterable:
-        items = [
-            create_schema(
-                field=sub_field,
-                generate_examples=generate_examples,
-                plugins=plugins,
-                schemas=schemas,
-                prefer_alias=prefer_alias,
+        Args:
+            field: A signature field instance.
+
+        Returns:
+            A schema instance.
+        """
+        return Schema(one_of=sort_schemas_and_references(list(map(self.for_field, field.children or []))))
+
+    def for_object_type(self, field: SignatureField) -> Schema:
+        """Create schema for object types (dict, Mapping, list, Sequence etc.) types.
+
+        Args:
+            field: A signature field instance.
+
+        Returns:
+            A schema instance.
+        """
+        if field.is_mapping:
+            return Schema(
+                type=OpenAPIType.OBJECT,
+                additional_properties=(
+                    self.for_field(field.children[1]) if field.children and len(field.children) == 2 else None
+                ),
             )
-            for sub_field in (field.children or ())
-        ]
-
-        return Schema(
-            type=OpenAPIType.ARRAY,
-            items=Schema(one_of=sort_schemas_and_references(items)) if len(items) > 1 else items[0],
-        )
 
-    if field.is_literal:
-        return create_literal_schema(field.field_type)
-
-    raise ImproperlyConfiguredException(
-        f"Parameter '{field.name}' with type '{field.field_type}' could not be mapped to an Open API type. "
-        f"This can occur if a user-defined generic type is resolved as a parameter. If '{field.name}' should "
-        "not be documented as a parameter, annotate it using the `Dependency` function, e.g., "
-        f"`{field.name}: ... = Dependency(...)`."
-    )
-
-
-def create_schema_for_builtin_generics(
-    field: SignatureField,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema:
-    """Handle builtin generic types.
+        if field.is_non_string_sequence or field.is_non_string_iterable:
+            items = list(map(self.for_field, field.children or ()))
+            return Schema(
+                type=OpenAPIType.ARRAY,
+                items=Schema(one_of=sort_schemas_and_references(items)) if len(items) > 1 else items[0],
+            )
 
-    Args:
-        field: A signature field instance.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
+        if field.is_literal:
+            return create_literal_schema(field.field_type)
 
-    Returns:
-        A schema instance.
-    """
-    origin = get_origin_or_inner_type(field.field_type)
+        raise ImproperlyConfiguredException(
+            f"Parameter '{field.name}' with type '{field.field_type}' could not be mapped to an Open API type. "
+            f"This can occur if a user-defined generic type is resolved as a parameter. If '{field.name}' should "
+            "not be documented as a parameter, annotate it using the `Dependency` function, e.g., "
+            f"`{field.name}: ... = Dependency(...)`."
+        )
+
+    def for_builtin_generics(self, field: SignatureField) -> Schema:
+        """Handle builtin generic types.
+
+        Args:
+            field: A signature field instance.
+
+        Returns:
+            A schema instance.
+        """
+        origin = get_origin_or_inner_type(field.field_type)
+        if origin is ClassicPagination:
+            return Schema(
+                type=OpenAPIType.OBJECT,
+                properties={
+                    "items": Schema(
+                        type=OpenAPIType.ARRAY,
+                        items=self.for_field(field.children[0]),  # type: ignore[index]
+                    ),
+                    "page_size": Schema(type=OpenAPIType.INTEGER, description="Number of items per page."),
+                    "current_page": Schema(type=OpenAPIType.INTEGER, description="Current page number."),
+                    "total_pages": Schema(type=OpenAPIType.INTEGER, description="Total number of pages."),
+                },
+            )
 
-    if origin is ClassicPagination:
-        return Schema(
-            type=OpenAPIType.OBJECT,
-            properties={
-                "items": Schema(
-                    type=OpenAPIType.ARRAY,
-                    items=create_schema(
-                        field=field.children[0],  # type: ignore[index]
-                        generate_examples=generate_examples,
-                        plugins=plugins,
-                        schemas=schemas,
-                        prefer_alias=prefer_alias,
+        if origin is OffsetPagination:
+            return Schema(
+                type=OpenAPIType.OBJECT,
+                properties={
+                    "items": Schema(
+                        type=OpenAPIType.ARRAY,
+                        items=self.for_field(field.children[0]),  # type: ignore[index]
                     ),
-                ),
-                "page_size": Schema(type=OpenAPIType.INTEGER, description="Number of items per page."),
-                "current_page": Schema(type=OpenAPIType.INTEGER, description="Current page number."),
-                "total_pages": Schema(type=OpenAPIType.INTEGER, description="Total number of pages."),
-            },
-        )
+                    "limit": Schema(type=OpenAPIType.INTEGER, description="Maximal number of items to send."),
+                    "offset": Schema(type=OpenAPIType.INTEGER, description="Offset from the beginning of the query."),
+                    "total": Schema(type=OpenAPIType.INTEGER, description="Total number of items."),
+                },
+            )
+
+        cursor_schema = self.not_generating_examples.for_field(field.children[0])  # type: ignore[index]
+        cursor_schema.description = "Unique ID, designating the last identifier in the given data set. This value can be used to request the 'next' batch of records."
 
-    if origin is OffsetPagination:
         return Schema(
             type=OpenAPIType.OBJECT,
             properties={
                 "items": Schema(
-                    type=OpenAPIType.ARRAY,
-                    items=create_schema(
-                        field=field.children[0],  # type: ignore[index]
-                        generate_examples=generate_examples,
-                        plugins=plugins,
-                        schemas=schemas,
-                        prefer_alias=prefer_alias,
-                    ),
+                    type=OpenAPIType.ARRAY, items=self.for_field(field=field.children[1])  # type: ignore[index]
                 ),
-                "limit": Schema(type=OpenAPIType.INTEGER, description="Maximal number of items to send."),
-                "offset": Schema(type=OpenAPIType.INTEGER, description="Offset from the beginning of the query."),
-                "total": Schema(type=OpenAPIType.INTEGER, description="Total number of items."),
+                "cursor": cursor_schema,
+                "results_per_page": Schema(type=OpenAPIType.INTEGER, description="Maximal number of items to send."),
             },
         )
 
-    cursor_schema = create_schema(
-        field=field.children[0],  # type: ignore[index]
-        generate_examples=False,
-        plugins=plugins,
-        schemas=schemas,
-        prefer_alias=prefer_alias,
-    )
-    cursor_schema.description = "Unique ID, designating the last identifier in the given data set. This value can be used to request the 'next' batch of records."
-
-    return Schema(
-        type=OpenAPIType.OBJECT,
-        properties={
-            "items": Schema(
-                type=OpenAPIType.ARRAY,
-                items=create_schema(
-                    field=field.children[1],  # type: ignore[index]
-                    generate_examples=generate_examples,
-                    plugins=plugins,
-                    schemas=schemas,
-                    prefer_alias=prefer_alias,
-                ),
-            ),
-            "cursor": cursor_schema,
-            "results_per_page": Schema(type=OpenAPIType.INTEGER, description="Maximal number of items to send."),
-        },
-    )
-
-
-def create_schema_for_pydantic_model(
-    field_type: type[BaseModel],
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema:
-    """Create a schema object for a given pydantic model class.
-
-    Args:
-        field_type: A pydantic model class.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias over the field name.
-
-    Returns:
-        A schema instance.
-    """
-
-    field_type_hints = get_type_hints(field_type)
-    model_config = getattr(field_type, "__config__", getattr(field_type, "model_config", Empty))
-    title = getattr(model_config, "title", None) if not isinstance(model_config, dict) else model_config.get("title")
-    example = (
-        getattr(model_config, "example", None) if not isinstance(model_config, dict) else model_config.get("example")
-    )
-
-    def get_name(f: ModelField) -> str:
-        return (f.alias or f.name) if prefer_alias else f.name
-
-    return Schema(
-        required=sorted(get_name(field) for field in field_type.__fields__.values() if field.required),
-        properties={
-            get_name(f): create_schema(
-                field=SignatureField.create(
-                    field_type=field_type_hints[f.name], name=get_name(f), default_value=f.field_info
-                ),
-                generate_examples=generate_examples,
-                plugins=plugins,
-                schemas=schemas,
-                prefer_alias=prefer_alias,
-            )
-            for f in field_type.__fields__.values()
-        },
-        type=OpenAPIType.OBJECT,
-        title=title or _get_type_schema_name(field_type),
-        examples=[Example(example)] if example else None,
-    )
-
-
-def create_schema_for_attrs_class(
-    field_type: type[AttrsInstance],
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema:
-    """Create a schema object for a given attrs class.
-
-    Args:
-        field_type: An attrs class.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
-
-    Returns:
-        A schema instance.
-    """
-    from attr import NOTHING
-    from attrs import fields_dict
-
-    field_type_hints = get_type_hints(field_type)
-    return Schema(
-        required=sorted(
-            [
-                field_name
-                for field_name, attribute in fields_dict(field_type).items()
-                if attribute.default is NOTHING and not is_optional_union(field_type_hints[field_name])
-            ]
-        ),
-        properties={
-            k: create_schema(
-                field=SignatureField.create(field_type=v, name=k),
-                generate_examples=generate_examples,
-                plugins=plugins,
-                schemas=schemas,
-                prefer_alias=prefer_alias,
-            )
-            for k, v in field_type_hints.items()
-        },
-        type=OpenAPIType.OBJECT,
-        title=_get_type_schema_name(field_type),
-    )
-
-
-def create_schema_for_struct_class(
-    field_type: type[Struct],
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema:
-    """Create a schema object for a given msgspec.Struct class.
-
-    Args:
-        field_type: A msgspec.Struct class.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
-
-    Returns:
-        A schema instance.
-    """
+    def for_plugin(self, field: SignatureField, plugin: OpenAPISchemaPluginProtocol) -> Schema | Reference:
+        """Create a schema using a plugin.
 
-    return Schema(
-        required=sorted(
-            [
-                field.encode_name
-                for field in msgspec_struct_fields(field_type)
-                if field.required and not is_optional_union(field.type)
-            ]
-        ),
-        properties={
-            field.encode_name: create_schema(
-                field=SignatureField.create(field_type=field.type, name=field.encode_name),
-                generate_examples=generate_examples,
-                plugins=plugins,
-                schemas=schemas,
-                prefer_alias=prefer_alias,
+        Args:
+            field: A signature field instance.
+            plugin: A plugin for the field type.
+
+        Returns:
+            A schema instance.
+        """
+        schema = plugin.to_openapi_schema(field.field_type)
+        if isinstance(schema, SchemaDataContainer):
+            return self.for_field(
+                SignatureField.create(
+                    field_type=schema.data_container,
+                    name=field.name,
+                    default_value=field.default_value,
+                    extra=field.extra,
+                    kwarg_model=field.kwarg_model,
+                )
             )
-            for field in msgspec_struct_fields(field_type)
-        },
-        type=OpenAPIType.OBJECT,
-        title=_get_type_schema_name(field_type),
-    )
+        return schema  # pragma: no cover
 
+    def for_pydantic_model(self, field_type: type[BaseModel]) -> Schema:
+        """Create a schema object for a given pydantic model class.
 
-def create_schema_for_dataclass(
-    field_type: type[DataclassProtocol],
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema:
-    """Create a schema object for a given dataclass class.
+        Args:
+            field_type: A pydantic model class.
 
-    Args:
-        field_type: A dataclass class.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
+        Returns:
+            A schema instance.
+        """
+        field_type_hints = get_type_hints(field_type, include_extras=True)
+        model_config = getattr(field_type, "__config__", getattr(field_type, "model_config", Empty))
+        if isinstance(model_config, dict):
+            title = model_config.get("title")
+            example = model_config.get("example")
+        else:
+            title = getattr(model_config, "title", None)
+            example = getattr(model_config, "example", None)
 
-    Returns:
-        A schema instance.
-    """
-    field_type_hints = get_type_hints(field_type)
-    return Schema(
-        required=sorted(
-            [
-                field.name
-                for field in fields(field_type)
-                if (
-                    field.default is MISSING
-                    and field.default_factory is MISSING
-                    and not is_optional_union(field_type_hints[field.name])
+        return Schema(
+            required=sorted(self.get_field_name(field) for field in field_type.__fields__.values() if field.required),
+            properties={
+                self.get_field_name(f): self.for_field(
+                    SignatureField.create(
+                        field_type=field_type_hints[f.name], name=self.get_field_name(f), default_value=f.field_info
+                    )
                 )
-            ]
-        ),
-        properties={
-            k: create_schema(
-                field=SignatureField.create(field_type=v, name=k),
-                generate_examples=generate_examples,
-                plugins=plugins,
-                schemas=schemas,
-                prefer_alias=prefer_alias,
-            )
-            for k, v in field_type_hints.items()
-        },
-        type=OpenAPIType.OBJECT,
-        title=_get_type_schema_name(field_type),
-    )
+                for f in field_type.__fields__.values()
+            },
+            type=OpenAPIType.OBJECT,
+            title=title or _get_type_schema_name(field_type),
+            examples=[Example(example)] if example else None,
+        )
 
+    def for_attrs_class(self, field_type: type[AttrsInstance]) -> Schema:
+        """Create a schema object for a given attrs class.
 
-def create_schema_for_typed_dict(
-    field_type: TypedDictClass,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema:
-    """Create a schema object for a given typed dict.
+        Args:
+            field_type: An attrs class.
 
-    Args:
-        field_type: A typed-dict class.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
+        Returns:
+            A schema instance.
+        """
+        from attr import NOTHING
+        from attrs import fields_dict
 
-    Returns:
-        A schema instance.
-    """
-    return Schema(
-        required=sorted(getattr(field_type, "__required_keys__", [])),
-        properties={
-            k: create_schema(
-                field=SignatureField.create(field_type=v, name=k),
-                generate_examples=generate_examples,
-                plugins=plugins,
-                schemas=schemas,
-                prefer_alias=prefer_alias,
-            )
-            for k, v in get_type_hints(field_type).items()
-        },
-        type=OpenAPIType.OBJECT,
-        title=_get_type_schema_name(field_type),
-    )
-
-
-def create_schema_for_plugin(
-    field: SignatureField,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-    plugin: OpenAPISchemaPluginProtocol,
-) -> Schema | Reference:
-    """Create a schema using a plugin.
-
-    Args:
-        field: A signature field instance.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
-        plugin: A plugin for the field type.
-
-    Returns:
-        A schema instance.
-    """
-
-    schema: Schema | Reference = plugin.to_openapi_schema(field.field_type)
-    if isinstance(schema, SchemaDataContainer):
-        return create_schema(
-            field=SignatureField.create(
-                field_type=schema.data_container,
-                name=field.name,
-                default_value=field.default_value,
-                extra=field.extra,
-                kwarg_model=field.kwarg_model,
+        field_type_hints = get_type_hints(field_type, include_extras=True)
+        return Schema(
+            required=sorted(
+                [
+                    field_name
+                    for field_name, attribute in fields_dict(field_type).items()
+                    if attribute.default is NOTHING and not is_optional_union(field_type_hints[field_name])
+                ]
             ),
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
+            properties={k: self.for_field(SignatureField.create(v, k)) for k, v in field_type_hints.items()},
+            type=OpenAPIType.OBJECT,
+            title=_get_type_schema_name(field_type),
         )
-    return schema  # pragma: no cover
 
+    def for_struct_class(self, field_type: type[Struct]) -> Schema:
+        """Create a schema object for a given msgspec.Struct class.
 
-def _process_schema_result(
-    field: SignatureField,
-    schema: Schema,
-    generate_examples: bool,
-    schemas: dict[str, Schema],
-) -> Schema | Reference:
-    if field.kwarg_model and field.is_const and not field.is_empty and schema.const is None:
-        schema.const = field.default_value
-
-    if field.kwarg_model:
-        for kwarg_model_key, schema_key in KWARG_MODEL_ATTRIBUTE_TO_OPENAPI_PROPERTY_MAP.items():
-            if (value := getattr(field.kwarg_model, kwarg_model_key, Empty)) and (
-                not isinstance(value, Hashable) or value not in UNDEFINED_SENTINELS
-            ):
-                setattr(schema, schema_key, value)
-
-    if not schema.examples and generate_examples:
-        schema.examples = create_examples_for_field(field=field)
-
-    if schema.title and schema.type in (OpenAPIType.OBJECT, OpenAPIType.ARRAY):
-        if schema.title in schemas and hash(schemas[schema.title]) != hash(schema):
-            raise ImproperlyConfiguredException(
-                f"Two different schemas with the title {schema.title} have been defined.\n\n"
-                f"first: {encode_json(schemas[schema.title].to_schema()).decode()}\n"
-                f"second: {encode_json(schema.to_schema()).decode()}\n\n"
-                f"To fix this issue, either rename the base classes from which these titles are derived or manually"
-                f"set a 'title' kwarg in the route handler."
-            )
-        schemas[schema.title] = schema
-        return Reference(ref=f"#/components/schemas/{schema.title}")
-    return schema
-
+        Args:
+            field_type: A msgspec.Struct class.
 
-def create_schema(
-    field: SignatureField,
-    generate_examples: bool,
-    plugins: list[OpenAPISchemaPluginProtocol],
-    schemas: dict[str, Schema],
-    prefer_alias: bool,
-) -> Schema | Reference:
-    """Create a Schema for a given SignatureField.
-
-    Args:
-        field: A signature field instance.
-        generate_examples: Whether to generate examples if none are given.
-        plugins: A list of plugins.
-        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
-        prefer_alias: Whether to prefer the alias name for the schema.
-
-    Returns:
-        A schema instance.
-    """
-    if field.is_optional:
-        result: Schema | Reference = create_schema_for_optional_field(
-            field=field,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
+        Returns:
+            A schema instance.
+        """
+        return Schema(
+            required=sorted(
+                [
+                    field.encode_name
+                    for field in msgspec_struct_fields(field_type)
+                    if field.required and not is_optional_union(field.type)
+                ]
+            ),
+            properties={
+                field.encode_name: self.for_field(SignatureField.create(field.type, field.encode_name))
+                for field in msgspec_struct_fields(field_type)
+            },
+            type=OpenAPIType.OBJECT,
+            title=_get_type_schema_name(field_type),
         )
 
-    elif field.is_union:
-        result = create_schema_for_union_field(
-            field=field,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
-        )
+    def for_dataclass(self, field_type: type[DataclassProtocol]) -> Schema:
+        """Create a schema object for a given dataclass class.
 
-    elif is_pydantic_model_class(annotation=field.field_type):
-        result = create_schema_for_pydantic_model(
-            field_type=field.field_type,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
-        )
+        Args:
+            field_type: A dataclass class.
 
-    elif is_attrs_class(annotation=field.field_type):
-        result = create_schema_for_attrs_class(
-            field_type=field.field_type,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
+        Returns:
+            A schema instance.
+        """
+        field_type_hints = get_type_hints(field_type, include_extras=True)
+        return Schema(
+            required=sorted(
+                [
+                    field.name
+                    for field in fields(field_type)
+                    if (
+                        field.default is MISSING
+                        and field.default_factory is MISSING
+                        and not is_optional_union(field_type_hints[field.name])
+                    )
+                ]
+            ),
+            properties={k: self.for_field(SignatureField.create(v, k)) for k, v in field_type_hints.items()},
+            type=OpenAPIType.OBJECT,
+            title=_get_type_schema_name(field_type),
         )
 
-    elif is_struct_class(annotation=field.field_type):
-        result = create_schema_for_struct_class(
-            field_type=field.field_type,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
-        )
+    def for_typed_dict(self, field_type: TypedDictClass) -> Schema:
+        """Create a schema object for a given typed dict.
 
-    elif is_dataclass_class(annotation=field.field_type):
-        result = create_schema_for_dataclass(
-            field_type=field.field_type,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
-        )
+        Args:
+            field_type: A typed-dict class.
 
-    elif is_typed_dict(annotation=field.field_type):
-        result = create_schema_for_typed_dict(
-            field_type=field.field_type,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
-        )
+        Returns:
+            A schema instance.
+        """
+        annotations: dict[str, Any] = {}
+        for k, v in get_type_hints(field_type, include_extras=True).items():
+            if get_origin(v) in (Required, NotRequired):
+                annotations[k] = get_args(v)[0]
+            else:
+                annotations[k] = v
 
-    elif plugins_for_annotation := [plugin for plugin in plugins if plugin.is_plugin_supported_type(field.field_type)]:
-        result = create_schema_for_plugin(
-            field=field,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
-            plugin=plugins_for_annotation[0],
+        return Schema(
+            required=sorted(getattr(field_type, "__required_keys__", [])),
+            properties={k: self.for_field(SignatureField.create(v, k)) for k, v in annotations.items()},
+            type=OpenAPIType.OBJECT,
+            title=_get_type_schema_name(field_type),
         )
 
-    elif is_pydantic_constrained_field(field.field_type) or (
-        isinstance(field.kwarg_model, (ParameterKwarg, BodyKwarg)) and field.kwarg_model.is_constrained
-    ):
-        result = create_constrained_field_schema(
-            field_type=field.field_type,
-            children=field.children,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
-            kwargs_model=field.kwarg_model,  # type: ignore[arg-type]
-        )
+    def for_constrained_field(self, field: SignatureField) -> Schema:
+        """Create Schema for Pydantic Constrained fields (created using constr(), conint() and so forth, or by subclassing
+        Constrained*)
+
+        Args:
+            field: A signature field instance.
+
+        Returns:
+            A schema instance.
+        """
+        kwargs_model = cast(Union[ParameterKwarg, BodyKwarg], field.kwarg_model)
+        if any(is_safe_subclass(field.field_type, t) for t in (int, float, Decimal)):
+            return create_numerical_constrained_field_schema(field.field_type, kwargs_model)
+        if any(is_safe_subclass(field.field_type, t) for t in (str, bytes)):  # type: ignore[arg-type]
+            return create_string_constrained_field_schema(field.field_type, kwargs_model)
+        if any(is_safe_subclass(field.field_type, t) for t in (date, datetime)):
+            return create_date_constrained_field_schema(field.field_type, kwargs_model)
+        return self.for_collection_constrained_field(field)
+
+    def for_collection_constrained_field(self, field: SignatureField) -> Schema:
+        """Create Schema from Constrained List/Set field.
+
+        Args:
+            field: A signature field instance.
+
+        Returns:
+            A schema instance.
+        """
+        schema = Schema(type=OpenAPIType.ARRAY)
+        kwargs_model = cast(Union[ParameterKwarg, BodyKwarg], field.kwarg_model)
+        if kwargs_model.min_items:
+            schema.min_items = kwargs_model.min_items
+        if kwargs_model.max_items:
+            schema.max_items = kwargs_model.max_items
+        if any(is_safe_subclass(field.field_type, t) for t in (set, frozenset)):  # type: ignore[arg-type]
+            schema.unique_items = True
+
+        item_creator = self.not_generating_examples
+        if field.children:
+            items = list(map(item_creator.for_field, field.children))
+            if len(items) > 1:
+                schema.items = Schema(one_of=sort_schemas_and_references(items))
+            else:
+                schema.items = items[0]
+        else:
+            schema.items = item_creator.for_field(
+                SignatureField.create(field.field_type.item_type, f"{field.field_type.__name__}Field")
+            )
+        return schema
 
-    elif field.children and not field.is_generic:
-        result = create_schema_for_object_type(
-            field=field,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
-        )
+    def get_field_name(self, field: ModelField) -> str:
+        """Get the preferred name for a model field.
 
-    elif field.is_generic and (
-        get_origin_or_inner_type(field.field_type) in (ClassicPagination, CursorPagination, OffsetPagination)
-    ):
-        result = create_schema_for_builtin_generics(
-            field=field,
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-            prefer_alias=prefer_alias,
-        )
-    else:
-        result = create_schema_for_annotation(annotation=field.field_type) or Schema()
+        Args:
+            field: A model field instance.
 
-    if isinstance(result, Reference):
-        return result
+        Returns:
+            The preferred name for the field.
+        """
+        return (field.alias or field.name) if self.prefer_alias else field.name
+
+    def process_schema_result(self, field: SignatureField, schema: Schema) -> Schema | Reference:
+        if field.kwarg_model and field.is_const and not field.is_empty and schema.const is None:
+            schema.const = field.default_value
+
+        if field.kwarg_model:
+            for kwarg_model_key, schema_key in KWARG_MODEL_ATTRIBUTE_TO_OPENAPI_PROPERTY_MAP.items():
+                if (value := getattr(field.kwarg_model, kwarg_model_key, Empty)) and (
+                    not isinstance(value, Hashable) or value not in UNDEFINED_SENTINELS
+                ):
+                    setattr(schema, schema_key, value)
+
+        if not schema.examples and self.generate_examples:
+            schema.examples = create_examples_for_field(field)
+
+        if schema.title and schema.type in (OpenAPIType.OBJECT, OpenAPIType.ARRAY):
+            if schema.title in self.schemas and hash(self.schemas[schema.title]) != hash(schema):
+                raise ImproperlyConfiguredException(
+                    f"Two different schemas with the title {schema.title} have been defined.\n\n"
+                    f"first: {encode_json(self.schemas[schema.title].to_schema()).decode()}\n"
+                    f"second: {encode_json(schema.to_schema()).decode()}\n\n"
+                    f"To fix this issue, either rename the base classes from which these titles are derived or manually"
+                    f"set a 'title' kwarg in the route handler."
+                )
 
-    return _process_schema_result(field=field, schema=result, generate_examples=generate_examples, schemas=schemas)
+            self.schemas[schema.title] = schema
+            return Reference(ref=f"#/components/schemas/{schema.title}")
+        return schema
```

### Comparing `litestar-2.0.0b1/litestar/_openapi/schema_generation/utils.py` & `litestar-2.0.0b2/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.0.0b2/litestar/_openapi/typescript_converter/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,24 +53,24 @@
                     deref_container(resolve_ref(field_value, components=components), components=components),
                 )
             elif isinstance(field_value, (Schema, dict, list)):
                 setattr(value, field.name, deref_container(field_value, components=components))
     return value
 
 
-def _deref_dict(value: dict, components: Components) -> dict:
+def _deref_dict(value: dict[str, Any], components: Components) -> dict[str, Any]:
     for k, v in value.items():
         if isinstance(v, Reference):
             value[k] = deref_container(resolve_ref(v, components=components), components=components)
         elif isinstance(v, (Schema, dict, list)):
             value[k] = deref_container(v, components=components)
     return value
 
 
-def _deref_list(values: list, components: Components) -> list:
+def _deref_list(values: list[Any], components: Components) -> list[Any]:
     for i, value in enumerate(values):
         if isinstance(value, Reference):
             values[i] = deref_container(resolve_ref(value, components=components), components=components)
         elif isinstance(value, (Schema, (dict, list))):
             values[i] = deref_container(value, components=components)
     return values
```

### Comparing `litestar-2.0.0b1/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.0.0b2/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_openapi/typescript_converter/types.py` & `litestar-2.0.0b2/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_openapi/utils.py` & `litestar-2.0.0b2/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_parsers.py` & `litestar-2.0.0b2/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/_signature/field.py` & `litestar-2.0.0b2/litestar/_signature/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,29 +172,30 @@
         """
         if kwarg_model:
             if default_value is Empty:
                 default_value = kwarg_model.default
 
         elif isinstance(default_value, FieldInfo):
             kwarg_model = _create_metadata_from_type(
-                value=default_value, model=BodyKwarg if name == "data" else ParameterKwarg, field_type=field_type
+                metadata=[default_value], model=BodyKwarg if name == "data" else ParameterKwarg, field_type=field_type
             )
 
         # this is for pydantic v1 only
         elif is_pydantic_constrained_field(field_type):
-            kwarg_model = _create_metadata_from_type(value=field_type, model=ParameterKwarg, field_type=field_type)
+            kwarg_model = _create_metadata_from_type(metadata=[field_type], model=ParameterKwarg, field_type=field_type)
 
         origin = get_origin(field_type)
 
         if not children and origin and (type_args := get_args(field_type)):
             if origin is Annotated:
                 field_type = normalize_type_annotation(type_args[0])
-                kwarg_model = kwarg_model or _create_metadata_from_type(
-                    value=type_args[1], model=BodyKwarg if name == "data" else ParameterKwarg, field_type=field_type
-                )
+                if len(type_args) > 1 and (metadata := list(type_args)[1:]):
+                    kwarg_model = kwarg_model or _create_metadata_from_type(
+                        metadata=metadata, model=BodyKwarg if name == "data" else ParameterKwarg, field_type=field_type
+                    )
             else:
                 children = tuple(SignatureField.create(arg) for arg in type_args)
 
         return SignatureField(
             name=name,
             field_type=normalize_type_annotation(field_type) if field_type is not Empty else Any,
             default_value=default_value if default_value not in UNDEFINED_SENTINELS else Empty,
```

### Comparing `litestar-2.0.0b1/litestar/_signature/models/attrs_signature_model.py` & `litestar-2.0.0b2/litestar/_signature/models/attrs_signature_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from datetime import date, datetime, time, timedelta, timezone
 from functools import lru_cache, partial
 from pathlib import PurePath
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    Union,
     cast,
 )
 from uuid import UUID
 
 from _decimal import Decimal
 from typing_extensions import get_args
 
 from litestar._signature.field import SignatureField
 from litestar._signature.models.base import ErrorMessage, SignatureModel
 from litestar.connection import ASGIConnection, Request, WebSocket
 from litestar.datastructures import ImmutableState, MultiDict, State, UploadFile
 from litestar.exceptions import MissingDependencyException
 from litestar.params import BodyKwarg, DependencyKwarg, ParameterKwarg
 from litestar.types import Empty
-from litestar.utils import compact
 from litestar.utils.predicates import is_optional_union, is_union
 from litestar.utils.typing import get_origin_or_inner_type, make_non_optional_union, unwrap_union
 
 try:
     import attr
     import attrs
     import cattrs
@@ -45,15 +45,15 @@
 except ImportError as e:
     raise MissingDependencyException("pytimeparse", "attrs") from e
 
 if TYPE_CHECKING:
     from litestar.utils.signature import ParsedSignature
 
 __all__ = ("AttrsSignatureModel",)
-key_re = re.compile("@ attribute (.*)|'(.*)'")
+key_re = re.compile("@ (attribute|index) (.*)|'(.*)'")
 TRUE_SET = {"1", "true", "on", "t", "y", "yes"}
 FALSE_SET = {"0", "false", "off", "f", "n", "no"}
 
 try:
     import pydantic
 
     def _structure_base_model(value: Any, cls: type[pydantic.BaseModel]) -> pydantic.BaseModel:
@@ -64,14 +64,19 @@
     pydantic_hooks: list[tuple[type[Any], Callable[[Any, type[Any]], Any]]] = [
         (pydantic.BaseModel, _structure_base_model),
     ]
 except ImportError:
     pydantic_hooks = []
 
 
+StructureException = Union[
+    cattrs.ClassValidationError, cattrs.IterableValidationError, ValueError, TypeError, AttributeError
+]
+
+
 def _pass_through_structure_hook(value: Any, _: type[Any]) -> Any:
     return value
 
 
 def _pass_through_unstructure_hook(value: Any) -> Any:
     return value
 
@@ -234,41 +239,14 @@
             self.register_structure_hook(cls, structure_hook)
             self.register_unstructure_hook(cls, _pass_through_unstructure_hook)
 
 
 _converter: Converter = Converter()
 
 
-def _extract_exceptions(e: Any) -> list[ErrorMessage]:
-    """Extracts and normalizes cattrs exceptions.
-
-    Args:
-        e: An ExceptionGroup - which is a py3.11 feature. We use hasattr instead of instance checks to avoid installing this.
-
-    Returns:
-        A list of normalized exception messages.
-    """
-    messages: list[ErrorMessage] = []
-    if hasattr(e, "exceptions"):
-        for exc in cast("list[Exception]", e.exceptions):
-            if hasattr(exc, "exceptions"):  # pragma: no cover
-                # cattrs raises an exception group, where each exception can potentially be an exception group.
-                # this case is not reproducible in any of our tests - and frankly I have no idea when it would occur,
-                # so this clause is defensive programming only.
-                messages.extend(_extract_exceptions(exc))
-                continue
-            if err_format := [
-                line
-                for line in traceback.format_exception(type(exc), value=exc, tb=exc.__traceback__)
-                if key_re.search(line)
-            ]:
-                messages.append({"key": key_re.findall(compact(err_format)[-1])[0][0].strip(), "message": str(exc)})
-    return messages
-
-
 def _create_validators(
     annotation: Any, kwargs_model: BodyKwarg | ParameterKwarg
 ) -> list[Callable[[Any, attrs.Attribute[Any], Any], Any]] | Callable[[Any, attrs.Attribute[Any], Any], Any]:
     validators: list[Callable[[Any, attrs.Attribute[Any], Any], Any]] = []
 
     for value, validator in [
         (kwargs_model.gt, attrs.validators.gt),
@@ -300,22 +278,130 @@
     """Model that represents a function signature that uses a pydantic specific type or types."""
 
     @classmethod
     def parse_values_from_connection_kwargs(cls, connection: ASGIConnection, **kwargs: Any) -> dict[str, Any]:
         try:
             signature = _converter.structure(obj=kwargs, cl=cls)
         except (cattrs.ClassValidationError, ValueError, TypeError, AttributeError) as e:
-            raise cls._create_exception(messages=_extract_exceptions(e), connection=connection) from e
+            raise cls._create_exception(messages=cls._extract_exceptions(e, connection), connection=connection) from e
 
         return cast("dict[str, Any]", _converter.unstructure(obj=signature))
 
     def to_dict(self) -> dict[str, Any]:
         return attrs.asdict(self)
 
     @classmethod
+    def _extract_exceptions(cls, e: StructureException, connection: ASGIConnection) -> list[ErrorMessage]:
+        """Extracts and normalizes cattrs exceptions.
+
+        Args:
+            e: An ExceptionGroup - which is a py3.11 feature. We use hasattr instead of instance checks to avoid installing this.
+            connection: The connection instance.
+
+        Returns:
+            A list of normalized exception messages.
+        """
+
+        error_messages: list[ErrorMessage] = []
+
+        if isinstance(e, cattrs.ClassValidationError):
+            for exc in cast("list[StructureException]", e.exceptions):
+                if messages := cls._get_messages_from_traceback(exc, connection):
+                    error_messages.extend(messages)
+
+        return error_messages
+
+    @classmethod
+    def _get_messages_from_traceback(cls, exc: StructureException, connection: ASGIConnection) -> list[ErrorMessage]:
+        """Gets a message from an attrs validation error.
+
+        The key will be a dot-separated string of the attribute path that failed
+        validation. The message will be the error message from the exception (or the
+        last exception in the exception group, when applicable).
+
+        Args:
+            exc: The exception to get the message from
+            connection: The connection instance
+
+        Returns:
+            An error message
+        """
+
+        error_data = cls._get_data_from_exception(exc=exc)
+        return cls._get_error_messages(error_data=error_data, connection=connection)
+
+    @classmethod
+    def _get_data_from_exception(
+        cls, exc: StructureException, prefix: str = "", error_data: dict | None = None
+    ) -> dict[str, str]:
+        """Gets the keys from an attrs validation error.
+
+        Handles nested structures (e.g. a model attribute references another
+        model) by going through all exceptions in the exception group
+        """
+
+        error_data = error_data or {}
+
+        if isinstance(exc, (cattrs.ClassValidationError, cattrs.IterableValidationError)):
+            formatted_exception = traceback.format_exception_only(type(exc), value=exc)
+            key = cls._get_key_from_formatted_exception(formatted_exception)
+
+            new_prefix = f"{prefix}.{key}" if prefix else key
+
+            for sub_exc in cast("list[StructureException]", exc.exceptions):
+                error_data = cls._get_data_from_exception(sub_exc, new_prefix, error_data)
+        # when using attrs as the preferred backend validation but
+        # pydantic as the model, you can still get pydantic
+        # validation errors.
+        elif isinstance(exc, pydantic.ValidationError):
+            formatted_exception = traceback.format_exception_only(type(exc), value=exc)
+            key = cls._get_key_from_formatted_exception(formatted_exception)
+
+            for error in exc.errors():
+                error_key = ".".join([key, *[str(loc) for loc in error["loc"]]])
+                error_data[error_key] = error["msg"]
+        else:
+            formatted_exception = traceback.format_exception(type(exc), value=exc, tb=exc.__traceback__)
+            key = cls._get_key_from_formatted_exception(formatted_exception)
+            key = f"{prefix}.{key}" if prefix else key
+
+            error_data[key] = str(exc)
+
+        return error_data
+
+    @classmethod
+    def _get_key_from_formatted_exception(cls, formatted_exception: list[str]) -> str:
+        """Gets the key from a formatted exception."""
+        return next(
+            (key for line in formatted_exception if (match := key_re.findall(line)) and (key := match[0][1].strip())),
+            "",
+        )
+
+    @classmethod
+    def _get_error_messages(cls, error_data: dict[str, str], connection: ASGIConnection) -> list[ErrorMessage]:
+        """Build an error message.
+
+        Args:
+            error_data: A mapping of error location (dot-notated) to their error.
+            connection: An ASGI connection instance.
+
+        Returns:
+            An ErrorMessage
+        """
+
+        messages: list[ErrorMessage] = []
+
+        for key, error in error_data.items():
+            keys = key.split(".")
+            message = super()._build_error_message(keys=keys, exc_msg=error, connection=connection)
+            messages.append(message)
+
+        return messages
+
+    @classmethod
     def populate_signature_fields(cls) -> None:
         cls.fields = {
             k: SignatureField.create(
                 field_type=attribute.type,
                 name=k,
                 default_value=attribute.default if attribute.default is not attr.NOTHING else Empty,
                 kwarg_model=attribute.metadata.get("kwargs_model", None) if attribute.metadata else None,
```

### Comparing `litestar-2.0.0b1/litestar/_signature/models/base.py` & `litestar-2.0.0b2/litestar/_signature/models/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, ClassVar, TypedDict
+from typing import TYPE_CHECKING, Any, ClassVar, Literal, Sequence, TypedDict, cast
 
 from litestar.enums import ScopeType
 from litestar.exceptions import InternalServerException, ValidationException
+from litestar.params import ParameterKwarg
 
 if TYPE_CHECKING:
+    from typing_extensions import NotRequired
+
     from litestar._signature.field import SignatureField
     from litestar.connection import ASGIConnection
     from litestar.utils.signature import ParsedSignature
 
 __all__ = ("SignatureModel",)
 
 
 class ErrorMessage(TypedDict):
-    key: str
+    # key may not be set in some cases, like when a query param is set but
+    # doesn't match the required length during `attrs` validation
+    # in this case, we don't show a key at all as it will be empty
+    key: NotRequired[str]
     message: str
+    source: NotRequired[Literal["cookie", "body", "header", "query"]]
 
 
 class SignatureModel(ABC):
     """Base model for Signature modelling."""
 
     dependency_name_set: ClassVar[set[str]]
     return_annotation: ClassVar[Any]
@@ -36,22 +43,65 @@
             messages: A list of error messages.
 
         Returns:
             An Exception
         """
         method = connection.method if hasattr(connection, "method") else ScopeType.WEBSOCKET  # pyright: ignore
         if client_errors := [
-            err_message for err_message in messages if err_message["key"] not in cls.dependency_name_set
+            err_message
+            for err_message in messages
+            if ("key" in err_message and err_message["key"] not in cls.dependency_name_set) or "key" not in err_message
         ]:
             return ValidationException(detail=f"Validation failed for {method} {connection.url}", extra=client_errors)
         return InternalServerException(
             detail=f"A dependency failed validation for {method} {connection.url}", extra=messages
         )
 
     @classmethod
+    def _build_error_message(cls, keys: Sequence[str], exc_msg: str, connection: ASGIConnection) -> ErrorMessage:
+        """Build an error message.
+
+        Args:
+            keys: A list of keys.
+            exc_msg: A message.
+            connection: An ASGI connection instance.
+
+        Returns:
+            An ErrorMessage
+        """
+
+        message: ErrorMessage = {"message": exc_msg}
+
+        if len(keys) > 1:
+            key_start = 0
+
+            if keys[0] == "data":
+                key_start = 1
+                message["source"] = "body"
+
+            message["key"] = ".".join(keys[key_start:])
+        elif keys:
+            key = keys[0]
+            message["key"] = key
+
+            if key in connection.query_params:
+                message["source"] = cast("Literal['cookie', 'body', 'header', 'query']", "query")
+
+            elif key in cls.fields and isinstance(cls.fields[key].kwarg_model, ParameterKwarg):
+                if cast(ParameterKwarg, cls.fields[key].kwarg_model).cookie:
+                    source = "cookie"
+                elif cast(ParameterKwarg, cls.fields[key].kwarg_model).header:
+                    source = "header"
+                else:
+                    source = "query"
+                message["source"] = cast("Literal['cookie', 'body', 'header', 'query']", source)
+
+        return message
+
+    @classmethod
     @abstractmethod
     def parse_values_from_connection_kwargs(cls, connection: ASGIConnection, **kwargs: Any) -> dict[str, Any]:
         """Extract values from the connection instance and return a dict of parsed values.
 
         Args:
             connection: The ASGI connection instance.
             **kwargs: A dictionary of kwargs.
```

### Comparing `litestar-2.0.0b1/litestar/_signature/models/pydantic_signature_model.py` & `litestar-2.0.0b2/litestar/_signature/models/pydantic_signature_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import asdict
 from typing import TYPE_CHECKING, Any
 
 from pydantic import BaseConfig, BaseModel, ValidationError, create_model
 from pydantic.fields import FieldInfo, ModelField
 
 from litestar._signature.field import SignatureField
-from litestar._signature.models.base import SignatureModel
+from litestar._signature.models.base import ErrorMessage, SignatureModel
 from litestar.constants import UNDEFINED_SENTINELS
 from litestar.params import BodyKwarg, DependencyKwarg, ParameterKwarg
 from litestar.types import Empty
 from litestar.utils.predicates import is_pydantic_constrained_field
 
 if TYPE_CHECKING:
     from litestar.connection import ASGIConnection
@@ -41,18 +41,16 @@
 
         Returns:
             A dictionary of parsed values
         """
         try:
             signature = cls(**kwargs)
         except ValidationError as e:
-            raise cls._create_exception(
-                messages=[{"key": str(exc["loc"][-1]), "message": exc["msg"]} for exc in e.errors()],
-                connection=connection,
-            ) from e
+            messages = cls._get_error_messages(e, connection)
+            raise cls._create_exception(messages=messages, connection=connection) from e
 
         return signature.to_dict()
 
     def to_dict(self) -> dict[str, Any]:
         """Normalize access to the signature model's dictionary method, because different backends use different methods
         for this.
 
@@ -141,16 +139,21 @@
                         default=kwargs_container.default if kwargs_container.default is not Empty else None,
                         kwargs_model=kwargs_container,
                         parsed_parameter=parameter,
                     )
                     if kwargs_container.skip_validation:
                         field_type = Any
                 else:
+                    kwargs: dict[str, Any] = {k: v for k, v in asdict(kwargs_container).items() if v is not Empty}
+
+                    if "pattern" in kwargs:
+                        kwargs["regex"] = kwargs["pattern"]
+
                     field_info = FieldInfo(
-                        **{k: v for k, v in asdict(kwargs_container).items() if v is not Empty},
+                        **kwargs,
                         kwargs_model=kwargs_container,
                         parsed_parameter=parameter,
                     )
             else:
                 field_info = FieldInfo(default=..., parsed_parameter=parameter)
 
                 if is_pydantic_constrained_field(parameter.default):
@@ -162,13 +165,25 @@
 
             field_definitions[parameter.name] = (field_type, field_info)
 
         model: type[PydanticSignatureModel] = create_model(  # type: ignore
             f"{fn_name}_signature_model",
             __base__=PydanticSignatureModel,
             __module__=fn_module or "pydantic.main",
-            **field_definitions,
+            **field_definitions,  # pyright: ignore
         )
         model.return_annotation = parsed_signature.return_type.annotation
         model.dependency_name_set = dependency_names
         model.populate_signature_fields()
         return model
+
+    @classmethod
+    def _get_error_messages(cls, e: ValidationError, connection: ASGIConnection) -> list[ErrorMessage]:
+        """Get error messages from a ValidationError."""
+        messages: list[ErrorMessage] = []
+
+        for exc in e.errors():
+            keys = [str(loc) for loc in exc["loc"]]
+            message = super()._build_error_message(keys=keys, exc_msg=exc["msg"], connection=connection)
+            messages.append(message)
+
+        return messages
```

### Comparing `litestar-2.0.0b1/litestar/_signature/utils.py` & `litestar-2.0.0b2/litestar/_signature/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,16 +143,14 @@
     """
     fn_name = getattr(fn, "__name__", "anonymous")
 
     dependency_names: set[str] = set()
 
     for parameter in parsed_signature.parameters.values():
         if isinstance(parameter.default, DependencyKwarg) and parameter.name not in dependency_name_set:
-            if not parameter.parsed_type.is_optional and (
-                isinstance(parameter.default, DependencyKwarg) and parameter.default.default is Empty
-            ):
+            if not parameter.parsed_type.is_optional and parameter.default.default is Empty:
                 raise ImproperlyConfiguredException(
                     f"Explicit dependency '{parameter.name}' for '{fn_name}' has no default value, "
                     f"or provided dependency."
                 )
             dependency_names.add(parameter.name)
     return dependency_names
```

### Comparing `litestar-2.0.0b1/litestar/app.py` & `litestar-2.0.0b2/litestar/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,54 +158,54 @@
         "template_engine",
         "websocket_class",
         "pdb_on_exception",
     )
 
     def __init__(
         self,
-        route_handlers: OptionalSequence[ControllerRouterHandler] = None,
+        route_handlers: OptionalSequence[ControllerRouterHandler] | None = None,
         *,
-        after_exception: OptionalSequence[AfterExceptionHookHandler] = None,
+        after_exception: OptionalSequence[AfterExceptionHookHandler] | None = None,
         after_request: AfterRequestHookHandler | None = None,
         after_response: AfterResponseHookHandler | None = None,
         allowed_hosts: Sequence[str] | AllowedHostsConfig | None = None,
         before_request: BeforeRequestHookHandler | None = None,
-        before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
+        before_send: OptionalSequence[BeforeMessageSendHookHandler] | None = None,
         cache_control: CacheControlHeader | None = None,
         compression_config: CompressionConfig | None = None,
         cors_config: CORSConfig | None = None,
         csrf_config: CSRFConfig | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         debug: bool | None = None,
         dependencies: Dependencies | None = None,
         etag: ETag | None = None,
         event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
         exception_handlers: ExceptionHandlersMap | None = None,
-        guards: OptionalSequence[Guard] = None,
-        listeners: OptionalSequence[EventListener] = None,
+        guards: OptionalSequence[Guard] | None = None,
+        listeners: OptionalSequence[EventListener] | None = None,
         logging_config: BaseLoggingConfig | EmptyType | None = Empty,
-        middleware: OptionalSequence[Middleware] = None,
+        middleware: OptionalSequence[Middleware] | None = None,
         multipart_form_part_limit: int = 1000,
-        on_app_init: OptionalSequence[OnAppInitHandler] = None,
-        on_shutdown: OptionalSequence[LifespanHook] = None,
-        on_startup: OptionalSequence[LifespanHook] = None,
+        on_app_init: OptionalSequence[OnAppInitHandler] | None = None,
+        on_shutdown: OptionalSequence[LifespanHook] | None = None,
+        on_startup: OptionalSequence[LifespanHook] | None = None,
         openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
         opt: Mapping[str, Any] | None = None,
         parameters: ParametersMap | None = None,
-        plugins: OptionalSequence[PluginProtocol] = None,
+        plugins: OptionalSequence[PluginProtocol] | None = None,
         request_class: type[Request] | None = None,
         response_cache_config: ResponseCacheConfig | None = None,
         response_class: ResponseType | None = None,
         response_cookies: ResponseCookies | None = None,
-        response_headers: OptionalSequence[ResponseHeader] = None,
+        response_headers: OptionalSequence[ResponseHeader] | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
-        security: OptionalSequence[SecurityRequirement] = None,
+        security: OptionalSequence[SecurityRequirement] | None = None,
         signature_namespace: Mapping[str, Any] | None = None,
         state: State | None = None,
-        static_files_config: OptionalSequence[StaticFilesConfig] = None,
+        static_files_config: OptionalSequence[StaticFilesConfig] | None = None,
         stores: StoreRegistry | dict[str, Store] | None = None,
         tags: Sequence[str] | None = None,
         template_config: TemplateConfig | None = None,
         type_encoders: TypeEncodersMap | None = None,
         websocket_class: type[WebSocket] | None = None,
         lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
         pdb_on_exception: bool | None = None,
```

### Comparing `litestar-2.0.0b1/litestar/background_tasks.py` & `litestar-2.0.0b2/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/channels/backends/base.py` & `litestar-2.0.0b2/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/channels/backends/memory.py` & `litestar-2.0.0b2/litestar/channels/backends/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/channels/backends/redis.py` & `litestar-2.0.0b2/litestar/channels/backends/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     @property
     def _pub_sub(self) -> PubSub:
         if self.__pub_sub is None:
             self.__pub_sub = self._redis.pubsub()
         return self.__pub_sub
 
     async def on_startup(self) -> None:
+        # this method should not do anything in this case
         pass
 
     async def on_shutdown(self) -> None:
         await self._pub_sub.reset()
 
     async def subscribe(self, channels: Iterable[str]) -> None:
         """Subscribe to ``channels``, and enable publishing to them"""
```

### Comparing `litestar-2.0.0b1/litestar/channels/plugin.py` & `litestar-2.0.0b2/litestar/channels/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/channels/subscriber.py` & `litestar-2.0.0b2/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/cli/_utils.py` & `litestar-2.0.0b2/litestar/cli/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from itertools import chain
 from os import getenv
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Generator, Iterable, Sequence, TypeVar, cast
 
 from rich import get_console
 from rich.table import Table
-from typing_extensions import Concatenate, ParamSpec
+from typing_extensions import Concatenate, ParamSpec, get_type_hints
 
 from litestar import Litestar, __version__
 from litestar.middleware import DefineMiddleware
 from litestar.utils import get_name
 
 RICH_CLICK_INSTALLED = False
 try:
@@ -153,15 +153,15 @@
     """
 
     def __init__(
         self,
         name: str | None = None,
         commands: dict[str, Command] | Sequence[Command] | None = None,
         **attrs: Any,
-    ):
+    ) -> None:
         """Init ``LitestarGroup``"""
         self.group_class = LitestarGroup
         super().__init__(name=name, commands=commands, **attrs)
 
     def add_command(self, cmd: Command, name: str | None = None) -> None:
         """Add command.
 
@@ -192,15 +192,15 @@
     """
 
     def __init__(
         self,
         name: str | None = None,
         commands: dict[str, Command] | Sequence[Command] | None = None,
         **attrs: Any,
-    ):
+    ) -> None:
         """Init ``LitestarExtensionGroup``"""
         super().__init__(name=name, commands=commands, **attrs)
 
         for entry_point in entry_points(group="litestar.commands"):
             command = entry_point.load()
             _wrap_commands([command])
             self.add_command(command, entry_point.name)
@@ -303,15 +303,17 @@
             app_string = f"{import_path}:create_app"
             console.print(f"Using Litestar factory [bright_blue]{app_string}")
             return LoadedApp(app=module.create_app(), app_path=app_string, is_factory=True)
 
         for attr, value in module.__dict__.items():
             if not callable(value):
                 continue
-            return_annotation = getattr(value, "__annotations__", {}).get("return")
+            return_annotation = (
+                get_type_hints(value, include_extras=True).get("return") if hasattr(value, "__annotations__") else None
+            )
             if not return_annotation:
                 continue
             if return_annotation in ("Litestar", Litestar):
                 app_string = f"{import_path}:{attr}"
                 console.print(f"Using Litestar factory [bright_blue]{app_string}")
                 return LoadedApp(app=value(), app_path=f"{app_string}", is_factory=True)
```

### Comparing `litestar-2.0.0b1/litestar/cli/commands/core.py` & `litestar-2.0.0b2/litestar/cli/commands/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/cli/commands/schema.py` & `litestar-2.0.0b2/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/cli/commands/sessions.py` & `litestar-2.0.0b2/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/cli/main.py` & `litestar-2.0.0b2/litestar/cli/main.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/config/allowed_hosts.py` & `litestar-2.0.0b2/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/config/app.py` & `litestar-2.0.0b2/litestar/config/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/config/compression.py` & `litestar-2.0.0b2/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/config/cors.py` & `litestar-2.0.0b2/litestar/config/cors.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     Sets the 'Access-Control-Max-Age' header.
     """
 
     def __post_init__(self) -> None:
         self.allow_headers = [v.lower() for v in self.allow_headers]
 
     @cached_property
-    def allowed_origins_regex(self) -> Pattern:
+    def allowed_origins_regex(self) -> Pattern[str]:
         """Get or create a compiled regex for allowed origins.
 
         Returns:
             A compiled regex of the allowed path.
         """
         origins = self.allow_origins
         if self.allow_origin_regex:
```

### Comparing `litestar-2.0.0b1/litestar/config/csrf.py` & `litestar-2.0.0b2/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/config/response_cache.py` & `litestar-2.0.0b2/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/connection/__init__.py` & `litestar-2.0.0b2/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/connection/base.py` & `litestar-2.0.0b2/litestar/connection/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         if self._headers is Empty:
             self.scope.setdefault("headers", [])
             self._headers = self.scope["_headers"] = parse_headers(tuple(self.scope["headers"]))  # type: ignore[typeddict-unknown-key]
 
         return Headers(self._headers)
 
     @property
-    def query_params(self) -> MultiDict:
+    def query_params(self) -> MultiDict[Any]:
         """Return the query parameters of this connection's ``Scope``.
 
         Returns:
             A normalized dict of query parameters. Multiple values for the same key are returned as a list.
         """
         if self._parsed_query is Empty:
             self._parsed_query = self.scope["_parsed_query"] = parse_query_string(self.scope.get("query_string", b""))  # type: ignore
```

### Comparing `litestar-2.0.0b1/litestar/connection/request.py` & `litestar-2.0.0b2/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/connection/websocket.py` & `litestar-2.0.0b2/litestar/connection/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/constants.py` & `litestar-2.0.0b2/litestar/constants.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/htmx/_utils.py` & `litestar-2.0.0b2/litestar/contrib/htmx/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING, Any, Callable, cast
 from urllib.parse import quote
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.serialization import encode_json
 
 __all__ = (
     "HTMXHeaders",
@@ -142,15 +142,15 @@
         "location": get_location_headers,
     }
 
     header: dict[str, Any] = {}
     response: dict[str, Any]
     key: str
     value: Any
+
     for key, value in hx_headers.items():
         if key in ["redirect", "refresh", "location", "replace_url"]:
-            response = htmx_headers_dict[key](value)
-            return response
+            return cast("dict[str, Any]", htmx_headers_dict[key](value))
         if value is not None:
             response = htmx_headers_dict[key](value)
             header.update(response)
     return header
```

### Comparing `litestar-2.0.0b1/litestar/contrib/htmx/request.py` & `litestar-2.0.0b2/litestar/contrib/htmx/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,11 +103,11 @@
 
 
 class HTMXRequest(Request):
     """HTMX Request class to work with HTMX client."""
 
     __slots__ = ("htmx",)
 
-    def __init__(self, scope: Scope, receive: Receive, send: Send):
+    def __init__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """Initialize :class:`HTMXRequest`"""
         super().__init__(scope=scope, receive=receive, send=send)
         self.htmx = HTMXDetails(self)
```

### Comparing `litestar-2.0.0b1/litestar/contrib/htmx/response.py` & `litestar-2.0.0b2/litestar/contrib/htmx/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
     def __init__(
         self,
         redirect_to: str,
         source: str | None = None,
         event: str | None = None,
         target: str | None = None,
-        swap: ReSwapMethod = None,
+        swap: ReSwapMethod | None = None,
         hx_headers: dict[str, Any] | None = None,
         values: dict[str, str] | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize HXLocation, Set status code to 200 (required by HTMX),
         and pass redirect url.
         """
```

### Comparing `litestar-2.0.0b1/litestar/contrib/htmx/types.py` & `litestar-2.0.0b2/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/jinja.py` & `litestar-2.0.0b2/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/jwt/__init__.py` & `litestar-2.0.0b2/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/jwt/jwt_auth.py` & `litestar-2.0.0b2/litestar/contrib/jwt/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/jwt/jwt_token.py` & `litestar-2.0.0b2/litestar/contrib/jwt/jwt_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/jwt/middleware.py` & `litestar-2.0.0b2/litestar/contrib/jwt/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         algorithm: str,
         auth_header: str,
         exclude: str | list[str] | None,
         exclude_opt_key: str,
         retrieve_user_handler: AsyncCallable[[Token, ASGIConnection[Any, Any, Any, Any]], Awaitable[Any]],
         scopes: Scopes,
         token_secret: str,
-    ):
+    ) -> None:
         """Check incoming requests for an encoded token in the auth header specified, and if present retrieve the user
         from persistence using the provided function.
 
         Args:
             algorithm: JWT hashing algorithm to use.
             app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
             auth_header: Request header key from which to retrieve the token. E.g. ``Authorization`` or ``X-Api-Key``.
@@ -116,15 +116,15 @@
         auth_cookie_key: str,
         auth_header: str,
         exclude: str | list[str] | None,
         exclude_opt_key: str,
         retrieve_user_handler: AsyncCallable[[Token, ASGIConnection[Any, Any, Any, Any]], Awaitable[Any]],
         scopes: Scopes,
         token_secret: str,
-    ):
+    ) -> None:
         """Check incoming requests for an encoded token in the auth header or cookie name specified, and if present
         retrieves the user from persistence using the provided function.
 
         Args:
             algorithm: JWT hashing algorithm to use.
             app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
             auth_cookie_key: Cookie name from which to retrieve the token. E.g. ``token`` or ``accessToken``.
```

### Comparing `litestar-2.0.0b1/litestar/contrib/mako.py` & `litestar-2.0.0b2/litestar/contrib/mako.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     from mako.template import Template as _MakoTemplate
     from pydantic import DirectoryPath
 
 
 class MakoTemplate(TemplateProtocol):
     """Mako template, implementing ``TemplateProtocol``"""
 
-    def __init__(self, template: _MakoTemplate, template_callables: list[tuple[str, Callable[[dict[str, Any]], Any]]]):
+    def __init__(
+        self, template: _MakoTemplate, template_callables: list[tuple[str, Callable[[dict[str, Any]], Any]]]
+    ) -> None:
         """Initialize a template.
 
         Args:
             template: Base ``MakoTemplate`` used by the underlying mako-engine
             template_callables: List of callables passed to the template
         """
         super().__init__()
```

### Comparing `litestar-2.0.0b1/litestar/contrib/msgspec.py` & `litestar-2.0.0b2/litestar/contrib/msgspec.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.0.0b2/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/opentelemetry/config.py` & `litestar-2.0.0b2/litestar/contrib/opentelemetry/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Callable
+from typing import TYPE_CHECKING, Any, Callable
 
 from litestar.contrib.opentelemetry._utils import get_route_details_from_scope
 from litestar.contrib.opentelemetry.middleware import (
     OpenTelemetryInstrumentationMiddleware,
 )
 from litestar.exceptions import MissingDependencyException
 from litestar.middleware.base import DefineMiddleware
@@ -32,15 +32,17 @@
 @dataclass
 class OpenTelemetryConfig:
     """Configuration class for the OpenTelemetry middleware.
 
     Consult the [OpenTelemetry ASGI documentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/asgi/asgi.html) for more info about the configuration options.
     """
 
-    scope_span_details_extractor: Callable[[Scope], tuple[str, dict]] = field(default=get_route_details_from_scope)
+    scope_span_details_extractor: Callable[[Scope], tuple[str, dict[str, Any]]] = field(
+        default=get_route_details_from_scope
+    )
     """Callback which should return a string and a tuple, representing the desired default span name and a dictionary
     with any additional span attributes to set.
     """
     server_request_hook_handler: OpenTelemetryHookHandler | None = field(default=None)
     """Optional callback which is called with the server span and ASGI scope object for every incoming request."""
     client_request_hook_handler: OpenTelemetryHookHandler | None = field(default=None)
     """Optional callback which is called with the internal span and an ASGI scope which is sent as a dictionary for when
```

### Comparing `litestar-2.0.0b1/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.0.0b2/litestar/contrib/opentelemetry/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class OpenTelemetryInstrumentationMiddleware(AbstractMiddleware):
     """OpenTelemetry Middleware."""
 
     __slots__ = ("open_telemetry_middleware",)
 
-    def __init__(self, app: ASGIApp, config: OpenTelemetryConfig):
+    def __init__(self, app: ASGIApp, config: OpenTelemetryConfig) -> None:
         """Middleware that adds OpenTelemetry instrumentation to the application.
 
         Args:
             app: The ``next`` ASGI app to call.
             config: An instance of :class:`OpenTelemetryConfig <.contrib.opentelemetry.OpenTelemetryConfig>`
         """
         super().__init__(app=app, scopes=config.scopes, exclude=config.exclude, exclude_opt_key=config.exclude_opt_key)
```

### Comparing `litestar-2.0.0b1/litestar/contrib/pydantic.py` & `litestar-2.0.0b2/litestar/contrib/pydantic.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/repository/abc/_async.py` & `litestar-2.0.0b2/litestar/contrib/repository/abc/_async.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/repository/abc/_sync.py` & `litestar-2.0.0b2/litestar/contrib/repository/abc/_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/repository/filters.py` & `litestar-2.0.0b2/litestar/contrib/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/repository/handlers.py` & `litestar-2.0.0b2/litestar/contrib/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/repository/testing/generic_mock_repository.py` & `litestar-2.0.0b2/litestar/contrib/repository/testing/generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/base.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     """Common attributes for SQLALchemy tables."""
 
     __name__: ClassVar[str]
     __table__: FromClause
 
     # noinspection PyMethodParameters
     @declared_attr.directive
-    def __tablename__(cls) -> str:  # pylint: disable=no-self-argument
+    def __tablename__(cls) -> str:
         """Infer table name from class name."""
         regexp = re.compile("((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z]))")
         return regexp.sub(r"_\1", cls.__name__).lower()
 
     def to_dict(self, exclude: set[str] | None = None) -> dict[str, Any]:
         """Convert model to dictionary.
```

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/dto.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     RelationshipProperty,
 )
 
 from litestar.dto.factory.abc import AbstractDTOFactory
 from litestar.dto.factory.data_structures import FieldDefinition
 from litestar.dto.factory.field import DTO_FIELD_META_KEY, DTOField, Mark
 from litestar.dto.factory.utils import get_model_type_hints
+from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types.empty import Empty
 from litestar.utils.helpers import get_fully_qualified_class_name
 from litestar.utils.signature import ParsedSignature
 
 if TYPE_CHECKING:
     from typing import Any, ClassVar, Collection, Generator
 
@@ -79,18 +80,23 @@
         elif isinstance(orm_descriptor.property, RelationshipProperty):
             elem = orm_descriptor.property
         else:
             raise NotImplementedError(f"Unhandled property type: '{orm_descriptor.property}'")
 
         default, default_factory = _detect_defaults(elem)
 
-        if (parsed_type := model_type_hints[key]).origin is Mapped:
-            (parsed_type,) = parsed_type.inner_types
-        else:
-            raise NotImplementedError(f"Expected 'Mapped' origin, got: '{parsed_type.origin}'")
+        try:
+            if (parsed_type := model_type_hints[key]).origin is Mapped:
+                (parsed_type,) = parsed_type.inner_types
+            else:
+                raise NotImplementedError(f"Expected 'Mapped' origin, got: '{parsed_type.origin}'")
+        except KeyError as e:
+            raise ImproperlyConfiguredException(
+                f"No type information found for '{orm_descriptor}'. Has a type annotation been added to the column?"
+            ) from e
 
         return [
             FieldDefinition(
                 name=key,
                 default=default,
                 parsed_type=parsed_type,
                 default_factory=default_factory,
```

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/common.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 class GenericSQLAlchemyConfig(Generic[EngineT, SessionT, SessionMakerT]):
     """Common SQLAlchemy Configuration."""
 
     create_engine_callable: Callable[[str], EngineT]
     """Callable that creates an :class:`AsyncEngine <sqlalchemy.ext.asyncio.AsyncEngine>` instance or instance of its
     subclass.
     """
-    session_config: GenericSessionConfig
+    session_config: GenericSessionConfig[Any, Any, Any]
     """Configuration options for either the :class:`async_sessionmaker <sqlalchemy.ext.asyncio.async_sessionmaker>`
     or :class:`sessionmaker <sqlalchemy.orm.sessionmaker>`.
     """
     session_maker_class: type[sessionmaker] | type[async_sessionmaker]
     """Sessionmaker class to use."""
     before_send_handler: BeforeMessageSendHookHandler
     """Handler to call before the ASGI message is sent.
```

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/engine.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/engine.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/init/plugin.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/init/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/plugins/serialization.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/plugins/serialization.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from sqlalchemy.orm import DeclarativeBase
 
 from litestar.contrib.sqlalchemy.dto import SQLAlchemyDTO
 from litestar.plugins import SerializationPluginProtocol
 
 from . import _slots_base
@@ -13,22 +13,22 @@
     from litestar.typing import ParsedType
 
 
 class SQLAlchemySerializationPlugin(SerializationPluginProtocol, _slots_base.SlotsBase):
     __slots__ = ()
 
     def __init__(self) -> None:
-        self._type_dto_map: dict[type[DeclarativeBase], type[SQLAlchemyDTO]] = {}
+        self._type_dto_map: dict[type[DeclarativeBase], type[SQLAlchemyDTO[Any]]] = {}
 
     def supports_type(self, parsed_type: ParsedType) -> bool:
         return (
             parsed_type.is_collection and parsed_type.has_inner_subclass_of(DeclarativeBase)
         ) or parsed_type.is_subclass_of(DeclarativeBase)
 
-    def create_dto_for_type(self, parsed_type: ParsedType) -> type[SQLAlchemyDTO]:
+    def create_dto_for_type(self, parsed_type: ParsedType) -> type[SQLAlchemyDTO[Any]]:
         # assumes that the type is a container of SQLAlchemy models or a single SQLAlchemy model
         for inner_type in parsed_type.inner_types:
             if inner_type.is_subclass_of(DeclarativeBase):
                 annotation = inner_type.annotation
                 break
         else:
             annotation = parsed_type.annotation
```

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_async.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Generic, Literal, cast
 
 from sqlalchemy import Result, Select, delete, over, select, text, update
 from sqlalchemy import func as sql_func
 
-from litestar.contrib.repository import (  # noqa: RUF100, F401
-    AbstractAsyncRepository,
-    AbstractSyncRepository,
-    RepositoryError,
-)
+from litestar.contrib.repository import AbstractAsyncRepository, RepositoryError
 from litestar.contrib.repository.filters import (
     BeforeAfter,
     CollectionFilter,
     FilterTypes,
     LimitOffset,
     OrderBy,
     SearchFilter,
@@ -23,16 +19,15 @@
 from .types import ModelT, RowT, SelectT
 
 if TYPE_CHECKING:
     from collections import abc
     from datetime import datetime
 
     from sqlalchemy.engine.interfaces import _CoreSingleExecuteParams
-    from sqlalchemy.ext.asyncio import AsyncSession  # noqa: RUF100, F401
-    from sqlalchemy.orm import Session  # noqa: RUF100, F401
+    from sqlalchemy.ext.asyncio import AsyncSession
 
 
 class SQLAlchemyAsyncRepository(AbstractAsyncRepository[ModelT], Generic[ModelT]):
     """SQLAlchemy based implementation of the repository interface."""
 
     match_fields: list[str] | str | None = None
```

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_sync.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Generic, Literal, cast
 
 from sqlalchemy import Result, Select, delete, over, select, text, update
 from sqlalchemy import func as sql_func
 
-from litestar.contrib.repository import (  # noqa: RUF100, F401
-    AbstractAsyncRepository,
-    AbstractSyncRepository,
-    RepositoryError,
-)
+from litestar.contrib.repository import AbstractSyncRepository, RepositoryError
 from litestar.contrib.repository.filters import (
     BeforeAfter,
     CollectionFilter,
     FilterTypes,
     LimitOffset,
     OrderBy,
     SearchFilter,
@@ -25,16 +21,15 @@
 from .types import ModelT, RowT, SelectT
 
 if TYPE_CHECKING:
     from collections import abc
     from datetime import datetime
 
     from sqlalchemy.engine.interfaces import _CoreSingleExecuteParams
-    from sqlalchemy.ext.asyncio import AsyncSession  # noqa: RUF100, F401
-    from sqlalchemy.orm import Session  # noqa: RUF100, F401
+    from sqlalchemy.orm import Session
 
 
 class SQLAlchemySyncRepository(AbstractSyncRepository[ModelT], Generic[ModelT]):
     """SQLAlchemy based implementation of the repository interface."""
 
     match_fields: list[str] | str | None = None
```

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/_util.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/_util.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/repository/types.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/repository/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/contrib/sqlalchemy/types.py` & `litestar-2.0.0b2/litestar/contrib/sqlalchemy/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     """
 
     impl = ORA_BLOB
     cache_ok = True
 
     @property
-    def python_type(self) -> type[dict]:
+    def python_type(self) -> type[dict[str, Any]]:
         return dict
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Initialize JSON type"""
         self.name = kwargs.pop("name", None)
         self.oracle_strict = kwargs.pop("oracle_strict", True)
```

### Comparing `litestar-2.0.0b1/litestar/controller.py` & `litestar-2.0.0b2/litestar/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from copy import copy
+from copy import copy, deepcopy
+from functools import partial
 from typing import TYPE_CHECKING, Any, Mapping, cast
 
 from litestar._layers.utils import narrow_response_cookies, narrow_response_headers
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers.base import BaseRouteHandler
 from litestar.handlers.http_handlers import HTTPRouteHandler
 from litestar.handlers.websocket_handlers import WebsocketRouteHandler
 from litestar.types.empty import Empty
 from litestar.utils import AsyncCallable, normalize_path
-from litestar.utils.helpers import unwrap_partial
 
 __all__ = ("Controller",)
 
 
 if TYPE_CHECKING:
     from litestar.datastructures import CacheControlHeader, ETag
     from litestar.dto.interface import DTOInterface
@@ -177,30 +177,25 @@
 
     def get_route_handlers(self) -> list[BaseRouteHandler]:
         """Get a controller's route handlers and set the controller as the handlers' owner.
 
         Returns:
             A list containing a copy of the route handlers defined on the controller
         """
+        from litestar import websocket_listener
+
         route_handlers: list[BaseRouteHandler] = []
-        route_handler_fields = [
-            f_name
-            for f_name in dir(self)
-            if f_name not in dir(Controller) and isinstance(getattr(self, f_name), BaseRouteHandler)
-        ]
-
-        for f_name in route_handler_fields:
-            source_route_handler = cast("BaseRouteHandler", getattr(self, f_name))
-
-            route_handler = copy(source_route_handler)
-            if hasattr(route_handler.fn.value, "func"):
-                route_handler.fn.value = unwrap_partial(route_handler.fn.value)
 
-            route_handler.owner = self
-            route_handlers.append(route_handler)
+        for field_name in set(dir(self)) - set(dir(Controller)):
+            if (attr := getattr(self, field_name, None)) and isinstance(attr, BaseRouteHandler):
+                # we are special casing here because the websocket_listener context cannot be deep copied without breaking
+                route_handler = deepcopy(attr) if not isinstance(attr, websocket_listener) else copy(attr)
+                route_handler.fn.value = partial(route_handler.fn.value, self)
+                route_handler.owner = self
+                route_handlers.append(route_handler)
 
         self.validate_route_handlers(route_handlers=route_handlers)
 
         return route_handlers
 
     def validate_route_handlers(self, route_handlers: list[BaseRouteHandler]) -> None:
         """Validate that the combination of path and decorator method or type are unique on the controller.
```

### Comparing `litestar-2.0.0b1/litestar/data_extractors.py` & `litestar-2.0.0b2/litestar/data_extractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 ResponseExtractorField = Literal["status_code", "headers", "body", "cookies"]
 
 
 class ExtractedRequestData(TypedDict, total=False):
     """Dictionary representing extracted request data."""
 
-    body: Coroutine
+    body: Coroutine[Any, Any, Any]
     client: tuple[str, int]
     content_type: tuple[str, dict[str, str]]
     cookies: dict[str, str]
     headers: dict[str, str]
     method: Method
     path: str
     path_params: dict[str, Any]
@@ -84,15 +84,15 @@
         extract_path_params: bool = True,
         extract_query: bool = True,
         extract_scheme: bool = True,
         obfuscate_cookies: set[str] | None = None,
         obfuscate_headers: set[str] | None = None,
         parse_body: bool = False,
         parse_query: bool = False,
-    ):
+    ) -> None:
         """Initialize ``ConnectionDataExtractor``
 
         Args:
             extract_body: Whether to extract body, (for requests only).
             extract_client: Whether to extract the client (host, port) mapping.
             extract_content_type: Whether to extract the content type and any options.
             extract_cookies: Whether to extract cookies.
@@ -301,15 +301,15 @@
         self,
         extract_body: bool = True,
         extract_cookies: bool = True,
         extract_headers: bool = True,
         extract_status_code: bool = True,
         obfuscate_cookies: set[str] | None = None,
         obfuscate_headers: set[str] | None = None,
-    ):
+    ) -> None:
         """Initialize ``ResponseDataExtractor`` with options.
 
         Args:
             extract_body: Whether to extract the body.
             extract_cookies: Whether to extract the cookies.
             extract_headers: Whether to extract the headers.
             extract_status_code: Whether to extract the status code.
```

### Comparing `litestar-2.0.0b1/litestar/datastructures/__init__.py` & `litestar-2.0.0b2/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/datastructures/cookie.py` & `litestar-2.0.0b2/litestar/datastructures/cookie.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Defaults to ``/``.
     """
     value: str | None = field(default=None)
     """Value for the cookie, if none given defaults to empty string."""
     max_age: int | None = field(default=None)
     """Maximal age of the cookie before its invalidated."""
     expires: int | None = field(default=None)
-    """Expiration date as unix MS timestamp."""
+    """Seconds from now until the cookie expires."""
     domain: str | None = field(default=None)
     """Domain for which the cookie is valid."""
     secure: bool | None = field(default=None)
     """Https is required for the cookie."""
     httponly: bool | None = field(default=None)
     """Forbids javascript to access the cookie via ``document.cookie``."""
     samesite: Literal["lax", "strict", "none"] = field(default="lax")
```

### Comparing `litestar-2.0.0b1/litestar/datastructures/headers.py` & `litestar-2.0.0b2/litestar/datastructures/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,20 +387,20 @@
     def validate_value(cls, value: Any, values: Dict[str, Any]) -> Any:
         """Ensure that either value is set or the instance is for ``documentation_only``."""
         if values.get("documentation_only") or value is not None:
             return value
         raise ValueError("value must be set if documentation_only is false")
 
 
-class _MediaType:
+class MediaTypeHeader:
     """A helper class for ``Accept`` header parsing."""
 
     __slots__ = ("maintype", "subtype", "params", "_params_str")
 
-    def __init__(self, type_str: str):
+    def __init__(self, type_str: str) -> None:
         # preserve the original parameters, because the order might be
         # changed in the dict
         self._params_str = "".join(type_str.partition(";")[1:])
 
         full_type, self.params = parse_content_header(type_str)
         self.maintype, _, self.subtype = full_type.partition("/")
 
@@ -424,15 +424,15 @@
             # no params or 'q' is the only one which we ignore
             specificity = 2
         else:
             specificity = 3
 
         return quality, specificity
 
-    def match(self, other: "_MediaType") -> bool:
+    def match(self, other: "MediaTypeHeader") -> bool:
         # Check parameters first, ignore the weight parameter 'q'.
         # Additional parameters on other are also ignored.
         for key, value in self.params.items():
             if key != "q" and value != other.params.get(key):
                 return False
 
         # Then check if the subtypes match, ignoring the wildcard '*'
@@ -447,16 +447,16 @@
 
 
 class Accept:
     """An ``Accept`` header."""
 
     __slots__ = ("_accepted_types",)
 
-    def __init__(self, accept_value: str):
-        self._accepted_types = [_MediaType(t) for t in accept_value.split(",")]
+    def __init__(self, accept_value: str) -> None:
+        self._accepted_types = [MediaTypeHeader(t) for t in accept_value.split(",")]
         self._accepted_types.sort(key=lambda t: t.priority, reverse=True)
 
     def __len__(self) -> int:
         return len(self._accepted_types)
 
     def __getitem__(self, key: int) -> str:
         return str(self._accepted_types[key])
@@ -473,15 +473,15 @@
             default: The media type that is returned if none of the provided types match.
 
         Returns:
             The best matching media type. If the matching provided type contains wildcard characters,
             they are replaced with the corresponding part of the accepted type. Otherwise the
             provided type is returned as-is.
         """
-        types = [_MediaType(t) for t in provided_types]
+        types = [MediaTypeHeader(t) for t in provided_types]
 
         for accepted in self._accepted_types:
             for provided in types:
                 if provided.match(accepted):
                     # Return the accepted type with wildcards replaced
                     # by concrete parts from the provided type
                     result = copy(provided)
```

### Comparing `litestar-2.0.0b1/litestar/datastructures/multi_dicts.py` & `litestar-2.0.0b2/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/datastructures/response_header.py` & `litestar-2.0.0b2/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/datastructures/state.py` & `litestar-2.0.0b2/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/datastructures/upload_file.py` & `litestar-2.0.0b2/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/datastructures/url.py` & `litestar-2.0.0b2/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/di.py` & `litestar-2.0.0b2/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/factory/_backends/abc.py` & `litestar-2.0.0b2/litestar/dto/factory/_backends/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 from __future__ import annotations
 
 import secrets
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Final, Generic, TypeVar, cast
 
-from litestar._openapi.schema_generation import create_schema
 from litestar._signature.field import SignatureField
 from litestar.dto.factory import DTOData, Mark
 from litestar.typing import ParsedType
 from litestar.utils.helpers import get_fully_qualified_class_name
 
 from .types import (
     CollectionType,
@@ -31,14 +30,15 @@
     should_mark_private,
     transfer_data,
 )
 
 if TYPE_CHECKING:
     from typing import AbstractSet, Callable, Generator
 
+    from litestar._openapi.schema_generation import SchemaCreator
     from litestar.dto.factory import DTOConfig
     from litestar.dto.factory.data_structures import FieldDefinition
     from litestar.dto.interface import ConnectionContext
     from litestar.dto.types import ForType
     from litestar.openapi.spec import Reference, Schema
     from litestar.types.serialization import LitestarEncodableType
 
@@ -325,22 +325,17 @@
             destination_type=self.transfer_model_type,  # type: ignore[arg-type]
             source_data=data,
             field_definitions=self.parsed_field_definitions,
             dto_for="return",
             parsed_type=self.context.parsed_type,
         )
 
-    def create_openapi_schema(
-        self, generate_examples: bool, schemas: dict[str, Schema], prefer_alias: bool
-    ) -> Reference | Schema:
+    def create_openapi_schema(self, schema_creator: SchemaCreator) -> Reference | Schema:
         """Create a RequestBody model for the given RouteHandler or return None."""
-        field = SignatureField.create(self.annotation)
-        return create_schema(
-            field=field, generate_examples=generate_examples, plugins=[], schemas=schemas, prefer_alias=prefer_alias
-        )
+        return schema_creator.for_field(SignatureField.create(self.annotation))
 
     def _create_transfer_type(
         self, parsed_type: ParsedType, exclude: AbstractSet[str], field_name: str, unique_name: str, nested_depth: int
     ) -> CompositeType | SimpleType:
         exclude = _filter_exclude(exclude, field_name)
 
         if parsed_type.is_union:
```

### Comparing `litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/backend.py` & `litestar-2.0.0b2/litestar/dto/factory/_backends/msgspec/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, NewType, TypeVar
 
-from msgspec import Struct, from_builtins
+from msgspec import Struct, convert
 
 from litestar.dto.factory._backends.abc import AbstractDTOBackend
 from litestar.serialization import decode_media_type
 
 from .utils import _create_struct_for_field_definitions
 
 if TYPE_CHECKING:
@@ -31,8 +31,8 @@
 
     def parse_raw(self, raw: bytes, connection_context: ConnectionContext) -> Struct | Collection[Struct]:
         return decode_media_type(  # type:ignore[no-any-return]
             raw, connection_context.request_encoding_type, type_=self.annotation
         )
 
     def parse_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
-        return from_builtins(builtins, self.annotation)
+        return convert(builtins, self.annotation)
```

### Comparing `litestar-2.0.0b1/litestar/dto/factory/_backends/msgspec/utils.py` & `litestar-2.0.0b2/litestar/dto/factory/_backends/msgspec/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/backend.py` & `litestar-2.0.0b2/litestar/dto/factory/_backends/pydantic/backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/factory/_backends/pydantic/utils.py` & `litestar-2.0.0b2/litestar/dto/factory/_backends/pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/factory/_backends/types.py` & `litestar-2.0.0b2/litestar/dto/factory/_backends/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/factory/_backends/utils.py` & `litestar-2.0.0b2/litestar/dto/factory/_backends/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/factory/abc.py` & `litestar-2.0.0b2/litestar/dto/factory/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 )
 
 if TYPE_CHECKING:
     from typing import Any, ClassVar, Collection, Generator
 
     from typing_extensions import Self
 
+    from litestar._openapi.schema_generation import SchemaCreator
     from litestar.dto.interface import HandlerContext
     from litestar.dto.types import ForType
     from litestar.openapi.spec import Reference, Schema
     from litestar.types.serialization import LitestarEncodableType
 
     from ._backends import AbstractDTOBackend
     from .data_structures import FieldDefinition
@@ -169,21 +170,20 @@
                 wrapper_attribute_name=wrapper_attribute_name,
             )
             backend = cls._type_backend_map.setdefault(key, backend_type(backend_context))
         cls._handler_backend_map[(handler_context.dto_for, handler_context.handler_id)] = backend
 
     @classmethod
     def create_openapi_schema(
-        cls, dto_for: ForType, handler_id: str, generate_examples: bool, schemas: dict[str, Schema], prefer_alias: bool
+        cls, dto_for: ForType, handler_id: str, schema_creator: SchemaCreator
     ) -> Reference | Schema:
         """Create an OpenAPI request body.
 
         Returns:
             OpenAPI request body.
         """
-        backend = cls._get_backend(dto_for, handler_id)
-        return backend.create_openapi_schema(generate_examples, schemas, prefer_alias)
+        return cls._get_backend(dto_for, handler_id).create_openapi_schema(schema_creator)
 
     @classmethod
     def _get_backend(cls, dto_for: ForType, handler_id: str) -> AbstractDTOBackend:
         """Return the backend for the handler/dto_for combo."""
         return cls._handler_backend_map[(dto_for, handler_id)]
```

### Comparing `litestar-2.0.0b1/litestar/dto/factory/config.py` & `litestar-2.0.0b2/litestar/dto/factory/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/factory/data_structures.py` & `litestar-2.0.0b2/litestar/dto/factory/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class DTOData(Generic[T]):
     """DTO validated data and utility methods."""
 
     __slots__ = ("_backend", "_data_as_builtins")
 
-    def __init__(self, backend: AbstractDTOBackend, data_as_builtins: Any) -> None:
+    def __init__(self, backend: AbstractDTOBackend[Any], data_as_builtins: Any) -> None:
         self._backend = backend
         self._data_as_builtins = data_as_builtins
 
     def create_instance(self, **kwargs: Any) -> T:
         """Create an instance of the DTO validated data.
 
         Args:
@@ -48,15 +48,15 @@
         return instance
 
     def as_builtins(self) -> Any:
         """Return the DTO validated data as builtins."""
         return self._data_as_builtins
 
 
-def _set_nested_dict_value(d: dict, keys: list[str], value: Any) -> None:
+def _set_nested_dict_value(d: dict[str, Any], keys: list[str], value: Any) -> None:
     if len(keys) == 1:
         d[keys[0]] = value
     else:
         key = keys[0]
         d.setdefault(key, {})
         _set_nested_dict_value(d[key], keys[1:], value)
```

### Comparing `litestar-2.0.0b1/litestar/dto/factory/field.py` & `litestar-2.0.0b2/litestar/dto/factory/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/factory/stdlib/dataclass.py` & `litestar-2.0.0b2/litestar/dto/factory/stdlib/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/factory/utils.py` & `litestar-2.0.0b2/litestar/dto/factory/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/dto/interface.py` & `litestar-2.0.0b2/litestar/dto/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from litestar.openapi.spec import Schema
 
 if TYPE_CHECKING:
     from typing import Any, Final
 
     from typing_extensions import Self
 
+    from litestar._openapi.schema_generation import SchemaCreator
     from litestar.openapi.spec import Reference
     from litestar.types import LitestarEncodableType
     from litestar.types.internal_types import AnyConnection
     from litestar.typing import ParsedType
 
     from .types import ForType
 
@@ -105,20 +106,15 @@
 
         Returns:
             Data type that the DTO represents.
         """
 
     @classmethod
     def create_openapi_schema(
-        cls,
-        dto_for: ForType,
-        handler_id: str,
-        generate_examples: bool,
-        schemas: dict[str, Schema],
-        prefer_alias: bool,
+        cls, dto_for: ForType, handler_id: str, schema_creator: SchemaCreator
     ) -> Reference | Schema:
         """Create an OpenAPI request body for the DTO.
 
         Returns:
             An optional :class:`RequestBody <.openapi.spec.request_body.RequestBody>` instance.
         """
         return Schema()
@@ -133,8 +129,7 @@
         Args:
             handler_context: A :class:`HandlerContext <.HandlerContext>` instance. Provides information about the
                 handler and application of the DTO.
 
         Raises:
             UnsupportedType: If the DTO type does not support the annotated type of ``parsed_type``.
         """
-        return
```

### Comparing `litestar-2.0.0b1/litestar/enums.py` & `litestar-2.0.0b2/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/events/emitter.py` & `litestar-2.0.0b2/litestar/events/emitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 class BaseEventEmitterBackend(AsyncContextManager["BaseEventEmitterBackend"], ABC):
     """Abstract class used to define event emitter backends."""
 
     __slots__ = ("listeners",)
 
     listeners: defaultdict[str, set[EventListener]]
 
-    def __init__(self, listeners: Sequence[EventListener]):
+    def __init__(self, listeners: Sequence[EventListener]) -> None:
         """Create an event emitter instance.
 
         Args:
             listeners: A list of listeners.
         """
         self.listeners = defaultdict(set)
         for listener in listeners:
@@ -61,15 +61,15 @@
 
 
 class SimpleEventEmitter(BaseEventEmitterBackend):
     """Event emitter the works only in the current process"""
 
     __slots__ = ("_queue", "_exit_stack", "_receive_stream", "_send_stream")
 
-    def __init__(self, listeners: Sequence[EventListener]):
+    def __init__(self, listeners: Sequence[EventListener]) -> None:
         """Create an event emitter instance.
 
         Args:
             listeners: A list of listeners.
         """
         super().__init__(listeners=listeners)
         self._receive_stream: MemoryObjectReceiveStream | None = None
```

### Comparing `litestar-2.0.0b1/litestar/events/listener.py` & `litestar-2.0.0b2/litestar/events/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class EventListener:
     """Decorator for event listeners"""
 
     __slots__ = ("event_ids", "fn", "listener_id")
 
     fn: AsyncCallable[Any, Any]
 
-    def __init__(self, *event_ids: str):
+    def __init__(self, *event_ids: str) -> None:
         """Create a decorator for event handlers.
 
         Args:
             *event_ids: The id of the event to listen to or a list of
                 event ids to listen to.
         """
         self.event_ids: frozenset[str] = frozenset(event_ids)
```

### Comparing `litestar-2.0.0b1/litestar/exceptions/__init__.py` & `litestar-2.0.0b2/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/exceptions/base_exceptions.py` & `litestar-2.0.0b2/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/exceptions/http_exceptions.py` & `litestar-2.0.0b2/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/exceptions/websocket_exceptions.py` & `litestar-2.0.0b2/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/file_system.py` & `litestar-2.0.0b2/litestar/file_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """
         return await open_file(file=file, mode=mode, buffering=buffering)  # type: ignore
 
 
 class FileSystemAdapter:
     """Wrapper around a ``FileSystemProtocol``, normalising its interface."""
 
-    def __init__(self, file_system: FileSystemProtocol):
+    def __init__(self, file_system: FileSystemProtocol) -> None:
         """Initialize an adapter from a given ``file_system``
 
         Args:
             file_system: A filesystem class adhering to the :class:`FileSystemProtocol <litestar.types.FileSystemProtocol>`
         """
         self.file_system = file_system
```

### Comparing `litestar-2.0.0b1/litestar/handlers/__init__.py` & `litestar-2.0.0b2/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/handlers/asgi_handlers.py` & `litestar-2.0.0b2/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/handlers/base.py` & `litestar-2.0.0b2/litestar/handlers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 from copy import copy
-from functools import partial
 from typing import TYPE_CHECKING, Any, Mapping, Sequence, cast
 
 from litestar._signature import create_signature_model
 from litestar._signature.field import SignatureField
 from litestar.di import Provide
 from litestar.dto.interface import HandlerContext
 from litestar.exceptions import ImproperlyConfiguredException
-from litestar.types import Dependencies, Empty, ExceptionHandlersMap, Guard, Middleware, TypeEncodersMap
+from litestar.types import Dependencies, Empty, ExceptionHandlersMap, Guard, MaybePartial, Middleware, TypeEncodersMap
 from litestar.utils import AsyncCallable, Ref, async_partial, get_name, normalize_path
 from litestar.utils.helpers import unwrap_partial
 from litestar.utils.predicates import is_async_callable
 from litestar.utils.signature import ParsedSignature, infer_request_encoding_from_parameter
 
 if TYPE_CHECKING:
     from typing_extensions import Self
@@ -23,15 +22,14 @@
     from litestar.connection import ASGIConnection
     from litestar.controller import Controller
     from litestar.dto.interface import DTOInterface
     from litestar.params import ParameterKwarg
     from litestar.plugins import SerializationPluginProtocol
     from litestar.router import Router
     from litestar.types import AnyCallable, AsyncAnyCallable, ExceptionHandler
-    from litestar.types.composite_types import MaybePartial
     from litestar.types.empty import EmptyType
 
 __all__ = ("BaseRouteHandler",)
 
 
 class BaseRouteHandler:
     """Base route handler.
@@ -403,19 +401,14 @@
 
     def _set_runtime_callables(self) -> None:
         """Optimize the ``route_handler.fn`` and any ``provider.dependency`` callables for runtime by doing the following:
 
         1. ensure that the ``self`` argument is preserved by binding it using partial.
         2. ensure sync functions are wrapped in AsyncCallable for sync_to_thread handlers.
         """
-        from litestar.controller import Controller
-
-        if isinstance(self.owner, Controller) and not hasattr(self.fn.value, "func"):
-            self.fn.value = partial(self.fn.value, self.owner)
-
         for provider in self.resolve_dependencies().values():
             if not is_async_callable(provider.dependency.value):
                 provider.has_sync_callable = False
                 if provider.sync_to_thread:
                     provider.dependency.value = async_partial(provider.dependency.value)
                 else:
                     provider.has_sync_callable = True
```

### Comparing `litestar-2.0.0b1/litestar/handlers/http_handlers/_utils.py` & `litestar-2.0.0b2/litestar/handlers/http_handlers/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,32 +83,25 @@
             response = await after_request(response)  # type: ignore[arg-type,misc]
 
         return response.to_asgi_response(app=app, request=request, encoded_headers=raw_headers)
 
     return handler
 
 
-def create_generic_asgi_response_handler(
-    after_request: AfterRequestHookHandler | None,
-    cookies: frozenset[Cookie],
-) -> AsyncAnyCallable:
+def create_generic_asgi_response_handler(after_request: AfterRequestHookHandler | None) -> AsyncAnyCallable:
     """Create a handler function for Responses.
 
     Args:
         after_request: An after request handler.
-        cookies: A set of pre-defined cookies.
 
     Returns:
         A handler function.
     """
 
     async def handler(data: ASGIApp, **kwargs: Any) -> ASGIApp:
-        if hasattr(data, "set_cookie"):
-            for cookie in cookies:
-                data.set_cookie(**cookie.dict)
         return await after_request(data) if after_request else data  # type: ignore
 
     return handler
 
 
 @lru_cache(1024)
 def normalize_headers(headers: frozenset[ResponseHeader]) -> dict[str, str]:
```

### Comparing `litestar-2.0.0b1/litestar/handlers/http_handlers/base.py` & `litestar-2.0.0b2/litestar/handlers/http_handlers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,14 @@
     from litestar.config.response_cache import CACHE_FOREVER
     from litestar.connection import Request
     from litestar.datastructures import CacheControlHeader, ETag
     from litestar.datastructures.headers import Header
     from litestar.dto.interface import DTOInterface
     from litestar.openapi.datastructures import ResponseSpec
     from litestar.openapi.spec import SecurityRequirement
-    from litestar.types import MaybePartial  # noqa: F401
-
 
 __all__ = ("HTTPRouteHandler", "route")
 
 
 class ResponseHandlerMap(TypedDict):
     default_handler: Callable[[Any], Awaitable[ASGIApp]] | EmptyType
     response_type_handler: Callable[[Any], Awaitable[ASGIApp]] | EmptyType
@@ -431,15 +429,15 @@
                 type_encoders=type_encoders,
             )
 
             if return_type.is_subclass_of(Response):
                 self._response_handler_mapping["default_handler"] = response_type_handler
             elif is_async_callable(return_annotation) or return_annotation is ASGIApp:
                 self._response_handler_mapping["default_handler"] = create_generic_asgi_response_handler(
-                    after_request=after_request, cookies=cookies
+                    after_request=after_request
                 )
             else:
                 self._response_handler_mapping["default_handler"] = create_data_handler(
                     after_request=after_request,
                     background=self.background,
                     cookies=cookies,
                     headers=headers,
```

### Comparing `litestar-2.0.0b1/litestar/handlers/http_handlers/decorators.py` & `litestar-2.0.0b2/litestar/handlers/http_handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.0.0b2/litestar/handlers/websocket_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.0.0b2/litestar/handlers/websocket_handlers/listener.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,22 @@
     Middleware,
     TypeEncodersMap,
 )
 from litestar.types.builtin_types import NoneType
 from litestar.utils import AsyncCallable
 from litestar.utils.signature import ParsedSignature
 
-from . import _utils
+from ._utils import (
+    ListenerContext,
+    create_handle_receive,
+    create_handle_send,
+    create_handler_function,
+    create_handler_signature,
+    create_stub_dependency,
+)
 from .route_handler import WebsocketRouteHandler
 
 if TYPE_CHECKING:
     from typing import Coroutine
 
     from litestar import Litestar, Router
     from litestar.dto.interface import DTOInterface
@@ -56,14 +63,15 @@
     returned
     """
 
     __slots__ = {
         "connection_accept_handler": "Callback to accept a WebSocket connection. By default, calls WebSocket.accept",
         "on_accept": "Callback invoked after a WebSocket connection has been accepted",
         "on_disconnect": "Callback invoked after a WebSocket connection has been closed",
+        "_initialized": None,
         "_pass_socket": None,
         "_receive_mode": None,
         "_send_mode": None,
         "_listener_context": None,
         "_connection_lifespan": None,
         "_dependency_stubs": None,
     }
@@ -170,16 +178,15 @@
             **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
         if connection_lifespan and any([on_accept, on_disconnect, connection_accept_handler is not WebSocket.accept]):
             raise ImproperlyConfiguredException(
                 "connection_lifespan can not be used with connection hooks "
                 "(on_accept, on_disconnect, connection_accept_handler)",
             )
-
-        self._listener_context = _utils.ListenerContext()
+        self._listener_context = ListenerContext()
         self._receive_mode: WebSocketMode = receive_mode
         self._send_mode: WebSocketMode = send_mode
         self._connection_lifespan = connection_lifespan
 
         self.connection_accept_handler = connection_accept_handler
         self.on_accept = AsyncCallable(on_accept) if on_accept else None
         self.on_disconnect = AsyncCallable(on_disconnect) if on_disconnect else None
@@ -193,30 +200,31 @@
             middleware=middleware,
             name=name,
             opt=opt,
             signature_namespace=signature_namespace,
             **kwargs,
         )
 
-        # need to be assigned after the super() call
+        # its important that this is assigned after the super() call
         self.dto = dto
         self.return_dto = return_dto
 
         if not self.dependencies:
             self.dependencies = {}
+
         self.dependencies = dict(self.dependencies)
-        self.dependencies["connection_lifespan_dependencies"] = _utils.create_stub_dependency(
+        self.dependencies["connection_lifespan_dependencies"] = create_stub_dependency(
             self._connection_lifespan or self.default_connection_lifespan
         )
+
         if self.on_accept:
-            self.dependencies["on_accept_dependencies"] = _utils.create_stub_dependency(self.on_accept.ref.value)
+            self.dependencies["on_accept_dependencies"] = create_stub_dependency(self.on_accept.ref.value)
+
         if self.on_disconnect:
-            self.dependencies["on_disconnect_dependencies"] = _utils.create_stub_dependency(
-                self.on_disconnect.ref.value
-            )
+            self.dependencies["on_disconnect_dependencies"] = create_stub_dependency(self.on_disconnect.ref.value)
 
     @asynccontextmanager
     async def default_connection_lifespan(
         self,
         socket: WebSocket,
         on_accept_dependencies: Optional[Dict[str, Any]] = None,  # noqa: UP007, UP006
         on_disconnect_dependencies: Optional[Dict[str, Any]] = None,  # noqa: UP007, UP006
@@ -234,14 +242,15 @@
             - Call :attr:`on_accept` if defined after a connection has been accepted
             - Call :attr:`on_disconnect` upon leaving the context
         """
         await self.connection_accept_handler(socket)
 
         if self.on_accept:
             await self.on_accept(**(on_accept_dependencies or {}))
+
         try:
             yield
         except WebSocketDisconnect:
             pass
         finally:
             if self.on_disconnect:
                 await self.on_disconnect(**(on_disconnect_dependencies or {}))
@@ -259,66 +268,70 @@
 
         if return_dto := self.resolve_return_dto():
             return_type = self._listener_context.listener_callback_signature.return_type
             return_dto.on_registration(HandlerContext("return", str(self), return_type))
 
     def __call__(self, listener_callback: AnyCallable) -> websocket_listener:
         self._listener_context.listener_callback = listener_callback
-        self._listener_context.handler_function = handler_function = _utils.create_handler_function(
+        self._listener_context.handler_function = handler_function = create_handler_function(
             listener_context=self._listener_context,
             lifespan_manager=self._connection_lifespan or self.default_connection_lifespan,
         )
         return super().__call__(handler_function)
 
     def on_registration(self, app: Litestar) -> None:
         self._set_listener_context()
         super().on_registration(app)
 
     def _create_signature_model(self, app: Litestar) -> None:
         """Create signature model for handler function."""
         if not self.signature_model:
-            new_signature = _utils.create_handler_signature(
+            new_signature = create_handler_signature(
                 self._listener_context.listener_callback_signature.original_signature
             )
             self.signature_model = create_signature_model(
                 dependency_name_set=self.dependency_name_set,
                 fn=cast("AnyCallable", self.fn.value),
                 preferred_validation_backend=app._preferred_validation_backend,
                 parsed_signature=ParsedSignature.from_signature(new_signature, self.resolve_signature_namespace()),
             )
 
     def _set_listener_context(self) -> None:
-        listener_context = self._listener_context
-        listener_context.listener_callback_signature = listener_callback_signature = ParsedSignature.from_fn(
-            listener_context.listener_callback, self.resolve_signature_namespace()
+        listener_callback_signature = ParsedSignature.from_fn(
+            self._listener_context.listener_callback, self.resolve_signature_namespace()
         )
 
         if "data" not in listener_callback_signature.parameters:
             raise ImproperlyConfiguredException("Websocket listeners must accept a 'data' parameter")
 
         for param in ("request", "body"):
             if param in listener_callback_signature.parameters:
                 raise ImproperlyConfiguredException(f"The {param} kwarg is not supported with websocket listeners")
 
-        listener_context.can_send_data = not listener_callback_signature.return_type.is_subclass_of(NoneType)
-        listener_context.pass_socket = "socket" in listener_callback_signature.parameters
-        listener_context.resolved_data_dto = resolved_data_dto = self.resolve_dto()
-        listener_context.resolved_return_dto = resolved_return_dto = self.resolve_return_dto()
-        listener_context.handle_receive = _utils.create_handle_receive(
+        resolved_data_dto = self.resolve_dto()
+        resolved_return_dto = self.resolve_return_dto()
+
+        self._listener_context.listener_callback_signature = listener_callback_signature
+        self._listener_context.can_send_data = not listener_callback_signature.return_type.is_subclass_of(NoneType)
+        self._listener_context.pass_socket = "socket" in listener_callback_signature.parameters
+        self._listener_context.resolved_data_dto = resolved_data_dto
+        self._listener_context.resolved_return_dto = resolved_return_dto
+        self._listener_context.handle_receive = create_handle_receive(
             resolved_data_dto, self._receive_mode, listener_callback_signature.parameters["data"].annotation
         )
         should_encode_to_json = not (
             listener_callback_signature.return_type.is_subclass_of((str, bytes))
             or (
                 listener_callback_signature.return_type.is_optional
                 and listener_callback_signature.return_type.has_inner_subclass_of((str, bytes))
             )
         )
         json_encoder = JsonEncoder(enc_hook=partial(default_serializer, type_encoders=self.resolve_type_encoders()))
-        listener_context.handle_send = _utils.create_handle_send(
+
+        self._listener_context.handle_send = create_handle_send(
             resolved_return_dto, json_encoder, should_encode_to_json, self._send_mode
         )
 
 
 class WebsocketListener(ABC):
     path: str | None | list[str] | None = None
     """A path fragment for the route handler function or a sequence of path fragments. If not given defaults to ``/``"""
```

### Comparing `litestar-2.0.0b1/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.0.0b2/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/logging/_utils.py` & `litestar-2.0.0b2/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/logging/config.py` & `litestar-2.0.0b2/litestar/logging/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/logging/picologging.py` & `litestar-2.0.0b2/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/logging/standard.py` & `litestar-2.0.0b2/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/_utils.py` & `litestar-2.0.0b2/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/allowed_hosts.py` & `litestar-2.0.0b2/litestar/middleware/allowed_hosts.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from litestar.config.allowed_hosts import AllowedHostsConfig
     from litestar.types import ASGIApp, Receive, Scope, Send
 
 
 class AllowedHostsMiddleware(AbstractMiddleware):
     """Middleware ensuring the host of a request originated in a trusted host."""
 
-    def __init__(self, app: ASGIApp, config: AllowedHostsConfig):
+    def __init__(self, app: ASGIApp, config: AllowedHostsConfig) -> None:
         """Initialize ``AllowedHostsMiddleware``.
 
         Args:
             app: The ``next`` ASGI app to call.
             config: An instance of AllowedHostsConfig.
         """
```

### Comparing `litestar-2.0.0b1/litestar/middleware/authentication.py` & `litestar-2.0.0b2/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/base.py` & `litestar-2.0.0b2/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/compression.py` & `litestar-2.0.0b2/litestar/middleware/compression.py`

 * *Files 8% similar despite different names*

```diff
@@ -166,17 +166,16 @@
             send: The ASGI send function.
             compression_encoding: The compression encoding used.
             scope: The ASGI connection scope
 
         Returns:
             An ASGI send function.
         """
-
-        buffer = BytesIO()
-        facade = CompressionFacade(buffer=buffer, compression_encoding=compression_encoding, config=self.config)
+        bytes_buffer = BytesIO()
+        facade = CompressionFacade(buffer=bytes_buffer, compression_encoding=compression_encoding, config=self.config)
 
         initial_message = Ref[Optional["HTTPResponseStartEvent"]](None)
         started = Ref[bool](False)
 
         async def send_wrapper(message: Message) -> None:
             """Handle and compresses the HTTP Message with brotli.
 
@@ -199,24 +198,24 @@
                         headers["Content-Encoding"] = compression_encoding
                         headers.extend_header_value("vary", "Accept-Encoding")
                         del headers["Content-Length"]
                         set_litestar_scope_state(scope, SCOPE_STATE_RESPONSE_COMPRESSED, True)
 
                         facade.write(body)
 
-                        message["body"] = buffer.getvalue()
-                        buffer.seek(0)
-                        buffer.truncate()
+                        message["body"] = bytes_buffer.getvalue()
+                        bytes_buffer.seek(0)
+                        bytes_buffer.truncate()
                         await send(initial_message.value)
                         await send(message)
 
                     elif len(body) >= self.config.minimum_size:
                         facade.write(body)
                         facade.close()
-                        body = buffer.getvalue()
+                        body = bytes_buffer.getvalue()
 
                         headers = MutableScopeHeaders(initial_message.value)
                         headers["Content-Encoding"] = compression_encoding
                         headers["Content-Length"] = str(len(body))
                         headers.extend_header_value("vary", "Accept-Encoding")
                         message["body"] = body
                         set_litestar_scope_state(scope, SCOPE_STATE_RESPONSE_COMPRESSED, True)
@@ -229,18 +228,18 @@
                         await send(message)
 
                 else:
                     facade.write(body)
                     if not more_body:
                         facade.close()
 
-                    message["body"] = buffer.getvalue()
+                    message["body"] = bytes_buffer.getvalue()
 
-                    buffer.seek(0)
-                    buffer.truncate()
+                    bytes_buffer.seek(0)
+                    bytes_buffer.truncate()
 
                     if not more_body:
-                        buffer.close()
+                        bytes_buffer.close()
 
                     await send(message)
 
         return send_wrapper
```

### Comparing `litestar-2.0.0b1/litestar/middleware/cors.py` & `litestar-2.0.0b2/litestar/middleware/cors.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class CORSMiddleware(AbstractMiddleware):
     """CORS Middleware."""
 
     __slots__ = ("config",)
 
-    def __init__(self, app: ASGIApp, config: CORSConfig):
+    def __init__(self, app: ASGIApp, config: CORSConfig) -> None:
         """Middleware that adds CORS validation to the application.
 
         Args:
             app: The ``next`` ASGI app to call.
             config: An instance of :class:`CORSConfig <litestar.config.cors.CORSConfig>`
         """
         super().__init__(app=app, scopes={ScopeType.HTTP})
```

### Comparing `litestar-2.0.0b1/litestar/middleware/csrf.py` & `litestar-2.0.0b2/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.0.0b2/litestar/middleware/exceptions/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/exceptions/middleware.py` & `litestar-2.0.0b2/litestar/middleware/exceptions/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,23 @@
 
     Args:
         exc: An exception.
 
     Returns:
         Response: HTTP response constructed from exception details.
     """
+    status_code = getattr(exc, "status_code", HTTP_500_INTERNAL_SERVER_ERROR)
+    if status_code == HTTP_500_INTERNAL_SERVER_ERROR:
+        detail = "Internal Server Error"
+    else:
+        detail = getattr(exc, "detail", repr(exc))
+
     content = ExceptionResponseContent(
-        status_code=getattr(exc, "status_code", HTTP_500_INTERNAL_SERVER_ERROR),
-        detail=getattr(exc, "detail", repr(exc)),
+        status_code=status_code,
+        detail=detail,
         headers=getattr(exc, "headers", None),
         extra=getattr(exc, "extra", None),
     )
     return content.to_response()
 
 
 class ExceptionHandlerMiddleware:
```

### Comparing `litestar-2.0.0b1/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.0.0b2/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.0.0b2/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/logging.py` & `litestar-2.0.0b2/litestar/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/rate_limit.py` & `litestar-2.0.0b2/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/session/base.py` & `litestar-2.0.0b2/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/session/client_side.py` & `litestar-2.0.0b2/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/middleware/session/server_side.py` & `litestar-2.0.0b2/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/config.py` & `litestar-2.0.0b2/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/controller.py` & `litestar-2.0.0b2/litestar/openapi/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from functools import cached_property
-from typing import TYPE_CHECKING, Callable, Literal
+from typing import TYPE_CHECKING, Any, Callable, Literal
 
 from yaml import dump as dump_yaml
 
 from litestar.constants import OPENAPI_NOT_INITIALIZED
 from litestar.controller import Controller
 from litestar.enums import MediaType, OpenAPIMediaType
 from litestar.exceptions import ImproperlyConfiguredException
@@ -70,26 +70,26 @@
     _dumped_modified_schema: str = ""
     # set the dto types to `None` to ensure that if a dto is supplied at the application layer, they don't apply to
     # this controller.
     dto = None
     return_dto = None
 
     @staticmethod
-    def get_schema_from_request(request: Request) -> OpenAPI:
+    def get_schema_from_request(request: Request[Any, Any, Any]) -> OpenAPI:
         """Return the OpenAPI pydantic model from the request instance.
 
         Args:
             request: A :class:`Litestar <.connection.Request>` instance.
 
         Returns:
             An :class:`OpenAPI <litestar.openapi.spec.open_api.OpenAPI>` instance.
         """
         return request.app.openapi_schema
 
-    def should_serve_endpoint(self, request: Request) -> bool:
+    def should_serve_endpoint(self, request: Request[Any, Any, Any]) -> bool:
         """Verify that the requested path is within the enabled endpoints in the openapi_config.
 
         Args:
             request: To be tested if endpoint enabled.
 
         Returns:
             A boolean.
@@ -134,15 +134,15 @@
         return {
             "redoc": self.render_redoc,
             "swagger": self.render_swagger_ui,
             "elements": self.render_stoplight_elements,
         }
 
     @get(path="/openapi.yaml", media_type=OpenAPIMediaType.OPENAPI_YAML, include_in_schema=False, sync_to_thread=False)
-    def retrieve_schema_yaml(self, request: Request) -> ASGIResponse:
+    def retrieve_schema_yaml(self, request: Request[Any, Any, Any]) -> ASGIResponse:
         """Return the OpenAPI schema as YAML with an ``application/vnd.oai.openapi`` Content-Type header.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
@@ -152,15 +152,15 @@
             content = dump_yaml(self.get_schema_from_request(request).to_schema(), default_flow_style=False).encode(
                 "utf-8"
             )
             return ASGIResponse(body=content, media_type=OpenAPIMediaType.OPENAPI_YAML)
         return ASGIResponse(body=b"", status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(path="/openapi.json", media_type=OpenAPIMediaType.OPENAPI_JSON, include_in_schema=False, sync_to_thread=False)
-    def retrieve_schema_json(self, request: Request) -> ASGIResponse:
+    def retrieve_schema_json(self, request: Request[Any, Any, Any]) -> ASGIResponse:
         """Return the OpenAPI schema as JSON with an ``application/vnd.oai.openapi+json`` Content-Type header.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
@@ -170,15 +170,15 @@
             return ASGIResponse(
                 body=encode_json(self.get_schema_from_request(request).to_schema()),
                 media_type=OpenAPIMediaType.OPENAPI_JSON,
             )
         return ASGIResponse(body=b"", status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(path="/", include_in_schema=False, sync_to_thread=False)
-    def root(self, request: Request) -> ASGIResponse:
+    def root(self, request: Request[Any, Any, Any]) -> ASGIResponse:
         """Render a static documentation site.
 
          The site to be rendered is based on the ``root_schema_site`` value set in the application's
          :class:`OpenAPIConfig <.openapi.OpenAPIConfig>`. Defaults to ``redoc``.
 
         Args:
             request:
@@ -197,59 +197,59 @@
         render_method = self.render_methods_map[config.root_schema_site]
 
         if self.should_serve_endpoint(request):
             return ASGIResponse(body=render_method(request), media_type=MediaType.HTML)
         return ASGIResponse(body=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(path="/swagger", include_in_schema=False, sync_to_thread=False)
-    def swagger_ui(self, request: Request) -> ASGIResponse:
+    def swagger_ui(self, request: Request[Any, Any, Any]) -> ASGIResponse:
         """Route handler responsible for rendering Swagger-UI.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with a rendered swagger documentation site
         """
         if self.should_serve_endpoint(request):
             return ASGIResponse(body=self.render_swagger_ui(request), media_type=MediaType.HTML)
         return ASGIResponse(body=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(path="/elements", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
-    def stoplight_elements(self, request: Request) -> ASGIResponse:
+    def stoplight_elements(self, request: Request[Any, Any, Any]) -> ASGIResponse:
         """Route handler responsible for rendering StopLight Elements.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with a rendered stoplight elements documentation site
         """
         if self.should_serve_endpoint(request):
             return ASGIResponse(body=self.render_stoplight_elements(request), media_type=MediaType.HTML)
         return ASGIResponse(body=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
     @get(path="/redoc", media_type=MediaType.HTML, include_in_schema=False, sync_to_thread=False)
-    def redoc(self, request: Request) -> ASGIResponse:  # pragma: no cover
+    def redoc(self, request: Request[Any, Any, Any]) -> ASGIResponse:  # pragma: no cover
         """Route handler responsible for rendering Redoc.
 
         Args:
             request:
                 A :class:`Request <.connection.Request>` instance.
 
         Returns:
             A response with a rendered redoc documentation site
         """
         if self.should_serve_endpoint(request):
             return ASGIResponse(body=self.render_redoc(request), media_type=MediaType.HTML)
         return ASGIResponse(body=self.render_404_page(), status_code=HTTP_404_NOT_FOUND, media_type=MediaType.HTML)
 
-    def render_swagger_ui(self, request: Request) -> bytes:
+    def render_swagger_ui(self, request: Request[Any, Any, Any]) -> bytes:
         """Render an HTML page for Swagger-UI.
 
         Notes:
             - override this method to customize the template.
 
         Args:
             request:
@@ -296,15 +296,15 @@
         <!DOCTYPE html>
             <html>
                 {head}
                 {body}
             </html>
         """.encode()
 
-    def render_stoplight_elements(self, request: Request) -> bytes:
+    def render_stoplight_elements(self, request: Request[Any, Any, Any]) -> bytes:
         """Render an HTML page for StopLight Elements.
 
         Notes:
             - override this method to customize the template.
 
         Args:
             request:
@@ -340,15 +340,15 @@
         <!DOCTYPE html>
             <html>
                 {head}
                 {body}
             </html>
         """.encode()
 
-    def render_redoc(self, request: Request) -> bytes:  # pragma: no cover
+    def render_redoc(self, request: Request[Any, Any, Any]) -> bytes:  # pragma: no cover
         """Render an HTML page for Redoc.
 
         Notes:
             - override this method to customize the template.
 
         Args:
             request:
```

### Comparing `litestar-2.0.0b1/litestar/openapi/datastructures.py` & `litestar-2.0.0b2/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/__init__.py` & `litestar-2.0.0b2/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/base.py` & `litestar-2.0.0b2/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/callback.py` & `litestar-2.0.0b2/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/components.py` & `litestar-2.0.0b2/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/contact.py` & `litestar-2.0.0b2/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/discriminator.py` & `litestar-2.0.0b2/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/encoding.py` & `litestar-2.0.0b2/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/enums.py` & `litestar-2.0.0b2/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/example.py` & `litestar-2.0.0b2/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/external_documentation.py` & `litestar-2.0.0b2/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/header.py` & `litestar-2.0.0b2/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/info.py` & `litestar-2.0.0b2/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/license.py` & `litestar-2.0.0b2/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/link.py` & `litestar-2.0.0b2/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/media_type.py` & `litestar-2.0.0b2/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/oauth_flow.py` & `litestar-2.0.0b2/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/oauth_flows.py` & `litestar-2.0.0b2/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/open_api.py` & `litestar-2.0.0b2/litestar/openapi/spec/open_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,14 @@
     from litestar.openapi.spec.info import Info
     from litestar.openapi.spec.path_item import PathItem
     from litestar.openapi.spec.paths import Paths
     from litestar.openapi.spec.reference import Reference
     from litestar.openapi.spec.security_requirement import SecurityRequirement
     from litestar.openapi.spec.tag import Tag
 
-try:
-    from pydantic.schema import schema as pydantic_schema_helper
-except ImportError:  # pragma: no cover
-
-    def pydantic_schema_helper(*args, **kwargs):  # type: ignore
-        ...
-
-
 __all__ = ("OpenAPI",)
 
 
 @dataclass
 class OpenAPI(BaseSchemaObject):
     """Root OpenAPI document."""
```

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/operation.py` & `litestar-2.0.0b2/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/parameter.py` & `litestar-2.0.0b2/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/path_item.py` & `litestar-2.0.0b2/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/paths.py` & `litestar-2.0.0b2/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/reference.py` & `litestar-2.0.0b2/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/request_body.py` & `litestar-2.0.0b2/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/response.py` & `litestar-2.0.0b2/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/responses.py` & `litestar-2.0.0b2/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/schema.py` & `litestar-2.0.0b2/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/security_requirement.py` & `litestar-2.0.0b2/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/security_scheme.py` & `litestar-2.0.0b2/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/server.py` & `litestar-2.0.0b2/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/server_variable.py` & `litestar-2.0.0b2/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/tag.py` & `litestar-2.0.0b2/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/openapi/spec/xml.py` & `litestar-2.0.0b2/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/pagination.py` & `litestar-2.0.0b2/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/params.py` & `litestar-2.0.0b2/litestar/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 __all__ = (
     "Body",
     "BodyKwarg",
     "Dependency",
     "DependencyKwarg",
     "KwargDefinition",
     "Parameter",
+    "ParameterKwarg",
 )
 
 
 if TYPE_CHECKING:
     from litestar.openapi.spec.example import Example
     from litestar.openapi.spec.external_documentation import (
         ExternalDocumentation,
```

### Comparing `litestar-2.0.0b1/litestar/partial.py` & `litestar-2.0.0b2/litestar/partial.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         for field_name, field_type in _extract_type_hints(item):
             if not isinstance(field_type, GenericAlias) or NoneType not in field_type.__args__:
                 field_definitions[field_name] = (Optional[field_type], None)
             else:
                 field_definitions[field_name] = (field_type, None)
 
         cls._models[item] = pydantic.create_model(
-            _create_partial_type_name(item), __base__=item, **field_definitions
+            _create_partial_type_name(item), __base__=item, **field_definitions  # pyright: ignore
         )  # type: ignore
 
     @classmethod
     def _create_partial_attrs_model(cls, item: type[attrs.AttrsInstance]) -> None:
         import attrs
 
         field_definitions: dict[str, Any] = {}
@@ -127,15 +127,15 @@
             else:
                 field_definitions[field_name] = field_type
 
         cls._models[item] = attrs.define(
             type(
                 _create_partial_type_name(item),
                 (item,),
-                {"__annotations__": field_definitions, **{k: None for k in field_definitions}},  # type: ignore[misc]
+                {"__annotations__": field_definitions, **{k: None for k in field_definitions}},
             )
         )
 
     @classmethod
     def _create_partial_dataclass(cls, item: type[DataclassProtocol]) -> None:
         """Receives a dataclass class and creates an all optional subclass of it.
```

### Comparing `litestar-2.0.0b1/litestar/plugins.py` & `litestar-2.0.0b2/litestar/plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/response/base.py` & `litestar-2.0.0b2/litestar/response/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         """Set a cookie on the response. If passed a :class:`Cookie <.datastructures.Cookie>` instance, keyword
         arguments will be ignored.
 
         Args:
             key: Key for the cookie or a :class:`Cookie <.datastructures.Cookie>` instance.
             value: Value for the cookie, if none given defaults to empty string.
             max_age: Maximal age of the cookie before its invalidated.
-            expires: Expiration date as unix MS timestamp.
+            expires: Seconds from now until the cookie expires.
             path: Path fragment that must exist in the request url for the cookie to be valid. Defaults to ``/``.
             domain: Domain for which the cookie is valid.
             secure: Https is required for the cookie.
             httponly: Forbids javascript to access the cookie via ``document.cookie``.
             samesite: Controls whether a cookie is sent with cross-site requests. Defaults to ``lax``.
 
         Returns:
```

### Comparing `litestar-2.0.0b1/litestar/response/file.py` & `litestar-2.0.0b2/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/response/redirect.py` & `litestar-2.0.0b2/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/response/streaming.py` & `litestar-2.0.0b2/litestar/response/streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from functools import partial
 from typing import TYPE_CHECKING, Any, AsyncGenerator, AsyncIterable, AsyncIterator, Callable, Iterable, Iterator, Union
 
 from anyio import CancelScope, create_task_group
 
 from litestar.enums import MediaType
 from litestar.response.base import ASGIResponse, Response
-from litestar.types.composite_types import StreamType
+from litestar.types.helper_types import StreamType
 from litestar.utils.helpers import filter_cookies, get_enum_string_value
 from litestar.utils.sync import AsyncIteratorWrapper
 
 if TYPE_CHECKING:
     from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.connection import Request
@@ -26,15 +26,15 @@
 
 
 class ASGIStreamingResponse(ASGIResponse):
     """A streaming response."""
 
     __slots__ = ("iterator",)
 
-    def __init__(self, *, iterator: StreamType, **kwargs: Any):
+    def __init__(self, *, iterator: StreamType, **kwargs: Any) -> None:
         """A low-level ASGI streaming response.
 
         Args:
             iterator: An async iterator or iterable.
             **kwargs: Additional keyword arguments propagated to :class:`ASGIResponse <.response.base.ASGIResponse>`.
         """
         super().__init__(**kwargs)
@@ -107,15 +107,15 @@
         *,
         background: BackgroundTask | BackgroundTasks | None = None,
         cookies: ResponseCookies | None = None,
         encoding: str = "utf-8",
         headers: ResponseHeaders | None = None,
         media_type: MediaType | OpenAPIMediaType | str | None = None,
         status_code: int | None = None,
-    ):
+    ) -> None:
         """Initialize the response.
 
         Args:
             content: A sync or async iterator or iterable.
             background: A :class:`BackgroundTask <.background_tasks.BackgroundTask>` instance or
                 :class:`BackgroundTasks <.background_tasks.BackgroundTasks>` to execute after the response is finished.
                 Defaults to None.
```

### Comparing `litestar-2.0.0b1/litestar/response/template.py` & `litestar-2.0.0b2/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/router.py` & `litestar-2.0.0b2/litestar/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,14 +213,15 @@
                         path=path,
                         route_handlers=http_handlers,
                     )
                     self.routes[existing_route_index] = route
                 else:
                     route = HTTPRoute(path=path, route_handlers=http_handlers)
                     self.routes.append(route)
+
                 routes.append(route)
 
             if websocket_handler := handlers_map.get("websocket"):
                 route = WebSocketRoute(path=path, route_handler=cast("WebsocketRouteHandler", websocket_handler))
                 self.routes.append(route)
                 routes.append(route)
 
@@ -244,14 +245,15 @@
                 for route_handler in route.route_handlers:
                     for method in route_handler.http_methods:
                         route_map[route.path][method] = route_handler
             else:
                 route_map[route.path][
                     "websocket" if isinstance(route, WebSocketRoute) else "asgi"
                 ] = route.route_handler
+
         return route_map
 
     @classmethod
     def get_route_handler_map(
         cls,
         value: Controller | RouteHandlerType | Router,
     ) -> dict[str, RouteHandlerMapItem]:
@@ -291,14 +293,15 @@
         # this narrows down to an ABC, but we assume a non-abstract subclass of the ABC superclass
         if is_class_and_subclass(value, WebsocketListener):  # type: ignore[type-abstract]
             return value(owner=self).to_handler()  # pyright: ignore
 
         if isinstance(value, Router):
             if value.owner:
                 raise ImproperlyConfiguredException(f"Router with path {value.path} has already been registered")
+
             if value is self:
                 raise ImproperlyConfiguredException("Cannot register a router on itself")
 
             value.owner = self
             return value
 
         if isinstance(value, (ASGIRouteHandler, HTTPRouteHandler, WebsocketRouteHandler)):
```

### Comparing `litestar-2.0.0b1/litestar/routes/asgi.py` & `litestar-2.0.0b2/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/routes/base.py` & `litestar-2.0.0b2/litestar/routes/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/routes/http.py` & `litestar-2.0.0b2/litestar/routes/http.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/routes/websocket.py` & `litestar-2.0.0b2/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/security/base.py` & `litestar-2.0.0b2/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/security/session_auth/auth.py` & `litestar-2.0.0b2/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/security/session_auth/middleware.py` & `litestar-2.0.0b2/litestar/security/session_auth/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from litestar.types import ASGIApp, Receive, Scope, Send
     from litestar.utils import AsyncCallable
 
 
 class MiddlewareWrapper:
     """Wrapper class that serves as the middleware entry point."""
 
-    def __init__(self, app: ASGIApp, config: SessionAuth):
+    def __init__(self, app: ASGIApp, config: SessionAuth[Any, Any]) -> None:
         """Wrap the SessionAuthMiddleware inside ExceptionHandlerMiddleware, and it wraps this inside SessionMiddleware.
         This allows the auth middleware to raise exceptions and still have the response handled, while having the
         session cleared.
 
         Args:
             app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
             config: An instance of SessionAuth.
@@ -76,15 +76,15 @@
     def __init__(
         self,
         app: ASGIApp,
         exclude: str | list[str] | None,
         exclude_opt_key: str,
         scopes: Scopes | None,
         retrieve_user_handler: AsyncCallable[[dict[str, Any], ASGIConnection[Any, Any, Any, Any]], Awaitable[Any]],
-    ):
+    ) -> None:
         """Session based authentication middleware.
 
         Args:
             app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
             exclude: A pattern or list of patterns to skip in the authentication middleware.
             exclude_opt_key: An identifier to use on routes to disable authentication and authorization checks for a particular route.
             scopes: ASGI scopes processed by the authentication middleware.
```

### Comparing `litestar-2.0.0b1/litestar/serialization.py` & `litestar-2.0.0b2/litestar/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/static_files/base.py` & `litestar-2.0.0b2/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/static_files/config.py` & `litestar-2.0.0b2/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/status_codes.py` & `litestar-2.0.0b2/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/stores/base.py` & `litestar-2.0.0b2/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/stores/file.py` & `litestar-2.0.0b2/litestar/stores/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class FileStore(NamespacedStore):
     """File based, thread and process safe, asynchronous key/value store."""
 
     __slots__ = {"path": "file path"}
 
-    def __init__(self, path: PathLike) -> None:
+    def __init__(self, path: PathLike[str]) -> None:
         """Initialize ``FileStorage``.
 
         Args:
             path: Path to store data under
         """
         self.path = Path(path)
```

### Comparing `litestar-2.0.0b1/litestar/stores/memory.py` & `litestar-2.0.0b2/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/stores/redis.py` & `litestar-2.0.0b2/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/stores/registry.py` & `litestar-2.0.0b2/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/template/base.py` & `litestar-2.0.0b2/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/template/config.py` & `litestar-2.0.0b2/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/testing/__init__.py` & `litestar-2.0.0b2/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/testing/client/__init__.py` & `litestar-2.0.0b2/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/testing/client/async_client.py` & `litestar-2.0.0b2/litestar/testing/client/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,40 +28,42 @@
     from litestar.middleware.session.base import BaseBackendConfig
 
 
 T = TypeVar("T", bound=ASGIApp)
 
 
 class AsyncTestClient(AsyncClient, BaseTestClient, Generic[T]):  # type: ignore[misc]
-    lifespan_handler: LifeSpanHandler
+    lifespan_handler: LifeSpanHandler[Any]
     exit_stack: AsyncExitStack
 
     def __init__(
         self,
         app: T,
         base_url: str = "http://testserver.local",
         raise_server_exceptions: bool = True,
         root_path: str = "",
         backend: AnyIOBackend = "asyncio",
         backend_options: Mapping[str, Any] | None = None,
         session_config: BaseBackendConfig | None = None,
+        timeout: float | None = None,
         cookies: CookieTypes | None = None,
-    ):
+    ) -> None:
         """An Async client implementation providing a context manager for testing applications asynchronously.
 
         Args:
             app: The instance of :class:`Litestar <litestar.app.Litestar>` under test.
             base_url: URL scheme and domain for test request paths, e.g. 'http://testserver'.
             raise_server_exceptions: Flag for the underlying test client to raise server exceptions instead of
                 wrapping them in an HTTP response.
             root_path: Path prefix for requests.
             backend: The async backend to use, options are "asyncio" or "trio".
             backend_options: 'anyio' options.
             session_config: Configuration for Session Middleware class to create raw session cookies for request to the
                 route handlers.
+            timeout: Request timeout
             cookies: Cookies to set on the client.
         """
         BaseTestClient.__init__(
             self,
             app=app,
             base_url=base_url,
             backend=backend,
@@ -77,14 +79,15 @@
             follow_redirects=True,
             cookies=cookies,
             transport=TestClientTransport(  # type: ignore [arg-type]
                 client=self,
                 raise_server_exceptions=raise_server_exceptions,
                 root_path=root_path,
             ),
+            timeout=timeout,
         )
 
     async def __aenter__(self) -> AsyncTestClient[T]:
         async with AsyncExitStack() as stack:
             self.blocking_portal = portal = stack.enter_context(self.portal())
             self.lifespan_handler = LifeSpanHandler(client=self)
```

### Comparing `litestar-2.0.0b1/litestar/testing/client/base.py` & `litestar-2.0.0b2/litestar/testing/client/base.py`

 * *Files identical despite different names*

```diff
@@ -71,15 +71,15 @@
         self,
         app: T,
         base_url: str = "http://testserver.local",
         backend: AnyIOBackend = "asyncio",
         backend_options: Mapping[str, Any] | None = None,
         session_config: BaseBackendConfig | None = None,
         cookies: CookieTypes | None = None,
-    ):
+    ) -> None:
         if "." not in base_url:
             warn(
                 f"The base_url {base_url!r} might cause issues. Try adding a domain name such as .local: "
                 f"'{base_url}.local'",
                 UserWarning,
                 stacklevel=1,
             )
@@ -89,15 +89,15 @@
         self.app = app
         self.base_url = base_url
         self.backend = backend
         self.backend_options = backend_options
         self.cookies = cookies
 
     @property
-    def session_backend(self) -> BaseSessionBackend:
+    def session_backend(self) -> BaseSessionBackend[Any]:
         if not self._session_backend:
             raise ImproperlyConfiguredException(
                 "Session has not been initialized for this TestClient instance. You can"
                 "do so by passing a configuration object to TestClient: TestClient(app=app, session_config=...)"
             )
         return self._session_backend
```

### Comparing `litestar-2.0.0b1/litestar/testing/client/sync_client.py` & `litestar-2.0.0b2/litestar/testing/client/sync_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,40 +31,42 @@
     from litestar.types.helper_types import OptionalSequence
 
 
 T = TypeVar("T", bound=ASGIApp)
 
 
 class TestClient(Client, BaseTestClient, Generic[T]):  # type: ignore[misc]
-    lifespan_handler: LifeSpanHandler
+    lifespan_handler: LifeSpanHandler[Any]
     exit_stack: ExitStack
 
     def __init__(
         self,
         app: T,
         base_url: str = "http://testserver.local",
         raise_server_exceptions: bool = True,
         root_path: str = "",
         backend: AnyIOBackend = "asyncio",
         backend_options: Mapping[str, Any] | None = None,
         session_config: BaseBackendConfig | None = None,
+        timeout: float | None = None,
         cookies: CookieTypes | None = None,
     ) -> None:
         """A client implementation providing a context manager for testing applications.
 
         Args:
             app: The instance of :class:`Litestar <litestar.app.Litestar>` under test.
             base_url: URL scheme and domain for test request paths, e.g. 'http://testserver'.
             raise_server_exceptions: Flag for the underlying test client to raise server exceptions instead of
                 wrapping them in an HTTP response.
             root_path: Path prefix for requests.
             backend: The async backend to use, options are "asyncio" or "trio".
             backend_options: ``anyio`` options.
             session_config: Configuration for Session Middleware class to create raw session cookies for request to the
                 route handlers.
+            timeout: Request timeout
             cookies: Cookies to set on the client.
         """
         BaseTestClient.__init__(
             self,
             app=app,
             base_url=base_url,
             backend=backend,
@@ -81,14 +83,15 @@
             follow_redirects=True,
             cookies=cookies,
             transport=TestClientTransport(  # type: ignore [arg-type]
                 client=self,
                 raise_server_exceptions=raise_server_exceptions,
                 root_path=root_path,
             ),
+            timeout=timeout,
         )
 
     def __enter__(self) -> TestClient[T]:
         with ExitStack() as stack:
             self.blocking_portal = portal = stack.enter_context(self.portal())
             self.lifespan_handler = LifeSpanHandler(client=self)
 
@@ -469,15 +472,15 @@
             timeout=timeout,
             extensions=extensions,
         )
 
     def websocket_connect(
         self,
         url: str,
-        subprotocols: OptionalSequence[str] = None,
+        subprotocols: OptionalSequence[str] | None = None,
         params: QueryParamTypes | None = None,
         headers: HeaderTypes | None = None,
         cookies: CookieTypes | None = None,
         auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
         follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
         timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
         extensions: Mapping[str, Any] | None = None,
```

### Comparing `litestar-2.0.0b1/litestar/testing/helpers.py` & `litestar-2.0.0b2/litestar/testing/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,63 +51,64 @@
         TypeEncodersMap,
     )
 
 
 def create_test_client(
     route_handlers: ControllerRouterHandler | Sequence[ControllerRouterHandler] | None = None,
     *,
-    after_exception: OptionalSequence[AfterExceptionHookHandler] = None,
+    after_exception: OptionalSequence[AfterExceptionHookHandler] | None = None,
     after_request: AfterRequestHookHandler | None = None,
     after_response: AfterResponseHookHandler | None = None,
     allowed_hosts: Sequence[str] | AllowedHostsConfig | None = None,
     backend: Literal["asyncio", "trio"] = "asyncio",
     backend_options: Mapping[str, Any] | None = None,
     base_url: str = "http://testserver.local",
     before_request: BeforeRequestHookHandler | None = None,
-    before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
+    before_send: OptionalSequence[BeforeMessageSendHookHandler] | None = None,
     cache_control: CacheControlHeader | None = None,
     compression_config: CompressionConfig | None = None,
     cors_config: CORSConfig | None = None,
     csrf_config: CSRFConfig | None = None,
     debug: bool = False,
     dependencies: Dependencies | None = None,
     dto: type[DTOInterface] | None | EmptyType = Empty,
     etag: ETag | None = None,
     event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
     exception_handlers: ExceptionHandlersMap | None = None,
-    guards: OptionalSequence[Guard] = None,
-    listeners: OptionalSequence[EventListener] = None,
+    guards: OptionalSequence[Guard] | None = None,
+    listeners: OptionalSequence[EventListener] | None = None,
     logging_config: BaseLoggingConfig | EmptyType | None = Empty,
-    middleware: OptionalSequence[Middleware] = None,
+    middleware: OptionalSequence[Middleware] | None = None,
     multipart_form_part_limit: int = 1000,
-    on_app_init: OptionalSequence[OnAppInitHandler] = None,
-    on_shutdown: OptionalSequence[LifespanHook] = None,
-    on_startup: OptionalSequence[LifespanHook] = None,
+    on_app_init: OptionalSequence[OnAppInitHandler] | None = None,
+    on_shutdown: OptionalSequence[LifespanHook] | None = None,
+    on_startup: OptionalSequence[LifespanHook] | None = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
-    plugins: OptionalSequence[PluginProtocol] = None,
+    plugins: OptionalSequence[PluginProtocol] | None = None,
     lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
     raise_server_exceptions: bool = True,
     pdb_on_exception: bool | None = None,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: ResponseType | None = None,
     response_cookies: ResponseCookies | None = None,
-    response_headers: OptionalSequence[ResponseHeader] = None,
+    response_headers: OptionalSequence[ResponseHeader] | None = None,
     return_dto: type[DTOInterface] | None | EmptyType = Empty,
     root_path: str = "",
-    security: OptionalSequence[SecurityRequirement] = None,
+    security: OptionalSequence[SecurityRequirement] | None = None,
     session_config: BaseBackendConfig | None = None,
     signature_namespace: Mapping[str, Any] | None = None,
     state: State | None = None,
-    static_files_config: OptionalSequence[StaticFilesConfig] = None,
+    static_files_config: OptionalSequence[StaticFilesConfig] | None = None,
     stores: StoreRegistry | dict[str, Store] | None = None,
     tags: Sequence[str] | None = None,
     template_config: TemplateConfig | None = None,
+    timeout: float | None = None,
     type_encoders: TypeEncodersMap | None = None,
     websocket_class: type[WebSocket] | None = None,
     _preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
 ) -> TestClient[Litestar]:
     """Create a Litestar app instance and initializes it.
 
     :class:`TestClient <litestar.testing.TestClient>` with it.
@@ -217,14 +218,15 @@
         stores: Central registry of :class:`Store <.stores.base.Store>` that will be available throughout the
             application. If this is a dictionary to it will be passed to a
             :class:`StoreRegistry <.stores.registry.StoreRegistry>`. If it is a
             :class:`StoreRegistry <.stores.registry.StoreRegistry>`, this instance will be used directly.
         tags: A sequence of string tags that will be appended to the schema of all route handlers under the
             application.
         template_config: An instance of :class:`TemplateConfig <.template.TemplateConfig>`
+        timeout: Request timeout
         type_encoders: A mapping of types to callables that transform them into types supported for serialization.
         websocket_class: An optional subclass of :class:`WebSocket <.connection.WebSocket>` to use for websocket
             connections.
 
     Returns:
         An instance of :class:`TestClient <.testing.TestClient>` with a created app instance.
     """
@@ -286,69 +288,71 @@
         app=app,
         backend=backend,
         backend_options=backend_options,
         base_url=base_url,
         raise_server_exceptions=raise_server_exceptions,
         root_path=root_path,
         session_config=session_config,
+        timeout=timeout,
     )
 
 
 def create_async_test_client(
     route_handlers: ControllerRouterHandler | Sequence[ControllerRouterHandler] | None = None,
     *,
-    after_exception: OptionalSequence[AfterExceptionHookHandler] = None,
+    after_exception: OptionalSequence[AfterExceptionHookHandler] | None = None,
     after_request: AfterRequestHookHandler | None = None,
     after_response: AfterResponseHookHandler | None = None,
     allowed_hosts: Sequence[str] | AllowedHostsConfig | None = None,
     backend: Literal["asyncio", "trio"] = "asyncio",
     backend_options: Mapping[str, Any] | None = None,
     base_url: str = "http://testserver.local",
     before_request: BeforeRequestHookHandler | None = None,
-    before_send: OptionalSequence[BeforeMessageSendHookHandler] = None,
+    before_send: OptionalSequence[BeforeMessageSendHookHandler] | None = None,
     cache_control: CacheControlHeader | None = None,
     compression_config: CompressionConfig | None = None,
     cors_config: CORSConfig | None = None,
     csrf_config: CSRFConfig | None = None,
     debug: bool = False,
     dependencies: Dependencies | None = None,
     dto: type[DTOInterface] | None | EmptyType = Empty,
     etag: ETag | None = None,
     event_emitter_backend: type[BaseEventEmitterBackend] = SimpleEventEmitter,
     exception_handlers: ExceptionHandlersMap | None = None,
-    guards: OptionalSequence[Guard] = None,
+    guards: OptionalSequence[Guard] | None = None,
     lifespan: list[Callable[[Litestar], AbstractAsyncContextManager] | AbstractAsyncContextManager] | None = None,
-    listeners: OptionalSequence[EventListener] = None,
+    listeners: OptionalSequence[EventListener] | None = None,
     logging_config: BaseLoggingConfig | EmptyType | None = Empty,
-    middleware: OptionalSequence[Middleware] = None,
+    middleware: OptionalSequence[Middleware] | None = None,
     multipart_form_part_limit: int = 1000,
-    on_app_init: OptionalSequence[OnAppInitHandler] = None,
-    on_shutdown: OptionalSequence[LifespanHook] = None,
-    on_startup: OptionalSequence[LifespanHook] = None,
+    on_app_init: OptionalSequence[OnAppInitHandler] | None = None,
+    on_shutdown: OptionalSequence[LifespanHook] | None = None,
+    on_startup: OptionalSequence[LifespanHook] | None = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
     pdb_on_exception: bool | None = None,
-    plugins: OptionalSequence[PluginProtocol] = None,
+    plugins: OptionalSequence[PluginProtocol] | None = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: ResponseType | None = None,
     response_cookies: ResponseCookies | None = None,
-    response_headers: OptionalSequence[ResponseHeader] = None,
+    response_headers: OptionalSequence[ResponseHeader] | None = None,
     return_dto: type[DTOInterface] | None | EmptyType = Empty,
     root_path: str = "",
-    security: OptionalSequence[SecurityRequirement] = None,
+    security: OptionalSequence[SecurityRequirement] | None = None,
     session_config: BaseBackendConfig | None = None,
     signature_namespace: Mapping[str, Any] | None = None,
     state: State | None = None,
-    static_files_config: OptionalSequence[StaticFilesConfig] = None,
+    static_files_config: OptionalSequence[StaticFilesConfig] | None = None,
     stores: StoreRegistry | dict[str, Store] | None = None,
     tags: Sequence[str] | None = None,
     template_config: TemplateConfig | None = None,
+    timeout: float | None = None,
     type_encoders: TypeEncodersMap | None = None,
     websocket_class: type[WebSocket] | None = None,
     _preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
 ) -> AsyncTestClient[Litestar]:
     """Create a Litestar app instance and initializes it.
 
     :class:`TestClient <litestar.testing.TestClient>` with it.
@@ -458,14 +462,15 @@
         stores: Central registry of :class:`Store <.stores.base.Store>` that will be available throughout the
             application. If this is a dictionary to it will be passed to a
             :class:`StoreRegistry <.stores.registry.StoreRegistry>`. If it is a
             :class:`StoreRegistry <.stores.registry.StoreRegistry>`, this instance will be used directly.
         tags: A sequence of string tags that will be appended to the schema of all route handlers under the
             application.
         template_config: An instance of :class:`TemplateConfig <.template.TemplateConfig>`
+        timeout: Request timeout
         type_encoders: A mapping of types to callables that transform them into types supported for serialization.
         websocket_class: An optional subclass of :class:`WebSocket <.connection.WebSocket>` to use for websocket
             connections.
 
     Returns:
         An instance of :class:`AsyncTestClient <litestar.testing.AsyncTestClient>` with a created app instance.
     """
@@ -527,8 +532,9 @@
         app=app,
         backend=backend,
         backend_options=backend_options,
         base_url=base_url,
         raise_server_exceptions=raise_server_exceptions,
         root_path=root_path,
         session_config=session_config,
+        timeout=timeout,
     )
```

### Comparing `litestar-2.0.0b1/litestar/testing/life_span_handler.py` & `litestar-2.0.0b2/litestar/testing/life_span_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 T = TypeVar("T", bound=BaseTestClient)
 
 
 class LifeSpanHandler(Generic[T]):
     __slots__ = "stream_send", "stream_receive", "client", "task"
 
-    def __init__(self, client: T):
+    def __init__(self, client: T) -> None:
         self.client = client
         self.stream_send = StapledObjectStream[Optional["LifeSpanSendMessage"]](*create_memory_object_stream(inf))
         self.stream_receive = StapledObjectStream["LifeSpanReceiveMessage"](*create_memory_object_stream(inf))
 
         with self.client.portal() as portal:
             self.task = portal.start_task_soon(self.lifespan)
             portal.call(self.wait_startup)
```

### Comparing `litestar-2.0.0b1/litestar/testing/request_factory.py` & `litestar-2.0.0b2/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/testing/transport.py` & `litestar-2.0.0b2/litestar/testing/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
     def handle_request(self, request: Request) -> Response:
         scope = self.parse_request(request=request)
         if scope["type"] == "websocket":
             scope.update(
                 subprotocols=[value.strip() for value in request.headers.get("sec-websocket-protocol", "").split(",")]
             )
-            session = WebSocketTestSession(client=self.client, scope=cast("WebSocketScope", scope))  # type: ignore [arg-type]
+            session = WebSocketTestSession(client=self.client, scope=cast("WebSocketScope", scope))  # type: ignore[arg-type]
             raise ConnectionUpgradeExceptionError(session)
 
         scope.update(method=request.method, http_version="1.1", extensions={"http.response.template": {}})
 
         raw_kwargs: dict[str, Any] = {"stream": BytesIO()}
 
         try:
```

### Comparing `litestar-2.0.0b1/litestar/testing/websocket_test_session.py` & `litestar-2.0.0b2/litestar/testing/websocket_test_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class WebSocketTestSession:
     exit_stack: ExitStack
 
     def __init__(
         self,
-        client: TestClient,
+        client: TestClient[Any],
         scope: WebSocketScope,
     ) -> None:
         self.client = client
         self.scope = scope
         self.accepted_subprotocol: str | None = None
         self.receive_queue: Queue[WebSocketReceiveMessage] = Queue()
         self.send_queue: Queue[WebSocketSendMessage | BaseException] = Queue()
```

### Comparing `litestar-2.0.0b1/litestar/types/__init__.py` & `litestar-2.0.0b2/litestar/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,26 +58,25 @@
     OnAppInitHandler,
     OperationIDCreator,
     Serializer,
 )
 from .composite_types import (
     Dependencies,
     ExceptionHandlersMap,
-    MaybePartial,
     Middleware,
     ParametersMap,
     PathType,
     ResponseCookies,
     ResponseHeaders,
     Scopes,
     TypeEncodersMap,
 )
 from .empty import Empty, EmptyType
 from .file_types import FileInfo, FileSystemProtocol
-from .helper_types import AnyIOBackend, OptionalSequence, SyncOrAsyncUnion
+from .helper_types import AnyIOBackend, MaybePartial, OptionalSequence, StreamType, SyncOrAsyncUnion
 from .internal_types import (
     ControllerRouterHandler,
     ReservedKwargs,
     ResponseType,
     RouteHandlerMapItem,
     RouteHandlerType,
 )
@@ -113,50 +112,51 @@
     "HTTPReceiveMessage",
     "HTTPRequestEvent",
     "HTTPResponseBodyEvent",
     "HTTPResponseStartEvent",
     "HTTPScope",
     "HTTPSendMessage",
     "HTTPServerPushEvent",
-    "LifespanHook",
     "LifeSpanReceive",
     "LifeSpanReceiveMessage",
     "LifeSpanScope",
     "LifeSpanSend",
     "LifeSpanSendMessage",
     "LifeSpanShutdownCompleteEvent",
     "LifeSpanShutdownEvent",
     "LifeSpanShutdownFailedEvent",
     "LifeSpanStartupCompleteEvent",
     "LifeSpanStartupEvent",
     "LifeSpanStartupFailedEvent",
+    "LifespanHook",
+    "LitestarEncodableType",
     "Logger",
     "MaybePartial",
     "Message",
     "Method",
     "Middleware",
     "OnAppInitHandler",
     "OperationIDCreator",
     "OptionalSequence",
     "ParametersMap",
     "PathType",
     "Receive",
     "ReceiveMessage",
     "ReservedKwargs",
     "ResponseCookies",
-    "ResponseType",
     "ResponseHeaders",
+    "ResponseType",
     "RouteHandlerMapItem",
     "RouteHandlerType",
     "Scope",
     "ScopeSession",
     "Scopes",
     "Send",
     "Serializer",
-    "LitestarEncodableType",
+    "StreamType",
     "SyncOrAsyncUnion",
     "TypeEncodersMap",
     "TypedDictClass",
     "WebSocketAcceptEvent",
     "WebSocketCloseEvent",
     "WebSocketConnectEvent",
     "WebSocketDisconnectEvent",
```

### Comparing `litestar-2.0.0b1/litestar/types/asgi_types.py` & `litestar-2.0.0b2/litestar/types/asgi_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Dict,
@@ -40,15 +41,17 @@
     Literal,
     Optional,
     Tuple,
     TypedDict,
     Union,
 )
 
-from litestar.enums import ScopeType
+from pydantic import BaseModel
+
+from litestar.types.empty import EmptyType
 
 __all__ = (
     "ASGIApp",
     "ASGIVersion",
     "BaseScope",
     "HeaderScope",
     "HTTPDisconnectEvent",
@@ -91,78 +94,78 @@
     "WebSocketScope",
     "WebSocketSendEvent",
     "WebSocketSendMessage",
 )
 
 
 if TYPE_CHECKING:
-    from pydantic import BaseModel
+    from typing_extensions import TypeAlias
 
     from litestar.app import Litestar
-    from litestar.types.empty import EmptyType
+    from litestar.enums import ScopeType
 
-    from .internal_types import RouteHandlerType
+    from .internal_types import LitestarType, RouteHandlerType
 
-Method = Literal["GET", "POST", "DELETE", "PATCH", "PUT", "HEAD", "TRACE", "OPTIONS"]
-ScopeSession = Optional[Union["EmptyType", Dict[str, Any], "BaseModel"]]
+Method: TypeAlias = Literal["GET", "POST", "DELETE", "PATCH", "PUT", "HEAD", "TRACE", "OPTIONS"]
+ScopeSession: TypeAlias = Optional[Union[EmptyType, Dict[str, Any], BaseModel]]
 
 
 class ASGIVersion(TypedDict):
     """ASGI spec version."""
 
     spec_version: str
     version: Literal["3.0"]
 
 
 class HeaderScope(TypedDict):
     """Base class for ASGI-scopes that supports headers."""
 
-    headers: "RawHeaders"
+    headers: RawHeaders
 
 
 class BaseScope(HeaderScope):
     """Base ASGI-scope."""
 
-    app: "Litestar"
+    app: LitestarType
     asgi: ASGIVersion
     auth: Any
-    client: Optional[Tuple[str, int]]
-    extensions: Optional[Dict[str, Dict[object, object]]]
+    client: tuple[str, int] | None
+    extensions: dict[str, dict[object, object]] | None
     http_version: str
     path: str
-    path_params: Dict[str, str]
+    path_params: dict[str, str]
     query_string: bytes
     raw_path: bytes
     root_path: str
-    route_handler: "RouteHandlerType"
+    route_handler: RouteHandlerType
     scheme: str
-    server: Optional[Tuple[str, Optional[int]]]
+    server: tuple[str, int | None] | None
     session: ScopeSession
-    state: Dict[str, Any]
+    state: dict[str, Any]
     user: Any
 
 
 class HTTPScope(BaseScope):
     """HTTP-ASGI-scope."""
 
-    method: "Method"
+    method: Method
     type: Literal[ScopeType.HTTP]
 
 
 class WebSocketScope(BaseScope):
     """WebSocket-ASGI-scope."""
 
-    subprotocols: List[str]
+    subprotocols: list[str]
     type: Literal[ScopeType.WEBSOCKET]
 
 
 class LifeSpanScope(TypedDict):
     """Lifespan-ASGI-scope."""
 
-    app: "Litestar"
+    app: Litestar
     asgi: ASGIVersion
     type: Literal["lifespan"]
 
 
 class HTTPRequestEvent(TypedDict):
     """ASGI `http.request` event."""
 
@@ -205,31 +208,31 @@
     type: Literal["websocket.connect"]
 
 
 class WebSocketAcceptEvent(HeaderScope):
     """ASGI `websocket.accept` event."""
 
     type: Literal["websocket.accept"]
-    subprotocol: Optional[str]
+    subprotocol: str | None
 
 
 class WebSocketReceiveEvent(TypedDict):
     """ASGI `websocket.receive` event."""
 
     type: Literal["websocket.receive"]
-    bytes: Optional[bytes]
-    text: Optional[str]
+    bytes: bytes | None
+    text: str | None
 
 
 class WebSocketSendEvent(TypedDict):
     """ASGI `websocket.send` event."""
 
     type: Literal["websocket.send"]
-    bytes: Optional[bytes]
-    text: Optional[str]
+    bytes: bytes | None
+    text: str | None
 
 
 class WebSocketResponseStartEvent(HeaderScope):
     """ASGI `websocket.http.response.start` event."""
 
     type: Literal["websocket.http.response.start"]
     status: int
@@ -251,15 +254,15 @@
 
 
 class WebSocketCloseEvent(TypedDict):
     """ASGI `websocket.close` event."""
 
     type: Literal["websocket.close"]
     code: int
-    reason: Optional[str]
+    reason: str | None
 
 
 class LifeSpanStartupEvent(TypedDict):
     """ASGI `lifespan.startup` event."""
 
     type: Literal["lifespan.startup"]
 
@@ -292,50 +295,50 @@
 class LifeSpanShutdownFailedEvent(TypedDict):
     """ASGI `lifespan.shutdown.failed` event."""
 
     type: Literal["lifespan.shutdown.failed"]
     message: str
 
 
-HTTPReceiveMessage = Union[
+HTTPReceiveMessage: TypeAlias = Union[
     HTTPRequestEvent,
     HTTPDisconnectEvent,
 ]
-WebSocketReceiveMessage = Union[
+WebSocketReceiveMessage: TypeAlias = Union[
     WebSocketConnectEvent,
     WebSocketReceiveEvent,
     WebSocketDisconnectEvent,
 ]
-LifeSpanReceiveMessage = Union[
+LifeSpanReceiveMessage: TypeAlias = Union[
     LifeSpanStartupEvent,
     LifeSpanShutdownEvent,
 ]
-HTTPSendMessage = Union[
+HTTPSendMessage: TypeAlias = Union[
     HTTPResponseStartEvent,
     HTTPResponseBodyEvent,
     HTTPServerPushEvent,
     HTTPDisconnectEvent,
 ]
-WebSocketSendMessage = Union[
+WebSocketSendMessage: TypeAlias = Union[
     WebSocketAcceptEvent,
     WebSocketSendEvent,
     WebSocketResponseStartEvent,
     WebSocketResponseBodyEvent,
     WebSocketCloseEvent,
 ]
-LifeSpanSendMessage = Union[
+LifeSpanSendMessage: TypeAlias = Union[
     LifeSpanStartupCompleteEvent,
     LifeSpanStartupFailedEvent,
     LifeSpanShutdownCompleteEvent,
     LifeSpanShutdownFailedEvent,
 ]
-LifeSpanReceive = Callable[..., Awaitable[LifeSpanReceiveMessage]]
-LifeSpanSend = Callable[[LifeSpanSendMessage], Awaitable[None]]
-Message = Union[HTTPSendMessage, WebSocketSendMessage]
-ReceiveMessage = Union[HTTPReceiveMessage, WebSocketReceiveMessage]
-Scope = Union[HTTPScope, WebSocketScope]
-Receive = Callable[..., Awaitable[Union[HTTPReceiveMessage, WebSocketReceiveMessage]]]
-Send = Callable[[Message], Awaitable[None]]
-ASGIApp = Callable[[Scope, Receive, Send], Awaitable[None]]
-RawHeaders = Iterable[Tuple[bytes, bytes]]
-RawHeadersList = List[Tuple[bytes, bytes]]
-WebSocketMode = Literal["text", "binary"]
+LifeSpanReceive: TypeAlias = Callable[..., Awaitable[LifeSpanReceiveMessage]]
+LifeSpanSend: TypeAlias = Callable[[LifeSpanSendMessage], Awaitable[None]]
+Message: TypeAlias = Union[HTTPSendMessage, WebSocketSendMessage]
+ReceiveMessage: TypeAlias = Union[HTTPReceiveMessage, WebSocketReceiveMessage]
+Scope: TypeAlias = Union[HTTPScope, WebSocketScope]
+Receive: TypeAlias = Callable[..., Awaitable[Union[HTTPReceiveMessage, WebSocketReceiveMessage]]]
+Send: TypeAlias = Callable[[Message], Awaitable[None]]
+ASGIApp: TypeAlias = Callable[[Scope, Receive, Send], Awaitable[None]]
+RawHeaders: TypeAlias = Iterable[Tuple[bytes, bytes]]
+RawHeadersList: TypeAlias = List[Tuple[bytes, bytes]]
+WebSocketMode: TypeAlias = Literal["text", "binary"]
```

### Comparing `litestar-2.0.0b1/litestar/types/file_types.py` & `litestar-2.0.0b2/litestar/types/file_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,38 @@
+from __future__ import annotations
+
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     AnyStr,
     Awaitable,
     Literal,
-    Optional,
     Protocol,
     TypedDict,
-    Union,
     overload,
 )
 
-from typing_extensions import NotRequired
-
 __all__ = ("FileInfo", "FileSystemProtocol")
 
 
 if TYPE_CHECKING:
     from _typeshed import OpenBinaryMode, OpenTextMode
     from anyio import AsyncFile
+    from typing_extensions import NotRequired
 
     from litestar.types.composite_types import PathType
 
 
 class FileInfo(TypedDict):
     """File information gathered from a file system."""
 
     created: float
     """Created time stamp, equal to 'stat_result.st_ctime'."""
-    destination: NotRequired[Optional[bytes]]
+    destination: NotRequired[bytes | None]
     """Output of loading a symbolic link."""
     gid: int
     """Group ID of owner."""
     ino: int
     """inode value."""
     islink: bool
     """True if the file is a symbolic link."""
@@ -56,50 +55,50 @@
 class FileSystemProtocol(Protocol):
     """Base protocol used to interact with a file-system.
 
     This protocol is commensurable with the file systems
     exported by the `fsspec <https://filesystem-spec.readthedocs.io/en/latest/>` library.
     """
 
-    def info(self, path: "PathType", **kwargs: Any) -> Union[FileInfo, Awaitable[FileInfo]]:
+    def info(self, path: PathType, **kwargs: Any) -> FileInfo | Awaitable[FileInfo]:
         """Retrieve information about a given file path.
 
         Args:
             path: A file path.
             **kwargs: Any additional kwargs.
 
         Returns:
             A dictionary of file info.
         """
         ...
 
     @overload
     def open(
         self,
-        file: "PathType",
-        mode: "OpenBinaryMode",
+        file: PathType,
+        mode: OpenBinaryMode,
         buffering: int = -1,
-    ) -> Union[IO[bytes], Awaitable["AsyncFile[bytes]"]]:
+    ) -> IO[bytes] | Awaitable[AsyncFile[bytes]]:
         ...
 
     @overload
     def open(
         self,
-        file: "PathType",
-        mode: "OpenTextMode",
+        file: PathType,
+        mode: OpenTextMode,
         buffering: int = -1,
-    ) -> Union[IO[str], Awaitable["AsyncFile[str]"]]:
+    ) -> IO[str] | Awaitable[AsyncFile[str]]:
         ...
 
     def open(  # pyright: ignore
         self,
-        file: "PathType",
+        file: PathType,
         mode: str,
         buffering: int = -1,
-    ) -> Union[IO[AnyStr], Awaitable["AsyncFile[AnyStr]"]]:
+    ) -> IO[AnyStr] | Awaitable[AsyncFile[AnyStr]]:
         """Return a file-like object from the filesystem.
 
         Notes:
             - The return value must function correctly in a context ``with`` block.
 
         Args:
             file: Path to the target file.
```

### Comparing `litestar-2.0.0b1/litestar/types/protocols.py` & `litestar-2.0.0b2/litestar/types/protocols.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,12 +103,12 @@
     __dataclass_fields__: ClassVar[dict[str, Any]]
 
 
 T_co = TypeVar("T_co", covariant=True)
 
 
 @runtime_checkable
-class InstantiableCollection(Collection[T_co], Protocol[T_co]):
+class InstantiableCollection(Collection[T_co], Protocol[T_co]):  # pyright: ignore
     """A protocol for instantiable collection types."""
 
     def __init__(self, iterable: Iterable[T_co], /) -> None:
         ...
```

### Comparing `litestar-2.0.0b1/litestar/types/serialization.py` & `litestar-2.0.0b2/litestar/types/serialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,23 @@
         StrictBool,
     )
     from pydantic.color import Color
     from typing_extensions import TypeAlias
 
     from litestar.types import DataclassProtocol
 
-__all__ = ("LitestarEncodableType",)
+__all__ = (
+    "LitestarEncodableType",
+    "EncodableBuiltinType",
+    "EncodableBuiltinCollectionType",
+    "EncodableStdLibType",
+    "EncodableStdLibIPType",
+    "EncodableMsgSpecType",
+    "EncodablePydanticType",
+)
 
 EncodableBuiltinType: TypeAlias = "None | bool | int | float | str | bytes | bytearray"
 EncodableBuiltinCollectionType: TypeAlias = "list | tuple | set | frozenset | dict | Collection"
 EncodableStdLibType: TypeAlias = (
     "date | datetime | deque | time | UUID | Decimal | Enum | IntEnum | DataclassProtocol | Path | PurePath | Pattern"
 )
 EncodableStdLibIPType: TypeAlias = (
```

### Comparing `litestar-2.0.0b1/litestar/typing.py` & `litestar-2.0.0b2/litestar/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections import abc
 from dataclasses import dataclass
 from typing import Any, AnyStr, Collection, ForwardRef, Mapping, TypeVar
 
 from typing_extensions import Annotated, NotRequired, Required, get_args, get_origin
 
-from litestar.types.builtin_types import UNION_TYPES, NoneType
+from litestar.types.builtin_types import NoneType, UnionTypes
 from litestar.utils.typing import get_instantiable_origin, get_safe_generic_origin, unwrap_annotation
 
 __all__ = ("ParsedType",)
 
 
 @dataclass(frozen=True, init=False)
 class ParsedType:
@@ -112,15 +112,15 @@
     def is_type_var(self) -> bool:
         """Whether the annotation is a TypeVar or not."""
         return isinstance(self.annotation, TypeVar)
 
     @property
     def is_union(self) -> bool:
         """Whether the annotation is a union type or not."""
-        return self.origin in UNION_TYPES
+        return self.origin in UnionTypes
 
     @property
     def is_optional(self) -> bool:
         """Whether the annotation is Optional or not."""
         return bool(self.is_union and NoneType in self.args)
 
     @property
@@ -142,18 +142,18 @@
         Args:
             cl: The type to check, or tuple of types. Passed as 2nd argument to ``issubclass()``.
 
         Returns:
             Whether the annotation is a subtype of the given type(s).
         """
         if self.origin:
-            if self.origin in UNION_TYPES:
+            if self.origin in UnionTypes:
                 return all(t.is_subclass_of(cl) for t in self.inner_types)
 
-            return self.origin not in UNION_TYPES and issubclass(self.origin, cl)
+            return self.origin not in UnionTypes and issubclass(self.origin, cl)
 
         if self.annotation is AnyStr:
             return issubclass(str, cl) or issubclass(bytes, cl)
         return self.annotation is not Any and not self.is_type_var and issubclass(self.annotation, cl)
 
     def has_inner_subclass_of(self, cl: type[Any] | tuple[type[Any], ...]) -> bool:
         """Whether any generic args are a subclass of the given type.
```

### Comparing `litestar-2.0.0b1/litestar/utils/__init__.py` & `litestar-2.0.0b2/litestar/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from litestar.utils.deprecation import deprecated, warn_deprecation
 
 from .helpers import Ref, encode_headers, get_enum_string_value, get_name, url_quote
 from .path import join_paths, normalize_path
 from .predicates import (
+    is_annotated_type,
     is_any,
     is_async_callable,
     is_attrs_class,
     is_class_and_subclass,
     is_class_var,
     is_dataclass_class,
     is_dataclass_instance,
@@ -44,14 +45,15 @@
     "find_index",
     "get_enum_string_value",
     "get_litestar_scope_state",
     "get_name",
     "get_origin_or_inner_type",
     "get_serializer_from_scope",
     "is_any",
+    "is_annotated_type",
     "is_async_callable",
     "is_attrs_class",
     "is_class_and_subclass",
     "is_class_var",
     "is_dataclass_class",
     "is_dataclass_instance",
     "is_generic",
```

### Comparing `litestar-2.0.0b1/litestar/utils/compat.py` & `litestar-2.0.0b2/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/utils/dataclass.py` & `litestar-2.0.0b2/litestar/utils/dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def extract_dataclass_fields(
     dt: DataclassProtocol,
     exclude_none: bool = False,
     exclude_empty: bool = False,
     include: AbstractSet[str] | None = None,
     exclude: AbstractSet[str] | None = None,
-) -> tuple[Field, ...]:
+) -> tuple[Field[Any], ...]:
     """Extract dataclass fields.
 
     Args:
         dt: A dataclass instance.
         exclude_none: Whether to exclude None values.
         exclude_empty: Whether to exclude Empty values.
         include: An iterable of fields to include.
@@ -40,15 +40,15 @@
     """
     include = include or set()
     exclude = exclude or set()
 
     if common := (include & exclude):
         raise ValueError(f"Fields {common} are both included and excluded.")
 
-    dataclass_fields: Iterable[Field] = fields(dt)
+    dataclass_fields: Iterable[Field[Any]] = fields(dt)
     if exclude_none:
         dataclass_fields = (field for field in dataclass_fields if getattr(dt, field.name) is not None)
     if exclude_empty:
         dataclass_fields = (field for field in dataclass_fields if getattr(dt, field.name) is not Empty)
     if include:
         dataclass_fields = (field for field in dataclass_fields if field.name in include)
     if exclude:
```

### Comparing `litestar-2.0.0b1/litestar/utils/deprecation.py` & `litestar-2.0.0b2/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/utils/helpers.py` & `litestar-2.0.0b2/litestar/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     Args:
         local_cookies: Cookies returned from the local scope.
         layered_cookies: Cookies returned from the layers.
 
     Returns:
         A unified list of cookies
     """
-    return [cookie for cookie in {*local_cookies, *layered_cookies} if not cookie.documentation_only]
+    return [cookie for cookie in {*local_cookies, *layered_cookies} if not cookie.documentation_only]  # noqa: PLC0208
 
 
 def url_quote(value: str | bytes) -> str:
     """Quote a URL.
 
     Args:
         value: A URL.
```

### Comparing `litestar-2.0.0b1/litestar/utils/path.py` & `litestar-2.0.0b2/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/utils/predicates.py` & `litestar-2.0.0b2/litestar/utils/predicates.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,21 @@
     TypeVar,
 )
 
 from msgspec import Struct
 from typing_extensions import (
     ParamSpec,
     TypeGuard,
+    _AnnotatedAlias,
     get_args,
     is_typeddict,
 )
 
 from litestar.types import Empty
-from litestar.types.builtin_types import UNION_TYPES, NoneType
+from litestar.types.builtin_types import NoneType, UnionTypes
 from litestar.utils.typing import get_origin_or_inner_type
 
 if TYPE_CHECKING:
     from litestar.types.builtin_types import TypedDictClass
     from litestar.types.callable_types import AnyGenerator
     from litestar.types.protocols import DataclassProtocol
 
@@ -233,43 +234,43 @@
 
     Returns:
         A typeguard determining whether the type is :data:`Any <typing.Any>`.
     """
     return (
         annotation is Any
         or getattr(annotation, "_name", "") == "typing.Any"
-        or (get_origin_or_inner_type(annotation) in UNION_TYPES and Any in get_args(annotation))
+        or (get_origin_or_inner_type(annotation) in UnionTypes and Any in get_args(annotation))
     )
 
 
 def is_union(annotation: Any) -> bool:
     """Given a type annotation determine if the annotation infers an optional union.
 
     Args:
         annotation: A type.
 
     Returns:
         A boolean determining whether the type is :data:`Union typing.Union>`.
     """
-    return get_origin_or_inner_type(annotation) in UNION_TYPES
+    return get_origin_or_inner_type(annotation) in UnionTypes
 
 
 def is_optional_union(annotation: Any) -> TypeGuard[Any | None]:
     """Given a type annotation determine if the annotation infers an optional union.
 
     Args:
         annotation: A type.
 
     Returns:
         A typeguard determining whether the type is :data:`Union typing.Union>` with a
             None value or :data:`Optional <typing.Optional>` which is equivalent.
     """
     origin = get_origin_or_inner_type(annotation)
     return origin is Optional or (
-        get_origin_or_inner_type(annotation) in UNION_TYPES and NoneType in get_args(annotation)
+        get_origin_or_inner_type(annotation) in UnionTypes and NoneType in get_args(annotation)
     )
 
 
 def is_typed_dict(annotation: Any) -> TypeGuard[TypedDictClass]:
     """Wrap :func:`typing.is_typeddict` in a :data:`typing.TypeGuard`.
 
     Args:
@@ -398,7 +399,19 @@
     Args:
         obj: type to be tested for sync or async generator.
 
     Returns:
         A boolean.
     """
     return isgeneratorfunction(obj) or isasyncgenfunction(obj)
+
+
+def is_annotated_type(annotation: Any) -> bool:
+    """Check if the given annotation is an Annotated.
+
+    Args:
+        annotation: A type annotation
+
+    Returns:
+        A boolean.
+    """
+    return isinstance(annotation, _AnnotatedAlias) and getattr(annotation, "__args__", None) is not None
```

### Comparing `litestar-2.0.0b1/litestar/utils/scope.py` & `litestar-2.0.0b2/litestar/utils/scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/utils/sequence.py` & `litestar-2.0.0b2/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/utils/signature.py` & `litestar-2.0.0b2/litestar/utils/signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/utils/sync.py` & `litestar-2.0.0b2/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/utils/typing.py` & `litestar-2.0.0b2/litestar/utils/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     TypeVar,
     Union,
     cast,
 )
 
 from typing_extensions import Annotated, NotRequired, Required, TypeGuard, get_args, get_origin
 
-from litestar.types.builtin_types import UNION_TYPES, NoneType
+from litestar.types.builtin_types import NoneType, UnionTypes
 
 __all__ = (
     "annotation_is_iterable_of_type",
     "get_instantiable_origin",
     "get_origin_or_inner_type",
     "get_safe_generic_origin",
     "instantiable_type_mapping",
@@ -104,15 +104,15 @@
     abc.Generator: t.Generator,
     abc.Reversible: t.Reversible,
     abc.Coroutine: t.Coroutine,
     abc.AsyncGenerator: t.AsyncGenerator,
     abc.AsyncIterable: t.AsyncIterable,
     abc.AsyncIterator: t.AsyncIterator,
     abc.Awaitable: t.Awaitable,
-    **{union_t: t.Union for union_t in UNION_TYPES},  # type:ignore[misc]
+    **{union_t: t.Union for union_t in UnionTypes},
 }
 """A mapping of types to equivalent types that are safe to be used as generics across all Python versions.
 
 This is necessary because occasionally we want to rebuild a generic outer type with different args, and types such as
 ``collections.abc.Mapping``, are not valid generic types in Python 3.8.
 """
```

### Comparing `litestar-2.0.0b1/litestar/utils/version.py` & `litestar-2.0.0b2/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/litestar/utils/warnings.py` & `litestar-2.0.0b2/litestar/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0b1/pyproject.toml` & `litestar-2.0.0b2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litestar"
-version = "2.0.0beta1"
+version = "2.0.0beta2"
 description = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
@@ -59,94 +59,101 @@
 "Reddit" = "https://www.reddit.com/r/litestarapi"
 "Discord" = "https://discord.gg/MmcwxztmQb"
 "Blog" = "https://blog.litestar.dev"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 alembic = { version = "*", optional = true }
+annotated-types = { version = "*", optional = true }
 anyio = ">=3"
 attrs = { version = "*", optional = true }
 brotli = { version = "*", optional = true }
 cattrs = { version = "*", optional = true }
 click = { version = "*", optional = true }
 cryptography = { version = "*", optional = true }
 fast-query-parsers = "*"
 httpx = ">=0.22"
 importlib-metadata = { version = "*", python = "<3.10" }
+importlib-resources = { version = ">=5.12.0", python = "<3.9" }
 jinja2 = { version = ">=3.1.2", optional = true }
 jsbeautifier = { version = "*", optional = true }
 mako = { version = ">=1.2.4", optional = true }
-msgspec = "*"
+msgspec = ">=0.16.0"
 multidict = ">=6.0.2"
 opentelemetry-instrumentation-asgi = { version = "*", optional = true }
 picologging = { version = "*", optional = true }
-polyfactory = ">=2"
+polyfactory = ">=2.3.2"
+prometheus-client = {version = "*", optional = true}
 pydantic = "<2"
 python-dateutil = { version = "*", optional = true }
 python-jose = { version = "*", optional = true }
 pytimeparse = { version = "*", optional = true }
 pyyaml = "*"
-redis = { version = ">=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3,!=4.5.5", optional = true, extras = ["hiredis"] }
+redis = { version = ">=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3,!=4.5.5", optional = true, extras = [
+    "hiredis",
+] }
 rich = { version = ">=13.0.0", optional = true }
 rich-click = { version = "*", optional = true }
 sqlalchemy = { version = ">=2.0.12", optional = true }
 structlog = { version = "*", optional = true }
+tortoise-orm = { version = ">=0.17.0", optional = true }
 typing-extensions = "*"
-uvicorn = {extras = ["standard"], version = "^0.22.0", optional = true}
-importlib-resources = { version="^5.12.0", python = "<3.9" }
+uvicorn = { extras = ["standard"], version = ">=0.22.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 aiosqlite = "*"
-rich-click = "*"
 alembic = "*"
+annotated-types = "*"
 asyncmy = "*"
 asyncpg = "*"
 attrs = "*"
 beanie = "*"
 beautifulsoup4 = "*"
 brotli = "*"
 cattrs = "*"
 click = "*"
 cryptography = "*"
-fakeredis = { extras = ["lua"], version = "2.11.0" }
+duckdb-engine = "*"
+fakeredis = { extras = ["lua"], version = "*" }
 freezegun = "*"
 fsspec = "*"
 greenlet = "*"
 hypothesis = "*"
 jinja2 = "*"
 jsbeautifier = "*"
 mako = "*"
 mongomock-motor = { version = "*", markers = "sys_platform != 'win32'" }
 opentelemetry-instrumentation-asgi = "*"
 opentelemetry-sdk = "*"
+oracledb = "*"
 piccolo = "*"
 picologging = "*"
 pre-commit = "*"
+prometheus-client = "*"
 psycopg = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-lazy-fixture = "*"
 pytest-mock = "*"
+pytest-rerunfailures = "*"
 python-dateutil = "*"
 python-dotenv = "*"
 python-jose = "*"
-oracledb = "*"
 pytimeparse = "*"
 redis = "*"
 rich = "*"
+rich-click = "*"
 sqlalchemy = ">=2.0"
+sqlalchemy-spanner = "*"
 starlette = "*"
 structlog = "*"
-tortoise-orm = ">=0.17.0"
+tortoise-orm = "*"
 trio = "*"
 uvicorn = "*"
-pytest-rerunfailures = "^11.1.2"
-duckdb-engine = "*"
-sqlalchemy-spanner = "*"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 auto-pytabs = { extras = ["sphinx"], version = "*" }
 black = "*"
@@ -163,51 +170,53 @@
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 asyncpg-stubs = "*"
 black = "*"
 blacken-docs = "*"
 mypy = "*"
-pylint = "*"
-pylint-pydantic = "*"
 pyright = "*"
 ruff = '*'
 slotscheck = "*"
 types-freezegun = "*"
 types-python-jose = "*"
 types-pyyaml = "*"
 types-redis = "*"
 types-beautifulsoup4 = "*"
 types-python-dateutil = "*"
 
 [tool.poetry.extras]
+annotated-types = ["annotated-types"]
 attrs = ["attrs", "cattrs", "python-dateutil", "pytimeparse"]
 brotli = ["brotli"]
 cli = ["click", "rich", "rich-click", "jsbeautifier", "uvicorn"]
 cryptography = ["cryptography"]
 jinja = ["jinja2"]
 jwt = ["python-jose", "cryptography"]
 opentelemetry = ["opentelemetry-instrumentation-asgi"]
 picologging = ["picologging"]
 redis = ["redis"]
 sqlalchemy = ["sqlalchemy", "alembic"]
 standard = ["click", "jinja2", "jsbeautifier", "rich", "uvicorn", "rich-click"]
 structlog = ["structlog"]
 tortoise-orm = ["tortoise-orm"]
+prometheus = ["prometheus-client"]
+
 full = [
     "alembic",
     "attrs",
     "brotli",
     "cattrs",
     "click",
     "cryptography",
     "jinja2",
     "jsbeautifier",
     "opentelemetry-instrumentation-asgi",
-    "python-dateutill",
+    "prometheus-client",
+    "python-dateutil",
     "python-jose",
     "pytimeparse",
     "redis",
     "rich",
     "sqlalchemy",
     "structlog",
     "uvicorn",
@@ -267,29 +276,24 @@
     "sqlalchemy_duckdb: SQLAlchemy Duckdb (duckdb-engine) Tests",
 ]
 
 [tool.pyright]
 include = ["litestar", "tests", "examples"]
 exclude = [
     "examples/plugins/sqlalchemy_plugin",
-    "litestar/contrib/sqlalchemy_1",
     "litestar/openapi",
-    "litestar/plugins",
-    "tests/contrib/sqlalchemy/test_dto.py",
-    "tests/contrib/sqlalchemy_1",
-    "tests/openapi",
-    "tests/plugins",
+    "tests/unit/test_contrib/test_sqlalchemy/test_dto.py",
 ]
 
 [tool.slotscheck]
 strict-imports = false
 
 [tool.ruff]
 select = [
-    "A", # flake8-builtins
+    "A",   # flake8-builtins
     "B",   # flake8-bugbear
     "BLE", # flake8-blind-except
     "C4",  # flake8-comprehensions
     "C90", # mccabe
     "D",   # pydocstyle
     "DJ",  # flake8-django
     "DTZ", # flake8-datetimez
@@ -318,29 +322,30 @@
     "TID", # flake8-tidy-imports
     "UP",  # pyupgrade
     "W",   # pycodestyle - warning
     "YTT", # flake8-2020
 ]
 
 ignore = [
-    "A003",  # flake8-builtins - class attribute {name} is shadowing a python builtin
-    "B010",  # flake8-bugbear - do not call setattr with a constant attribute value
-    "D100",  # pydocstyle - missing docstring in public module
-    "D101",  # pydocstyle - missing docstring in public class
-    "D102",  # pydocstyle - missing docstring in public method
-    "D103",  # pydocstyle - missing docstring in public function
-    "D104",  # pydocstyle - missing docstring in public package
-    "D105",  # pydocstyle - missing docstring in magic method
-    "D106",  # pydocstyle - missing docstring in public nested class
-    "D107",  # pydocstyle - missing docstring in __init__
-    "D202",  # pydocstyle - no blank lines allowed after function docstring
-    "D205",  # pydocstyle - 1 blank line required between summary line and description
-    "D415",  # pydocstyle - first line should end with a period, question mark, or exclamation point
-    "E501",  # pycodestyle line too long, handled by black
-    "PLW2901"  # pylint - for loop variable overwritten by assignment target
+    "A003",    # flake8-builtins - class attribute {name} is shadowing a python builtin
+    "B010",    # flake8-bugbear - do not call setattr with a constant attribute value
+    "D100",    # pydocstyle - missing docstring in public module
+    "D101",    # pydocstyle - missing docstring in public class
+    "D102",    # pydocstyle - missing docstring in public method
+    "D103",    # pydocstyle - missing docstring in public function
+    "D104",    # pydocstyle - missing docstring in public package
+    "D105",    # pydocstyle - missing docstring in magic method
+    "D106",    # pydocstyle - missing docstring in public nested class
+    "D107",    # pydocstyle - missing docstring in __init__
+    "D202",    # pydocstyle - no blank lines allowed after function docstring
+    "D205",    # pydocstyle - 1 blank line required between summary line and description
+    "D415",    # pydocstyle - first line should end with a period, question mark, or exclamation point
+    "E501",    # pycodestyle line too long, handled by black
+    "PLW2901", # pylint - for loop variable overwritten by assignment target
+    "RUF012",  # Ruff-specific rule - annotated with classvar
 ]
 line-length = 120
 src = ["litestar", "tests", "docs/examples"]
 target-version = "py38"
 
 [tool.ruff.pydocstyle]
 convention = "google"
@@ -351,15 +356,15 @@
 [tool.ruff.pep8-naming]
 classmethod-decorators = [
     "classmethod",
     "pydantic.root_validator",
     "pydantic.validator",
     "sqlalchemy.ext.declarative.declared_attr",
     "sqlalchemy.orm.declared_attr.directive",
-    "sqlalchemy.orm.declared_attr"
+    "sqlalchemy.orm.declared_attr",
 ]
 
 [tool.ruff.isort]
 known-first-party = ["litestar", "tests", "examples"]
 
 [tool.ruff.per-file-ignores]
 "tests/**/*.*" = [
@@ -418,18 +423,17 @@
 "litestar/exceptions/*.*" = ["N818"]
 "litestar/handlers/**/*.*" = ["N801"]
 "litestar/_openapi/schema_generation/schema.py" = ["C901"]
 "litestar/params.py" = ["N802"]
 "test_apps/**/*.*" = ["D", "TRY", "EM", "S", "PTH"]
 "tools/**/*.*" = ["D", "ARG", "EM", "TRY", "G", "FBT"]
 
-
 [tool.unasyncd]
 add_editors_note = true
-
+ruff_fix = true
 
 [tool.unasyncd.files]
 "litestar/contrib/sqlalchemy/repository/_async.py" = "litestar/contrib/sqlalchemy/repository/_sync.py"
 "litestar/contrib/repository/abc/_async.py" = "litestar/contrib/repository/abc/_sync.py"
 
 [tool.unasyncd.per_file_add_replacements."litestar/contrib/repository/abc/_async.py"]
 "AbstractAsyncRepository" = "AbstractSyncRepository"
```

### Comparing `litestar-2.0.0b1/PKG-INFO` & `litestar-2.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litestar
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Litestar - A production-ready, highly performant, extensible ASGI API Framework
 Home-page: https://litestar.dev/
 License: MIT
 Keywords: api,rest,http,asgi,pydantic,litestar,starlite,framework,websocket,litestar
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -21,72 +21,77 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
+Provides-Extra: annotated-types
 Provides-Extra: attrs
 Provides-Extra: brotli
 Provides-Extra: cli
 Provides-Extra: cryptography
 Provides-Extra: full
 Provides-Extra: jinja
 Provides-Extra: jwt
 Provides-Extra: opentelemetry
 Provides-Extra: picologging
+Provides-Extra: prometheus
 Provides-Extra: redis
 Provides-Extra: sqlalchemy
 Provides-Extra: standard
 Provides-Extra: structlog
 Provides-Extra: tortoise-orm
 Requires-Dist: alembic ; extra == "sqlalchemy" or extra == "full"
+Requires-Dist: annotated-types ; extra == "annotated-types"
 Requires-Dist: anyio (>=3)
 Requires-Dist: attrs ; extra == "attrs" or extra == "full"
 Requires-Dist: brotli ; extra == "brotli" or extra == "full"
 Requires-Dist: cattrs ; extra == "attrs" or extra == "full"
 Requires-Dist: click ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: cryptography ; extra == "cryptography" or extra == "jwt" or extra == "full"
 Requires-Dist: fast-query-parsers
 Requires-Dist: httpx (>=0.22)
 Requires-Dist: importlib-metadata ; python_version < "3.10"
-Requires-Dist: importlib-resources (>=5.12.0,<6.0.0) ; python_version < "3.9"
+Requires-Dist: importlib-resources (>=5.12.0) ; python_version < "3.9"
 Requires-Dist: jinja2 (>=3.1.2) ; extra == "jinja" or extra == "standard" or extra == "full"
 Requires-Dist: jsbeautifier ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: mako (>=1.2.4)
-Requires-Dist: msgspec
+Requires-Dist: msgspec (>=0.16.0)
 Requires-Dist: multidict (>=6.0.2)
 Requires-Dist: opentelemetry-instrumentation-asgi ; extra == "opentelemetry" or extra == "full"
 Requires-Dist: picologging ; extra == "picologging"
-Requires-Dist: polyfactory (>=2)
+Requires-Dist: polyfactory (>=2.3.2)
+Requires-Dist: prometheus-client ; extra == "prometheus" or extra == "full"
 Requires-Dist: pydantic (<2)
-Requires-Dist: python-dateutil ; extra == "attrs"
+Requires-Dist: python-dateutil ; extra == "attrs" or extra == "full"
 Requires-Dist: python-jose ; extra == "jwt" or extra == "full"
 Requires-Dist: pytimeparse ; extra == "attrs" or extra == "full"
 Requires-Dist: pyyaml
 Requires-Dist: redis[hiredis] (>=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3,!=4.5.5) ; extra == "redis" or extra == "full"
 Requires-Dist: rich (>=13.0.0) ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: rich-click ; extra == "cli" or extra == "standard"
 Requires-Dist: sqlalchemy (>=2.0.12) ; extra == "sqlalchemy" or extra == "full"
 Requires-Dist: structlog ; extra == "structlog" or extra == "full"
+Requires-Dist: tortoise-orm (>=0.17.0) ; extra == "tortoise-orm"
 Requires-Dist: typing-extensions
-Requires-Dist: uvicorn[standard] (>=0.22.0,<0.23.0) ; extra == "cli" or extra == "standard" or extra == "full"
+Requires-Dist: uvicorn[standard] (>=0.22.0) ; extra == "cli" or extra == "standard" or extra == "full"
 Project-URL: Blog, https://blog.litestar.dev
 Project-URL: Changelog, https://github.com/litestar-org/litestar/releases/
 Project-URL: Documentation, https://docs.litestar.dev/
 Project-URL: Discord, https://discord.gg/MmcwxztmQb
 Project-URL: Issue Tracker, https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
 Project-URL: Repository, https://github.com/litestar-org/litestar
 Project-URL: Reddit, https://www.reddit.com/r/litestarapi
 Project-URL: Twitter, https://twitter.com/LitestarAPI
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable -->
 <p align="center">
-  <img src="artwork/banner-light.svg" alt="Litestar Logo - Light" width="100%" height="auto" />
+  <img src="https://github.com/litestar-org/litestar/blob/ecb4412055710f78124710990584aa24fc6c9a55/artwork/banner-light.svg" alt="Litestar Logo - Light" width="100%" height="auto" />
 </p>
 <!-- markdownlint-restore -->
 
 <div align="center">
 
 [![ci](https://github.com/litestar-org/litestar/actions/workflows/ci.yaml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/ci.yaml)
 [![PyPI - Version](https://badge.fury.io/py/litestar.svg)](https://badge.fury.io/py/litestar)
@@ -130,15 +135,15 @@
 pip install litestar
 ```
 
 **Litestar 2.0 is coming out soon**, bringing many new features and improvements.
 You can check out the alpha version by instead running
 
 ```shell
-pip install litestar==2.0.0alpha7
+pip install litestar==2.0.0beta1
 ```
 
 ## Quick Start
 
 ```python
 from litestar import Litestar, get
```

