# Comparing `tmp/dipdup-6.5.9.tar.gz` & `tmp/dipdup-7.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipdup-6.5.9.tar", max compression
+gzip compressed data, was "dipdup-7.0.0rc1.tar", last modified: Fri Jul 21 13:04:17 2023, max compression
```

## Comparing `dipdup-6.5.9.tar` & `dipdup-7.0.0rc1.tar`

### file list

```diff
@@ -1,169 +1,1111 @@
--rw-r--r--   0        0        0     1067 2023-07-11 14:03:03.119680 dipdup-6.5.9/LICENSE
--rw-r--r--   0        0        0     3992 2023-07-11 14:03:03.119680 dipdup-6.5.9/README.md
--rw-r--r--   0        0        0     2786 2023-07-11 14:03:03.147680 dipdup-6.5.9/pyproject.toml
--rw-r--r--   0        0        0      213 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/__init__.py
--rw-r--r--   0        0        0      106 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/__main__.py
--rw-r--r--   0        0        0      585 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/baking_bad.py
--rw-r--r--   0        0        0    19164 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/cli.py
--rw-r--r--   0        0        0    22413 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/codegen.py
--rw-r--r--   0        0        0    70122 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/config.py
--rw-r--r--   0        0        0    25902 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/context.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/coinbase/__init__.py
--rw-r--r--   0        0        0     2387 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/coinbase/datasource.py
--rw-r--r--   0        0        0     1309 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/coinbase/models.py
--rw-r--r--   0        0        0     6291 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/datasource.py
--rw-r--r--   0        0        0     2420 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/factory.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/ipfs/__init__.py
--rw-r--r--   0        0        0      688 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/ipfs/datasource.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/metadata/__init__.py
--rw-r--r--   0        0        0     1773 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/metadata/datasource.py
--rw-r--r--   0        0        0      161 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/metadata/enums.py
--rw-r--r--   0        0        0     2172 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/subscription.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/tzkt/__init__.py
--rw-r--r--   0        0        0    47179 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/tzkt/datasource.py
--rw-r--r--   0        0        0     9895 2023-07-11 14:03:03.147680 dipdup-6.5.9/src/dipdup/datasources/tzkt/models.py
--rw-r--r--   0        0        0    25010 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/dipdup.py
--rw-r--r--   0        0        0     2013 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/enums.py
--rw-r--r--   0        0        0     2192 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/env.py
--rw-r--r--   0        0        0     9500 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/exceptions.py
--rw-r--r--   0        0        0     2734 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/fetcher.py
--rw-r--r--   0        0        0    25590 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/hasura.py
--rw-r--r--   0        0        0     9884 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/http.py
--rw-r--r--   0        0        0     7414 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/index.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/big_map/__init__.py
--rw-r--r--   0        0        0     3033 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/big_map/fetcher.py
--rw-r--r--   0        0        0     7103 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/big_map/index.py
--rw-r--r--   0        0        0     2131 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/big_map/matcher.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/event/__init__.py
--rw-r--r--   0        0        0     1402 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/event/fetcher.py
--rw-r--r--   0        0        0     5324 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/event/index.py
--rw-r--r--   0        0        0     3297 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/event/matcher.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/head/__init__.py
--rw-r--r--   0        0        0     2320 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/head/index.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/operation/__init__.py
--rw-r--r--   0        0        0    19397 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/operation/fetcher.py
--rw-r--r--   0        0        0    13470 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/operation/index.py
--rw-r--r--   0        0        0     8314 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/operation/matcher.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/token_transfer/__init__.py
--rw-r--r--   0        0        0     1357 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/token_transfer/fetcher.py
--rw-r--r--   0        0        0     5377 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/token_transfer/index.py
--rw-r--r--   0        0        0     1791 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/indexes/token_transfer/matcher.py
--rwxr-xr-x   0        0        0     8269 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/install.py
--rw-r--r--   0        0        0    22702 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/models.py
--rw-r--r--   0        0        0    10978 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/project.py
--rw-r--r--   0        0        0      203 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/.dockerignore.j2
--rw-r--r--   0        0        0     2097 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/.gitignore.j2
--rw-r--r--   0        0        0      431 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/Dockerfile.j2
--rw-r--r--   0        0        0      474 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/README.md.j2
--rw-r--r--   0        0        0      489 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/dipdup.dev.yml.j2
--rw-r--r--   0        0        0      481 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/dipdup.prod.yml.j2
--rw-r--r--   0        0        0     2907 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/docker-compose.swarm.yml.j2
--rw-r--r--   0        0        0     1341 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/docker-compose.yml.j2
--rw-r--r--   0        0        0       37 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/replay.json.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/src/{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/src/{{cookiecutter.package}}/py.typed.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/__init__.py.j2
--rw-r--r--   0        0        0      197 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/base/tests/test_{{cookiecutter.package}}/test_{{cookiecutter.package}}.py.j2
--rw-r--r--   0        0        0      128 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/blank/dipdup.yml.j2
--rw-r--r--   0        0        0       95 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-auction.json
--rw-r--r--   0        0        0       98 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-big-maps.json
--rw-r--r--   0        0        0       83 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-dao.json
--rw-r--r--   0        0        0       83 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-dex.json
--rw-r--r--   0        0        0       95 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-domains.json
--rw-r--r--   0        0        0       92 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-events.json
--rw-r--r--   0        0        0      101 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-factories.json
--rw-r--r--   0        0        0       86 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-head.json
--rw-r--r--   0        0        0      119 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-nft-marketplace.json
--rw-r--r--   0        0        0       83 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-raw.json
--rw-r--r--   0        0        0      119 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-token-transfers.json
--rw-r--r--   0        0        0       89 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo-token.json
--rw-r--r--   0        0        0     1116 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      918 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2
--rw-r--r--   0        0        0     1624 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2
--rw-r--r--   0        0        0      853 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_withdraw.py.j2
--rw-r--r--   0        0        0     1524 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      779 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      847 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2
--rw-r--r--   0        0        0     1713 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2
--rw-r--r--   0        0        0      840 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      702 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      416 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     4878 2023-07-11 14:03:03.151680 dipdup-6.5.9/src/dipdup/projects/demo_dex/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0     1842 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1769 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2
--rw-r--r--   0        0        0      587 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2
--rw-r--r--   0        0        0     1642 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2
--rw-r--r--   0        0        0     1689 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2
--rw-r--r--   0        0        0     1039 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2
--rw-r--r--   0        0        0      960 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2
--rw-r--r--   0        0        0     1868 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2
--rw-r--r--   0        0        0     1795 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2
--rw-r--r--   0        0        0      581 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2
--rw-r--r--   0        0        0     1636 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2
--rw-r--r--   0        0        0     1655 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2
--rw-r--r--   0        0        0     1160 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2
--rw-r--r--   0        0        0      956 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2
--rw-r--r--   0        0        0      948 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      900 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      564 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2
--rw-r--r--   0        0        0      536 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2
--rw-r--r--   0        0        0     1475 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2
--rw-r--r--   0        0        0      819 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      592 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_events/dipdup.yml.j2
--rw-r--r--   0        0        0      976 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      716 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_factory_origination.py.j2
--rw-r--r--   0        0        0      416 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_origination.py.j2
--rw-r--r--   0        0        0      523 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2
--rw-r--r--   0        0        0      858 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      333 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_head/dipdup.yml.j2
--rw-r--r--   0        0        0     1230 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      586 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_cancel_swap.py.j2
--rw-r--r--   0        0        0     1018 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_collect.py.j2
--rw-r--r--   0        0        0      949 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      866 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2
--rw-r--r--   0        0        0     1382 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      486 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_raw/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      350 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/handlers/on_operation.py.j2
--rw-r--r--   0        0        0      235 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_raw/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      787 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      453 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      647 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2
--rw-r--r--   0        0        0      945 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0      456 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/dipdup.yml.j2
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/__init__.py.j2
--rw-r--r--   0        0        0      550 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2
--rw-r--r--   0        0        0      822 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2
--rw-r--r--   0        0        0      389 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/models.py.j2
--rw-r--r--   0        0        0     1226 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/linters_default/Makefile.j2
--rw-r--r--   0        0        0     1032 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/linters_default/pyproject.toml.j2
--rw-r--r--   0        0        0      923 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/linters_none/Makefile.j2
--rw-r--r--   0        0        0      552 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/projects/linters_none/pyproject.toml.j2
--rw-r--r--   0        0        0     4008 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/prometheus.py
--rw-r--r--   0        0        0        0 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/py.typed
--rw-r--r--   0        0        0     4845 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/scheduler.py
--rw-r--r--   0        0        0     6041 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/sentry.py
--rw-r--r--   0        0        0      199 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/sql/dipdup_head_status.sql
--rw-r--r--   0        0        0     2111 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/sql/truncate_schema.sql
--rw-r--r--   0        0        0      227 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/templates/callback.py.j2
--rw-r--r--   0        0        0      157 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/templates/models.py.j2
--rw-r--r--   0        0        0     3271 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/transactions.py
--rw-r--r--   0        0        0     4760 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/utils/__init__.py
--rw-r--r--   0        0        0     1824 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/utils/codegen.py
--rw-r--r--   0        0        0    11504 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/utils/database.py
--rw-r--r--   0        0        0     2044 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/utils/sys.py
--rw-r--r--   0        0        0     4513 2023-07-11 14:03:03.155680 dipdup-6.5.9/src/dipdup/yaml.py
--rw-r--r--   0        0        0     5904 1970-01-01 00:00:00.000000 dipdup-6.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-21 12:53:39.283624 dipdup-7.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3783 2023-07-21 12:53:39.283624 dipdup-7.0.0rc1/README.md
+-rw-r--r--   0        0        0     4491 2023-07-21 13:04:17.446156 dipdup-7.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_auction/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_auction/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1155 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      149 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      399 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/.keep
+-rw-r--r--   0        0        0      148 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/Dockerfile
+-rw-r--r--   0        0        0      348 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2686 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1247 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/compose.yaml
+-rw-r--r--   0        0        0      279 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1132 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/handlers/.keep
+-rw-r--r--   0        0        0      913 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/handlers/on_bid.py
+-rw-r--r--   0        0        0     1619 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/handlers/on_create_auction.py
+-rw-r--r--   0        0        0      712 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/handlers/on_withdraw.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/models/.keep
+-rw-r--r--   0        0        0     1445 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:55:57.658913 dipdup-7.0.0rc1/src/demo_auction/py.typed
+-rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/.keep
+-rw-r--r--   0        0        0      177 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/tzcolors_auction/tezos_parameters/bid.py
+-rw-r--r--   0        0        0      381 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/tzcolors_auction/tezos_parameters/create_auction.py
+-rw-r--r--   0        0        0      187 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/tzcolors_auction/tezos_parameters/withdraw.py
+-rw-r--r--   0        0        0      555 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_auction/types/tzcolors_auction/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_big_maps/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_big_maps/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1158 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      150 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      401 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      404 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/.keep
+-rw-r--r--   0        0        0      150 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/Dockerfile
+-rw-r--r--   0        0        0      350 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2688 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1248 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/compose.yaml
+-rw-r--r--   0        0        0      280 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/deploy/swarm.env.default
+-rw-r--r--   0        0        0      781 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/handlers/.keep
+-rw-r--r--   0        0        0      846 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/handlers/on_update_expiry_map.py
+-rw-r--r--   0        0        0     1688 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/handlers/on_update_records.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/models/.keep
+-rw-r--r--   0        0        0      667 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:56:31.459605 dipdup-7.0.0rc1/src/demo_big_maps/py.typed
+-rw-r--r--   0        0        0     1093 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/.keep
+-rw-r--r--   0        0        0      199 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_key.py
+-rw-r--r--   0        0        0      203 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/name_registry/tezos_big_maps/store_expiry_map_value.py
+-rw-r--r--   0        0        0      194 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_key.py
+-rw-r--r--   0        0        0      489 2023-07-21 12:53:39.299624 dipdup-7.0.0rc1/src/demo_big_maps/types/name_registry/tezos_big_maps/store_records_value.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_blank/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_blank/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1159 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      147 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      395 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      402 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/.keep
+-rw-r--r--   0        0        0      144 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/Dockerfile
+-rw-r--r--   0        0        0      344 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2682 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1245 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/compose.yaml
+-rw-r--r--   0        0        0      248 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/deploy/swarm.env.default
+-rw-r--r--   0        0        0       37 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/handlers/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/models/.keep
+-rw-r--r--   0        0        0     1242 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/models/__init__.py
+-rw-r--r--   0        0        0     1091 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_blank/types/.keep
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_dao/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_dao/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1148 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      391 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      389 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/.keep
+-rw-r--r--   0        0        0      140 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/Dockerfile
+-rw-r--r--   0        0        0      340 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2678 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1243 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/compose.yaml
+-rw-r--r--   0        0        0      275 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-21 12:53:39.303624 dipdup-7.0.0rc1/src/demo_dao/deploy/swarm.env.default
+-rw-r--r--   0        0        0      694 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/handlers/.keep
+-rw-r--r--   0        0        0      408 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/handlers/on_origination.py
+-rw-r--r--   0        0        0      506 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/handlers/on_propose.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/models/.keep
+-rw-r--r--   0        0        0      782 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:56:12.871220 dipdup-7.0.0rc1/src/demo_dao/py.typed
+-rw-r--r--   0        0        0     1078 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/types/.keep
+-rw-r--r--   0        0        0      360 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/types/registry/tezos_parameters/propose.py
+-rw-r--r--   0        0        0     2523 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dao/types/registry/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_dex/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_dex/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1163 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      391 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      404 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/.keep
+-rw-r--r--   0        0        0      140 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/Dockerfile
+-rw-r--r--   0        0        0      340 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2678 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1243 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/compose.yaml
+-rw-r--r--   0        0        0      246 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/deploy/swarm.env.default
+-rw-r--r--   0        0        0     4896 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/.keep
+-rw-r--r--   0        0        0     1829 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_divest_liquidity.py
+-rw-r--r--   0        0        0     1737 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_invest_liquidity.py
+-rw-r--r--   0        0        0      579 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_origination.py
+-rw-r--r--   0        0        0     1610 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_tez_to_token.py
+-rw-r--r--   0        0        0     1676 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_token_to_tez.py
+-rw-r--r--   0        0        0     1022 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_transfer.py
+-rw-r--r--   0        0        0      962 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_withdraw_profit.py
+-rw-r--r--   0        0        0     1855 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_divest_liquidity.py
+-rw-r--r--   0        0        0     1763 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_invest_liquidity.py
+-rw-r--r--   0        0        0      573 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_origination.py
+-rw-r--r--   0        0        0     1604 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_tez_to_token.py
+-rw-r--r--   0        0        0     1642 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_token_to_tez.py
+-rw-r--r--   0        0        0     1143 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_transfer.py
+-rw-r--r--   0        0        0      958 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_withdraw_profit.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/models/.keep
+-rw-r--r--   0        0        0      916 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:55:45.466652 dipdup-7.0.0rc1/src/demo_dex/py.typed
+-rw-r--r--   0        0        0     1093 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/.keep
+-rw-r--r--   0        0        0      340 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/fa12_token/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      739 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/fa12_token/tezos_storage.py
+-rw-r--r--   0        0        0      504 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/fa2_token/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0     1093 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/fa2_token/tezos_storage.py
+-rw-r--r--   0        0        0      311 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/divest_liquidity.py
+-rw-r--r--   0        0        0      201 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/invest_liquidity.py
+-rw-r--r--   0        0        0      297 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/tez_to_token_payment.py
+-rw-r--r--   0        0        0      313 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/token_to_tez_payment.py
+-rw-r--r--   0        0        0      340 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      199 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_parameters/withdraw_profit.py
+-rw-r--r--   0        0        0     1455 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa12/tezos_storage.py
+-rw-r--r--   0        0        0      311 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/divest_liquidity.py
+-rw-r--r--   0        0        0      201 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/invest_liquidity.py
+-rw-r--r--   0        0        0      297 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/tez_to_token_payment.py
+-rw-r--r--   0        0        0      313 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/token_to_tez_payment.py
+-rw-r--r--   0        0        0      504 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      199 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_parameters/withdraw_profit.py
+-rw-r--r--   0        0        0     1491 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_dex/types/quipu_fa2/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_domains/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_domains/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1157 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      149 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      399 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      402 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/.keep
+-rw-r--r--   0        0        0      148 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/Dockerfile
+-rw-r--r--   0        0        0      348 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2686 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1247 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/compose.yaml
+-rw-r--r--   0        0        0      279 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/deploy/swarm.env.default
+-rw-r--r--   0        0        0      900 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/handlers/.keep
+-rw-r--r--   0        0        0      553 2023-07-21 12:53:39.307624 dipdup-7.0.0rc1/src/demo_domains/handlers/on_admin_update.py
+-rw-r--r--   0        0        0      525 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/handlers/on_execute.py
+-rw-r--r--   0        0        0     1437 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/handlers/on_storage_diff.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/models/.keep
+-rw-r--r--   0        0        0      630 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:55:31.318375 dipdup-7.0.0rc1/src/demo_domains/py.typed
+-rw-r--r--   0        0        0     1091 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/types/.keep
+-rw-r--r--   0        0        0      194 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/types/name_registry/tezos_parameters/admin_update.py
+-rw-r--r--   0        0        0      305 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/types/name_registry/tezos_parameters/execute.py
+-rw-r--r--   0        0        0     1134 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_domains/types/name_registry/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_events/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_events/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1156 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      148 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      397 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/.keep
+-rw-r--r--   0        0        0      146 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/Dockerfile
+-rw-r--r--   0        0        0      346 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2684 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1246 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/compose.yaml
+-rw-r--r--   0        0        0      249 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/deploy/swarm.env.default
+-rw-r--r--   0        0        0      590 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/handlers/.keep
+-rw-r--r--   0        0        0      311 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/handlers/on_move_event.py
+-rw-r--r--   0        0        0      237 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/handlers/on_other_event.py
+-rw-r--r--   0        0        0      311 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/handlers/on_roll_event.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/models/.keep
+-rw-r--r--   0        0        0     1242 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/models/__init__.py
+-rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/types/.keep
+-rw-r--r--   0        0        0      317 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/types/events_contract/tezos_events/move.py
+-rw-r--r--   0        0        0      266 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_events/types/events_contract/tezos_events/roll.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_evm_events/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_evm_events/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1173 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/abi/.keep
+-rw-r--r--   0        0        0    11460 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/abi/eth_usdt/abi.json
+-rw-r--r--   0        0        0     2420 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/abi/eth_usdt/events.json
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      152 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      405 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      421 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/configs/replay.yaml
+-rw-r--r--   0        0        0      409 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/.keep
+-rw-r--r--   0        0        0      154 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/Dockerfile
+-rw-r--r--   0        0        0      354 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2692 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1250 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/compose.yaml
+-rw-r--r--   0        0        0      335 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      371 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/deploy/swarm.env.default
+-rw-r--r--   0        0        0      752 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/handlers/.keep
+-rw-r--r--   0        0        0      992 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/models/.keep
+-rw-r--r--   0        0        0      368 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/models/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/types/.keep
+-rw-r--r--   0        0        0      331 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_evm_events/types/eth_usdt/evm_events/transfer.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_factories/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_factories/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1172 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      151 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      403 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      419 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/.keep
+-rw-r--r--   0        0        0      152 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/Dockerfile
+-rw-r--r--   0        0        0      352 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2690 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1249 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/compose.yaml
+-rw-r--r--   0        0        0      281 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/deploy/swarm.env.default
+-rw-r--r--   0        0        0      704 2023-07-21 12:53:39.311625 dipdup-7.0.0rc1/src/demo_factories/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/handlers/.keep
+-rw-r--r--   0        0        0      420 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/handlers/on_origination.py
+-rw-r--r--   0        0        0      524 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/handlers/on_propose.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/models/.keep
+-rw-r--r--   0        0        0      782 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:56:27.503526 dipdup-7.0.0rc1/src/demo_factories/py.typed
+-rw-r--r--   0        0        0     1108 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/types/.keep
+-rw-r--r--   0        0        0      360 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/types/registry/tezos_parameters/propose.py
+-rw-r--r--   0        0        0     2523 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_factories/types/registry/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_head/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_head/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1158 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      146 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      393 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/.keep
+-rw-r--r--   0        0        0      142 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/Dockerfile
+-rw-r--r--   0        0        0      342 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2680 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1244 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/compose.yaml
+-rw-r--r--   0        0        0      276 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/deploy/swarm.env.default
+-rw-r--r--   0        0        0      292 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/handlers/.keep
+-rw-r--r--   0        0        0      237 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/handlers/on_mainnet_head.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/models/.keep
+-rw-r--r--   0        0        0     1242 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/models/__init__.py
+-rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_head/types/.keep
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_nft_marketplace/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_nft_marketplace/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1166 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      157 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      415 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      419 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/configs/replay.yaml
+-rw-r--r--   0        0        0      452 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/.keep
+-rw-r--r--   0        0        0      164 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/Dockerfile
+-rw-r--r--   0        0        0      364 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2702 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1255 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/compose.yaml
+-rw-r--r--   0        0        0      383 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      414 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/swarm.env.default
+-rw-r--r--   0        0        0     1262 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/.keep
+-rw-r--r--   0        0        0      605 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_cancel_swap.py
+-rw-r--r--   0        0        0     1037 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_collect.py
+-rw-r--r--   0        0        0      977 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_mint.py
+-rw-r--r--   0        0        0      885 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/handlers/on_swap.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/models/.keep
+-rw-r--r--   0        0        0     1306 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:55:43.058599 dipdup-7.0.0rc1/src/demo_nft_marketplace/py.typed
+-rw-r--r--   0        0        0     1108 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/.keep
+-rw-r--r--   0        0        0      192 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/cancel_swap.py
+-rw-r--r--   0        0        0      281 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/collect.py
+-rw-r--r--   0        0        0      317 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/mint_objkt.py
+-rw-r--r--   0        0        0      299 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_parameters/swap.py
+-rw-r--r--   0        0        0      777 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_minter/tezos_storage.py
+-rw-r--r--   0        0        0      343 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_objkts/tezos_parameters/mint.py
+-rw-r--r--   0        0        0     1094 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_nft_marketplace/types/hen_objkts/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_raw/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_raw/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1185 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      391 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      426 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/configs/replay.yaml
+-rw-r--r--   0        0        0      356 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/.keep
+-rw-r--r--   0        0        0      140 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/Dockerfile
+-rw-r--r--   0        0        0      340 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2678 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1243 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/compose.yaml
+-rw-r--r--   0        0        0      275 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      318 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/deploy/swarm.env.default
+-rw-r--r--   0        0        0      462 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/handlers/.keep
+-rw-r--r--   0        0        0      350 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/handlers/on_operation.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.315625 dipdup-7.0.0rc1/src/demo_raw/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/models/.keep
+-rw-r--r--   0        0        0      245 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:56:38.667706 dipdup-7.0.0rc1/src/demo_raw/py.typed
+-rw-r--r--   0        0        0     1115 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_raw/types/.keep
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_token/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_token/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1157 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      147 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      395 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      400 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/.keep
+-rw-r--r--   0        0        0      144 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/Dockerfile
+-rw-r--r--   0        0        0      344 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2682 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1245 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/compose.yaml
+-rw-r--r--   0        0        0      248 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/deploy/swarm.env.default
+-rw-r--r--   0        0        0      783 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/handlers/.keep
+-rw-r--r--   0        0        0      436 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/handlers/on_balance_update.py
+-rw-r--r--   0        0        0      630 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/handlers/on_mint.py
+-rw-r--r--   0        0        0      928 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/handlers/on_transfer.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/models/.keep
+-rw-r--r--   0        0        0      370 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:55:31.318375 dipdup-7.0.0rc1/src/demo_token/py.typed
+-rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/types/.keep
+-rw-r--r--   0        0        0      263 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/types/tzbtc/tezos_parameters/mint.py
+-rw-r--r--   0        0        0      340 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/types/tzbtc/tezos_parameters/transfer.py
+-rw-r--r--   0        0        0      398 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token/types/tzbtc/tezos_storage.py
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_token_transfers/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_token_transfers/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1166 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/abi/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      157 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      415 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      419 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/configs/replay.yaml
+-rw-r--r--   0        0        0      327 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/.keep
+-rw-r--r--   0        0        0      164 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/Dockerfile
+-rw-r--r--   0        0        0      364 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2702 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1255 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/compose.yaml
+-rw-r--r--   0        0        0      258 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      289 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/deploy/swarm.env.default
+-rw-r--r--   0        0        0      472 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/handlers/.keep
+-rw-r--r--   0        0        0      545 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/handlers/on_balance_update.py
+-rw-r--r--   0        0        0      836 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/handlers/on_token_transfer.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/models/.keep
+-rw-r--r--   0        0        0      370 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:56:09.391146 dipdup-7.0.0rc1/src/demo_token_transfers/py.typed
+-rw-r--r--   0        0        0     1108 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_token_transfers/types/.keep
+-rw-r--r--   0        0        0      255 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/.dockerignore
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/.gitignore
+-rw-r--r--   0        0        0        1 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_uniswap/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-21 12:55:01.173701 dipdup-7.0.0rc1/src/demo_uniswap/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     1178 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/.keep
+-rw-r--r--   0        0        0     4418 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/factory/abi.json
+-rw-r--r--   0        0        0      919 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/factory/events.json
+-rw-r--r--   0        0        0    19609 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/pool/abi.json
+-rw-r--r--   0        0        0     3559 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/pool/events.json
+-rw-r--r--   0        0        0    24313 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/position_manager/abi.json
+-rw-r--r--   0        0        0     1984 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/abi/position_manager/events.json
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/.keep
+-rw-r--r--   0        0        0      379 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/dipdup.compose.yaml
+-rw-r--r--   0        0        0      149 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/dipdup.sqlite.yaml
+-rw-r--r--   0        0        0      399 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/dipdup.swarm.yaml
+-rw-r--r--   0        0        0      423 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/configs/replay.yaml
+-rw-r--r--   0        0        0      424 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/.env.default
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/.keep
+-rw-r--r--   0        0        0      148 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/Dockerfile
+-rw-r--r--   0        0        0      348 2023-07-21 12:53:39.319625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/compose.sqlite.yaml
+-rw-r--r--   0        0        0     2686 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/compose.swarm.yaml
+-rw-r--r--   0        0        0     1247 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/compose.yaml
+-rw-r--r--   0        0        0      347 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/sqlite.env.default
+-rw-r--r--   0        0        0      386 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/deploy/swarm.env.default
+-rw-r--r--   0        0        0     2236 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/dipdup.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/graphql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/.keep
+-rw-r--r--   0        0        0     3060 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/factory/pool_created.py
+-rw-r--r--   0        0        0      531 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/burn.py
+-rw-r--r--   0        0        0      291 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/flash.py
+-rw-r--r--   0        0        0      871 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/initialize.py
+-rw-r--r--   0        0        0     1330 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/mint.py
+-rw-r--r--   0        0        0     6558 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/pool/swap.py
+-rw-r--r--   0        0        0     1227 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/collect.py
+-rw-r--r--   0        0        0     1361 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/decrease_liquidity.py
+-rw-r--r--   0        0        0     1449 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/increase_liquidity.py
+-rw-r--r--   0        0        0     1172 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/handlers/position_manager/transfer.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hasura/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/.keep
+-rw-r--r--   0        0        0      378 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/on_index_rollback.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/on_reindex.py
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/on_restart.py
+-rw-r--r--   0        0        0      145 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/hooks/on_synchronized.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/.keep
+-rw-r--r--   0        0        0    19932 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/abi.py
+-rw-r--r--   0        0        0     4162 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/pool.py
+-rw-r--r--   0        0        0     2824 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/position.py
+-rw-r--r--   0        0        0     1477 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/repo.py
+-rw-r--r--   0        0        0      561 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/tick.py
+-rw-r--r--   0        0        0     7160 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/models/token.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/py.typed
+-rw-r--r--   0        0        0     1112 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/on_index_rollback/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/on_reindex/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/on_restart/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/sql/on_synchronized/.keep
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/.keep
+-rw-r--r--   0        0        0      321 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/factory/evm_events/pool_created.py
+-rw-r--r--   0        0        0      330 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/burn.py
+-rw-r--r--   0        0        0      339 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/collect.py
+-rw-r--r--   0        0        0      328 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/flash.py
+-rw-r--r--   0        0        0      275 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/initialize.py
+-rw-r--r--   0        0        0      346 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/mint.py
+-rw-r--r--   0        0        0      351 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/pool/evm_events/swap.py
+-rw-r--r--   0        0        0      303 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/position_manager/evm_events/collect.py
+-rw-r--r--   0        0        0      323 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/position_manager/evm_events/decrease_liquidity.py
+-rw-r--r--   0        0        0      323 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/position_manager/evm_events/increase_liquidity.py
+-rw-r--r--   0        0        0      333 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/demo_uniswap/types/position_manager/evm_events/transfer.py
+-rw-r--r--   0        0        0      213 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/__init__.py
+-rw-r--r--   0        0        0      105 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/__main__.py
+-rw-r--r--   0        0        0      512 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/api.py
+-rw-r--r--   0        0        0    21805 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/cli.py
+-rw-r--r--   0        0        0     7560 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/codegen/__init__.py
+-rw-r--r--   0        0        0     7038 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/codegen/evm_subsquid.py
+-rw-r--r--   0        0        0    18129 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/codegen/tezos_tzkt.py
+-rw-r--r--   0        0        0    41898 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/__init__.py
+-rw-r--r--   0        0        0      554 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/abi_etherscan.py
+-rw-r--r--   0        0        0      690 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/coinbase.py
+-rw-r--r--   0        0        0     1469 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/evm.py
+-rw-r--r--   0        0        0     1273 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/evm_node.py
+-rw-r--r--   0        0        0     1375 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/evm_subsquid.py
+-rw-r--r--   0        0        0     2578 2023-07-21 12:53:39.323625 dipdup-7.0.0rc1/src/dipdup/config/evm_subsquid_events.py
+-rw-r--r--   0        0        0     1495 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/evm_subsquid_operations.py
+-rw-r--r--   0        0        0      446 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/http.py
+-rw-r--r--   0        0        0      519 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/ipfs.py
+-rw-r--r--   0        0        0     1532 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos.py
+-rw-r--r--   0        0        0     2157 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt.py
+-rw-r--r--   0        0        0     3758 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_big_maps.py
+-rw-r--r--   0        0        0     3074 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_events.py
+-rw-r--r--   0        0        0     1424 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_head.py
+-rw-r--r--   0        0        0    12744 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_operations.py
+-rw-r--r--   0        0        0     3110 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_token_transfers.py
+-rw-r--r--   0        0        0      745 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/config/tzip_metadata.py
+-rw-r--r--   0        0        0    28058 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/context.py
+-rw-r--r--   0        0        0    14006 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/database.py
+-rw-r--r--   0        0        0     4474 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/abi_etherscan.py
+-rw-r--r--   0        0        0     2274 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/coinbase.py
+-rw-r--r--   0        0        0    12321 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/evm_node.py
+-rw-r--r--   0        0        0     4013 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/evm_subsquid.py
+-rw-r--r--   0        0        0      399 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/http.py
+-rw-r--r--   0        0        0      524 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/ipfs.py
+-rw-r--r--   0        0        0    43369 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/tezos_tzkt.py
+-rw-r--r--   0        0        0     1545 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/datasources/tzip_metadata.py
+-rw-r--r--   0        0        0    30432 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/dipdup.py
+-rw-r--r--   0        0        0     1803 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/env.py
+-rw-r--r--   0        0        0     8274 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/exceptions.py
+-rw-r--r--   0        0        0     3981 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/fetcher.py
+-rw-r--r--   0        0        0     6724 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/fields.py
+-rw-r--r--   0        0        0    25644 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/hasura.py
+-rw-r--r--   0        0        0    11008 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/http.py
+-rw-r--r--   0        0        0     7426 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/index.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/fetcher.py
+-rw-r--r--   0        0        0    10389 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/index.py
+-rw-r--r--   0        0        0     3439 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/matcher.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_events/parser.py
+-rw-r--r--   0        0        0      406 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/evm_subsquid_operations/index.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/__init__.py
+-rw-r--r--   0        0        0     3181 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/fetcher.py
+-rw-r--r--   0        0        0     7320 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/index.py
+-rw-r--r--   0        0        0     2684 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/__init__.py
+-rw-r--r--   0        0        0     1480 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/fetcher.py
+-rw-r--r--   0        0        0     5539 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/index.py
+-rw-r--r--   0        0        0     3888 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/matcher.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_head/__init__.py
+-rw-r--r--   0        0        0     2349 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_head/index.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/__init__.py
+-rw-r--r--   0        0        0    20276 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py
+-rw-r--r--   0        0        0    13485 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/index.py
+-rw-r--r--   0        0        0     9135 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/matcher.py
+-rw-r--r--   0        0        0     7612 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/parser.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/__init__.py
+-rw-r--r--   0        0        0     1432 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py
+-rw-r--r--   0        0        0     5520 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py
+-rw-r--r--   0        0        0     1808 2023-07-21 12:53:39.327625 dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py
+-rwxr-xr-x   0        0        0     9379 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/install.py
+-rw-r--r--   0        0        0    20461 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/__init__.py
+-rw-r--r--   0        0        0     1309 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/coinbase.py
+-rw-r--r--   0        0        0     3596 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/evm_node.py
+-rw-r--r--   0        0        0     5045 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/evm_subsquid.py
+-rw-r--r--   0        0        0    19800 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/tezos_tzkt.py
+-rw-r--r--   0        0        0      165 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/models/tzip_metadata.py
+-rw-r--r--   0        0        0     6687 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/package.py
+-rw-r--r--   0        0        0     7091 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/performance.py
+-rw-r--r--   0        0        0     7834 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/project.py
+-rw-r--r--   0        0        0      256 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/.dockerignore.j2
+-rw-r--r--   0        0        0      341 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/.gitignore.j2
+-rw-r--r--   0        0        0     1163 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/README.md.j2
+-rw-r--r--   0        0        0      380 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/configs/dipdup.compose.yaml.j2
+-rw-r--r--   0        0        0      159 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/configs/dipdup.sqlite.yaml.j2
+-rw-r--r--   0        0        0      418 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/configs/dipdup.swarm.yaml.j2
+-rw-r--r--   0        0        0      221 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/Dockerfile.j2
+-rw-r--r--   0        0        0      367 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/compose.sqlite.yaml.j2
+-rw-r--r--   0        0        0     2748 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/compose.swarm.yaml.j2
+-rw-r--r--   0        0        0     1273 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/deploy/compose.yaml.j2
+-rw-r--r--   0        0        0     1282 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/base/pyproject.toml.j2
+-rw-r--r--   0        0        0     1151 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/dipdup.yaml.j2
+-rw-r--r--   0        0        0      935 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2
+-rw-r--r--   0        0        0     1641 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2
+-rw-r--r--   0        0        0      734 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_withdraw.py.j2
+-rw-r--r--   0        0        0     1448 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/models/__init__.py.j2
+-rw-r--r--   0        0        0      114 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/replay.yaml
+-rw-r--r--   0        0        0      798 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/dipdup.yaml.j2
+-rw-r--r--   0        0        0      865 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2
+-rw-r--r--   0        0        0     1707 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/handlers/on_update_records.py.j2
+-rw-r--r--   0        0        0      669 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/models/__init__.py.j2
+-rw-r--r--   0        0        0      118 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/replay.yaml
+-rw-r--r--   0        0        0       49 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_blank/dipdup.yaml.j2
+-rw-r--r--   0        0        0      116 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_blank/replay.yaml
+-rw-r--r--   0        0        0      721 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/dipdup.yaml.j2
+-rw-r--r--   0        0        0      431 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      540 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      784 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/models/__init__.py.j2
+-rw-r--r--   0        0        0      103 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/replay.yaml
+-rw-r--r--   0        0        0     4923 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1885 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1793 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      602 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2
+-rw-r--r--   0        0        0     1666 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1732 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1056 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2
+-rw-r--r--   0        0        0      996 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_withdraw_profit.py.j2
+-rw-r--r--   0        0        0     1911 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2
+-rw-r--r--   0        0        0     1819 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2
+-rw-r--r--   0        0        0      596 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_origination.py.j2
+-rw-r--r--   0        0        0     1660 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2
+-rw-r--r--   0        0        0     1698 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_token_to_tez.py.j2
+-rw-r--r--   0        0        0     1177 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2
+-rw-r--r--   0        0        0      992 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2
+-rw-r--r--   0        0        0      918 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/models/__init__.py.j2
+-rw-r--r--   0        0        0      118 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/replay.yaml
+-rw-r--r--   0        0        0      919 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/dipdup.yaml.j2
+-rw-r--r--   0        0        0      581 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2
+-rw-r--r--   0        0        0      553 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_execute.py.j2
+-rw-r--r--   0        0        0     1456 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2
+-rw-r--r--   0        0        0      632 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/models/__init__.py.j2
+-rw-r--r--   0        0        0      116 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/replay.yaml
+-rw-r--r--   0        0        0      611 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_events/dipdup.yaml.j2
+-rw-r--r--   0        0        0      114 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_events/replay.yaml
+-rw-r--r--   0        0        0      765 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_evm_events/dipdup.yaml.j2
+-rw-r--r--   0        0        0     1005 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_evm_events/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      370 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_evm_events/models/__init__.py.j2
+-rw-r--r--   0        0        0      135 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_evm_events/replay.yaml
+-rw-r--r--   0        0        0      719 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/dipdup.yaml.j2
+-rw-r--r--   0        0        0      431 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/handlers/on_origination.py.j2
+-rw-r--r--   0        0        0      540 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2
+-rw-r--r--   0        0        0      784 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/models/__init__.py.j2
+-rw-r--r--   0        0        0      133 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/replay.yaml
+-rw-r--r--   0        0        0      317 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_head/dipdup.yaml.j2
+-rw-r--r--   0        0        0      114 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_head/replay.yaml
+-rw-r--r--   0        0        0     1265 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2
+-rw-r--r--   0        0        0      603 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_cancel_swap.py.j2
+-rw-r--r--   0        0        0     1035 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_collect.py.j2
+-rw-r--r--   0        0        0      973 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      883 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/handlers/on_swap.py.j2
+-rw-r--r--   0        0        0     1309 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2
+-rw-r--r--   0        0        0      133 2023-07-21 12:53:39.331625 dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/replay.yaml
+-rw-r--r--   0        0        0      489 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_raw/dipdup.yaml.j2
+-rw-r--r--   0        0        0      364 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_raw/handlers/on_operation.py.j2
+-rw-r--r--   0        0        0      247 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_raw/models/__init__.py.j2
+-rw-r--r--   0        0        0      140 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_raw/replay.yaml
+-rw-r--r--   0        0        0      806 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/dipdup.yaml.j2
+-rw-r--r--   0        0        0      448 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      664 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/handlers/on_mint.py.j2
+-rw-r--r--   0        0        0      962 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2
+-rw-r--r--   0        0        0      372 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/models/__init__.py.j2
+-rw-r--r--   0        0        0      114 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token/replay.yaml
+-rw-r--r--   0        0        0      475 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/dipdup.yaml.j2
+-rw-r--r--   0        0        0      545 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2
+-rw-r--r--   0        0        0      836 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/handlers/on_token_transfer.py.j2
+-rw-r--r--   0        0        0      372 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/models/__init__.py.j2
+-rw-r--r--   0        0        0      133 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/replay.yaml
+-rw-r--r--   0        0        0     2255 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/dipdup.yaml.j2
+-rw-r--r--   0        0        0     3097 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/factory/pool_created.py.j2
+-rw-r--r--   0        0        0      568 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/burn.py.j2
+-rw-r--r--   0        0        0      310 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/flash.py.j2
+-rw-r--r--   0        0        0      899 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/initialize.py.j2
+-rw-r--r--   0        0        0     1376 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/mint.py.j2
+-rw-r--r--   0        0        0     6631 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/pool/swap.py.j2
+-rw-r--r--   0        0        0     1264 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/collect.py.j2
+-rw-r--r--   0        0        0     1398 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/decrease_liquidity.py.j2
+-rw-r--r--   0        0        0     1486 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/increase_liquidity.py.j2
+-rw-r--r--   0        0        0     1200 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/handlers/position_manager/transfer.py.j2
+-rw-r--r--   0        0        0    19933 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/__init__.py.j2
+-rw-r--r--   0        0        0      374 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/abi.py.j2
+-rw-r--r--   0        0        0     4226 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/pool.py.j2
+-rw-r--r--   0        0        0     2844 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/position.py.j2
+-rw-r--r--   0        0        0     1478 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/repo.py.j2
+-rw-r--r--   0        0        0      571 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/tick.py.j2
+-rw-r--r--   0        0        0     7188 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/models/token.py.j2
+-rw-r--r--   0        0        0      137 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/projects/demo_uniswap/replay.yaml
+-rw-r--r--   0        0        0     4008 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/prometheus.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/py.typed
+-rw-r--r--   0        0        0     1631 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/pysignalr.py
+-rw-r--r--   0        0        0     1722 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/report.py
+-rw-r--r--   0        0        0     4867 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/scheduler.py
+-rw-r--r--   0        0        0     4613 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/sentry.py
+-rw-r--r--   0        0        0      199 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/sql/dipdup_head_status.sql
+-rw-r--r--   0        0        0     2111 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/sql/truncate_schema.sql
+-rw-r--r--   0        0        0     2163 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/subscriptions.py
+-rw-r--r--   0        0        0     1791 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/sys.py
+-rw-r--r--   0        0        0      227 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/templates/callback.py.j2
+-rw-r--r--   0        0        0     1242 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/templates/models.py
+-rw-r--r--   0        0        0      186 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/templates/replay.yaml.j2
+-rw-r--r--   0        0        0     3290 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/transactions.py
+-rw-r--r--   0        0        0     6763 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/utils.py
+-rw-r--r--   0        0        0     5411 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/src/dipdup/yaml.py
+-rw-r--r--   0        0        0      952 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      496 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/asdf.yml
+-rw-r--r--   0        0        0     1267 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_auction.yml
+-rw-r--r--   0        0        0      825 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_big_maps.yml
+-rw-r--r--   0        0        0      790 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_dao.yml
+-rw-r--r--   0        0        0     5057 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_dex.yml
+-rw-r--r--   0        0        0      943 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_domains.yml
+-rw-r--r--   0        0        0      923 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_factories.yml
+-rw-r--r--   0        0        0     1361 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_nft_marketplace.yml
+-rw-r--r--   0        0        0      635 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_raw.yml
+-rw-r--r--   0        0        0      756 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_token.yml
+-rw-r--r--   0        0        0      572 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_token_transfers.yml
+-rw-r--r--   0        0        0      572 2023-07-21 12:53:39.335625 dipdup-7.0.0rc1/tests/configs/demo_token_transfers_2.yml
+-rw-r--r--   0        0        0      572 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/demo_token_transfers_3.yml
+-rw-r--r--   0        0        0      859 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/demo_token_transfers_4.yml
+-rw-r--r--   0        0        0     1297 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/dipdup.yml
+-rw-r--r--   0        0        0      521 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/hen_subjkt.yml
+-rw-r--r--   0        0        0      496 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/hjkl.yml
+-rw-r--r--   0        0        0      546 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/kolibri_ovens.yml
+-rw-r--r--   0        0        0      684 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/operation_filters.yml
+-rw-r--r--   0        0        0      496 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/qwer.yml
+-rw-r--r--   0        0        0      496 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/rewq.yml
+-rw-r--r--   0        0        0      534 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/yupana.yml
+-rw-r--r--   0        0        0      496 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/configs/zxcv.yml
+-rw-r--r--   0        0        0     1285 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/profile_abi_decoding.py
+-rw-r--r--   0        0        0        2 2023-07-21 12:55:34.610438 dipdup-7.0.0rc1/tests/replays/024e925225593fe9cd80f5a114201f74d9f3631cea6f03add3e88fc91fafd2d7
+-rw-r--r--   0        0        0    11605 2023-07-21 12:53:39.339625 dipdup-7.0.0rc1/tests/replays/0535b2dcc93076e6026fa48cc501adaed47b7b060e6483d8312f40c184d7287d
+-rw-r--r--   0        0        0  2577538 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/064e788d2566d748f516b17c6a43ab34259443cc9537f0dec7c1a5a2bce704b2
+-rw-r--r--   0        0        0      305 2023-07-21 12:56:47.355883 dipdup-7.0.0rc1/tests/replays/0b7d26b8f2813d12a80b9e96cc6f0bb186bf9ac5c5b0c0b3bb2cc8d750126843
+-rw-r--r--   0        0        0      784 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/0eaaba2830dbdd3a80286fbc367084bce6e55c678e21da178a7eb16beef6c997
+-rw-r--r--   0        0        0       20 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/1165d42ccbdd0f6c25cece69d2c579da07655a30d04f18840350a153a98827a0
+-rw-r--r--   0        0        0     7446 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/1228b36594bb93d619170ad49373f1ceec52d10faafdd727b37f3cdeffd663db
+-rw-r--r--   0        0        0     4947 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/13afdf001ce3d6a0219c0f7f6d372d9b645770e5f4304576f7f7a37b45af96fc
+-rw-r--r--   0        0        0      310 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/1430e37dce64ecb83499da8feaa3c0906e4fdf5d0a3c3570174645e97ba54bc4
+-rw-r--r--   0        0        0    13275 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/14408f393a3e399b241184f858e70396e3b8313e32ee1a984913d43fb74dcfec
+-rw-r--r--   0        0        0   855628 2023-07-21 12:55:48.762722 dipdup-7.0.0rc1/tests/replays/14cba0424c66b1869edc8e18ca3079856083cc3db7e68ef61fce165b6d7e1a6d
+-rw-r--r--   0        0        0      129 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/14d37c70764fe50b4ea590691d5614f613f96b8ad98c5df189564778616f5261
+-rw-r--r--   0        0        0      246 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/185f6628ac43f6ca728c5b79b7b81a3c3671efce7f14030a06a27e90cf641dea
+-rw-r--r--   0        0        0      986 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/18d85ceab66daf057861b99b7e223a25067197b3b77edbf060390df58cb65eaa
+-rw-r--r--   0        0        0     1448 2023-07-21 12:53:39.351626 dipdup-7.0.0rc1/tests/replays/19441b677ef5fd8ca39c37e6ddd2a7d9bc8cb3ab282b2a91ce4d8430f56f0fa9
+-rw-r--r--   0        0        0   612008 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/1a43bd7d1397cc3169ad267cd2ef083a5a63eaac7ed5186aadfc01bb53636214
+-rw-r--r--   0        0        0  1154515 2023-07-21 12:55:49.350735 dipdup-7.0.0rc1/tests/replays/1c07d3d72acc637fb46c59d0a6dc9749f3412a5d527ca2eb0cccc01720fda1c7
+-rw-r--r--   0        0        0    89590 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/1c34d1f810ae474395893bf67fb8cfb27b0506ab94eebec42cd4d2d21bf3dfcd
+-rw-r--r--   0        0        0        2 2023-07-21 12:55:34.610438 dipdup-7.0.0rc1/tests/replays/1c717490846300e1639e96a0c1438b6dd2abd6de013c5edec49042fa364c06e6
+-rw-r--r--   0        0        0    12263 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/252fd058cfef21f9b5b7f4367f730ec7d41647253d7cc7ccfb1e22d42d1f366a
+-rw-r--r--   0        0        0     1167 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/27373c23411bf37b605c8d0ead9a0e6c6c1f1718ce7863b095b759811e44e155
+-rw-r--r--   0        0        0     1121 2023-07-21 12:53:39.355626 dipdup-7.0.0rc1/tests/replays/2a45ec6372b45e46199a6af24272cb93586777a0522cd1203b3eeef213ce4583
+-rw-r--r--   0        0        0   209761 2023-07-21 12:55:49.434737 dipdup-7.0.0rc1/tests/replays/31cc70e13495f58ecde80847bc6c9e08536cc426c03bd2aa8c45c1b2c798e155
+-rw-r--r--   0        0        0 21118960 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/31dd376b771f347a0d6fe4dd132a1f96f809274429b78ec86dd742e5589fbc23
+-rw-r--r--   0        0        0  1807578 2023-07-21 12:55:35.338455 dipdup-7.0.0rc1/tests/replays/32e3a13cc470d8720ce28f5eaff327340fb25cbe712e5b5a348af1bc3c92235a
+-rw-r--r--   0        0        0       65 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/33349b63491dc976a7a2332d3cca3bd9b3b831c02a6f474bb925876c1838633a
+-rw-r--r--   0        0        0        2 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/34f3e33d677f85b633cb85c6dd205beb40e3d9c40cfafc7084b82c8123a54de1
+-rw-r--r--   0        0        0    45221 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/36072e13c9ce265bb81142b8816da8c31bd9180e7c663ea4169bd259af107382
+-rw-r--r--   0        0        0    81885 2023-07-21 12:53:39.411627 dipdup-7.0.0rc1/tests/replays/377ac31d6316391ed138df44bec374d65202f0577603e80465ced3c09140f78c
+-rw-r--r--   0        0        0    54602 2023-07-21 12:56:00.634976 dipdup-7.0.0rc1/tests/replays/383899084f79460e96fd311bb64e4925738c486b39d6281539456c5fcac41620
+-rw-r--r--   0        0        0      642 2023-07-21 12:56:29.599568 dipdup-7.0.0rc1/tests/replays/39b8664d1bca5d374ff905c8a3a396b53d19ee469dc37545a8ca6b080bd0e9e0
+-rw-r--r--   0        0        0     1200 2023-07-21 12:56:48.327902 dipdup-7.0.0rc1/tests/replays/3a2bd8b6b72bf18152d2550c106789fa9b8abc98ea9d759a6597b7ebfbab0fc2
+-rw-r--r--   0        0        0    81885 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/3c9ad6f98f79e72185ea58c4777115750c658c5defd616664212095bd440c10c
+-rw-r--r--   0        0        0      332 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/3fdba02cbc415eba224604f4fea130acd4565d31e4a83cdbb679ec0b76c798ab
+-rw-r--r--   0        0        0  3369404 2023-07-21 12:56:17.091309 dipdup-7.0.0rc1/tests/replays/42b7bf0da866257ef98e1f7124d2d21fe7d13228c076fffa32331da423f36933
+-rw-r--r--   0        0        0      619 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/43cb0ab415d8b8b3f7addc3e82ea27d93b2c66ff55c117e1e0c7c64a0fcfc3f2
+-rw-r--r--   0        0        0   530743 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/440173d32e95111ca7b080ccc4dc09bfab23c8361919b2c113f0ff9ab445eec2
+-rw-r--r--   0        0        0  1594116 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/489233ce9373f7de4f7a9053055c74bc0df999bfe939ed67d98b6d67e676e35a
+-rw-r--r--   0        0        0   109726 2023-07-21 12:55:46.378672 dipdup-7.0.0rc1/tests/replays/4a57776d93475adfd9c49b6c3295a7cedfc23b73733a1fb5f0c985ee039dc5dc
+-rw-r--r--   0        0        0      984 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/4aa7f9b0657be0c44baf2caed8c7cb08d02097a4095cf6417f78cba3a25e8423
+-rw-r--r--   0        0        0       67 2023-07-21 12:56:44.951834 dipdup-7.0.0rc1/tests/replays/4fbdb4667971fab446a5ac5937a7c8cc6ef5813ff00af24b6fd1b1a0427bedbb
+-rw-r--r--   0        0        0   192680 2023-07-21 12:55:46.178667 dipdup-7.0.0rc1/tests/replays/5483a0e11009e0f186bf70c214e2597d267a75a1e19152a9e7ed1ec257ce88ca
+-rw-r--r--   0        0        0       65 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/56eb33fbb563bf03ea7639659fae5102222d6e3cea882febf71f01bd383c6eed
+-rw-r--r--   0        0        0    40432 2023-07-21 12:56:00.458973 dipdup-7.0.0rc1/tests/replays/587613799ebfae42b1884016d1a44a452d68e70e3ed80641d90b8e7657ba8ee5
+-rw-r--r--   0        0        0       32 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5b004196490632859ec1b019d640f6bbb93fc86a433c8969e10f36f51ac2c78d
+-rw-r--r--   0        0        0     1907 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5b7c31b4b73bc57e8296e6051b3bc7b2302b32588d8fbcafce8a66de3be743df
+-rw-r--r--   0        0        0     7609 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5b99bc4beb6a9a33f7d2f118426458e4c788e0ab6d9e51949d3ccbf8b4003fc1
+-rw-r--r--   0        0        0      939 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5d21060ba8e78279d2d1edaa2f266ecf36105eaccef5ebed15748441651f76fd
+-rw-r--r--   0        0        0      400 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/5f63ef9dd15459ae14e715bb79da8f033a24b54504212ebc873ee8aa95679606
+-rw-r--r--   0        0        0       67 2023-07-21 12:56:45.119838 dipdup-7.0.0rc1/tests/replays/60f48c13c47a1347786a6dcf6f741874e7b30b587d148faa67d15067bb3871de
+-rw-r--r--   0        0        0       21 2023-07-21 12:53:39.415628 dipdup-7.0.0rc1/tests/replays/62e95f1d55b756895289374b351a1da94505ec2d95a1652c97765f36a2ef9341
+-rw-r--r--   0        0        0   211527 2023-07-21 12:55:50.442758 dipdup-7.0.0rc1/tests/replays/6cc8d741a41b76983cd7e0f63e8f22a4c67cd946888f45a5b7ead8c3bb5ad2f1
+-rw-r--r--   0        0        0   944885 2023-07-21 12:53:39.419628 dipdup-7.0.0rc1/tests/replays/6cff8d120db8fd3926a45714ce7f1d0560803eb5a7b4a413b64fee1b7fd7a8ff
+-rw-r--r--   0        0        0      132 2023-07-21 12:56:45.951854 dipdup-7.0.0rc1/tests/replays/6d0c5443d41a15551acb41adc10d36d4895f5786d6922a878b5c5414610e0ebc
+-rw-r--r--   0        0        0      754 2023-07-21 12:56:46.687869 dipdup-7.0.0rc1/tests/replays/6d76a3c3f427ff534c551de1793cb1d1dfbd22ccad97f5917a9f9b201a3f9804
+-rw-r--r--   0        0        0      494 2023-07-21 12:53:39.419628 dipdup-7.0.0rc1/tests/replays/7132f07560319399092782debe6eb28926e961d8af215ce11e2c0efd8dab06da
+-rw-r--r--   0        0        0      451 2023-07-21 12:56:47.519886 dipdup-7.0.0rc1/tests/replays/739d17c86095aac3da3508a16dc1c9ae9459ea86eeb09f62aaefc32de2997918
+-rw-r--r--   0        0        0        2 2023-07-21 12:56:51.639967 dipdup-7.0.0rc1/tests/replays/759b79ec12b1305d9fa8e1a5218e62bb3d3ad913580e19914d30d8aa09920ae4
+-rw-r--r--   0        0        0   209456 2023-07-21 12:53:39.419628 dipdup-7.0.0rc1/tests/replays/7669ea717d9759748aed86302326b79be5157a1a36d13b39b00f06bcbe22b309
+-rw-r--r--   0        0        0      520 2023-07-21 12:53:39.419628 dipdup-7.0.0rc1/tests/replays/76d49ae3b723376c88ca65a3080a273e098d226932a1a49c38fbc4421e7c2e64
+-rw-r--r--   0        0        0    50588 2023-07-21 12:56:19.739365 dipdup-7.0.0rc1/tests/replays/7b6cf9b8c69712bf26ed09059352ec740606969bf20eab0dedda870273f4fde9
+-rw-r--r--   0        0        0 21649088 2023-07-21 12:56:18.547340 dipdup-7.0.0rc1/tests/replays/7b9c78209f98b2c3a6678ed224fa686eee25c3c63dddd7f9af77c734b0dfabb8
+-rw-r--r--   0        0        0   108455 2023-07-21 12:56:34.275649 dipdup-7.0.0rc1/tests/replays/7d4a99edf5845445bbeb894ad34b063c985ca061ffed162093721c0032210e31
+-rw-r--r--   0        0        0      807 2023-07-21 12:56:49.403924 dipdup-7.0.0rc1/tests/replays/803e05a8d0bb9e7cfb49530271d43ea62111b6419e7cded2d221f7e0e0c92ece
+-rw-r--r--   0        0        0   517204 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/80921fd33043def891912a6ad57d76664399564fd813950eb11f4a0e69e3e28f
+-rw-r--r--   0        0        0      129 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/815c066c21f7d2697ef107cad4624a9c4079a7a1dab7974d606fc42b81fe93c8
+-rw-r--r--   0        0        0      939 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/816d08f71c84537ea8df05a40678b1addca15bf3a73c0e927c75d9f9c0f2d418
+-rw-r--r--   0        0        0      395 2023-07-21 12:56:49.115918 dipdup-7.0.0rc1/tests/replays/8335acc6585656ec3a4301cd8b089401f2dc2c7d758b381c96c730e610b67f7b
+-rw-r--r--   0        0        0   207502 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/84cf46aa9c8dbd3ca6c3d946c749713e6c70a6a20d9cc69b4156235fd099b2e3
+-rw-r--r--   0        0        0        2 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/8ad31f6cf9c873b1fd9827b621529c43966f8376a86fcac3b1d20c260b78007e
+-rw-r--r--   0        0        0       65 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/91787fdbd1634f277b20ac46cb30eba9770f83df7189df0903e22f5f4bbe1efa
+-rw-r--r--   0        0        0     1151 2023-07-21 12:56:50.067937 dipdup-7.0.0rc1/tests/replays/93516225810a23a6799f2f9a1dee055ca79a66ee2b8d0f32be820c9c385e936b
+-rw-r--r--   0        0        0      494 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/9ce1bc12a2adeddcf9d8854c4b63a8e65b58d9206fb8d2e3eedb24c44ea7f28a
+-rw-r--r--   0        0        0       22 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/9de859083ed1dd278893f60b5a60feab02a04637327a664af23f52dabb139fe6
+-rw-r--r--   0        0        0      706 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/9e6e907842da2cd494c558ea5ecc211fd12e56bfc547450978fb7dfe03853e58
+-rw-r--r--   0        0        0     6981 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/a3ce91a1b0d505cc221f0e201781466ba1e2d6dc7b624b9bc75a03ce3dbb0f92
+-rw-r--r--   0        0        0    38974 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/a795ef429bde71b3ba66b545c0048f57a78ab5d2247772761d8efe86567199b9
+-rw-r--r--   0        0        0        2 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/a840afa5674efd06639c4692a8bfe9ed6e1346bfe9c414209eec5d9126333242
+-rw-r--r--   0        0        0      675 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/aa8fe6037996b296bf9a3011e45cd9ecb92fb728592a843f91b03b2848cb1fb1
+-rw-r--r--   0        0        0     1882 2023-07-21 12:56:12.215206 dipdup-7.0.0rc1/tests/replays/acc952ba1905717315212f952ed689d7b8f683165b31c0a7a25199aed9fda27f
+-rw-r--r--   0        0        0      356 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/aeee37b6f63a3177e0e27ac472008c3cba3d30ebee691fb45de1bae91a87f2ce
+-rw-r--r--   0        0        0       67 2023-07-21 12:56:44.787831 dipdup-7.0.0rc1/tests/replays/af37212b31e932f269c42c7f34ad8f3849bd8aed244652c41b9327c508985ce5
+-rw-r--r--   0        0        0     1200 2023-07-21 12:56:42.831792 dipdup-7.0.0rc1/tests/replays/b3af887f7ad8172af75b94a09bedfb9ae1e14f8819a36d6ce9f709721068263b
+-rw-r--r--   0        0        0  1214926 2023-07-21 12:55:48.978727 dipdup-7.0.0rc1/tests/replays/b49fb33ee80345b70414ad08806a860e2139c20d98a5150c6ccd1b28a90f311e
+-rw-r--r--   0        0        0     2271 2023-07-21 12:56:41.487764 dipdup-7.0.0rc1/tests/replays/bec4433b4206f00c2310a7961cff7f539434b9161b45673793aa5a3b50234313
+-rw-r--r--   0        0        0      310 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/bed2329e63d559db2fb81c69606e715d1f90aaacab6ae45b33516e7828841a3c
+-rw-r--r--   0        0        0       65 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/bf941ceae7a6e3c40406438e067f137131e6605924a93d43bafc77682b602c55
+-rw-r--r--   0        0        0   759209 2023-07-21 12:55:49.114730 dipdup-7.0.0rc1/tests/replays/c0202a433296436c27458b3d5ec5c72d5e2d47ff77c939ce399780cc0f3e56bc
+-rw-r--r--   0        0        0    19100 2023-07-21 12:53:39.423628 dipdup-7.0.0rc1/tests/replays/c369836c15d9ed15477002b850d5cbb96b1ff5ff33e917b812ab9c0905063957
+-rw-r--r--   0        0        0   918908 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/c8e8698717ada415bc10405da983c8357165914dd0219f3d09bb9a939705242d
+-rw-r--r--   0        0        0   691878 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/cc162df04c4990c79f7507dd915601fd4d58c947a248156cbe302a64adfe898a
+-rw-r--r--   0        0        0     7446 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/cc5d3d4a58d5cb6bc7270d38c797b7740b79f913590ef0164abd50e58fba9405
+-rw-r--r--   0        0        0      301 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/cc648800928fd43f8e72db1d41115c26a22346c9c7831172fe422c1765cd67f2
+-rw-r--r--   0        0        0      960 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/d0a594d14bcb3fbf916092ec6707dfd3c9f48f53f0a1ad40a32023e7a87f8ef5
+-rw-r--r--   0        0        0     2403 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/d62748a927a09395579b5790c8f871cc8653081cf4475abc93173989f950b92b
+-rw-r--r--   0        0        0     9089 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/d94397f6ecec8ce25f87177fe410f6498d7d30a04360506c0cd300d291c167e7
+-rw-r--r--   0        0        0      132 2023-07-21 12:56:43.959814 dipdup-7.0.0rc1/tests/replays/db797e6bf4c1b9c3237af5dec694fb1b6d21418a5a2f7947eb7f54d4e9201baf
+-rw-r--r--   0        0        0   548925 2023-07-21 12:56:18.855346 dipdup-7.0.0rc1/tests/replays/dc86d5e346c85e6f7953d7e01298a9db64d778e5ba717ddd07fff8b589081e98
+-rw-r--r--   0        0        0    20467 2023-07-21 12:55:34.782442 dipdup-7.0.0rc1/tests/replays/dca9cf4f9f27623f10975d369444899458ab9ea85c22af2da6ce6ce8c09c2b58
+-rw-r--r--   0        0        0      700 2023-07-21 12:53:39.427628 dipdup-7.0.0rc1/tests/replays/df62701276d6dbf4860058cc582c0b4f7b583758f4f5be96c9ee045757c151e3
+-rw-r--r--   0        0        0   151396 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/e39ebba701031aa13dfd9eb5dba1effd2938e96682d1030dcbd70172f9f190a9
+-rw-r--r--   0        0        0     7917 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/e4a563a0b19379a44e9d2dc398131e9fd30d6039ff4ffacf1252db0bf8b433aa
+-rw-r--r--   0        0        0       67 2023-07-21 12:56:45.283841 dipdup-7.0.0rc1/tests/replays/e82ba90c8570b92c0b1fc360b853aca3f1d7de457aacb9f6f19fa3e43879a8b3
+-rw-r--r--   0        0        0      132 2023-07-21 12:56:44.123818 dipdup-7.0.0rc1/tests/replays/e9fa56a94eb559c550dfbca4b27ef350a0b4a787afbe60205482a38223dcea04
+-rw-r--r--   0        0        0   713724 2023-07-21 12:56:42.639788 dipdup-7.0.0rc1/tests/replays/eb8b6b33cb2e165d1a3a73c09938d3083671a82ad73d4c0cff1fb2a5e5715f76
+-rw-r--r--   0        0        0    11290 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/eb8e2c3ce2fe7792d2c8e81c61d37821275b64021343103b0c955042ae802189
+-rw-r--r--   0        0        0      584 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/ece1ebe13f9391555230d6b94f33d66a922e2ca71ef5fd39bbd8c2c37ddf54ec
+-rw-r--r--   0        0        0     1089 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/ed3ec9fd9226e9f765b96dc1d5d5a455a7b2505da530961826910b08db693070
+-rw-r--r--   0        0        0    17245 2023-07-21 12:56:24.819472 dipdup-7.0.0rc1/tests/replays/f3d608f99e6b92e28a064bb9c10c3c605c9c817383c1eebcc68f663d1d23d650
+-rw-r--r--   0        0        0    32513 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/f60e794a9be14263cb10e48546ba5610302cc3e7af0a114a593bb50eb85ba5e7
+-rw-r--r--   0        0        0       21 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/fd9e33296006ad295c9fdc4868763f954a9c6d7c81d543ba198c14a72eea7e6b
+-rw-r--r--   0        0        0      832 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/replays/ff51b3535acc2972090ecd5db3af8f827464c9d92f1aa661630976e5b4ed4cbe
+-rw-r--r--   0        0        0     4599 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/asdf.json
+-rw-r--r--   0        0        0     6704 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/ftzfun.json
+-rw-r--r--   0        0        0     3445 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/hen_subjkt.json
+-rw-r--r--   0        0        0     5210 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/hjkl.json
+-rw-r--r--   0        0        0     2097 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/kolibri_ovens.json
+-rw-r--r--   0        0        0    11186 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/ooQuCAKBHkmWy2VciDAV9c6CFTywuMLupLzVoKDwS1xvR4EdRng.json
+-rw-r--r--   0        0        0     1811 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/origination_amount.json
+-rw-r--r--   0        0        0     4256 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/qwer.json
+-rw-r--r--   0        0        0     5307 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/rewq.json
+-rw-r--r--   0        0        0    38178 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/yupana.json
+-rw-r--r--   0        0        0     5909 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/responses/zxcv.json
+-rw-r--r--   0        0        0     1077 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/asdf/storage.json
+-rw-r--r--   0        0        0     2116 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/hen_subjkt/storage.json
+-rw-r--r--   0        0        0     1638 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/hjkl/storage.json
+-rw-r--r--   0        0        0      800 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/kolibri_ovens/storage.json
+-rw-r--r--   0        0        0     1005 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/qwer/storage.json
+-rw-r--r--   0        0        0     2212 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/rewq/storage.json
+-rw-r--r--   0        0        0    12561 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/yupana/storage.json
+-rw-r--r--   0        0        0     2660 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/schemas/zxcv/storage.json
+-rw-r--r--   0        0        0     3767 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_config/test_callbacks.py
+-rw-r--r--   0        0        0     4643 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_config/test_config.py
+-rw-r--r--   0        0        0     4138 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_config/test_custom_config.py
+-rw-r--r--   0        0        0     2486 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_context.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/__init__.py
+-rw-r--r--   0        0        0      814 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_ipfs.py
+-rw-r--r--   0        0        0      663 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_metadata.py
+-rw-r--r--   0        0        0     8304 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_tzkt.py
+-rw-r--r--   0        0        0     1223 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_tzkt_blocks.py
+-rw-r--r--   0        0        0     1971 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_tzkt_buffer.py
+-rw-r--r--   0        0        0     1433 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_datasources/test_tzkt_quotes.py
+-rw-r--r--   0        0        0     8601 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_demos.py
+-rw-r--r--   0        0        0     2734 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_dipdup.py
+-rw-r--r--   0        0        0     5045 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_hasura.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_http.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_index/__init__.py
+-rw-r--r--   0        0        0     3714 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_index/test_operation.py
+-rw-r--r--   0        0        0     5772 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_introspection.py
+-rw-r--r--   0        0        0    14279 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_models.py
+-rw-r--r--   0        0        0    13401 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_rollback.py
+-rw-r--r--   0        0        0     2628 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/asdf/__init__.py
+-rw-r--r--   0        0        0      504 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/asdf/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/bazaar/__init__.py
+-rw-r--r--   0        0        0      564 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/bazaar/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/ftzfun/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/ftzfun/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/hen_subjkt/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/hen_subjkt/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/hjkl/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/hjkl/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/kolibri_ovens/__init__.py
+-rw-r--r--   0        0        0      232 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/kolibri_ovens/set_delegate.py
+-rw-r--r--   0        0        0      392 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/kolibri_ovens/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/listofmaps/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/listofmaps/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/qwer/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/qwer/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/rewq/__init__.py
+-rw-r--r--   0        0        0      831 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/rewq/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/tezotop/__init__.py
+-rw-r--r--   0        0        0      740 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/tezotop/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/yupana/__init__.py
+-rw-r--r--   0        0        0     2721 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/yupana/storage.py
+-rw-r--r--   0        0        0        0 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/zxcv/__init__.py
+-rw-r--r--   0        0        0     1048 2023-07-21 12:53:39.431628 dipdup-7.0.0rc1/tests/types/zxcv/storage.py
+-rw-r--r--   0        0        0     5723 1970-01-01 00:00:00.000000 dipdup-7.0.0rc1/PKG-INFO
```

### Comparing `dipdup-6.5.9/LICENSE` & `dipdup-7.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.9/README.md` & `dipdup-7.0.0rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,29 @@
 [![Twitter](https://badgen.net/badge/icon/dipdup_io?icon=twitter&label=)](https://twitter.com/dipdup_io)
 [![GitHub stars](https://img.shields.io/github/stars/dipdup-io/dipdup?color=2c2c2c)](https://github.com/dipdup-io/dipdup)
 [![PyPI monthly downloads](https://img.shields.io/pypi/dm/dipdup?color=2c2c2c)](https://pypi.org/project/dipdup/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dipdup?color=2c2c2c)](https://www.python.org)
-[![License: MIT](https://img.shields.io/github/license/dipdup-io/dipdup?color=2c2c2c)](https://github.com/dipdup-io/dipdup/blob/master/LICENSE)
+[![License: MIT](https://img.shields.io/github/license/dipdup-io/dipdup?color=2c2c2c)](https://github.com/dipdup-io/dipdup/blob/next/LICENSE)
 <br>
 [![Latest stable release](https://img.shields.io/github/v/release/dipdup-io/dipdup?label=stable%20release&color=2c2c2c)](https://github.com/dipdup-io/dipdup/releases)
 [![Latest pre-release](https://img.shields.io/github/v/release/dipdup-io/dipdup?include_prereleases&label=latest%20release&color=2c2c2c)](https://github.com/dipdup-io/dipdup/releases)
 [![GitHub issues](https://img.shields.io/github/issues/dipdup-io/dipdup?color=2c2c2c)](https://github.com/dipdup-io/dipdup/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/dipdup-io/dipdup?color=2c2c2c)](https://github.com/dipdup-io/dipdup/pulls)
 
-```text
-        ____   _         ____              
-       / __ \ (_)____   / __ \ __  __ ____ 
-      / / / // // __ \ / / / // / / // __ \
-     / /_/ // // /_/ // /_/ // /_/ // /_/ /
-    /_____//_// .___//_____/ \__,_// .___/ 
-             /_/                  /_/      
-```
+<h3 align="center"><img src="https://actual-docs.interface-1bp.pages.dev/_nuxt/logo.9b02ab5e.svg" alt="DipDup logo"></h3>
 
 DipDup is a Python framework for building smart contract indexers. It helps developers focus on business logic instead of writing a boilerplate to store and serve data. DipDup-based indexers are selective, which means only required data is requested. This approach allows to achieve faster indexing times and decreased load on underlying APIs.
 
 * **Ready to build your first indexer?** Head to [Quickstart](https://docs.dipdup.io/quickstart).
 
 * **Looking for examples?** Check out [Demo Projects](https://docs.dipdup.io/examples/demo-projects) and [Built with DipDup](https://docs.dipdup.io/examples/built-with-dipdup) pages.
 
 * **Want to participate?** Vote for [open issues](https://github.com/dipdup-io/dipdup/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc), join [discussions](https://github.com/dipdup-io/dipdup/discussions) or [become a sponsor](https://github.com/sponsors/dipdup-io).
 
-* **Have a question?** Join our [Discord](https://discord.gg/sfqjBpmU) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
+* **Have a question?** Join our [Discord](https://discord.gg/NbANhqCJHA) or tag @dipdup_io on [Twitter](https://twitter.com/dipdup_io).
 
 This project is maintained by the [Baking Bad](https://bakingbad.dev/) team.
 <br>
 Development is supported by [Tezos Foundation](https://tezos.foundation/).
 
 ## Thanks
 
@@ -56,12 +49,11 @@
 - [@Karantezsure](https://github.com/Karantezsure)
 - [@mystdeim](https://github.com/mystdeim)
 - [@nikos-kalomoiris](https://github.com/nikos-kalomoiris)
 - [@pravind](https://github.com/pravind)
 - [@sbihel](https://github.com/sbihel)
 - [@tezosmiami](https://github.com/tezosmiami)
 - [@tomsib2001](https://github.com/tomsib2001)
-- [@TristanAllaire](https://github.com/TristanAllaire)
 - [@veqtor](https://github.com/veqtor)
 - [@xflpt](https://github.com/xflpt)
 
 If we forgot to mention you, or you want to update your record, please, open an issue or pull request.
```

### Comparing `dipdup-6.5.9/src/dipdup/cli.py` & `dipdup-7.0.0rc1/src/dipdup/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,73 @@
 # NOTE: All imports except the basic ones are very lazy in this module. Let's keep it that way.
 import asyncio
 import atexit
 import logging
 import sys
 from contextlib import AsyncExitStack
 from contextlib import suppress
+from copy import copy
+from dataclasses import dataclass
+from functools import partial
 from functools import wraps
 from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import TypeVar
 from typing import cast
 
 import asyncclick as click
 
 from dipdup import __version__
-from dipdup import env
-from dipdup.utils.sys import IGNORE_CONFIG_CMDS
-from dipdup.utils.sys import set_up_logging
-from dipdup.utils.sys import set_up_process
-
-DEFAULT_CONFIG_NAME = 'dipdup.yml'
+from dipdup.install import EPILOG
+from dipdup.install import WELCOME_ASCII
+from dipdup.performance import metrics
+from dipdup.report import REPORTS_PATH
+from dipdup.report import ReportHeader
+from dipdup.report import save_report
+from dipdup.sys import set_up_process
+
+_click_wrap_text = click.formatting.wrap_text
+
+
+def _wrap_text(text: str, *a: Any, **kw: Any) -> str:
+    # NOTE: WELCOME_ASCII and EPILOG
+    if text.startswith(('    ')):
+        return text
+    if text.startswith(('\0\n')):
+        return text[2:]
+    return _click_wrap_text(text, *a, **kw)
+
+
+click.formatting.wrap_text = _wrap_text
+
+ROOT_CONFIG = 'dipdup.yaml'
+CONFIG_RE = r'dipdup.*\.ya?ml'
+
+# NOTE: Do not try to load config for these commands as they don't need it
+NO_CONFIG_CMDS = {
+    'new',
+    'install',
+    'uninstall',
+    'update',
+}
+# NOTE: Our signal handler conflicts with Click's one in prompt mode
+NO_SIGNALS_CMDS = {
+    *NO_CONFIG_CMDS,
+    None,
+    'schema',
+    'wipe',
+}
 
+if TYPE_CHECKING:
+    from dipdup.config import DipDupConfig
 
-_logger = logging.getLogger('dipdup.cli')
+_logger = logging.getLogger(__name__)
 
 
 def echo(message: str) -> None:
     with suppress(BrokenPipeError):
         click.echo(message)
 
 
@@ -41,39 +80,56 @@
             click.echo(error.help(), err=True)
         else:
             click.echo(Error.default_help())
 
     atexit.register(_print)
 
 
+def _print_report(name: str) -> None:
+    atexit.register(partial(click.echo, f'Report saved; run `dipdup report show {name}` to view it'))
+
+
 WrappedCommandT = TypeVar('WrappedCommandT', bound=Callable[..., Awaitable[None]])
 
 
+@dataclass
+class CLIContext:
+    config_paths: list[str]
+    config: 'DipDupConfig'
+
+
 def _cli_wrapper(fn: WrappedCommandT) -> WrappedCommandT:
     @wraps(fn)
     async def wrapper(ctx: click.Context, *args: Any, **kwargs: Any) -> None:
-        set_up_process(ctx.invoked_subcommand)
+        signals = ctx.invoked_subcommand not in NO_SIGNALS_CMDS
+        set_up_process(signals)
 
         try:
             await fn(ctx, *args, **kwargs)
         except (KeyboardInterrupt, asyncio.CancelledError):
             pass
         except Exception as e:
-            from dipdup.sentry import save_crashdump
-
-            crashdump_path = save_crashdump(e)
-            _logger.info(f'Unhandled exception caught, crashdump saved to `{crashdump_path}`')
+            package = ctx.obj.config.package if ctx.obj else 'unknown'
+            report_id = save_report(package, e)
+            _print_report(report_id)
             _print_help(e)
-            raise e
+
+            if metrics:
+                raise e
+            sys.exit(1)
+
+        if fn.__name__ == 'run':
+            package = ctx.obj.config.package
+            save_report(package, None)
 
     return cast(WrappedCommandT, wrapper)
 
 
 async def _check_version() -> None:
-    if 'rc' in __version__:
+    if 'rc' in __version__ or 'b' in __version__:
         _logger.warning(
             'You are running a pre-release version of DipDup. Please, report any issues to the GitHub repository.'
         )
         _logger.info('Set `skip_version_check` flag in config to hide this message.')
         return
 
     import aiohttp
@@ -86,104 +142,93 @@
         latest_version = response_json['tag_name']
 
         if __version__ != latest_version:
             _logger.warning('You are running an outdated version of DipDup. Please run `dipdup update`.')
             _logger.info('Set `skip_version_check` flag in config to hide this message.')
 
 
-@click.group(context_settings={'max_content_width': 120})
+@click.group(
+    context_settings={'max_content_width': 120},
+    help=WELCOME_ASCII,
+    epilog=EPILOG,
+)
 @click.version_option(__version__)
 @click.option(
     '--config',
     '-c',
     type=str,
     multiple=True,
-    help=f'A path to DipDup project config (default: {DEFAULT_CONFIG_NAME}).',
-    default=[DEFAULT_CONFIG_NAME],
+    help='A path to DipDup project config.',
+    default=[ROOT_CONFIG],
     metavar='PATH',
 )
 @click.option(
     '--env-file',
     '-e',
     type=str,
     multiple=True,
     help='A path to .env file containing `KEY=value` strings.',
     default=[],
     metavar='PATH',
 )
 @click.pass_context
 @_cli_wrapper
 async def cli(ctx: click.Context, config: list[str], env_file: list[str]) -> None:
-    """Manage and run DipDup indexers.
-
-    Documentation: https://docs.dipdup.io
-
-    Issues: https://github.com/dipdup-io/dipdup/issues
-    """
-    if env.DOCKER_IMAGE == 'pytezos':
-        _logger.warning('`-pytezos` image is deprecated and will be removed in the next major release')
-    elif env.DOCKER_IMAGE == 'slim':
-        _logger.warning('`-slim` image will be based on Ubuntu instead of Alpine in the next major release')
-
     # NOTE: Workaround for help pages. First argument check is for the test runner.
     args = sys.argv[1:] if sys.argv else ['--help']
-    if '--help' in args or args in (['config'], ['hasura'], ['schema']):
+    if '--help' in args or args in (['config'], ['hasura'], ['schema']) or args[0] in ('self', 'report'):
         return
 
     from dotenv import load_dotenv
 
     from dipdup.exceptions import ConfigurationError
+    from dipdup.sys import set_up_logging
 
     set_up_logging()
 
     env_file_paths = [Path(file) for file in env_file]
     config_paths = [Path(file) for file in config]
 
     # NOTE: Apply env files before loading config
     for env_path in env_file_paths:
         if not env_path.is_file():
             raise ConfigurationError(f'env file `{env_path}` does not exist')
         _logger.info('Applying env_file `%s`', env_path)
         load_dotenv(env_path, override=True)
 
     # NOTE: These commands need no other preparations
-    if ctx.invoked_subcommand in IGNORE_CONFIG_CMDS:
+    if ctx.invoked_subcommand in NO_CONFIG_CMDS:
         logging.getLogger('dipdup').setLevel(logging.INFO)
         return
 
-    from dataclasses import dataclass
-
-    from dipdup.codegen import CodeGenerator
+    from dipdup import env
     from dipdup.config import DipDupConfig
-    from dipdup.exceptions import ConfigurationError
     from dipdup.exceptions import InitializationRequiredError
+    from dipdup.package import DipDupPackage
     from dipdup.sentry import init_sentry
 
     _config = DipDupConfig.load(config_paths)
     _config.set_up_logging()
 
     init_sentry(_config)
 
     # NOTE: Imports will be loaded later if needed
-    _config.initialize(skip_imports=True)
+    _config.initialize()
 
     # NOTE: Fire and forget, do not block instant commands
     if not any((_config.advanced.skip_version_check, env.TEST, env.CI)):
         asyncio.ensure_future(_check_version())
 
-    # NOTE: Avoid import errors if project package is incomplete
     try:
-        CodeGenerator(_config, {}).create_package()
+        # NOTE: Avoid early import errors if project package is incomplete.
+        # NOTE: `ConfigurationError` will be raised with more details.
+        DipDupPackage(_config.package_path).create()
     except Exception as e:
-        raise InitializationRequiredError(f'Failed to create a project package: {e}') from e
-
-    @dataclass
-    class CLIContext:
-        config_paths: list[str]
-        config: DipDupConfig
+        if ctx.invoked_subcommand != 'init':
+            raise InitializationRequiredError(f'Failed to create a project package: {e}') from e
 
     ctx.obj = CLIContext(
         config_paths=config,
         config=_config,
     )
 
 
@@ -202,79 +247,47 @@
     config.initialize()
 
     dipdup = DipDup(config)
     await dipdup.run()
 
 
 @cli.command()
-@click.option('--overwrite-types', is_flag=True, help='Regenerate existing types.')
-@click.option('--keep-schemas', is_flag=True, help='Do not remove JSONSchemas after generating types.')
+@click.option('--force', '-f', is_flag=True, help='Regenerate existing types and ABIs.')
 @click.pass_context
 @_cli_wrapper
-async def init(ctx: click.Context, overwrite_types: bool, keep_schemas: bool) -> None:
+async def init(ctx: click.Context, force: bool) -> None:
     """Generate project tree, callbacks and types.
 
     This command is idempotent, meaning it won't overwrite previously generated files unless asked explicitly.
     """
-    from dipdup.config import DipDupConfig
     from dipdup.dipdup import DipDup
 
     config: DipDupConfig = ctx.obj.config
     dipdup = DipDup(config)
-    await dipdup.init(overwrite_types, keep_schemas)
+    await dipdup.init(force)
 
 
 @cli.command()
 @click.pass_context
 @_cli_wrapper
 async def migrate(ctx: click.Context) -> None:
     """
     Migrate project to the new spec version.
 
     If you're getting `MigrationRequiredError` after updating DipDup, this command will fix imports and type annotations to match the current `spec_version`. Review and commit changes after running it.
     """
     _logger.info('Project is already at the latest version, no further actions required')
 
 
-@cli.command()
-@click.pass_context
-@_cli_wrapper
-async def status(ctx: click.Context) -> None:
-    """Show the current status of indexes in the database."""
-    from dipdup.config import DipDupConfig
-    from dipdup.models import Index
-    from dipdup.utils.database import tortoise_wrapper
-
-    config: DipDupConfig = ctx.obj.config
-    url = config.database.connection_string
-    models = f'{config.package}.models'
-
-    table: list[tuple[str, str, str | int]] = [('name', 'status', 'level')]
-    async with tortoise_wrapper(
-        url=url,
-        models=models,
-        timeout=config.database.connection_timeout,
-        decimal_precision=config.advanced.decimal_precision,
-    ):
-        async for index in Index.filter().order_by('name'):
-            row = (index.name, index.status.value, index.level)
-            table.append(row)
-
-    # NOTE: Lazy import to speed up startup
-    from tabulate import tabulate
-
-    echo(tabulate(table, tablefmt='plain'))
-
-
 @cli.group()
 @click.pass_context
 @_cli_wrapper
 async def config(ctx: click.Context) -> None:
     """Commands to manage DipDup configuration."""
-    ...
+    pass
 
 
 @config.command(name='export')
 @click.option('--unsafe', is_flag=True, help='Resolve environment variables or use default values from config.')
 @click.option('--full', is_flag=True, help='Resolve index templates.')
 @click.pass_context
 @_cli_wrapper
@@ -287,59 +300,58 @@
     from dipdup.config import DipDupConfig
 
     config = DipDupConfig.load(
         paths=ctx.obj.config.paths,
         environment=unsafe,
     )
     if full:
-        config.initialize(skip_imports=True)
+        config.initialize()
     echo(config.dump())
 
 
 @config.command(name='env')
-@click.option('--file', '-f', type=str, default=None, help='Output to file instead of stdout.')
+@click.option('--output', '-o', type=str, default=None, help='Output to file instead of stdout.')
 @click.pass_context
 @_cli_wrapper
-async def config_env(ctx: click.Context, file: str | None) -> None:
+async def config_env(ctx: click.Context, output: str | None) -> None:
     """Dump environment variables used in DipDup config.
 
     If variable is not set, default value will be used.
     """
     from dipdup.config import DipDupConfig
 
     config = DipDupConfig.load(
         paths=ctx.obj.config.paths,
         environment=True,
     )
-    content = '\n'.join(f'{k}={v}' for k, v in config.environment.items())
-    if file:
-        with open(file, 'w') as f:
-            f.write(content)
+    content = '\n'.join(f'{k}={v}' for k, v in sorted(config.environment.items()))
+    if output:
+        Path(output).write_text(content)
     else:
         echo(content)
 
 
 @cli.group(help='Commands related to Hasura integration.')
 @click.pass_context
 @_cli_wrapper
 async def hasura(ctx: click.Context) -> None:
-    ...
+    pass
 
 
 @hasura.command(name='configure')
 @click.option('--force', is_flag=True, help='Proceed even if Hasura is already configured.')
 @click.pass_context
 @_cli_wrapper
 async def hasura_configure(ctx: click.Context, force: bool) -> None:
     """Configure Hasura GraphQL Engine to use with DipDup."""
     from dipdup.config import DipDupConfig
     from dipdup.config import PostgresDatabaseConfig
+    from dipdup.database import tortoise_wrapper
     from dipdup.exceptions import ConfigurationError
     from dipdup.hasura import HasuraGateway
-    from dipdup.utils.database import tortoise_wrapper
 
     config: DipDupConfig = ctx.obj.config
     if not config.hasura:
         raise ConfigurationError('`hasura` config section is empty')
     hasura_gateway = HasuraGateway(
         package=config.package,
         hasura_config=config.hasura,
@@ -348,59 +360,58 @@
 
     async with AsyncExitStack() as stack:
         await stack.enter_async_context(
             tortoise_wrapper(
                 url=config.database.connection_string,
                 models=config.package,
                 timeout=config.database.connection_timeout,
-                decimal_precision=config.advanced.decimal_precision,
             )
         )
         await stack.enter_async_context(hasura_gateway)
 
         await hasura_gateway.configure(force)
 
 
 @cli.group()
 @click.pass_context
 @_cli_wrapper
 async def schema(ctx: click.Context) -> None:
     """Commands to manage database schema."""
-    ...
+    pass
 
 
 @schema.command(name='approve')
 @click.pass_context
 @_cli_wrapper
 async def schema_approve(ctx: click.Context) -> None:
     """Continue to use existing schema after reindexing was triggered."""
+
     from dipdup.config import DipDupConfig
+    from dipdup.database import tortoise_wrapper
     from dipdup.models import Index
     from dipdup.models import Schema
-    from dipdup.utils.database import tortoise_wrapper
 
     config: DipDupConfig = ctx.obj.config
     url = config.database.connection_string
     models = f'{config.package}.models'
 
     _logger.info('Approving schema `%s`', url)
 
     async with tortoise_wrapper(
         url=url,
         models=models,
         timeout=config.database.connection_timeout,
         decimal_precision=config.advanced.decimal_precision,
     ):
-        # TODO: Non-nullable fields, remove in 7.0
         await Schema.filter(name=config.schema_name).update(
             reindex=None,
-            hash='',
+            hash=None,
         )
         await Index.filter().update(
-            config_hash='',
+            config_hash=None,
         )
 
     _logger.info('Schema approved')
 
 
 @schema.command(name='wipe')
 @click.option('--immune', is_flag=True, help='Drop immune tables too.')
@@ -409,26 +420,31 @@
 @_cli_wrapper
 async def schema_wipe(ctx: click.Context, immune: bool, force: bool) -> None:
     """
     Drop all database tables, functions and views.
 
     WARNING: This action is irreversible! All indexed data will be lost!
     """
-    from tortoise import Tortoise
-
-    from dipdup.config import DipDupConfig
-    from dipdup.config import PostgresDatabaseConfig
-    from dipdup.utils.database import get_connection
-    from dipdup.utils.database import tortoise_wrapper
-    from dipdup.utils.database import wipe_schema
+    from dipdup.config import SqliteDatabaseConfig
+    from dipdup.exceptions import ConfigurationError
 
     config: DipDupConfig = ctx.obj.config
     url = config.database.connection_string
     models = f'{config.package}.models'
 
+    # NOTE: Don't be confused by the name of `--immune` flag, we want to drop all tables if it's set.
+    immune_tables = set() if immune else config.database.immune_tables | {'dipdup_meta'}
+
+    if isinstance(config.database, SqliteDatabaseConfig) and immune_tables:
+        message = 'Support for immune tables in SQLite is experimental and requires `advanced.unsafe_sqlite` flag set'
+        if config.advanced.unsafe_sqlite:
+            _logger.warning(message)
+        else:
+            raise ConfigurationError(message)
+
     if not force:
         try:
             assert sys.__stdin__.isatty()
             click.confirm(
                 f"You're about to wipe schema `{url}`. All indexed data will be irreversibly lost, are you sure?",
                 abort=True,
             )
@@ -436,47 +452,46 @@
             click.echo('Not in a TTY, skipping confirmation')
         except click.Abort:
             click.echo('\nAborted')
             quit(0)
 
     _logger.info('Wiping schema `%s`', url)
 
+    from dipdup.database import get_connection
+    from dipdup.database import tortoise_wrapper
+    from dipdup.database import wipe_schema
+
     async with tortoise_wrapper(
         url=url,
         models=models,
         timeout=config.database.connection_timeout,
         decimal_precision=config.advanced.decimal_precision,
     ):
         conn = get_connection()
-        if isinstance(config.database, PostgresDatabaseConfig):
-            await wipe_schema(
-                conn=conn,
-                schema_name=config.database.schema_name,
-                # NOTE: Don't be confused by the name of `--immune` flag, we want to drop all tables if it's set.
-                immune_tables=config.database.immune_tables if not immune else set(),
-            )
-        else:
-            await Tortoise._drop_databases()
+        await wipe_schema(
+            conn=conn,
+            schema_name=config.database.schema_name,
+            immune_tables=immune_tables,
+        )
 
     _logger.info('Schema wiped')
 
 
 @schema.command(name='init')
 @click.pass_context
 @_cli_wrapper
 async def schema_init(ctx: click.Context) -> None:
     """
     Prepare a database for running DipDip.
 
     This command creates tables based on your models, then executes `sql/on_reindex` to finish preparation - the same things DipDup does when run on a clean database.
     """
-    from dipdup.config import DipDupConfig
+    from dipdup.database import generate_schema
+    from dipdup.database import get_connection
     from dipdup.dipdup import DipDup
-    from dipdup.utils.database import generate_schema
-    from dipdup.utils.database import get_connection
 
     config: DipDupConfig = ctx.obj.config
     url = config.database.connection_string
     dipdup = DipDup(config)
 
     _logger.info('Initializing schema `%s`', url)
 
@@ -500,20 +515,21 @@
 @click.pass_context
 @_cli_wrapper
 async def schema_export(ctx: click.Context) -> None:
     """Print SQL schema including scripts from `sql/on_reindex`.
 
     This command may help you debug inconsistency between project models and expected SQL schema.
     """
+
     from tortoise.utils import get_schema_sql
 
-    from dipdup.config import DipDupConfig
+    from dipdup import env
+    from dipdup.database import get_connection
+    from dipdup.database import tortoise_wrapper
     from dipdup.utils import iter_files
-    from dipdup.utils.database import get_connection
-    from dipdup.utils.database import tortoise_wrapper
 
     config: DipDupConfig = ctx.obj.config
     url = config.database.connection_string
     models = f'{config.package}.models'
     package_path = env.get_package_path(config.package)
 
     async with tortoise_wrapper(
@@ -534,71 +550,179 @@
         echo(output)
 
 
 @cli.command()
 @click.pass_context
 @click.option('--quiet', '-q', is_flag=True, help='Use default values for all prompts.')
 @click.option('--force', '-f', is_flag=True, help='Overwrite existing files.')
-@click.option('--replay', '-r', type=click.Path(exists=True), default=None, help='Replay a previously saved state.')
+@click.option(
+    '--replay',
+    '-r',
+    type=click.Path(exists=True, path_type=Path),
+    default=None,
+    help='Replay a previously saved state.',
+)
 @_cli_wrapper
 async def new(
     ctx: click.Context,
     quiet: bool,
     force: bool,
-    replay: str | None,
+    replay: Path | None,
 ) -> None:
     """Create a new project interactively."""
-    from dipdup.project import BaseProject
+    from dipdup.project import DEFAULT_ANSWERS
+    from dipdup.project import answers_from_replay
+    from dipdup.project import answers_from_terminal
+    from dipdup.project import render_project
+
+    if quiet:
+        answers = copy(DEFAULT_ANSWERS)
+    elif replay:
+        answers = answers_from_replay(replay)
+    else:
+        answers = answers_from_terminal()
+    render_project(answers, force)
+
 
-    project = BaseProject()
-    project.run(quiet, replay)
-    project.render(force)
+@cli.group()
+@click.pass_context
+@_cli_wrapper
+async def self(ctx: click.Context) -> None:
+    """Commands to manage local DipDup installation."""
+    pass
 
 
-@cli.command()
+@self.command(name='install')
 @click.pass_context
 @click.option('--quiet', '-q', is_flag=True, help='Use default values for all prompts.')
 @click.option('--force', '-f', is_flag=True, help='Force reinstall.')
+@click.option('--version', '-v', default=None, help='Install DipDup from a specific version.')
 @click.option('--ref', '-r', default=None, help='Install DipDup from a specific git ref.')
 @click.option('--path', '-p', default=None, help='Install DipDup from a local path.')
 @_cli_wrapper
-async def install(
+async def self_install(
     ctx: click.Context,
     quiet: bool,
     force: bool,
+    version: str | None,
     ref: str | None,
     path: str | None,
 ) -> None:
     """Install DipDup for the current user."""
     import dipdup.install
 
-    dipdup.install.install(quiet, force, ref, path)
+    dipdup.install.install(quiet, force, version, ref, path)
 
 
-@cli.command()
+@self.command(name='uninstall')
 @click.pass_context
 @click.option('--quiet', '-q', is_flag=True, help='Use default values for all prompts.')
 @_cli_wrapper
-async def uninstall(
+async def self_uninstall(
     ctx: click.Context,
     quiet: bool,
 ) -> None:
     """Uninstall DipDup for the current user."""
     import dipdup.install
 
     dipdup.install.uninstall(quiet)
 
 
-@cli.command()
+@self.command(name='update')
 @click.pass_context
 @click.option('--quiet', '-q', is_flag=True, help='Use default values for all prompts.')
 @click.option('--force', '-f', is_flag=True, help='Force reinstall.')
 @_cli_wrapper
-async def update(
+async def self_update(
     ctx: click.Context,
     quiet: bool,
     force: bool,
 ) -> None:
     """Update DipDup for the current user."""
     import dipdup.install
 
-    dipdup.install.install(quiet, force, None, None)
+    dipdup.install.install(quiet, force, None, None, None)
+
+
+@cli.group(invoke_without_command=True)
+@click.pass_context
+@_cli_wrapper
+async def report(ctx: click.Context) -> None:
+    """List and manage reports."""
+    if ctx.invoked_subcommand:
+        return
+
+    header = tuple(ReportHeader.__annotations__.keys())
+    rows = []
+    for path in REPORTS_PATH.iterdir():
+        if path.suffix not in ('.yml', '.yaml'):
+            continue
+
+        from ruamel.yaml import YAML
+
+        event = YAML(typ='base').load(path)
+        row = [event.get(key, 'none')[:80] for key in header]
+        rows.append(row)
+
+    rows.sort(key=lambda row: str(row[3]))
+
+    from tabulate import tabulate
+
+    echo(tabulate(rows, headers=header))
+
+
+@report.command(name='show')
+@click.pass_context
+@click.argument('id', type=str)
+@_cli_wrapper
+async def report_show(ctx: click.Context, id: str) -> None:
+    path = REPORTS_PATH / f'{id}.yaml'
+    if not path.exists():
+        echo('No such report')
+        return
+    print(path.read_text())
+
+
+@report.command(name='rm')
+@click.pass_context
+@click.argument('id', type=str, required=False)
+@click.option('--all', '-a', is_flag=True, help='Remove all reports.')
+@_cli_wrapper
+async def report_rm(ctx: click.Context, id: str | None, all: bool) -> None:
+    if all and id:
+        echo('Please specify either name or --all')
+        return
+    if all:
+        path = REPORTS_PATH
+        for file in path.iterdir():
+            file.unlink()
+        return
+
+    path = REPORTS_PATH / f'{id}.yaml'
+    if not path.exists():
+        echo('No such report')
+        return
+    path.unlink()
+
+
+@cli.group()
+@click.pass_context
+@_cli_wrapper
+async def package(ctx: click.Context) -> None:
+    """Inspect and manage project package."""
+    pass
+
+
+@package.command(name='tree')
+@click.pass_context
+@_cli_wrapper
+async def package_tree(ctx: click.Context) -> None:
+    from dipdup.package import DipDupPackage
+    from dipdup.package import draw_package_tree
+
+    config: DipDupConfig = ctx.obj.config
+    package = DipDupPackage(config.package_path)
+    package.create()
+    tree = package.discover()
+    echo(f'{package.name} [{package.root.relative_to(Path.cwd())}]')
+    for line in draw_package_tree(package.root, tree):
+        echo(line)
```

### Comparing `dipdup-6.5.9/src/dipdup/codegen.py` & `dipdup-7.0.0rc1/src/dipdup/codegen/tezos_tzkt.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,61 +4,52 @@
 * Callback codegen with Jinja2 templates
 * Types codegen with datamodel-codegen
 
 For `dipdup new` templates processing see `dipdup.project` module.
 
 Please, keep imports lazy to speed up startup.
 """
-import logging
-import re
-import subprocess
 from pathlib import Path
-from shutil import rmtree
-from shutil import which
 from typing import Any
 from typing import cast
 
-import orjson as json
+import orjson
 
-from dipdup import env
-from dipdup.config import BigMapIndexConfig
-from dipdup.config import CallbackMixin
-from dipdup.config import ContractConfig
-from dipdup.config import DatasourceConfigU
+from dipdup.codegen import CodeGenerator
+from dipdup.codegen import TypeClass
 from dipdup.config import DipDupConfig
-from dipdup.config import EventIndexConfig
-from dipdup.config import HeadIndexConfig
 from dipdup.config import IndexTemplateConfig
-from dipdup.config import OperationHandlerOriginationPatternConfig as OriginationPatternConfig
-from dipdup.config import OperationHandlerPatternConfigU as PatternConfigU
-from dipdup.config import OperationHandlerTransactionPatternConfig as TransactionPatternConfig
-from dipdup.config import OperationIndexConfig
-from dipdup.config import OperationUnfilteredIndexConfig
-from dipdup.config import TokenTransferIndexConfig
-from dipdup.config import TzktDatasourceConfig
-from dipdup.config import UnknownEventHandlerConfig
-from dipdup.config import event_hooks
-from dipdup.datasources.datasource import Datasource
-from dipdup.datasources.tzkt.datasource import TzktDatasource
-from dipdup.exceptions import ConfigInitializationException
+from dipdup.config import system_hooks
+from dipdup.config.tezos import TezosContractConfig
+from dipdup.config.tezos_tzkt import TzktDatasourceConfig
+from dipdup.config.tezos_tzkt_big_maps import TzktBigMapsIndexConfig
+from dipdup.config.tezos_tzkt_events import TzktEventsIndexConfig
+from dipdup.config.tezos_tzkt_events import TzktEventsUnknownEventHandlerConfig
+from dipdup.config.tezos_tzkt_head import TzktHeadIndexConfig
+from dipdup.config.tezos_tzkt_operations import OperationsHandlerOriginationPatternConfig as OriginationPatternConfig
+from dipdup.config.tezos_tzkt_operations import OperationsHandlerPatternConfigU as PatternConfigU
+from dipdup.config.tezos_tzkt_operations import OperationsHandlerTransactionPatternConfig as TransactionPatternConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsIndexConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsUnfilteredIndexConfig
+from dipdup.datasources import Datasource
+from dipdup.datasources.tezos_tzkt import TzktDatasource
 from dipdup.exceptions import ConfigurationError
-from dipdup.exceptions import FeatureAvailabilityError
 from dipdup.exceptions import FrameworkException
-from dipdup.utils import import_submodules
+from dipdup.package import DipDupPackage
+from dipdup.utils import json_dumps
 from dipdup.utils import pascal_to_snake
 from dipdup.utils import snake_to_pascal
-from dipdup.utils.codegen import load_template
-from dipdup.utils.codegen import touch
-from dipdup.utils.codegen import write
-
-KEEP_MARKER = '.keep'
-PYTHON_MARKER = '__init__.py'
-PEP_561_MARKER = 'py.typed'
-MODELS_MODULE = 'models.py'
-CALLBACK_TEMPLATE = 'callback.py.j2'
+from dipdup.utils import write
+
+
+def match_entrypoint_schema(entrypoint_name: str, entrypoint_schemas: list[dict[str, Any]]) -> dict[str, Any]:
+    if entrypoint_name == 'default' and len(entrypoint_schemas) == 1:
+        return entrypoint_schemas[0]['parameterSchema']  # type: ignore[no-any-return]
+
+    return next(ep['parameterSchema'] for ep in entrypoint_schemas if ep['name'] == entrypoint_name)
 
 
 def preprocess_storage_jsonschema(schema: dict[str, Any]) -> dict[str, Any]:
     """Preprocess `big_map` sections in JSONSchema.
 
     TzKT returns them as unions since before merging big map diffs there are just `int` pointers.
     We apply big map diffs to storage so there's no need to include `int` in type signature.
@@ -87,96 +78,160 @@
         }
     elif schema.get('$comment') == 'big_map':
         return cast(dict[str, Any], schema['oneOf'][1])
     else:
         return schema
 
 
-# TODO: Pick refactoring from `ref/config-module`
-class ProjectPaths:
-    def __init__(self, root: Path) -> None:
-        self.root = root
-        self.models = root / MODELS_MODULE
-        self.schemas = root / 'schemas'
-        self.types = root / 'types'
-        self.handlers = root / 'handlers'
-        self.hooks = root / 'hooks'
-        self.sql = root / 'sql'
-        self.graphql = root / 'graphql'
-        self.hasura = root / 'hasura'
-
-    def create_package(self) -> None:
-        """Create Python package skeleton if not exists"""
-        touch(self.root / PYTHON_MARKER)
-        touch(self.root / PEP_561_MARKER)
-
-        touch(self.types / PYTHON_MARKER)
-        touch(self.handlers / PYTHON_MARKER)
-        touch(self.hooks / PYTHON_MARKER)
-
-        touch(self.sql / KEEP_MARKER)
-        touch(self.graphql / KEEP_MARKER)
-        touch(self.hasura / KEEP_MARKER)
-
-        if not self.models.is_file():
-            template = load_template('templates', f'{MODELS_MODULE}.j2')
-            models_code = template.render()
-            write(self.models, models_code)
+class TzktCodeGenerator(CodeGenerator):
+    """Generates package based on config, invoked from `init` CLI command"""
 
+    def __init__(
+        self,
+        config: DipDupConfig,
+        package: DipDupPackage,
+        datasources: dict[str, Datasource[Any]],
+    ) -> None:
+        super().__init__(
+            config=config,
+            package=package,
+            datasources=datasources,
+        )
+        self._schemas: dict[str, dict[str, dict[str, Any]]] = {}
 
-class CodeGenerator:
-    """Generates package based on config, invoked from `init` CLI command"""
+    async def generate_abi(self) -> None:
+        pass
+
+    async def generate_schemas(self) -> None:
+        """Fetch JSONSchemas for all contracts used in config"""
+        self._logger.info('Fetching contract schemas')
+
+        unused_operation_templates = [
+            t for t in self._config.templates.values() if isinstance(t, TzktOperationsIndexConfig)
+        ]
+
+        for index_config in self._config.indexes.values():
+            if isinstance(index_config, TzktOperationsIndexConfig):
+                await self._fetch_operation_index_schema(index_config)
+                template = cast(TzktOperationsIndexConfig, index_config.parent)
+                if template in unused_operation_templates:
+                    unused_operation_templates.remove(template)
+            elif isinstance(index_config, TzktBigMapsIndexConfig):
+                await self._fetch_big_map_index_schema(index_config)
+            elif isinstance(index_config, TzktEventsIndexConfig):
+                await self._fetch_event_index_schema(index_config)
+            else:
+                pass
 
-    def __init__(self, config: DipDupConfig, datasources: dict[DatasourceConfigU, Datasource]) -> None:
-        self._logger = logging.getLogger('dipdup.codegen')
-        self._config = config
-        self._datasources = datasources
-        self._schemas: dict[TzktDatasourceConfig, dict[str, dict[str, Any]]] = {}
-        self._pkg = ProjectPaths(env.get_package_path(config.package))
-
-    def create_package(self) -> None:
-        self._pkg.create_package()
-
-    async def init(self, overwrite_types: bool = False, keep_schemas: bool = False) -> None:
-        self._logger.info('Initializing project')
-        self.create_package()
-
-        await self.fetch_schemas()
-        await self.generate_types(overwrite_types)
-        await self.generate_hooks()
-        await self.generate_handlers()
-        if not keep_schemas:
-            await self.cleanup()
-        await self.verify_package()
-
-    @staticmethod
-    def __match_entrypoint_schema(
-        entrypoint_name: str, entrypoint_schemas: list[dict[str, dict[str, Any] | Any]]
+        # NOTE: Euristics for complex cases like templated `similar_to` factories.
+        # NOTE: Try different contracts and datasources from config until one succeeds.
+        for template_config in unused_operation_templates:
+            self._logger.warning(
+                'Unused operation template `%s`. Ignore this warning if it is used in a factory.', template_config.name
+            )
+            datasource_name = template_config.datasource
+            if isinstance(datasource_name, str) and datasource_name in self._config.datasources:
+                datasource_config = self._config.get_tzkt_datasource(datasource_name)
+                template_config.datasource = datasource_config
+                await self._fetch_operation_index_schema(template_config)
+            else:
+                self._logger.info('Unresolved `datasource` field, trying to guess it.')
+                for possible_datasource_config in self._config.datasources.values():
+                    if not isinstance(possible_datasource_config, TzktDatasourceConfig):
+                        continue
+                    # NOTE: Do not modify config without necessity
+                    template_config.datasource = possible_datasource_config
+                    template_config.contracts = [
+                        c for c in self._config.contracts.values() if isinstance(c, TezosContractConfig)
+                    ]
+                    try:
+                        await self._fetch_operation_index_schema(template_config)
+                    except FrameworkException:
+                        continue
+
+    async def generate_handlers(self) -> None:
+        """Generate handler stubs with typehints from templates if not exist"""
+        for index_config in self._config.indexes.values():
+            if isinstance(index_config, IndexTemplateConfig):
+                continue
+            # NOTE: Always single handler
+            if isinstance(index_config, (TzktOperationsUnfilteredIndexConfig, TzktHeadIndexConfig)):
+                await self._generate_callback(index_config.handler_config, 'handlers')
+                continue
+
+            for handler_config in index_config.handlers:
+                await self._generate_callback(handler_config, 'handlers')
+
+    async def generate_hooks(self) -> None:
+        for hook_configs in self._config.hooks.values(), system_hooks.values():
+            for hook_config in hook_configs:
+                await self._generate_callback(hook_config, 'hooks', sql=True)
+
+    async def generate_system_hooks(self) -> None:
+        pass
+
+    def get_typeclass_name(self, schema_path: Path) -> str:
+        module_name = schema_path.stem
+        if schema_path.name == 'tezos_storage.json':
+            class_name = f'{schema_path.parent.name}_storage'
+        elif schema_path.parent.name == 'tezos_parameters':
+            class_name = f'{module_name}_parameter'
+        elif schema_path.parent.name == 'tezos_events':
+            class_name = f'{module_name}_payload'
+        else:
+            class_name = module_name
+        return class_name
+
+    async def _get_schema(
+        self,
+        datasource_config: TzktDatasourceConfig,
+        contract_config: TezosContractConfig,
     ) -> dict[str, Any]:
-        if entrypoint_name == 'default' and len(entrypoint_schemas) == 1:
-            return entrypoint_schemas[0]['parameterSchema']
+        """Get contract JSONSchema from TzKT or from cache"""
+        datasource = self._datasources[datasource_config.name]
+        if not isinstance(datasource, TzktDatasource):
+            raise FrameworkException('`tzkt` datasource expected')
 
-        return next(ep['parameterSchema'] for ep in entrypoint_schemas if ep['name'] == entrypoint_name)
+        if isinstance(contract_config.address, str):
+            address = contract_config.address
+        elif isinstance(contract_config.code_hash, str):
+            address = contract_config.code_hash
+        elif isinstance(contract_config.code_hash, int):
+            address = await datasource.get_contract_address(contract_config.code_hash, 0)
+        else:
+            raise FrameworkException('No address or code hash provided, check earlier')
+
+        name = datasource_config.name
+        if name not in self._schemas:
+            self._schemas[name] = {}
+        if address not in self._schemas[name]:
+            self._logger.info('Fetching schemas for contract `%s`', address)
+            address_schemas_json = await datasource.get_jsonschemas(address)
+            self._schemas[name][address] = address_schemas_json
+        return self._schemas[name][address]
 
     async def _fetch_operation_pattern_schema(
         self,
         operation_pattern_config: PatternConfigU,
         datasource_config: TzktDatasourceConfig,
     ) -> None:
         contract_config = operation_pattern_config.typed_contract
         if contract_config is None:
             return
 
         # NOTE: A very special case; unresolved `operation` template to spawn from factory indexes.
         elif isinstance(contract_config, str) and contract_config in self._config.contracts:
-            contract_config = self._config.contracts[contract_config]
+            contract_config = self._config.get_tezos_contract(contract_config)
 
         elif isinstance(contract_config, str):
             self._logger.info('Unresolved `contract` field, trying to guess it.')
             for possible_contract_config in self._config.contracts.values():
+                if not isinstance(possible_contract_config, TezosContractConfig):
+                    continue
+
                 if isinstance(operation_pattern_config, TransactionPatternConfig):
                     operation_pattern_config.destination = possible_contract_config
                 elif isinstance(operation_pattern_config, OriginationPatternConfig):
                     operation_pattern_config.originated_contract = possible_contract_config
                 try:
                     await self._fetch_operation_pattern_schema(
                         operation_pattern_config,
@@ -186,331 +241,157 @@
                 except FrameworkException:
                     self._logger.info("It's not `%s`", possible_contract_config.address)
                     continue
 
             return
 
         contract_schemas = await self._get_schema(datasource_config, contract_config)
-        contract_schemas_path = self._pkg.schemas / contract_config.module_name
+        contract_schemas_path = self._package.schemas / contract_config.module_name
 
-        storage_schema_path = contract_schemas_path / 'storage.json'
+        storage_schema_path = contract_schemas_path / 'tezos_storage.json'
         storage_schema = preprocess_storage_jsonschema(contract_schemas['storageSchema'])
 
-        write(storage_schema_path, json.dumps(storage_schema, option=json.OPT_INDENT_2))
+        write(storage_schema_path, json_dumps(storage_schema))
 
         if not isinstance(operation_pattern_config, TransactionPatternConfig):
             return
 
-        parameter_schemas_path = contract_schemas_path / 'parameter'
+        parameter_schemas_path = contract_schemas_path / 'tezos_parameters'
         entrypoint = cast(str, operation_pattern_config.entrypoint)
 
         try:
-            entrypoint_schema = self.__match_entrypoint_schema(
+            entrypoint_schema = match_entrypoint_schema(
                 entrypoint,
                 contract_schemas['entrypoints'],
             )
         except StopIteration as e:
             raise ConfigurationError(f'Contract `{contract_config.address}` has no entrypoint `{entrypoint}`') from e
 
         entrypoint = entrypoint.replace('.', '_').lstrip('_')
         entrypoint_schema_path = parameter_schemas_path / f'{entrypoint}.json'
-        written = write(entrypoint_schema_path, json.dumps(entrypoint_schema, option=json.OPT_INDENT_2))
+        written = write(entrypoint_schema_path, json_dumps(entrypoint_schema))
         if not written and contract_config.typename is not None:
-            with open(entrypoint_schema_path, 'r') as file:
-                existing_schema = json.loads(file.read())
+            existing_schema = orjson.loads(entrypoint_schema_path.read_text())
             if entrypoint_schema != existing_schema:
                 self._logger.warning(
                     'Contract `%s` falsely claims to be a `%s`', contract_config.address, contract_config.typename
                 )
 
-    async def _fetch_operation_index_schema(self, index_config: OperationIndexConfig) -> None:
+    async def _fetch_operation_index_schema(self, index_config: TzktOperationsIndexConfig) -> None:
         for handler_config in index_config.handlers:
             for operation_pattern_config in handler_config.pattern:
                 await self._fetch_operation_pattern_schema(
                     operation_pattern_config,
-                    index_config.datasource_config,
+                    index_config.datasource,
                 )
 
-    async def _fetch_big_map_index_schema(self, index_config: BigMapIndexConfig) -> None:
+    async def _fetch_big_map_index_schema(self, index_config: TzktBigMapsIndexConfig) -> None:
         for handler_config in index_config.handlers:
             contract_config = handler_config.contract
 
-            contract_schemas = await self._get_schema(index_config.datasource_config, contract_config)
+            contract_schemas = await self._get_schema(index_config.datasource, contract_config)
 
-            contract_schemas_path = self._pkg.schemas / contract_config.module_name
-            big_map_schemas_path = contract_schemas_path / 'big_map'
+            contract_schemas_path = self._package.schemas / contract_config.module_name
+            big_map_schemas_path = contract_schemas_path / 'tezos_big_maps'
 
             try:
                 big_map_schema = next(ep for ep in contract_schemas['bigMaps'] if ep['path'] == handler_config.path)
             except StopIteration as e:
                 raise ConfigurationError(
                     f'Contract `{contract_config.address}` has no big map path `{handler_config.path}`'
                 ) from e
             big_map_path = handler_config.path.replace('.', '_')
             big_map_key_schema = big_map_schema['keySchema']
             big_map_key_schema_path = big_map_schemas_path / f'{big_map_path}_key.json'
-            write(big_map_key_schema_path, json.dumps(big_map_key_schema, option=json.OPT_INDENT_2))
+            write(
+                big_map_key_schema_path,
+                json_dumps(
+                    big_map_key_schema,
+                ),
+            )
 
             big_map_value_schema = big_map_schema['valueSchema']
             big_map_value_schema_path = big_map_schemas_path / f'{big_map_path}_value.json'
-            write(big_map_value_schema_path, json.dumps(big_map_value_schema, option=json.OPT_INDENT_2))
+            write(big_map_value_schema_path, json_dumps(big_map_value_schema))
 
-    async def _fetch_event_index_schema(self, index_config: EventIndexConfig) -> None:
+    async def _fetch_event_index_schema(self, index_config: TzktEventsIndexConfig) -> None:
         for handler_config in index_config.handlers:
-            if isinstance(handler_config, UnknownEventHandlerConfig):
+            if isinstance(handler_config, TzktEventsUnknownEventHandlerConfig):
                 continue
 
             contract_config = handler_config.contract
             contract_schemas = await self._get_schema(
-                index_config.datasource_config,
+                index_config.datasource,
                 contract_config,
             )
-            contract_schemas_path = self._pkg.schemas / contract_config.module_name
-            event_schemas_path = contract_schemas_path / 'event'
+            contract_schemas_path = self._package.schemas / contract_config.module_name
+            event_schemas_path = contract_schemas_path / 'tezos_events'
 
             try:
                 event_schema = next(ep for ep in contract_schemas['events'] if ep['tag'] == handler_config.tag)
             except StopIteration as e:
                 raise ConfigurationError(
                     f'Contract `{contract_config.address}` has no event with tag `{handler_config.tag}`'
                 ) from e
 
             event_tag = handler_config.tag.replace('.', '_')
             event_schema = event_schema['eventSchema']
             event_schema_path = event_schemas_path / f'{event_tag}.json'
-            write(event_schema_path, json.dumps(event_schema, option=json.OPT_INDENT_2))
+            write(event_schema_path, json_dumps(event_schema))
 
-    async def fetch_schemas(self) -> None:
-        """Fetch JSONSchemas for all contracts used in config"""
-        self._logger.info('Fetching contract schemas')
-
-        unused_operation_templates = [t for t in self._config.templates.values() if isinstance(t, OperationIndexConfig)]
-
-        for index_config in self._config.indexes.values():
-            if isinstance(index_config, OperationIndexConfig):
-                await self._fetch_operation_index_schema(index_config)
-                template = cast(OperationIndexConfig, index_config.parent)
-                if template in unused_operation_templates:
-                    unused_operation_templates.remove(template)
-            elif isinstance(index_config, BigMapIndexConfig):
-                await self._fetch_big_map_index_schema(index_config)
-            elif isinstance(index_config, EventIndexConfig):
-                await self._fetch_event_index_schema(index_config)
-            elif isinstance(index_config, HeadIndexConfig):
-                pass
-            elif isinstance(index_config, TokenTransferIndexConfig):
-                pass
-            elif isinstance(index_config, OperationUnfilteredIndexConfig):
-                pass
-            elif isinstance(index_config, IndexTemplateConfig):
-                raise ConfigInitializationException
-            else:
-                raise NotImplementedError(f'Index kind `{index_config.kind}` is not supported')
-
-        # NOTE: Euristics for complex cases like templated `similar_to` factories.
-        # NOTE: Try different contracts and datasources from config until one succeeds.
-        for template_config in unused_operation_templates:
-            self._logger.warning(
-                'Unused operation template `%s`. Ignore this warning if it is used in a factory.', template_config.name
-            )
-            datasource_name = template_config.datasource
-            if isinstance(datasource_name, str) and datasource_name in self._config.datasources:
-                datasource_config = self._config.get_tzkt_datasource(datasource_name)
-                template_config.datasource = datasource_config
-                await self._fetch_operation_index_schema(template_config)
-            else:
-                self._logger.info('Unresolved `datasource` field, trying to guess it.')
-                for possible_datasource_config in self._config.datasources.values():
-                    if not isinstance(possible_datasource_config, TzktDatasourceConfig):
-                        continue
-                    # NOTE: Do not modify config without necessity
-                    template_config.datasource = possible_datasource_config
-                    template_config.contracts = list(self._config.contracts.values())
-                    try:
-                        await self._fetch_operation_index_schema(template_config)
-                    except FrameworkException:
-                        continue
-
-    async def _generate_type(self, schema_path: Path, force: bool) -> None:
-        rel_path = schema_path.relative_to(self._pkg.schemas)
-        type_pkg_path = self._pkg.types / rel_path
-
-        if schema_path.is_dir():
-            touch(type_pkg_path / PYTHON_MARKER)
-            return
-
-        if not schema_path.name.endswith('.json'):
-            self._logger.warning('Skipping `%s`: not a JSON', schema_path)
-            return
-
-        module_name = schema_path.stem
-        output_path = type_pkg_path.parent / f'{pascal_to_snake(module_name)}.py'
-        if output_path.exists() and not force:
-            self._logger.info('Skipping `%s`: type already exists', schema_path)
-            return
-
-        # NOTE: Skip if the first line starts with "# dipdup: ignore"
-        # TODO: Replace with `immune_types` in config
-        if output_path.exists():
-            with open(output_path) as type_file:
-                first_line = type_file.readline()
-                if re.match(r'^#\s+dipdup:\s+ignore\s*', first_line):
-                    self._logger.info('Skipping `%s`: "# dipdup: ignore" marker found', output_path)
-                    return
-
-        datamodel_codegen = which('datamodel-codegen')
-        if not datamodel_codegen:
-            raise FeatureAvailabilityError(
-                feature='codegen',
-                reason='datamodel-codegen is not installed. Are you in the `-slim` Docker image? If not - run `dipdup-install`.',
-            )
-
-        if schema_path.name == 'storage.json':
-            class_name = f'{schema_path.parent.name}_storage'
-        elif schema_path.parent.name == 'parameter':
-            class_name = f'{module_name}_parameter'
-        elif schema_path.parent.name == 'event':
-            class_name = f'{module_name}_payload'
-        else:
-            class_name = module_name
-
-        class_name = snake_to_pascal(class_name).lstrip('_')
-
-        self._logger.info('Generating type `%s`', class_name)
-        output_path.parent.mkdir(parents=True, exist_ok=True)
-        (output_path.parent / PYTHON_MARKER).touch(exist_ok=True)
-        args = [
-            datamodel_codegen,
-            '--input',
-            str(schema_path),
-            '--output',
-            str(output_path),
-            '--class-name',
-            class_name,
-            '--disable-timestamp',
-            '--input-file-type',
-            'jsonschema',
-            '--target-python-version',
-            '3.10',
-        ]
-        self._logger.debug(' '.join(args))
-        subprocess.run(args, check=True)
-
-    async def generate_types(self, overwrite_types: bool = False) -> None:
-        """Generate typeclasses from fetched JSONSchemas: contract's storage, parameters, big maps and events."""
-
-        self._logger.info('Creating `types` package')
-        touch(self._pkg.types / PYTHON_MARKER)
-
-        for path in self._pkg.schemas.glob('**/*'):
-            await self._generate_type(path, overwrite_types)
-
-    async def generate_handlers(self) -> None:
-        """Generate handler stubs with typehints from templates if not exist"""
-        for index_config in self._config.indexes.values():
-            if isinstance(index_config, IndexTemplateConfig):
-                continue
-            if isinstance(index_config, OperationUnfilteredIndexConfig):
-                await self._generate_callback(index_config.handler_config)
-                continue
-
-            for handler_config in index_config.handlers:
-                await self._generate_callback(handler_config)
-
-    async def generate_hooks(self) -> None:
-        for hook_configs in self._config.hooks.values(), event_hooks.values():
-            for hook_config in hook_configs:
-                await self._generate_callback(hook_config, sql=True)
-
-    async def cleanup(self) -> None:
-        """Remove fetched JSONSchemas"""
-        self._logger.info('Cleaning up')
-        rmtree(self._pkg.schemas, ignore_errors=True)
-
-    async def verify_package(self) -> None:
-        submodules = import_submodules(self._config.package)
-        self._logger.info('Package `%s` is valid; %d submodules found', self._config.package, len(submodules))
-
-    async def _get_schema(
+    async def get_schemas(
         self,
-        datasource_config: TzktDatasourceConfig,
-        contract_config: ContractConfig,
+        datasource: TzktDatasource,
+        contract_config: TezosContractConfig,
     ) -> dict[str, Any]:
         """Get contract JSONSchema from TzKT or from cache"""
-        datasource = self._datasources[datasource_config]
-        if not isinstance(datasource, TzktDatasource):
-            raise FrameworkException('`tzkt` datasource expected')
+        schemas: dict[str, Any] = {}
 
         if isinstance(contract_config.address, str):
             address = contract_config.address
         elif isinstance(contract_config.code_hash, str):
             address = contract_config.code_hash
         elif isinstance(contract_config.code_hash, int):
             address = await datasource.get_contract_address(contract_config.code_hash, 0)
         else:
             raise FrameworkException('No address or code hash provided, check earlier')
 
-        if datasource_config not in self._schemas:
-            self._schemas[datasource_config] = {}
-        if address not in self._schemas[datasource_config]:
+        if datasource.name not in schemas:
+            schemas[datasource.name] = {}
+        if address not in schemas[datasource.name]:
             self._logger.info('Fetching schemas for contract `%s`', address)
             address_schemas_json = await datasource.get_jsonschemas(address)
-            self._schemas[datasource_config][address] = address_schemas_json
-        return self._schemas[datasource_config][address]
+            schemas[datasource.name][address] = address_schemas_json
+        return cast(dict[str, Any], schemas[datasource.name][address])
 
-    async def _generate_callback(self, callback_config: CallbackMixin, sql: bool = False) -> None:
-        original_callback = callback_config.callback
-        subpackages = callback_config.callback.split('.')
-        subpackages, callback = subpackages[:-1], subpackages[-1]
-
-        callback_path = Path(
-            self._pkg.root,
-            f'{callback_config.kind}s',
-            *subpackages,
-            f'{callback}.py',
-        )
 
-        if callback_path.exists():
-            return
+def get_storage_type(package: DipDupPackage, typename: str) -> TypeClass:
+    cls_name = snake_to_pascal(typename) + 'Storage'
+    return package.get_type(typename, 'tezos_storage', cls_name)
 
-        self._logger.info('Generating %s callback `%s`', callback_config.kind, callback)
-        callback_template = load_template('templates', CALLBACK_TEMPLATE)
 
-        arguments = callback_config.format_arguments()
-        imports = set(callback_config.format_imports(self._config.package))
+def get_parameter_type(package: DipDupPackage, typename: str, entrypoint: str) -> TypeClass:
+    entrypoint = entrypoint.lstrip('_')
+    module_name = f'tezos_parameters.{pascal_to_snake(entrypoint)}'
+    cls_name = snake_to_pascal(entrypoint) + 'Parameter'
+    return package.get_type(typename, module_name, cls_name)
 
-        code: list[str] = []
-        if sql:
-            code.append(f"await ctx.execute_sql('{original_callback}')")
-            if callback == 'on_index_rollback':
-                code.append('await ctx.rollback(')
-                code.append('    index=index.name,')
-                code.append('    from_level=from_level,')
-                code.append('    to_level=to_level,')
-                code.append(')')
-        else:
-            code.append('...')
 
-        # NOTE: Fix missing generic type annotation for `Index[IndexConfig]` to comply with `mypy --strict`
-        processed_arguments = tuple(
-            f'{a},  # type: ignore[type-arg]' if a.startswith('index: Index') else a for a in arguments
-        )
+def get_event_payload_type(package: DipDupPackage, typename: str, tag: str) -> TypeClass:
+    tag = pascal_to_snake(tag.replace('.', '_'))
+    module_name = f'tezos_event.{tag}'
+    cls_name = snake_to_pascal(f'{tag}_payload')
+    return package.get_type(typename, module_name, cls_name)
 
-        callback_code = callback_template.render(
-            callback=callback,
-            arguments=tuple(processed_arguments),
-            imports=sorted(dict.fromkeys(imports)),
-            code=code,
-        )
-        write(callback_path, callback_code)
 
-        if not sql:
-            return
+def get_big_map_key_type(package: DipDupPackage, typename: str, path: str) -> TypeClass:
+    path = pascal_to_snake(path.replace('.', '_'))
+    module_name = f'tezos_big_maps.{path}_key'
+    cls_name = snake_to_pascal(path + '_key')
+    return package.get_type(typename, module_name, cls_name)
 
-        # NOTE: Preserve the same structure as in `handlers`
-        sql_path = Path(
-            self._pkg.sql,
-            *subpackages,
-            callback,
-            KEEP_MARKER,
-        )
-        touch(sql_path)
+
+def get_big_map_value_type(package: DipDupPackage, typename: str, path: str) -> TypeClass:
+    path = pascal_to_snake(path.replace('.', '_'))
+    module_name = f'tezos_big_maps.{path}_value'
+    cls_name = snake_to_pascal(path + '_value')
+    return package.get_type(typename, module_name, cls_name)
```

### Comparing `dipdup-6.5.9/src/dipdup/context.py` & `dipdup-7.0.0rc1/src/dipdup/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,91 @@
 import asyncio
 import importlib
-import logging
 import os
 import sys
 from collections import deque
 from contextlib import AsyncExitStack
 from contextlib import ExitStack
 from contextlib import contextmanager
 from contextlib import suppress
 from pathlib import Path
 from pprint import pformat
+from types import ModuleType
 from typing import Any
 from typing import Awaitable
 from typing import Iterator
-from typing import NoReturn
+from typing import Literal
 from typing import TypeVar
 from typing import cast
 
-from tortoise import Tortoise
 from tortoise.exceptions import OperationalError
 
 from dipdup import env
-from dipdup.config import BigMapIndexConfig
-from dipdup.config import ContractConfig
+from dipdup.config import ContractConfigU
 from dipdup.config import DipDupConfig
-from dipdup.config import EventHookConfig
-from dipdup.config import EventIndexConfig
 from dipdup.config import HandlerConfig
-from dipdup.config import HeadIndexConfig
 from dipdup.config import HookConfig
-from dipdup.config import OperationIndexConfig
-from dipdup.config import OperationUnfilteredIndexConfig
-from dipdup.config import PostgresDatabaseConfig
 from dipdup.config import ResolvedIndexConfigU
-from dipdup.config import TokenTransferIndexConfig
-from dipdup.datasources.coinbase.datasource import CoinbaseDatasource
-from dipdup.datasources.datasource import Datasource
-from dipdup.datasources.datasource import HttpDatasource
-from dipdup.datasources.ipfs.datasource import IpfsDatasource
-from dipdup.datasources.metadata.datasource import MetadataDatasource
-from dipdup.datasources.tzkt.datasource import TzktDatasource
-from dipdup.enums import ReindexingAction
-from dipdup.enums import ReindexingReason
+from dipdup.config.evm import EvmContractConfig
+from dipdup.config.evm_subsquid_events import SubsquidEventsIndexConfig
+from dipdup.config.evm_subsquid_operations import SubsquidOperationsIndexConfig
+from dipdup.config.tezos import TezosContractConfig
+from dipdup.config.tezos_tzkt_big_maps import TzktBigMapsIndexConfig
+from dipdup.config.tezos_tzkt_events import TzktEventsIndexConfig
+from dipdup.config.tezos_tzkt_head import TzktHeadIndexConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsIndexConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsUnfilteredIndexConfig
+from dipdup.config.tezos_tzkt_token_transfers import TzktTokenTransfersIndexConfig
+from dipdup.database import execute_sql
+from dipdup.database import execute_sql_query
+from dipdup.database import get_connection
+from dipdup.database import wipe_schema
+from dipdup.datasources import Datasource
+from dipdup.datasources import IndexDatasource
+from dipdup.datasources.coinbase import CoinbaseDatasource
+from dipdup.datasources.evm_node import EvmNodeDatasource
+from dipdup.datasources.evm_subsquid import SubsquidDatasource
+from dipdup.datasources.http import HttpDatasource
+from dipdup.datasources.ipfs import IpfsDatasource
+from dipdup.datasources.tezos_tzkt import TzktDatasource
+from dipdup.datasources.tzip_metadata import TzipMetadataDatasource
 from dipdup.exceptions import CallbackError
-from dipdup.exceptions import CallbackTypeError
 from dipdup.exceptions import ConfigurationError
 from dipdup.exceptions import ContractAlreadyExistsError
 from dipdup.exceptions import FrameworkException
 from dipdup.exceptions import InitializationRequiredError
 from dipdup.exceptions import ReindexingRequiredError
 from dipdup.models import Contract
 from dipdup.models import ContractMetadata
 from dipdup.models import Index
 from dipdup.models import ModelUpdate
+from dipdup.models import ReindexingAction
+from dipdup.models import ReindexingReason
 from dipdup.models import Schema
 from dipdup.models import TokenMetadata
+from dipdup.package import DipDupPackage
+from dipdup.performance import _CacheManager
+from dipdup.performance import _MetricManager
+from dipdup.performance import _QueueManager
+from dipdup.performance import caches
+from dipdup.performance import metrics
+from dipdup.performance import queues
 from dipdup.prometheus import Metrics
 from dipdup.transactions import TransactionManager
 from dipdup.utils import FormattedLogger
-from dipdup.utils.database import execute_sql
-from dipdup.utils.database import execute_sql_query
-from dipdup.utils.database import get_connection
-from dipdup.utils.database import wipe_schema
-
-DatasourceT = TypeVar('DatasourceT', bound=Datasource)
 
-
-# FIXME: Singletons shared by all contexts
-pending_indexes: deque[Any] = deque()
-pending_hooks: deque[Awaitable[None]] = deque()
-rolled_back_indexes: set[str] = set()
+DatasourceT = TypeVar('DatasourceT', bound=Datasource[Any])
 
 
 class MetadataCursor:
     _contract = 0
     _token = 0
 
-    def __call__(cls) -> NoReturn:
-        raise NotImplementedError('MetadataCursor is a singleton class')
+    def __init__(self) -> None:
+        raise FrameworkException('MetadataCursor is a singleton class')
 
     @classmethod
     async def initialize(cls) -> None:
         """Initialize metadata cursor from the database."""
         if last_contract := await ContractMetadata.filter().order_by('-update_id').first():
             cls._contract = last_contract.update_id
         if last_token := await TokenMetadata.filter().order_by('-update_id').first():
@@ -99,84 +103,58 @@
         cls._token += 1
         return cls._token
 
 
 class DipDupContext:
     """Common execution context for handler and hook callbacks.
 
-    :param datasources: Mapping of available datasources
     :param config: DipDup configuration
+    :param package: DipDup package
+    :param datasources: Mapping of available datasources
     :param logger: Context-aware logger instance
     """
 
     def __init__(
         self,
-        datasources: dict[str, Datasource],
         config: DipDupConfig,
-        callbacks: 'CallbackManager',
+        package: DipDupPackage,
+        datasources: dict[str, Datasource[Any]],
         transactions: TransactionManager,
     ) -> None:
-        self.datasources = datasources
         self.config = config
-        self._callbacks = callbacks
-        self._transactions = transactions
+        self.package = package
+        self.datasources = datasources
+        self.transactions = transactions
+
         self.logger = FormattedLogger('dipdup.context')
+        self._pending_indexes: deque[Any] = deque()
+        self._pending_hooks: deque[Awaitable[None]] = deque()
+        self._rolled_back_indexes: set[str] = set()
+        self._handlers: dict[tuple[str, str], HandlerConfig] = {}
+        self._hooks: dict[str, HookConfig] = {}
 
     def __str__(self) -> str:
         return pformat(self.__dict__)
 
-    async def fire_hook(
-        self,
-        name: str,
-        fmt: str | None = None,
-        wait: bool = True,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
-        """Fire hook with given name and arguments.
-
-        :param name: Hook name
-        :param fmt: Format string for `ctx.logger` messages
-        :param wait: Wait for hook to finish or fire and forget
-        """
-        await self._callbacks.fire_hook(self, name, fmt, wait, *args, **kwargs)
-
-    async def _fire_handler(
-        self,
-        name: str,
-        index: str,
-        datasource: TzktDatasource,
-        fmt: str | None = None,
-        *args: Any,
-        **kwargs: Any,
-    ) -> None:
-        """Fire handler with given name and arguments.
-
-        :param name: Handler name
-        :param index: Index name
-        :param datasource: An instance of datasource that triggered the handler
-        :param fmt: Format string for `ctx.logger` messages
-        """
-        await self._callbacks._fire_handler(self, name, index, datasource, fmt, *args, **kwargs)
-
-    async def execute_sql(self, name: str, *args: Any, **kwargs: Any) -> None:
-        """Executes SQL script(s) with given name.
-
-        If the `name` path is a directory, all `.sql` scripts within it will be executed in alphabetical order.
-
-        :param name: File or directory within project's `sql` directory
-        """
-        await self._callbacks.execute_sql(self, name, *args, **kwargs)
-
-    async def execute_sql_query(self, name: str, *args: Any) -> Any:
-        """Executes SQL query with given name
-
-        :param name: SQL query name within `<project>/sql` directory
-        """
-        return await self._callbacks.execute_sql_query(self, name, *args)
+    # TODO: The next four properties are process-global. Document later.
+    @property
+    def env(self) -> ModuleType:
+        return env
+
+    @property
+    def caches(self) -> _CacheManager:
+        return caches
+
+    @property
+    def metrics(self) -> _MetricManager:
+        return metrics
+
+    @property
+    def queues(self) -> _QueueManager:
+        return queues
 
     async def restart(self) -> None:
         """Restart process and continue indexing."""
         os.execl(sys.executable, sys.executable, *sys.argv)
 
     async def reindex(
         self,
@@ -195,15 +173,15 @@
             context['message'] = reason
             reason = ReindexingReason.manual
 
         action = self.config.advanced.reindex.get(reason, ReindexingAction.exception)
         self.logger.warning('Reindexing requested: reason `%s`, action `%s`', reason.value, action.value)
 
         if action == ReindexingAction.ignore:
-            # NOTE: Recalculate hashes on the next run
+            # NOTE: Recalculate hashes on the next _hooks_loop
             if reason == ReindexingReason.schema_modified:
                 await Schema.filter(name=self.config.schema_name).update(hash='')
             elif reason == ReindexingReason.config_modified:
                 await Index.filter().update(config_hash='')
             return
 
         elif action == ReindexingAction.exception:
@@ -211,42 +189,42 @@
             if not schema.reindex:
                 schema.reindex = reason
                 await schema.save()
             raise ReindexingRequiredError(schema.reindex, context)
 
         elif action == ReindexingAction.wipe:
             conn = get_connection()
-            if isinstance(self.config.database, PostgresDatabaseConfig):
-                await wipe_schema(
-                    conn=conn,
-                    schema_name=self.config.database.schema_name,
-                    immune_tables=self.config.database.immune_tables,
-                )
-            else:
-                await Tortoise._drop_databases()
+            immune_tables = self.config.database.immune_tables | {'dipdup_meta'}
+            await wipe_schema(
+                conn=conn,
+                schema_name=self.config.database.schema_name,
+                immune_tables=immune_tables,
+            )
             await self.restart()
 
         else:
             raise NotImplementedError
 
     async def add_contract(
         self,
+        kind: Literal['tezos'] | Literal['evm'],
         name: str,
         address: str | None = None,
         typename: str | None = None,
         code_hash: str | int | None = None,
     ) -> None:
         """Adds contract to the inventory.
 
         :param name: Contract name
         :param address: Contract address
         :param typename: Alias for the contract script
         :param code_hash: Contract code hash
+        :param kind: Either 'tezos' or 'evm' allowed
         """
-        self.logger.info('Creating contract `%s` with typename `%s`', name, typename)
+        self.logger.info('Creating %s contract `%s` with typename `%s`', kind, name, typename)
         addresses, code_hashes = self.config._contract_addresses, self.config._contract_code_hashes
 
         if name in self.config.contracts:
             raise ContractAlreadyExistsError(name)
 
         if address:
             if address in addresses:
@@ -254,33 +232,43 @@
             addresses[address] = name
 
         if code_hash:
             if code_hash in self.config._contract_code_hashes:
                 raise ContractAlreadyExistsError(code_hashes[code_hash])
             code_hashes[code_hash] = name
 
-        contract_config = ContractConfig(
-            address=address,
-            code_hash=code_hash,
-            typename=typename,
-        )
+        contract_config: ContractConfigU
+        if kind == 'tezos':
+            contract_config = TezosContractConfig(
+                kind=kind,
+                address=address,
+                code_hash=code_hash,
+                typename=typename,
+            )
+        elif kind == 'evm':
+            contract_config = EvmContractConfig(
+                kind=kind,
+                address=address,
+                typename=typename,
+            )
+        else:
+            raise NotImplementedError(kind)
+
         contract_config._name = name
         self.config.contracts[name] = contract_config
-
-        # FIXME: No `code_hash` field in the database
-        if code_hash:
-            joined_address: str | None = f'{address or ""}:{code_hash or ""}'
-        else:
-            joined_address = address
+        if isinstance(contract_config, TezosContractConfig):
+            code_hash = contract_config.code_hash
 
         with suppress(OperationalError):
             await Contract(
                 name=contract_config.name,
-                address=joined_address,
+                address=contract_config.address,
                 typename=contract_config.typename,
+                code_hash=code_hash,
+                kind=kind,
             ).save()
 
     async def add_index(
         self,
         name: str,
         template: str,
         values: dict[str, Any],
@@ -295,96 +283,113 @@
         :param values: Mapping of values to fill template with
         """
         self.config.add_index(name, template, values, first_level, last_level)
         await self._spawn_index(name, state)
 
     async def _spawn_index(self, name: str, state: Index | None = None) -> None:
         # NOTE: Avoiding circular import
-        from dipdup.indexes.big_map.index import BigMapIndex
-        from dipdup.indexes.event.index import EventIndex
-        from dipdup.indexes.head.index import HeadIndex
-        from dipdup.indexes.operation.index import OperationIndex
-        from dipdup.indexes.token_transfer.index import TokenTransferIndex
+        from dipdup.config.evm_node import EvmNodeDatasourceConfig
+        from dipdup.indexes.evm_subsquid_events.index import SubsquidEventsIndex
+        from dipdup.indexes.evm_subsquid_operations.index import SubsquidOperationsIndex
+        from dipdup.indexes.tezos_tzkt_big_maps.index import TzktBigMapsIndex
+        from dipdup.indexes.tezos_tzkt_events.index import TzktEventsIndex
+        from dipdup.indexes.tezos_tzkt_head.index import TzktHeadIndex
+        from dipdup.indexes.tezos_tzkt_operations.index import TzktOperationsIndex
+        from dipdup.indexes.tezos_tzkt_token_transfers.index import TzktTokenTransfersIndex
 
         index_config = cast(ResolvedIndexConfigU, self.config.get_index(name))
-        index: OperationIndex | BigMapIndex | HeadIndex | TokenTransferIndex | EventIndex
+        index: TzktOperationsIndex | TzktBigMapsIndex | TzktHeadIndex | TzktTokenTransfersIndex | TzktEventsIndex | SubsquidOperationsIndex | SubsquidEventsIndex
 
         datasource_name = index_config.datasource.name
-        datasource = self.get_tzkt_datasource(datasource_name)
+        datasource: TzktDatasource | SubsquidDatasource
+        node_configs: tuple[EvmNodeDatasourceConfig, ...] = ()
 
-        if isinstance(index_config, (OperationIndexConfig, OperationUnfilteredIndexConfig)):
-            index = OperationIndex(self, index_config, datasource)
-        elif isinstance(index_config, BigMapIndexConfig):
-            index = BigMapIndex(self, index_config, datasource)
-        elif isinstance(index_config, HeadIndexConfig):
-            index = HeadIndex(self, index_config, datasource)
-        elif isinstance(index_config, TokenTransferIndexConfig):
-            index = TokenTransferIndex(self, index_config, datasource)
-        elif isinstance(index_config, EventIndexConfig):
-            index = EventIndex(self, index_config, datasource)
+        if isinstance(index_config, (TzktOperationsIndexConfig, TzktOperationsUnfilteredIndexConfig)):
+            datasource = self.get_tzkt_datasource(datasource_name)
+            index = TzktOperationsIndex(self, index_config, datasource)
+        elif isinstance(index_config, TzktBigMapsIndexConfig):
+            datasource = self.get_tzkt_datasource(datasource_name)
+            index = TzktBigMapsIndex(self, index_config, datasource)
+        elif isinstance(index_config, TzktHeadIndexConfig):
+            datasource = self.get_tzkt_datasource(datasource_name)
+            index = TzktHeadIndex(self, index_config, datasource)
+        elif isinstance(index_config, TzktTokenTransfersIndexConfig):
+            datasource = self.get_tzkt_datasource(datasource_name)
+            index = TzktTokenTransfersIndex(self, index_config, datasource)
+        elif isinstance(index_config, TzktEventsIndexConfig):
+            datasource = self.get_tzkt_datasource(datasource_name)
+            index = TzktEventsIndex(self, index_config, datasource)
+        elif isinstance(index_config, SubsquidEventsIndexConfig):
+            datasource = self.get_subsquid_datasource(datasource_name)
+            node_field = index_config.datasource.node
+            if node_field:
+                node_configs = node_configs + node_field if isinstance(node_field, tuple) else (node_field,)
+            index = SubsquidEventsIndex(self, index_config, datasource)
+        elif isinstance(index_config, SubsquidOperationsIndexConfig):
+            raise NotImplementedError
         else:
             raise NotImplementedError
 
-        await datasource.add_index(index_config)
+        datasource.add_index(index_config)
+        for node_config in node_configs:
+            node_datasource = self.get_evm_node_datasource(node_config.name)
+            node_datasource.add_index(index_config)
+
         handlers = (
             (index_config.handler_config,)
-            if isinstance(index_config, OperationUnfilteredIndexConfig)
+            if isinstance(index_config, (TzktOperationsUnfilteredIndexConfig, TzktHeadIndexConfig))
             else index_config.handlers
         )
         for handler_config in handlers:
-            self._callbacks.register_handler(handler_config)
+            self.register_handler(handler_config)
         await index.initialize_state(state)
 
         # NOTE: IndexDispatcher will handle further initialization when it's time
-        pending_indexes.append(index)
+        self._pending_indexes.append(index)
 
     # TODO: disable_index(name: str)
 
     async def update_contract_metadata(
         self,
         network: str,
         address: str,
-        metadata: dict[str, Any],
+        metadata: dict[str, Any] | None,
     ) -> None:
         """
         Inserts or updates corresponding rows in the internal `dipdup_contract_metadata` table
         to provide a generic metadata interface (see docs).
 
         :param network: Network name (e.g. `mainnet`)
         :param address: Contract address
         :param metadata: Contract metadata to insert/update
         """
-        if not self.config.advanced.metadata_interface:
-            return
         update_id = MetadataCursor.contract()
         await ContractMetadata.update_or_create(
             network=network,
             contract=address,
             defaults={'metadata': metadata, 'update_id': update_id},
         )
 
     async def update_token_metadata(
         self,
         network: str,
         address: str,
         token_id: str,
-        metadata: dict[str, Any],
+        metadata: dict[str, Any] | None,
     ) -> None:
         """
         Inserts or updates corresponding rows in the internal `dipdup_token_metadata` table
         to provide a generic metadata interface (see docs).
 
         :param network: Network name (e.g. `mainnet`)
         :param address: Contract address
         :param token_id: Token ID
         :param metadata: Token metadata to insert/update
         """
 
-        if not self.config.advanced.metadata_interface:
-            return
         if not all(str.isdigit(c) for c in token_id):
             raise ValueError('`token_id` must be a number')
 
         update_id = MetadataCursor.token()
         await TokenMetadata.update_or_create(
             network=network,
             contract=address,
@@ -393,279 +398,212 @@
         )
 
     def _get_datasource(self, name: str, type_: type[DatasourceT]) -> DatasourceT:
         datasource = self.datasources.get(name)
         if not datasource:
             raise ConfigurationError(f'Datasource `{name}` is missing')
         if not isinstance(datasource, type_):
-            raise ConfigurationError(f'Datasource `{name}` is not a `{type.__name__}`')
+            raise ConfigurationError(f'Datasource `{name}` is not a `{type_.__name__}`')
         return datasource
 
     def get_tzkt_datasource(self, name: str) -> TzktDatasource:
-        """Get `tzkt` datasource by name"""
+        """Get `tezos.tzkt` datasource by name"""
         return self._get_datasource(name, TzktDatasource)
 
+    def get_subsquid_datasource(self, name: str) -> SubsquidDatasource:
+        """Get `evm.subsquid` datasource by name"""
+        return self._get_datasource(name, SubsquidDatasource)
+
+    def get_evm_node_datasource(self, name: str) -> EvmNodeDatasource:
+        """Get `evm.node` datasource by name or by linked `evm.subsquid` datasource name"""
+        with suppress(ConfigurationError):
+            return self._get_datasource(name, EvmNodeDatasource)
+        with suppress(ConfigurationError):
+            subsquid = self._get_datasource(name, SubsquidDatasource)
+            # NOTE: Multiple nodes can be linked to a single subsquid. Network is the same, so grab any.
+            random_node = subsquid._config.random_node
+            if random_node is None:
+                raise ConfigurationError(f'No `evm.node` datasources linked to `{name}`')
+            return self._get_datasource(random_node.name, EvmNodeDatasource)
+        raise ConfigurationError(f'`{name}` datasource is neither `evm.node` nor `evm.subsquid`')
+
     def get_coinbase_datasource(self, name: str) -> CoinbaseDatasource:
         """Get `coinbase` datasource by name"""
         return self._get_datasource(name, CoinbaseDatasource)
 
-    def get_metadata_datasource(self, name: str) -> MetadataDatasource:
+    def get_metadata_datasource(self, name: str) -> TzipMetadataDatasource:
         """Get `metadata` datasource by name"""
-        return self._get_datasource(name, MetadataDatasource)
+        return self._get_datasource(name, TzipMetadataDatasource)
 
     def get_ipfs_datasource(self, name: str) -> IpfsDatasource:
         """Get `ipfs` datasource by name"""
         return self._get_datasource(name, IpfsDatasource)
 
     def get_http_datasource(self, name: str) -> HttpDatasource:
         """Get `http` datasource by name"""
         return self._get_datasource(name, HttpDatasource)
 
-
-class HookContext(DipDupContext):
-    """Execution context of hook callbacks.
-
-    :param hook_config: Configuration of the current hook
-    """
-
-    def __init__(
-        self,
-        datasources: dict[str, Datasource],
-        config: DipDupConfig,
-        callbacks: 'CallbackManager',
-        transactions: TransactionManager,
-        logger: FormattedLogger,
-        hook_config: HookConfig,
-    ) -> None:
-        super().__init__(datasources, config, callbacks, transactions)
-        self.logger = logger
-        self.hook_config = hook_config
-
-    @classmethod
-    def _wrap(
-        cls,
-        ctx: DipDupContext,
-        logger: FormattedLogger,
-        hook_config: HookConfig,
-    ) -> 'HookContext':
-        return cls(
-            datasources=ctx.datasources,
-            config=ctx.config,
-            callbacks=ctx._callbacks,
-            transactions=ctx._transactions,
-            logger=logger,
-            hook_config=hook_config,
-        )
-
     async def rollback(self, index: str, from_level: int, to_level: int) -> None:
         """Rollback index to a given level reverting all changes made since that level.
 
         :param index: Index name
         :param from_level: Level to rollback from
         :param to_level: Level to rollback to
         """
         self.logger.info('Rolling back `%s`: %s -> %s', index, from_level, to_level)
         if from_level <= to_level:
             raise FrameworkException(f'Attempt to rollback in future: {from_level} <= {to_level}')
-        if from_level - to_level > self.config.advanced.rollback_depth:
+
+        rollback_depth = self.config.advanced.rollback_depth
+        if rollback_depth is None:
+            raise FrameworkException('`rollback_depth` is not set')
+        if from_level - to_level > rollback_depth:
             # TODO: Need more context
             await self.reindex(ReindexingReason.rollback)
 
         models = importlib.import_module(f'{self.config.package}.models')
-        async with self._transactions.in_transaction():
+        async with self.transactions.in_transaction():
             updates = await ModelUpdate.filter(
                 level__lte=from_level,
                 level__gt=to_level,
                 index=index,
             ).order_by('-id')
 
             if updates:
                 self.logger.info(f'Reverting {len(updates)} updates')
             for update in updates:
                 model = getattr(models, update.model_name)
                 await update.revert(model)
 
         await Index.filter(name=index).update(level=to_level)
-        rolled_back_indexes.add(index)
-
-
-class TemplateValuesdict(dict[str, Any]):
-    """dictionary with template values."""
-
-    def __init__(self, ctx: Any, **kwargs: Any) -> None:
-        self.ctx = ctx
-        super().__init__(**kwargs)
-
-    def __getitem__(self, key: str) -> Any:
-        try:
-            return dict.__getitem__(self, key)
-        except KeyError as e:
-            raise ConfigurationError(
-                f'Index `{self.ctx.index_config.name}` requires `{key}` template value to be set'
-            ) from e
-
-
-class HandlerContext(DipDupContext):
-    """Execution context of handler callbacks.
-
-    :param handler_config: Configuration of the current handler
-    :param datasource: Index datasource instance
-    """
-
-    def __init__(
-        self,
-        datasources: dict[str, Datasource],
-        config: DipDupConfig,
-        callbacks: 'CallbackManager',
-        transactions: TransactionManager,
-        logger: FormattedLogger,
-        handler_config: HandlerConfig,
-        datasource: TzktDatasource,
-    ) -> None:
-        super().__init__(datasources, config, callbacks, transactions)
-        self.logger = logger
-        self.handler_config = handler_config
-        self.datasource = datasource
-        template_values = handler_config.parent.template_values if handler_config.parent else {}
-        self.template_values = TemplateValuesdict(self, **template_values)
-
-    @classmethod
-    def _wrap(
-        cls,
-        ctx: DipDupContext,
-        logger: FormattedLogger,
-        handler_config: HandlerConfig,
-        datasource: TzktDatasource,
-    ) -> 'HandlerContext':
-        return cls(
-            datasources=ctx.datasources,
-            config=ctx.config,
-            callbacks=ctx._callbacks,
-            transactions=ctx._transactions,
-            logger=logger,
-            handler_config=handler_config,
-            datasource=datasource,
-        )
-
-
-class CallbackManager:
-    def __init__(self, package: str) -> None:
-        self._logger = logging.getLogger('dipdup.callback')
-        self._package = package
-        self._handlers: dict[tuple[str, str], HandlerConfig] = {}
-        self._hooks: dict[str, HookConfig] = {}
+        self._rolled_back_indexes.add(index)
 
-    async def run(self) -> None:
-        self._logger.debug('Starting CallbackManager loop')
+    # TODO: Use DipDupPackage for some parts below
+    async def _hooks_loop(self) -> None:
+        self.logger.debug('Starting CallbackManager loop')
         while True:
-            while pending_hooks:
-                await pending_hooks.popleft()
+            while self._pending_hooks:
+                await self._pending_hooks.popleft()
             # TODO: Replace with asyncio.Event
             await asyncio.sleep(1)
 
     def register_handler(self, handler_config: HandlerConfig) -> None:
         if not handler_config.parent:
             raise FrameworkException('Handler must have a parent index')
 
         # NOTE: Same handlers can be linked to different indexes, we need to use exact config
         key = (handler_config.callback, handler_config.parent.name)
         if key not in self._handlers:
             self._handlers[key] = handler_config
-            handler_config.initialize_callback_fn(self._package)
 
     def register_hook(self, hook_config: HookConfig) -> None:
         key = hook_config.callback
         if key not in self._hooks:
             self._hooks[key] = hook_config
-            hook_config.initialize_callback_fn(self._package)
 
-    async def _fire_handler(
+    async def fire_handler(
         self,
-        ctx: 'DipDupContext',
         name: str,
         index: str,
-        datasource: TzktDatasource,
+        datasource: IndexDatasource[Any],
         fmt: str | None = None,
         *args: Any,
         **kwargs: Any,
     ) -> None:
-        module = f'{self._package}.handlers.{name}'
+        """Fire handler with given name and arguments.
+
+        :param name: Handler name
+        :param index: Index name
+        :param datasource: An instance of datasource that triggered the handler
+        :param fmt: Format string for `ctx.logger` messages
+        """
+        module = f'{self.package.name}.handlers.{name}'
         handler_config = self._get_handler(name, index)
         new_ctx = HandlerContext._wrap(
-            ctx,
+            self,
             logger=FormattedLogger(module, fmt),
             handler_config=handler_config,
             datasource=datasource,
         )
         # NOTE: Handlers are not atomic, levels are. Do not open transaction here.
         with self._callback_wrapper(module):
-            await handler_config.callback_fn(new_ctx, *args, **kwargs)
+            fn = self.package.get_callback('handlers', name, name.split('.')[-1])
+            await fn(new_ctx, *args, **kwargs)
 
     async def fire_hook(
         self,
-        ctx: 'DipDupContext',
         name: str,
         fmt: str | None = None,
         wait: bool = True,
         *args: Any,
         **kwargs: Any,
     ) -> None:
-        module = f'{self._package}.hooks.{name}'
-        hook_config = self._get_hook(name)
+        """Fire hook with given name and arguments.
 
-        if isinstance(hook_config, EventHookConfig):
-            if isinstance(ctx, (HandlerContext, HookContext)):
-                raise FrameworkException('Event hooks cannot be fired manually')
+        :param name: Hook name
+        :param fmt: Format string for `ctx.logger` messages
+        :param wait: Wait for hook to finish or fire and forget
+        :param args: Positional arguments to pass to the hook
+        :param kwargs: Keyword arguments to pass to the hook
+        """
+        module = f'{self.package.name}.hooks.{name}'
+        hook_config = self._get_hook(name)
 
         new_ctx = HookContext._wrap(
-            ctx,
+            self,
             logger=FormattedLogger(module, fmt),
             hook_config=hook_config,
         )
 
-        self._verify_arguments(new_ctx, *args, **kwargs)
-
         async def _wrapper() -> None:
             async with AsyncExitStack() as stack:
                 stack.enter_context(self._callback_wrapper(module))
                 if hook_config.atomic:
                     # NOTE: Do not use versioned transactions here
-                    await stack.enter_async_context(new_ctx._transactions.in_transaction())
+                    await stack.enter_async_context(new_ctx.transactions.in_transaction())
 
-                await hook_config.callback_fn(new_ctx, *args, **kwargs)
+                fn = self.package.get_callback('hooks', name, name)
+                await fn(new_ctx, *args, **kwargs)
 
-        if wait:
-            await _wrapper()
-        else:
-            pending_hooks.append(_wrapper())
+        coro = _wrapper()
+        await coro if wait else self._pending_hooks.append(coro)
 
     async def execute_sql(
         self,
-        ctx: 'DipDupContext',
         name: str,
         *args: Any,
         **kwargs: Any,
     ) -> None:
-        """Execute SQL script included with the project"""
+        """Executes SQL script(s) with given name.
+
+        If the `name` path is a directory, all `.sql` scripts within it will be executed in alphabetical order.
+
+        :param name: File or directory within project's `sql` directory
+        :param args: Positional arguments to pass to the script
+        :param kwargs: Keyword arguments to pass to the script
+        """
         # NOTE: Modified `package_path` breaks SQL discovery.
         if env.TEST:
             return
 
-        sql_path = self._get_sql_path(ctx, name)
+        sql_path = self._get_sql_path(name)
         conn = get_connection()
         await execute_sql(conn, sql_path, *args, **kwargs)
 
     async def execute_sql_query(
         self,
-        ctx: 'DipDupContext',
         name: str,
         *values: Any,
     ) -> Any:
-        """Execute SQL query included with the project"""
-        sql_path = self._get_sql_path(ctx, name)
+        """Executes SQL query with given name included with the project
+
+        :param name: SQL query name within `sql` directory
+        """
+
+        sql_path = self._get_sql_path(name)
         conn = get_connection()
         return await execute_sql_query(conn, sql_path, *values)
 
     @contextmanager
     def _callback_wrapper(self, module: str) -> Iterator[None]:
         with ExitStack() as stack:
             try:
@@ -674,44 +612,129 @@
                 yield
             # NOTE: Do not wrap known errors like ProjectImportError
             except FrameworkException:
                 raise
             except Exception as e:
                 raise CallbackError(module, e) from e
 
-    # FIXME: kwargs are ignored, no false alarms though
-    @classmethod
-    def _verify_arguments(cls, ctx: HookContext, *args: Any, **kwargs: Any) -> None:
-        kwargs_annotations = ctx.hook_config.locate_arguments()
-        args_names = tuple(kwargs_annotations.keys())
-        args_annotations = tuple(kwargs_annotations.values())
-
-        for i, arg in enumerate(args):
-            expected_type = args_annotations[i]
-            if expected_type and not isinstance(arg, expected_type):
-                raise CallbackTypeError(
-                    name=ctx.hook_config.callback,
-                    kind='hook',
-                    arg=args_names[i],
-                    type_=type(arg),
-                    expected_type=expected_type,
-                )
-
     def _get_handler(self, name: str, index: str) -> HandlerConfig:
         try:
             return self._handlers[(name, index)]
         except KeyError as e:
             raise ConfigurationError(f'Attempt to fire unregistered handler `{name}` of index `{index}`') from e
 
     def _get_hook(self, name: str) -> HookConfig:
         try:
             return self._hooks[name]
         except KeyError as e:
             raise ConfigurationError(f'Attempt to fire unregistered hook `{name}`') from e
 
-    def _get_sql_path(self, ctx: 'DipDupContext', name: str) -> Path:
+    def _get_sql_path(self, name: str) -> Path:
         subpackages = name.split('.')
-        sql_path = Path(env.get_package_path(ctx.config.package), 'sql', *subpackages)
+        sql_path = Path(env.get_package_path(self.config.package), 'sql', *subpackages)
         if not sql_path.exists():
             raise InitializationRequiredError(f'Missing SQL directory for hook `{name}`')
 
         return sql_path
+
+
+class HookContext(DipDupContext):
+    """Execution context of hook callbacks.
+
+    :param hook_config: Configuration of the current hook
+    """
+
+    def __init__(
+        self,
+        config: DipDupConfig,
+        package: DipDupPackage,
+        datasources: dict[str, Datasource[Any]],
+        transactions: TransactionManager,
+        logger: FormattedLogger,
+        hook_config: HookConfig,
+    ) -> None:
+        super().__init__(
+            config=config,
+            package=package,
+            datasources=datasources,
+            transactions=transactions,
+        )
+        self.logger = logger
+        self.hook_config = hook_config
+
+    @classmethod
+    def _wrap(
+        cls,
+        ctx: DipDupContext,
+        logger: FormattedLogger,
+        hook_config: HookConfig,
+    ) -> 'HookContext':
+        return cls(
+            config=ctx.config,
+            package=ctx.package,
+            datasources=ctx.datasources,
+            transactions=ctx.transactions,
+            logger=logger,
+            hook_config=hook_config,
+        )
+
+
+class _TemplateValues(dict[str, Any]):
+    def __init__(self, index: str, values: Any) -> None:
+        self._index = index
+        super().__init__(values)
+
+    def __getitem__(self, key: str) -> Any:
+        try:
+            return dict.__getitem__(self, key)
+        except KeyError as e:
+            raise ConfigurationError(f'Index `{self._index}` requires `{key}` template value to be set') from e
+
+
+class HandlerContext(DipDupContext):
+    """Execution context of handler callbacks.
+
+    :param handler_config: Configuration of the current handler
+    :param datasource: Index datasource instance
+    """
+
+    def __init__(
+        self,
+        config: DipDupConfig,
+        package: DipDupPackage,
+        datasources: dict[str, Datasource[Any]],
+        transactions: TransactionManager,
+        logger: FormattedLogger,
+        handler_config: HandlerConfig,
+        datasource: IndexDatasource[Any],
+    ) -> None:
+        super().__init__(
+            config=config,
+            package=package,
+            datasources=datasources,
+            transactions=transactions,
+        )
+        self.logger = logger
+        self.handler_config = handler_config
+        self.datasource = datasource
+        self.template_values = _TemplateValues(
+            handler_config.parent.name if handler_config.parent else 'unknown',
+            handler_config.parent.template_values if handler_config.parent else {},
+        )
+
+    @classmethod
+    def _wrap(
+        cls,
+        ctx: DipDupContext,
+        logger: FormattedLogger,
+        handler_config: HandlerConfig,
+        datasource: IndexDatasource[Any],
+    ) -> 'HandlerContext':
+        return cls(
+            config=ctx.config,
+            package=ctx.package,
+            datasources=ctx.datasources,
+            transactions=ctx.transactions,
+            logger=logger,
+            handler_config=handler_config,
+            datasource=datasource,
+        )
```

### Comparing `dipdup-6.5.9/src/dipdup/datasources/coinbase/datasource.py` & `dipdup-7.0.0rc1/src/dipdup/datasources/coinbase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import logging
 from datetime import datetime
 from datetime import timedelta
 from datetime import timezone
 from typing import Any
 from typing import cast
 
-from dipdup.config import HTTPConfig
-from dipdup.datasources.coinbase.models import CandleData
-from dipdup.datasources.coinbase.models import CandleInterval
-from dipdup.datasources.datasource import Datasource
+from dipdup.config import HttpConfig
+from dipdup.config.coinbase import CoinbaseDatasourceConfig
+from dipdup.datasources import Datasource
+from dipdup.models.coinbase import CandleData
+from dipdup.models.coinbase import CandleInterval
 
 CANDLES_REQUEST_LIMIT = 300
 API_URL = 'https://api.pro.coinbase.com'
 
 
-class CoinbaseDatasource(Datasource):
-    _default_http_config = HTTPConfig(
+class CoinbaseDatasource(Datasource[CoinbaseDatasourceConfig]):
+    _default_http_config = HttpConfig(
         retry_sleep=1,
         retry_multiplier=1.1,
         ratelimit_rate=10,
         ratelimit_period=1,
     )
 
-    def __init__(self, url: str = API_URL, http_config: HTTPConfig | None = None) -> None:
-        super().__init__(url, http_config)
-        self._logger = logging.getLogger('dipdup.coinbase')
-
     async def run(self) -> None:
         pass
 
     async def get_oracle_prices(self) -> dict[str, Any]:
         return cast(
             dict[str, Any],
             await self.request(
                 'get',
                 url='oracle',
             ),
         )
 
     async def get_candles(
-        self, since: datetime, until: datetime, interval: CandleInterval, ticker: str = 'XTZ-USD'
+        self,
+        since: datetime,
+        until: datetime,
+        interval: CandleInterval,
+        ticker: str,
     ) -> list[CandleData]:
         candles = []
         for _since, _until in self._split_candle_requests(since, until, interval):
             candles_json = await self.request(
                 'get',
                 url=f'products/{ticker}/candles',
                 params={
@@ -52,15 +52,18 @@
                     'granularity': interval.seconds,
                 },
             )
             candles += [CandleData.from_json(c) for c in candles_json]
         return sorted(candles, key=lambda c: c.timestamp)
 
     def _split_candle_requests(
-        self, since: datetime, until: datetime, interval: CandleInterval
+        self,
+        since: datetime,
+        until: datetime,
+        interval: CandleInterval,
     ) -> list[tuple[datetime, datetime]]:
         request_interval_limit = timedelta(seconds=interval.seconds * CANDLES_REQUEST_LIMIT)
         request_intervals = []
         while since + request_interval_limit < until:
             request_intervals.append((since, since + request_interval_limit))
             since += request_interval_limit
         request_intervals.append((since, until))
```

### Comparing `dipdup-6.5.9/src/dipdup/datasources/coinbase/models.py` & `dipdup-7.0.0rc1/src/dipdup/models/coinbase.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.9/src/dipdup/datasources/metadata/datasource.py` & `dipdup-7.0.0rc1/src/dipdup/datasources/tzip_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,44 @@
-import logging
 from typing import Any
 from typing import cast
 
-from dipdup.config import HTTPConfig
-from dipdup.datasources.datasource import GraphQLDatasource
-from dipdup.datasources.metadata.enums import MetadataNetwork
+from dipdup.config import HttpConfig
+from dipdup.config.tzip_metadata import TzipMetadataDatasourceConfig
+from dipdup.datasources import Datasource
 
 
-class MetadataDatasource(GraphQLDatasource):
-    _default_http_config = HTTPConfig(
+class TzipMetadataDatasource(Datasource[TzipMetadataDatasourceConfig]):
+    _default_http_config = HttpConfig(
         retry_sleep=1,
         retry_multiplier=1.1,
         retry_count=10,
         ratelimit_rate=10,
         ratelimit_period=1,
     )
 
-    def __init__(self, url: str, network: MetadataNetwork, http_config: HTTPConfig | None = None) -> None:
-        super().__init__(url, http_config)
-        self._logger = logging.getLogger('dipdup.metadata')
-        self._network = network
-
     async def get_contract_metadata(self, address: str) -> dict[str, Any] | None:
         response = await self.request(
             'get',
             url='api/rest/contract_metadata',
             params={
-                'network': self._network.value,
+                'network': self._config.network.value,
                 'contract': address,
             },
         )
         response = response['contract_metadata']
         if response:
             return cast(dict[str, Any], response[0]['metadata'])
         return None
 
     async def get_token_metadata(self, address: str, token_id: int) -> dict[str, Any] | None:
         response = await self.request(
             'get',
             url='api/rest/token_metadata',
             params={
-                'network': self._network.value,
+                'network': self._config.network.value,
                 'contract': address,
                 'token_id': token_id,
             },
         )
         response = response['token_metadata']
         if response:
             return cast(
```

### Comparing `dipdup-6.5.9/src/dipdup/datasources/subscription.py` & `dipdup-7.0.0rc1/src/dipdup/subscriptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 import logging
-from abc import abstractmethod
-from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Set
 
 from dipdup.exceptions import FrameworkException
 
-_logger = logging.getLogger('dipdup.datasource')
+_logger = logging.getLogger(__name__)
 
 
 class Subscription:
-    type: str
-    method: str
-
-    @abstractmethod
-    def get_request(self) -> Any:
-        ...
+    pass
 
 
 class SubscriptionManager:
     def __init__(self, merge_subscriptions: bool = False) -> None:
         self._merge_subscriptions: bool = merge_subscriptions
         self._subscriptions: Dict[Optional[Subscription], Optional[int]] = {None: None}
 
@@ -41,19 +34,24 @@
     def reset(self) -> None:
         self._subscriptions = dict.fromkeys(self._subscriptions, None)
 
     def set_sync_level(self, subscription: Optional[Subscription], level: int) -> None:
         if subscription not in self._subscriptions:
             raise FrameworkException(f'Subscription does not exist: {subscription}')
 
+        if subscription is None:
+            for sub in self._subscriptions:
+                self._subscriptions[sub] = level
+            return
+
         if self._subscriptions[subscription]:
             # NOTE: Updating sync level with merge_subscriptions=True will cause resync
             if self._merge_subscriptions:
                 return
-            _logger.warning('%s sync level updated: %s -> %s', subscription, self._subscriptions[subscription], level)
+            _logger.debug('%s sync level updated: %s -> %s', subscription, self._subscriptions[subscription], level)
 
         self._subscriptions[subscription] = level
 
     def get_sync_level(self, subscription: Subscription) -> Optional[int]:
         if subscription not in self._subscriptions:
             raise FrameworkException(f'Subscription does not exist: {subscription}')
         return self._subscriptions[subscription] or self._subscriptions[None]
```

### Comparing `dipdup-6.5.9/src/dipdup/datasources/tzkt/datasource.py` & `dipdup-7.0.0rc1/src/dipdup/datasources/tezos_tzkt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import asyncio
 import logging
-from abc import ABC
-from abc import abstractmethod
 from asyncio import Event
 from collections import defaultdict
 from collections import deque
-from datetime import datetime
-from datetime import timezone
-from decimal import Decimal
+from dataclasses import fields
 from enum import Enum
 from functools import partial
 from typing import Any
 from typing import AsyncIterator
 from typing import Awaitable
 from typing import Callable
 from typing import Generator
@@ -20,32 +16,32 @@
 from typing import Sequence
 from typing import cast
 
 import pysignalr.exceptions
 from pysignalr.client import SignalRClient
 from pysignalr.messages import CompletionMessage
 
-from dipdup import baking_bad
-from dipdup.config import HTTPConfig
-from dipdup.config import ResolvedIndexConfigU
-from dipdup.datasources.datasource import IndexDatasource
-from dipdup.datasources.subscription import Subscription
-from dipdup.datasources.tzkt.models import HeadSubscription
-from dipdup.enums import MessageType
-from dipdup.enums import TokenStandard
+from dipdup.config import HttpConfig
+from dipdup.config.tezos_tzkt import TZKT_API_URLS
+from dipdup.config.tezos_tzkt import TzktDatasourceConfig
+from dipdup.datasources import IndexDatasource
 from dipdup.exceptions import DatasourceError
 from dipdup.exceptions import FrameworkException
-from dipdup.models import BigMapAction
-from dipdup.models import BigMapData
-from dipdup.models import BlockData
-from dipdup.models import EventData
-from dipdup.models import HeadBlockData
-from dipdup.models import OperationData
-from dipdup.models import QuoteData
-from dipdup.models import TokenTransferData
+from dipdup.models import Head
+from dipdup.models import MessageType
+from dipdup.models.tezos_tzkt import HeadSubscription
+from dipdup.models.tezos_tzkt import TzktBigMapData
+from dipdup.models.tezos_tzkt import TzktBlockData
+from dipdup.models.tezos_tzkt import TzktEventData
+from dipdup.models.tezos_tzkt import TzktHeadBlockData
+from dipdup.models.tezos_tzkt import TzktMessageType
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktQuoteData
+from dipdup.models.tezos_tzkt import TzktSubscription
+from dipdup.models.tezos_tzkt import TzktTokenTransferData
 from dipdup.utils import FormattedLogger
 from dipdup.utils import split_by_chunks
 
 ORIGINATION_REQUEST_LIMIT = 100
 OPERATION_FIELDS = (
     'type',
     'id',
@@ -80,27 +76,63 @@
     'originatedContract',
 )
 TRANSACTION_OPERATION_FIELDS = (
     *OPERATION_FIELDS,
     'parameter',
     'hasInternals',
 )
+BIGMAP_FIELDS = (
+    'ptr',
+    'contract',
+    'path',
+    'tags',
+    'active',
+    'firstLevel',
+    'lastLevel',
+    'totalKeys',
+    'activeKeys',
+    'updates',
+    'keyType',
+    'valueType',
+)
+TZKT_TOKEN_TRANSFER_DATA_FIELDS = (
+    'token',
+    'from',
+    'to',
+    'id',
+    'level',
+    'timestamp',
+    'amount',
+    'transactionId',
+    'originationId',
+    'migrationId',
+)
+
 
+EmptyCallback = Callable[[], Awaitable[None]]
+HeadCallback = Callable[['TzktDatasource', TzktHeadBlockData], Awaitable[None]]
+OperationsCallback = Callable[['TzktDatasource', tuple[TzktOperationData, ...]], Awaitable[None]]
+TokenTransfersCallback = Callable[['TzktDatasource', tuple[TzktTokenTransferData, ...]], Awaitable[None]]
+BigMapsCallback = Callable[['TzktDatasource', tuple[TzktBigMapData, ...]], Awaitable[None]]
+EventsCallback = Callable[['TzktDatasource', tuple[TzktEventData, ...]], Awaitable[None]]
+# TODO: move somewhere
+RollbackCallback = Callable[['IndexDatasource', MessageType, int, int], Awaitable[None]]
 
-class TzktMessageType(Enum):
+
+class TzktMessageAction(Enum):
     STATE = 0
     DATA = 1
     REORG = 2
 
 
 MessageData = dict[str, Any] | list[dict[str, Any]]
 
 
 class BufferedMessage(NamedTuple):
-    type: MessageType
+    type: TzktMessageType
     data: MessageData
 
 
 class MessageBuffer:
     """Buffers realtime TzKT messages and yields them by level.
 
     Initially, it was a mitigation for TzKT's reorgs.
@@ -110,21 +142,21 @@
         self._logger = logging.getLogger('dipdup.tzkt')
         self._size = size
         self._messages: dict[int, list[BufferedMessage]] = {}
 
     def __len__(self) -> int:
         return len(self._messages)
 
-    def add(self, type_: MessageType, level: int, data: MessageData) -> None:
+    def add(self, type_: TzktMessageType, level: int, data: MessageData) -> None:
         """Add a message to the buffer."""
         if level not in self._messages:
             self._messages[level] = []
         self._messages[level].append(BufferedMessage(type_, data))
 
-    def rollback(self, type_: MessageType, channel_level: int, message_level: int) -> bool:
+    def rollback(self, type_: TzktMessageType, channel_level: int, message_level: int) -> bool:
         """Drop buffered messages in reversed order while possible, return if successful."""
         self._logger.info('`%s` rollback requested: %s -> %s', type_.value, channel_level, message_level)
         levels = range(channel_level, message_level, -1)
         for level in levels:
             if level not in self._messages:
                 return False
 
@@ -162,88 +194,181 @@
     def get_code_hashes(self, address: str) -> tuple[int, int]:
         return self._address_to_hashes[address]
 
     def get_address(self, code_hash: int, type_hash: int) -> str:
         return self._hashes_to_address[(code_hash, type_hash)]
 
 
-class SignalRDatasource(IndexDatasource, ABC):
-    async def run(self) -> None:
-        self._logger.info('Establishing realtime connection')
-        signalr_client = self._get_signalr_client()
-        retry_sleep = self._http_config.retry_sleep
-
-        for _ in range(1, self._http_config.retry_count + 1):
-            try:
-                await signalr_client.run()
-            except pysignalr.exceptions.ConnectionError as e:
-                self._logger.error('Websocket connection error: %s', e)
-                await self.emit_disconnected()
-                await asyncio.sleep(retry_sleep)
-                retry_sleep *= self._http_config.retry_multiplier
-
-        raise DatasourceError(datasource=self.name, msg='Websocket connection failed')
-
-    @abstractmethod
-    def _get_signalr_client(self) -> SignalRClient:
-        ...
-
-
-class TzktDatasource(SignalRDatasource):
-    _default_http_config = HTTPConfig(
+class TzktDatasource(IndexDatasource[TzktDatasourceConfig]):
+    _default_http_config = HttpConfig(
         retry_sleep=1,
         retry_multiplier=1.1,
         retry_count=10,
         ratelimit_rate=100,
         ratelimit_period=1,
         connection_limit=25,
-        batch_size=1000,
+        batch_size=10_000,
     )
 
     def __init__(
         self,
-        url: str,
-        http_config: HTTPConfig | None = None,
-        merge_subscriptions: bool = False,
-        buffer_size: int = 0,
+        config: TzktDatasourceConfig,
     ) -> None:
-        super().__init__(url, http_config, merge_subscriptions)
+        super().__init__(config)
         self._logger = logging.getLogger('dipdup.tzkt')
-        self._buffer = MessageBuffer(buffer_size)
+        self._buffer = MessageBuffer(config.buffer_size)
         self._contract_hashes = ContractHashes()
 
+        self._on_connected_callbacks: set[EmptyCallback] = set()
+        self._on_disconnected_callbacks: set[EmptyCallback] = set()
+        self._on_head_callbacks: set[HeadCallback] = set()
+        self._on_operations_callbacks: set[OperationsCallback] = set()
+        self._on_token_transfers_callbacks: set[TokenTransfersCallback] = set()
+        self._on_big_maps_callbacks: set[BigMapsCallback] = set()
+        self._on_events_callbacks: set[EventsCallback] = set()
+        self._on_rollback_callbacks: set[RollbackCallback] = set()
+        self._network: str | None = None
+
         self._signalr_client: SignalRClient | None = None
-        self._channel_levels: defaultdict[MessageType, int | None] = defaultdict(lambda: None)
+        self._channel_levels: defaultdict[TzktMessageType, int | None] = defaultdict(lambda: None)
 
     async def __aenter__(self) -> None:
         try:
             await super().__aenter__()
 
             protocol = await self.request('get', 'v1/protocols/current')
             category = 'self-hosted'
-            if (instance := baking_bad.TZKT_API_URLS.get(self.url)) is not None:
+            if (instance := TZKT_API_URLS.get(self.url)) is not None:
                 category = f'hosted ({instance})'
             self._logger.info(
                 '%s, protocol v%s (%s)',
                 category,
                 protocol['code'],
                 protocol['hash'][:8] + '…' + protocol['hash'][-6:],
             )
         except Exception as e:
             raise DatasourceError(f'Failed to connect to TzKT: {e}', self.name) from e
 
     @property
+    def network(self) -> str:
+        if not self._network:
+            raise FrameworkException('Network is not set')
+        return self._network
+
+    @property
     def request_limit(self) -> int:
         return self._http_config.batch_size
 
+    # FIXME: Join retry logic with other index datasources
+    async def run(self) -> None:
+        self._logger.info('Establishing realtime connection')
+        signalr_client = self._get_signalr_client()
+        retry_sleep = self._http_config.retry_sleep
+
+        for _ in range(1, self._http_config.retry_count + 1):
+            try:
+                await signalr_client.run()
+            except pysignalr.exceptions.ConnectionError as e:
+                self._logger.error('Websocket connection error: %s', e)
+                await self.emit_disconnected()
+                await asyncio.sleep(retry_sleep)
+                retry_sleep *= self._http_config.retry_multiplier
+
+        raise DatasourceError('Websocket connection failed', self.name)
+
+    async def initialize(self) -> None:
+        head_block = await self.get_head_block()
+        self.set_network(head_block.chain)
+        self.set_sync_level(
+            subscription=None,
+            level=head_block.level,
+        )
+
+        db_head = await Head.filter(name=self.name).first()
+        if not db_head:
+            return
+
+        # FIXME: No ctx to throw reorg; VERY IMPORTANT CHECK
+        # NOTE: Ensure that no reorgs happened while we were offline
+        # actual_head = await self.get_block(db_head.level)
+        # if db_head.hash != actual_head.hash:
+        #     await self._ctx.reindex(
+        #         ReindexingReason.rollback,
+        #         datasource=self.name,
+        #         level=db_head.level,
+        #         stored_block_hash=db_head.hash,
+        #         actual_block_hash=actual_head.hash,
+        #     )
+
+    def call_on_head(self, fn: HeadCallback) -> None:
+        self._on_head_callbacks.add(fn)
+
+    def call_on_operations(self, fn: OperationsCallback) -> None:
+        self._on_operations_callbacks.add(fn)
+
+    def call_on_token_transfers(self, fn: TokenTransfersCallback) -> None:
+        self._on_token_transfers_callbacks.add(fn)
+
+    def call_on_big_maps(self, fn: BigMapsCallback) -> None:
+        self._on_big_maps_callbacks.add(fn)
+
+    def call_on_events(self, fn: EventsCallback) -> None:
+        self._on_events_callbacks.add(fn)
+
+    def call_on_rollback(self, fn: RollbackCallback) -> None:
+        self._on_rollback_callbacks.add(fn)
+
+    def call_on_connected(self, fn: EmptyCallback) -> None:
+        self._on_connected_callbacks.add(fn)
+
+    def call_on_disconnected(self, fn: EmptyCallback) -> None:
+        self._on_disconnected_callbacks.add(fn)
+
+    async def emit_head(self, head: TzktHeadBlockData) -> None:
+        for fn in self._on_head_callbacks:
+            await fn(self, head)
+
+    async def emit_operations(self, operations: tuple[TzktOperationData, ...]) -> None:
+        for fn in self._on_operations_callbacks:
+            await fn(self, operations)
+
+    async def emit_token_transfers(self, token_transfers: tuple[TzktTokenTransferData, ...]) -> None:
+        for fn in self._on_token_transfers_callbacks:
+            await fn(self, token_transfers)
+
+    async def emit_big_maps(self, big_maps: tuple[TzktBigMapData, ...]) -> None:
+        for fn in self._on_big_maps_callbacks:
+            await fn(self, big_maps)
+
+    async def emit_events(self, events: tuple[TzktEventData, ...]) -> None:
+        for fn in self._on_events_callbacks:
+            await fn(self, events)
+
+    async def emit_rollback(self, type_: MessageType, from_level: int, to_level: int) -> None:
+        for fn in self._on_rollback_callbacks:
+            await fn(self, type_, from_level, to_level)
+
+    async def emit_connected(self) -> None:
+        for fn in self._on_connected_callbacks:
+            await fn()
+
+    async def emit_disconnected(self) -> None:
+        for fn in self._on_disconnected_callbacks:
+            await fn()
+
+    def set_network(self, network: str) -> None:
+        if self._network:
+            raise FrameworkException('Network is already set')
+        self._network = network
+
     def set_logger(self, name: str) -> None:
         super().set_logger(name)
         self._buffer._logger = FormattedLogger(self._buffer._logger.name, name + ': {}')
 
-    def get_channel_level(self, message_type: MessageType) -> int:
+    def get_channel_level(self, message_type: TzktMessageType) -> int:
         """Get current level of the channel, or sync level if no messages were received yet."""
         channel_level = self._channel_levels[message_type]
         if channel_level is None:
             # NOTE: If no data messages were received since run, use sync level instead
             # NOTE: There's only one sync level for all channels, otherwise `Index.process` would fail
             channel_level = self.get_sync_level(HeadSubscription())
             if channel_level is None:
@@ -253,71 +378,80 @@
 
     async def get_similar_contracts(
         self,
         address: str,
         strict: bool = False,
         offset: int | None = None,
         limit: int | None = None,
-    ) -> tuple[str, ...]:
+    ) -> tuple[dict[str, str], ...]:
         """Get addresses of contracts that share the same code hash or type hash"""
         entrypoint = 'same' if strict else 'similar'
         self._logger.info('Fetching `%s` contracts for address `%s`', entrypoint, address)
 
         params = self._get_request_params(
             offset=offset,
             limit=limit,
-            select=('id', 'address'),
+            select=(
+                'id',
+                'address',
+            ),
+            values=True,
+            cursor=True,
         )
-        response = await self.request(
+        return await self._request_values_dict(
             'get',
             url=f'v1/contracts/{address}/{entrypoint}',
             params=params,
         )
-        # FIXME: No cursor iteration, need 'id' in select
-        return tuple(item['address'] for item in response)
 
     async def iter_similar_contracts(
         self,
         address: str,
         strict: bool = False,
-    ) -> AsyncIterator[tuple[str, ...]]:
+    ) -> AsyncIterator[tuple[dict[str, str], ...]]:
         async for batch in self._iter_batches(
             self.get_similar_contracts,
             address,
             strict,
-            cursor=False,
+            cursor=True,
         ):
             yield batch
 
     async def get_originated_contracts(
         self,
         address: str,
         offset: int | None = None,
         limit: int | None = None,
-    ) -> tuple[str, ...]:
+    ) -> tuple[dict[str, str], ...]:
         """Get addresses of contracts originated from given address"""
         self._logger.info('Fetching originated contracts for address `%s`', address)
         params = self._get_request_params(
             offset=offset,
             limit=limit,
-            select=('id', 'address'),
+            select=(
+                'id',
+                'address',
+            ),
+            values=True,
+            cursor=True,
         )
-        response = await self.request(
+        return await self._request_values_dict(
             'get',
-            url=f'v1/accounts/{address}/contracts',
-            params=params,
+            url='v1/contracts',
+            params={
+                'creator.eq': address,
+                **params,
+            },
         )
-        # FIXME: No cursor iteration, need 'id' in select
-        return tuple(item['address'] for item in response)
 
-    async def iter_originated_contracts(self, address: str) -> AsyncIterator[tuple[str, ...]]:
+    async def iter_originated_contracts(self, address: str) -> AsyncIterator[tuple[dict[str, str], ...]]:
         async for batch in self._iter_batches(
             self.get_originated_contracts,
             address,
-            cursor=False,
+            cursor=True,
         ):
             yield batch
 
     async def get_contract_summary(self, address: str) -> dict[str, Any]:
         """Get contract summary"""
         self._logger.info('Fetching contract summary for address `%s`', address)
         return cast(
@@ -425,81 +559,83 @@
         address: str,
         offset: int | None = None,
         limit: int | None = None,
     ) -> tuple[dict[str, Any], ...]:
         params = self._get_request_params(
             offset=offset,
             limit=limit,
+            select=BIGMAP_FIELDS,
+            values=True,
         )
-        big_maps = await self.request(
+        return await self._request_values_dict(
             'get',
             url=f'v1/contracts/{address}/bigmaps',
             params=params,
         )
-        return tuple(big_maps)
 
     async def iter_contract_big_maps(
         self,
         address: str,
     ) -> AsyncIterator[tuple[dict[str, Any], ...]]:
         async for batch in self._iter_batches(
             self.get_contract_big_maps,
             address,
             cursor=False,
         ):
             yield batch
 
-    async def get_head_block(self) -> HeadBlockData:
+    async def get_head_block(self) -> TzktHeadBlockData:
         """Get latest block (head)"""
         self._logger.info('Fetching latest block')
         head_block_json = await self.request(
             'get',
             url='v1/head',
         )
-        return self.convert_head_block(head_block_json)
+        return TzktHeadBlockData.from_json(head_block_json)
 
-    async def get_block(self, level: int) -> BlockData:
+    async def get_block(self, level: int) -> TzktBlockData:
         """Get block by level"""
         self._logger.info('Fetching block %s', level)
         block_json = await self.request(
             'get',
             url=f'v1/blocks/{level}',
         )
-        return self.convert_block(block_json)
+        return TzktBlockData.from_json(block_json)
 
     async def get_migration_originations(
         self,
         first_level: int | None = None,
         last_level: int | None = None,
         offset: int | None = None,
         limit: int | None = None,
-    ) -> tuple[OperationData, ...]:
+    ) -> tuple[TzktOperationData, ...]:
         """Get contracts originated from migrations"""
         self._logger.info('Fetching contracts originated with migrations')
         params = self._get_request_params(
             first_level=first_level,
             last_level=last_level,
             offset=offset,
             limit=limit,
             select=ORIGINATION_MIGRATION_FIELDS,
+            values=True,
             cursor=True,
             kind='origination',
         )
-        raw_migrations = await self.request(
+        raw_migrations = await self._request_values_dict(
             'get',
             url='v1/operations/migrations',
             params=params,
         )
-        return tuple(self.convert_migration_origination(m) for m in raw_migrations)
+        return tuple(TzktOperationData.from_migration_json(m) for m in raw_migrations)
 
     async def iter_migration_originations(
         self,
         first_level: int | None = None,
         last_level: int | None = None,
-    ) -> AsyncIterator[tuple[OperationData, ...]]:
+    ) -> AsyncIterator[tuple[TzktOperationData, ...]]:
         async for batch in self._iter_batches(
             self.get_migration_originations,
             first_level,
             last_level,
         ):
             yield batch
 
@@ -507,104 +643,112 @@
         self,
         addresses: set[str] | None = None,
         code_hashes: set[int] | None = None,
         first_level: int | None = None,
         last_level: int | None = None,
         offset: int | None = None,
         limit: int | None = None,
-    ) -> tuple[OperationData, ...]:
+    ) -> tuple[TzktOperationData, ...]:
         offset, limit = offset or 0, limit or self.request_limit
         raw_originations: list[dict[str, Any]] = []
         params = self._get_request_params(
             first_level=first_level,
             last_level=last_level,
             offset=offset,
             limit=limit,
             select=ORIGINATION_OPERATION_FIELDS,
+            values=True,
             status='applied',
             cursor=bool(code_hashes) or bool(not code_hashes and not addresses),
         )
 
         # NOTE: TzKT may hit URL length limit with hundreds of originations in a single request.
         # NOTE: Chunk of 100 addresses seems like a reasonable choice - URL of ~4000 characters.
         # NOTE: Other operation requests won't hit that limit.
         if addresses and not code_hashes:
             # FIXME: No pagination because of URL length limit workaround
             for addresses_chunk in split_by_chunks(list(addresses), ORIGINATION_REQUEST_LIMIT):
-                raw_originations += await self.request(
+                raw_originations += list(
+                    await self._request_values_dict(
+                        'get',
+                        url='v1/operations/originations',
+                        params={
+                            **params,
+                            'originatedContract.in': ','.join(addresses_chunk),
+                        },
+                    )
+                )
+        elif code_hashes and not addresses:
+            raw_originations += list(
+                await self._request_values_dict(
                     'get',
                     url='v1/operations/originations',
                     params={
                         **params,
-                        'originatedContract.in': ','.join(addresses_chunk),
+                        # FIXME: Need a helper for this join
+                        'codeHash.in': ','.join(str(h) for h in code_hashes),
                     },
                 )
-        elif code_hashes and not addresses:
-            raw_originations += await self.request(
-                'get',
-                url='v1/operations/originations',
-                params={
-                    **params,
-                    # FIXME: Need a helper for this join
-                    'codeHash.in': ','.join(str(h) for h in code_hashes),
-                },
             )
         elif not addresses and not code_hashes:
-            raw_originations += await self.request(
-                'get',
-                url='v1/operations/originations',
-                params=params,
+            raw_originations += list(
+                await self._request_values_dict(
+                    'get',
+                    url='v1/operations/originations',
+                    params=params,
+                )
             )
         elif addresses and code_hashes:
             raise FrameworkException('Either `addresses` or `code_hashes` should be specified')
 
         # NOTE: `type` field needs to be set manually when requesting operations by specific type
-        return tuple(self.convert_operation(op, type_='origination') for op in raw_originations)
+        return tuple(TzktOperationData.from_json(op, type_='origination') for op in raw_originations)
 
     async def get_transactions(
         self,
         field: str,
         addresses: set[str] | None,
         code_hashes: set[int] | None,
         first_level: int | None = None,
         last_level: int | None = None,
         offset: int | None = None,
         limit: int | None = None,
-    ) -> tuple[OperationData, ...]:
+    ) -> tuple[TzktOperationData, ...]:
         params = self._get_request_params(
             first_level,
             last_level,
             offset,
             limit,
             TRANSACTION_OPERATION_FIELDS,
             cursor=True,
+            values=True,
             status='applied',
             sort='level',
         )
         if addresses and not code_hashes:
             params[f'{field}.in'] = ','.join(addresses)
         elif code_hashes and not addresses:
             params[f'{field}CodeHash.in'] = ','.join(str(h) for h in code_hashes)
 
-        raw_transactions = await self.request(
+        raw_transactions = await self._request_values_dict(
             'get',
             url='v1/operations/transactions',
             params=params,
         )
 
         # NOTE: `type` field needs to be set manually when requesting operations by specific type
-        return tuple(self.convert_operation(op, type_='transaction') for op in raw_transactions)
+        return tuple(TzktOperationData.from_json(op, type_='transaction') for op in raw_transactions)
 
     async def iter_transactions(
         self,
         field: str,
         addresses: set[str],
         first_level: int,
         last_level: int,
-    ) -> AsyncIterator[tuple[OperationData, ...]]:
+    ) -> AsyncIterator[tuple[TzktOperationData, ...]]:
         async for batch in self._iter_batches(
             self.get_transactions,
             field,
             addresses,
             first_level,
             last_level,
         ):
@@ -614,15 +758,15 @@
         self,
         addresses: set[str],
         paths: set[str],
         first_level: int,
         last_level: int,
         offset: int | None = None,
         limit: int | None = None,
-    ) -> tuple[BigMapData, ...]:
+    ) -> tuple[TzktBigMapData, ...]:
         params = self._get_request_params(
             first_level=first_level,
             last_level=last_level,
             offset=offset,
             limit=limit,
         )
         raw_big_maps = await self.request(
@@ -630,70 +774,70 @@
             url='v1/bigmaps/updates',
             params={
                 **params,
                 'contract.in': ','.join(addresses),
                 'path.in': ','.join(paths),
             },
         )
-        return tuple(self.convert_big_map(bm) for bm in raw_big_maps)
+        return tuple(TzktBigMapData.from_json(bm) for bm in raw_big_maps)
 
     async def iter_big_maps(
         self,
         addresses: set[str],
         paths: set[str],
         first_level: int,
         last_level: int,
-    ) -> AsyncIterator[tuple[BigMapData, ...]]:
+    ) -> AsyncIterator[tuple[TzktBigMapData, ...]]:
         async for batch in self._iter_batches(
             self.get_big_maps,
             addresses,
             paths,
             first_level,
             last_level,
             cursor=False,
         ):
             yield batch
 
-    async def get_quote(self, level: int) -> QuoteData:
+    async def get_quote(self, level: int) -> TzktQuoteData:
         """Get quote for block"""
         self._logger.info('Fetching quotes for level %s', level)
         quote_json = await self.request(
             'get',
             url='v1/quotes',
             params={'level': level},
         )
-        return self.convert_quote(quote_json[0])
+        return TzktQuoteData.from_json(quote_json[0])
 
     async def get_quotes(
         self,
         first_level: int,
         last_level: int,
         offset: int | None = None,
         limit: int | None = None,
-    ) -> tuple[QuoteData, ...]:
+    ) -> tuple[TzktQuoteData, ...]:
         """Get quotes for blocks"""
         offset, limit = offset or 0, limit or self.request_limit
         self._logger.info('Fetching quotes for levels %s-%s', first_level, last_level)
         quotes_json = await self.request(
             'get',
             url='v1/quotes',
             params={
                 'level.ge': first_level,
                 'level.le': last_level,
                 'offset.cr': offset,
                 'limit': limit,
             },
         )
-        return tuple(self.convert_quote(quote) for quote in quotes_json)
+        return tuple(TzktQuoteData.from_json(quote) for quote in quotes_json)
 
     async def iter_quotes(
         self,
         first_level: int,
         last_level: int,
-    ) -> AsyncIterator[tuple[QuoteData, ...]]:
+    ) -> AsyncIterator[tuple[TzktQuoteData, ...]]:
         """Iterate quotes for blocks"""
         async for batch in self._iter_batches(
             self.get_quotes,
             first_level,
             last_level,
         ):
             yield batch
@@ -704,114 +848,112 @@
         token_ids: set[int],
         from_addresses: set[str],
         to_addresses: set[str],
         first_level: int,
         last_level: int,
         offset: int | None = None,
         limit: int | None = None,
-    ) -> tuple[TokenTransferData, ...]:
+    ) -> tuple[TzktTokenTransferData, ...]:
         """Get token transfers for contract"""
-        offset, limit = offset or 0, limit or self.request_limit
-
-        raw_token_transfers = await self.request(
-            'get',
-            url='v1/tokens/transfers',
-            params={
+        params = self._get_request_params(
+            first_level,
+            last_level,
+            offset=offset or 0,
+            limit=limit,
+            select=TZKT_TOKEN_TRANSFER_DATA_FIELDS,
+            values=True,
+            cursor=True,
+            **{
                 'token.contract.in': ','.join(token_addresses),
                 'token.id.in': ','.join(str(token_id) for token_id in token_ids),
                 'from.in': ','.join(from_addresses),
                 'to.in': ','.join(to_addresses),
-                'level.ge': first_level,
-                'level.le': last_level,
-                'offset': offset,
-                'limit': limit,
             },
         )
-        return tuple(self.convert_token_transfer(item) for item in raw_token_transfers)
+        raw_token_transfers = await self._request_values_dict('get', url='v1/tokens/transfers', params=params)
+        return tuple(TzktTokenTransferData.from_json(item) for item in raw_token_transfers)
 
     async def iter_token_transfers(
         self,
         token_addresses: set[str],
         token_ids: set[int],
         from_addresses: set[str],
         to_addresses: set[str],
         first_level: int,
         last_level: int,
-    ) -> AsyncIterator[tuple[TokenTransferData, ...]]:
+    ) -> AsyncIterator[tuple[TzktTokenTransferData, ...]]:
         """Iterate token transfers for contract"""
         async for batch in self._iter_batches(
             self.get_token_transfers,
             token_addresses,
             token_ids,
             from_addresses,
             to_addresses,
             first_level,
             last_level,
-            cursor=False,
+            cursor=True,
         ):
             yield batch
 
     async def get_events(
         self,
         addresses: set[str],
         tags: set[str],
         first_level: int,
         last_level: int,
         offset: int | None = None,
         limit: int | None = None,
-    ) -> tuple[EventData, ...]:
+    ) -> tuple[TzktEventData, ...]:
+        # FIXME: no tests for function
         offset, limit = offset or 0, limit or self.request_limit
-        raw_events = await self.request(
+        raw_events = await self._request_values_dict(
             'get',
             url='v1/contracts/events',
             params={
                 'contract.in': ','.join(addresses),
                 'tag.in': ','.join(tags),
                 'level.ge': first_level,
                 'level.le': last_level,
-                # TODO: Cursor supported?
-                'offset': offset,
+                'select.values': ','.join(f.name for f in fields(TzktEventData)),
+                'offset.cr': offset,
                 'limit': limit,
             },
         )
-        return tuple(self.convert_event(e) for e in raw_events)
+        return tuple(TzktEventData.from_json(e) for e in raw_events)
 
     async def iter_events(
         self,
         addresses: set[str],
         tags: set[str],
         first_level: int,
         last_level: int,
-    ) -> AsyncIterator[tuple[EventData, ...]]:
+    ) -> AsyncIterator[tuple[TzktEventData, ...]]:
         async for batch in self._iter_batches(
             self.get_events,
             addresses,
             tags,
             first_level,
             last_level,
             cursor=False,
         ):
             yield batch
 
-    async def add_index(self, index_config: ResolvedIndexConfigU) -> None:
-        """Register index config in internal mappings and matchers. Find and register subscriptions."""
-        for subscription in index_config.subscriptions:
-            self._subscriptions.add(subscription)
-
     async def subscribe(self) -> None:
         missing_subscriptions = self._subscriptions.missing_subscriptions
         if not missing_subscriptions:
             return
 
         self._logger.info('Subscribing to %s channels', len(missing_subscriptions))
-        tasks = (self._subscribe(subscription) for subscription in missing_subscriptions)
-        await asyncio.gather(*tasks)
+        for subscription in missing_subscriptions:
+            if not isinstance(subscription, TzktSubscription):
+                raise FrameworkException(f'Expected TzktSubscription, got {subscription}')
+            await self._subscribe(subscription)
         self._logger.info('Subscribed to %s channels', len(missing_subscriptions))
 
-    async def _subscribe(self, subscription: Subscription) -> None:
+    async def _subscribe(self, subscription: TzktSubscription) -> None:
         self._logger.debug('Subscribing to %s', subscription)
         method = subscription.method
         request: list[dict[str, Any]] = subscription.get_request()
 
         event = Event()
 
         async def _on_subscribe(message: CompletionMessage) -> None:
@@ -820,21 +962,38 @@
             level = cast(int, message.result)
             self._subscriptions.set_sync_level(subscription, level)
             event.set()
 
         await self._send(method, request, _on_subscribe)
         await event.wait()
 
+    async def _request_values_dict(self, *args: Any, **kwargs: Any) -> tuple[dict[str, Any], ...]:
+        # NOTE: basicaly this function create dict from list of tuples request
+        # NOTE: this is necessary because for TZKT API cursor iteration is more efficient and asking only values is more efficient too """
+        try:
+            fields = kwargs.get('params', {})['select.values'].split(',')
+        except KeyError as e:
+            raise DatasourceError('No fields selected, no select.values param in request', self.name) from e
+        if len(fields) == 1:
+            raise DatasourceError(
+                '_request_values_dict does not support one field request because tzkt will return plain list', self.name
+            )
+
+        # NOTE: select.values supported for methods with multiple objects in response only
+        response: list[list[str]] = await self.request(*args, **kwargs)
+        return tuple([dict(zip(fields, values)) for values in response])
+
     def _get_request_params(
         self,
         first_level: int | None = None,
         last_level: int | None = None,
         offset: int | None = None,
         limit: int | None = None,
         select: tuple[str, ...] | None = None,
+        values: bool = False,  # return only list of chosen values instead of dict
         cursor: bool = False,
         sort: str | None = None,
         **kwargs: Any,
     ) -> dict[str, Any]:
         params: dict[str, Any] = {
             'limit': limit or self.request_limit,
         }
@@ -844,15 +1003,16 @@
             params['level.le'] = last_level
         if offset:
             if cursor:
                 params['offset.cr'] = offset
             else:
                 params['offset'] = offset
         if select:
-            params['select'] = ','.join(select)
+            #  filter fields
+            params['select.values' if values else 'select'] = ','.join(select)
         if sort:
             if sort.startswith('-'):
                 sort_param_name = 'sort.desc'
                 sort = sort[1:]
             else:
                 sort_param_name = 'sort'
             params[sort_param_name] = sort
@@ -900,19 +1060,19 @@
             max_size=None,
         )
 
         self._signalr_client.on_open(self._on_connected)
         self._signalr_client.on_close(self._on_disconnected)
         self._signalr_client.on_error(self._on_error)
 
-        self._signalr_client.on('operations', partial(self._on_message, MessageType.operation))
-        self._signalr_client.on('transfers', partial(self._on_message, MessageType.token_transfer))
-        self._signalr_client.on('bigmaps', partial(self._on_message, MessageType.big_map))
-        self._signalr_client.on('head', partial(self._on_message, MessageType.head))
-        self._signalr_client.on('events', partial(self._on_message, MessageType.event))
+        self._signalr_client.on('operations', partial(self._on_message, TzktMessageType.operation))
+        self._signalr_client.on('transfers', partial(self._on_message, TzktMessageType.token_transfer))
+        self._signalr_client.on('bigmaps', partial(self._on_message, TzktMessageType.big_map))
+        self._signalr_client.on('head', partial(self._on_message, TzktMessageType.head))
+        self._signalr_client.on('events', partial(self._on_message, TzktMessageType.event))
 
         return self._signalr_client
 
     async def _send(
         self,
         method: str,
         arguments: list[dict[str, Any]],
@@ -933,341 +1093,113 @@
         self._contract_hashes.reset()
         await self.emit_disconnected()
 
     async def _on_error(self, message: CompletionMessage) -> NoReturn:
         """Raise exception from WS server's error message"""
         raise DatasourceError(datasource=self.name, msg=cast(str, message.error))
 
-    async def _on_message(self, type_: MessageType, message: list[dict[str, Any]]) -> None:
+    async def _on_message(self, type_: TzktMessageType, message: list[dict[str, Any]]) -> None:
         """Parse message received from Websocket, ensure it's correct in the current context and yield data."""
         # NOTE: Parse messages and either buffer or yield data
         for item in message:
-            tzkt_type = TzktMessageType(item['type'])
+            action = TzktMessageAction(item['type'])
             # NOTE: Legacy, sync level returned by TzKT during negotiation
-            if tzkt_type == TzktMessageType.STATE:
+            if action == TzktMessageAction.STATE:
                 continue
 
             message_level = item['state']
             channel_level = self.get_channel_level(type_)
             self._channel_levels[type_] = message_level
 
             self._logger.info(
                 'Realtime message received: %s, %s, %s -> %s',
                 type_.value,
-                tzkt_type.name,
+                action.name,
                 channel_level,
                 message_level,
             )
 
             # NOTE: Put data messages to buffer by level
-            if tzkt_type == TzktMessageType.DATA:
+            if action == TzktMessageAction.DATA:
                 self._buffer.add(type_, message_level, item['data'])
 
             # NOTE: Try to process rollback automatically, emit if failed
-            elif tzkt_type == TzktMessageType.REORG:
+            elif action == TzktMessageAction.REORG:
                 if self._buffer.rollback(type_, channel_level, message_level):
                     self._logger.info('Rolled back blocks were dropped from realtime message buffer')
                 else:
                     self._logger.info('Rolled back blocks are not buffered; proceeding to database rollback')
                     await self.emit_rollback(type_, channel_level, message_level)
 
             else:
-                raise NotImplementedError(f'Unknown message type: {tzkt_type}')
+                raise NotImplementedError(f'Unknown message type: {action}')
 
         # NOTE: Process extensive data from buffer
         for buffered_message in self._buffer.yield_from():
-            if buffered_message.type == MessageType.operation:
+            if buffered_message.type == TzktMessageType.operation:
                 await self._process_operations_data(cast(list[dict[str, Any]], buffered_message.data))
-            elif buffered_message.type == MessageType.token_transfer:
+            elif buffered_message.type == TzktMessageType.token_transfer:
                 await self._process_token_transfers_data(cast(list[dict[str, Any]], buffered_message.data))
-            elif buffered_message.type == MessageType.big_map:
+            elif buffered_message.type == TzktMessageType.big_map:
                 await self._process_big_maps_data(cast(list[dict[str, Any]], buffered_message.data))
-            elif buffered_message.type == MessageType.head:
+            elif buffered_message.type == TzktMessageType.head:
                 await self._process_head_data(cast(dict[str, Any], buffered_message.data))
-            elif buffered_message.type == MessageType.event:
+            elif buffered_message.type == TzktMessageType.event:
                 await self._process_events_data(cast(list[dict[str, Any]], buffered_message.data))
             else:
                 raise NotImplementedError(f'Unknown message type: {buffered_message.type}')
 
     async def _process_operations_data(self, data: list[dict[str, Any]]) -> None:
         """Parse and emit raw operations from WS"""
-        level_operations: defaultdict[int, deque[OperationData]] = defaultdict(deque)
+        level_operations: defaultdict[int, deque[TzktOperationData]] = defaultdict(deque)
 
         for operation_json in data:
             if operation_json['status'] != 'applied':
                 continue
             if 'hash' in operation_json:
-                operation = self.convert_operation(operation_json)
+                operation = TzktOperationData.from_json(operation_json)
             else:
-                operation = self.convert_migration_origination(operation_json)
+                operation = TzktOperationData.from_migration_json(operation_json)
             level_operations[operation.level].append(operation)
 
         for _level, operations in level_operations.items():
             await self.emit_operations(tuple(operations))
 
     async def _process_token_transfers_data(self, data: list[dict[str, Any]]) -> None:
         """Parse and emit raw token transfers from WS"""
-        level_token_transfers: defaultdict[int, deque[TokenTransferData]] = defaultdict(deque)
+        level_token_transfers: defaultdict[int, deque[TzktTokenTransferData]] = defaultdict(deque)
 
         for token_transfer_json in data:
-            token_transfer = self.convert_token_transfer(token_transfer_json)
+            token_transfer = TzktTokenTransferData.from_json(token_transfer_json)
             level_token_transfers[token_transfer.level].append(token_transfer)
 
         for _level, token_transfers in level_token_transfers.items():
             await self.emit_token_transfers(tuple(token_transfers))
 
     async def _process_big_maps_data(self, data: list[dict[str, Any]]) -> None:
         """Parse and emit raw big map diffs from WS"""
-        level_big_maps: defaultdict[int, deque[BigMapData]] = defaultdict(deque)
+        level_big_maps: defaultdict[int, deque[TzktBigMapData]] = defaultdict(deque)
 
-        big_maps: deque[BigMapData] = deque()
+        big_maps: deque[TzktBigMapData] = deque()
         for big_map_json in data:
-            big_map = self.convert_big_map(big_map_json)
+            big_map = TzktBigMapData.from_json(big_map_json)
             level_big_maps[big_map.level].append(big_map)
 
         for _level, big_maps in level_big_maps.items():
             await self.emit_big_maps(tuple(big_maps))
 
     async def _process_head_data(self, data: dict[str, Any]) -> None:
         """Parse and emit raw head block from WS"""
-        block = self.convert_head_block(data)
+        block = TzktHeadBlockData.from_json(data)
         await self.emit_head(block)
 
     async def _process_events_data(self, data: list[dict[str, Any]]) -> None:
         """Parse and emit raw big map diffs from WS"""
-        level_events: defaultdict[int, deque[EventData]] = defaultdict(deque)
+        level_events: defaultdict[int, deque[TzktEventData]] = defaultdict(deque)
 
-        events: deque[EventData] = deque()
+        events: deque[TzktEventData] = deque()
         for event_json in data:
-            event = self.convert_event(event_json)
+            event = TzktEventData.from_json(event_json)
             level_events[event.level].append(event)
 
         for _level, events in level_events.items():
             await self.emit_events(tuple(events))
-
-    @classmethod
-    def convert_operation(
-        cls,
-        operation_json: dict[str, Any],
-        type_: str | None = None,
-    ) -> OperationData:
-        """Convert raw operation message from WS/REST into dataclass"""
-        # NOTE: Migration originations are handled in a separate method
-        sender_json = operation_json.get('sender') or {}
-        target_json = operation_json.get('target') or {}
-        initiator_json = operation_json.get('initiator') or {}
-        delegate_json = operation_json.get('delegate') or {}
-        parameter_json = operation_json.get('parameter') or {}
-        originated_contract_json = operation_json.get('originatedContract') or {}
-
-        if (amount := operation_json.get('contractBalance')) is None:
-            amount = operation_json.get('amount')
-
-        entrypoint, parameter = parameter_json.get('entrypoint'), parameter_json.get('value')
-        if target_json.get('address', '').startswith('KT1'):
-            # NOTE: TzKT returns None for `default` entrypoint
-            if entrypoint is None:
-                entrypoint = 'default'
-
-                # NOTE: Empty parameter in this case means `{"prim": "Unit"}`
-                if parameter is None:
-                    parameter = {}
-
-        return OperationData(
-            type=type_ or operation_json['type'],
-            id=operation_json['id'],
-            level=operation_json['level'],
-            timestamp=_parse_timestamp(operation_json['timestamp']),
-            block=operation_json.get('block'),
-            hash=operation_json['hash'],
-            counter=operation_json['counter'],
-            sender_address=sender_json.get('address'),
-            sender_code_hash=operation_json.get('senderCodeHash'),
-            target_address=target_json.get('address'),
-            target_code_hash=operation_json.get('targetCodeHash'),
-            initiator_address=initiator_json.get('address'),
-            amount=amount,
-            status=operation_json['status'],
-            has_internals=operation_json.get('hasInternals'),
-            sender_alias=operation_json['sender'].get('alias'),
-            nonce=operation_json.get('nonce'),
-            target_alias=target_json.get('alias'),
-            initiator_alias=initiator_json.get('alias'),
-            entrypoint=entrypoint,
-            parameter_json=parameter,
-            originated_contract_address=originated_contract_json.get('address'),
-            originated_contract_alias=originated_contract_json.get('alias'),
-            originated_contract_type_hash=originated_contract_json.get('typeHash'),
-            originated_contract_code_hash=originated_contract_json.get('codeHash'),
-            originated_contract_tzips=originated_contract_json.get('tzips'),
-            storage=operation_json.get('storage'),
-            diffs=operation_json.get('diffs') or (),
-            delegate_address=delegate_json.get('address'),
-            delegate_alias=delegate_json.get('alias'),
-        )
-
-    @classmethod
-    def convert_migration_origination(
-        cls,
-        migration_origination_json: dict[str, Any],
-    ) -> OperationData:
-        """Convert raw migration message from REST into dataclass"""
-        return OperationData(
-            type='migration',
-            id=migration_origination_json['id'],
-            level=migration_origination_json['level'],
-            timestamp=_parse_timestamp(migration_origination_json['timestamp']),
-            block=migration_origination_json.get('block'),
-            originated_contract_address=migration_origination_json['account']['address'],
-            originated_contract_alias=migration_origination_json['account'].get('alias'),
-            amount=migration_origination_json['balanceChange'],
-            storage=migration_origination_json.get('storage'),
-            diffs=migration_origination_json.get('diffs') or (),
-            status='applied',
-            has_internals=False,
-            hash='[none]',
-            counter=0,
-            sender_address='[none]',
-            sender_code_hash=None,
-            target_address=None,
-            target_code_hash=None,
-            initiator_address=None,
-        )
-
-    @classmethod
-    def convert_big_map(
-        cls,
-        big_map_json: dict[str, Any],
-    ) -> BigMapData:
-        """Convert raw big map diff message from WS/REST into dataclass"""
-        action = BigMapAction(big_map_json['action'])
-        active = action not in (BigMapAction.REMOVE, BigMapAction.REMOVE_KEY)
-        return BigMapData(
-            id=big_map_json['id'],
-            level=big_map_json['level'],
-            # NOTE: missing `operation_id` field in API to identify operation
-            operation_id=big_map_json['level'],
-            timestamp=_parse_timestamp(big_map_json['timestamp']),
-            bigmap=big_map_json['bigmap'],
-            contract_address=big_map_json['contract']['address'],
-            path=big_map_json['path'],
-            action=action,
-            active=active,
-            key=big_map_json.get('content', {}).get('key'),
-            value=big_map_json.get('content', {}).get('value'),
-        )
-
-    @classmethod
-    def convert_block(
-        cls,
-        block_json: dict[str, Any],
-    ) -> BlockData:
-        """Convert raw block message from REST into dataclass"""
-        return BlockData(
-            level=block_json['level'],
-            hash=block_json['hash'],
-            timestamp=_parse_timestamp(block_json['timestamp']),
-            proto=block_json['proto'],
-            priority=block_json.get('priority'),
-            validations=block_json['validations'],
-            deposit=block_json['deposit'],
-            reward=block_json['reward'],
-            fees=block_json['fees'],
-            nonce_revealed=block_json['nonceRevealed'],
-            baker_address=block_json.get('baker', {}).get('address'),
-            baker_alias=block_json.get('baker', {}).get('alias'),
-        )
-
-    @classmethod
-    def convert_head_block(
-        cls,
-        head_block_json: dict[str, Any],
-    ) -> HeadBlockData:
-        """Convert raw head block message from WS/REST into dataclass"""
-        return HeadBlockData(
-            chain=head_block_json['chain'],
-            chain_id=head_block_json['chainId'],
-            cycle=head_block_json['cycle'],
-            level=head_block_json['level'],
-            hash=head_block_json['hash'],
-            protocol=head_block_json['protocol'],
-            next_protocol=head_block_json['nextProtocol'],
-            timestamp=_parse_timestamp(head_block_json['timestamp']),
-            voting_epoch=head_block_json['votingEpoch'],
-            voting_period=head_block_json['votingPeriod'],
-            known_level=head_block_json['knownLevel'],
-            last_sync=head_block_json['lastSync'],
-            synced=head_block_json['synced'],
-            quote_level=head_block_json['quoteLevel'],
-            quote_btc=Decimal(head_block_json['quoteBtc']),
-            quote_eur=Decimal(head_block_json['quoteEur']),
-            quote_usd=Decimal(head_block_json['quoteUsd']),
-            quote_cny=Decimal(head_block_json['quoteCny']),
-            quote_jpy=Decimal(head_block_json['quoteJpy']),
-            quote_krw=Decimal(head_block_json['quoteKrw']),
-            quote_eth=Decimal(head_block_json['quoteEth']),
-            quote_gbp=Decimal(head_block_json['quoteGbp']),
-        )
-
-    @classmethod
-    def convert_quote(cls, quote_json: dict[str, Any]) -> QuoteData:
-        """Convert raw quote message from REST into dataclass"""
-        return QuoteData(
-            level=quote_json['level'],
-            timestamp=_parse_timestamp(quote_json['timestamp']),
-            btc=Decimal(quote_json['btc']),
-            eur=Decimal(quote_json['eur']),
-            usd=Decimal(quote_json['usd']),
-            cny=Decimal(quote_json['cny']),
-            jpy=Decimal(quote_json['jpy']),
-            krw=Decimal(quote_json['krw']),
-            eth=Decimal(quote_json['eth']),
-            gbp=Decimal(quote_json['gbp']),
-        )
-
-    @classmethod
-    def convert_token_transfer(cls, token_transfer_json: dict[str, Any]) -> TokenTransferData:
-        """Convert raw token transfer message from REST or WS into dataclass"""
-        token_json = token_transfer_json.get('token') or {}
-        contract_json = token_json.get('contract') or {}
-        from_json = token_transfer_json.get('from') or {}
-        to_json = token_transfer_json.get('to') or {}
-        standard = token_json.get('standard')
-        metadata = token_json.get('metadata')
-        return TokenTransferData(
-            id=token_transfer_json['id'],
-            level=token_transfer_json['level'],
-            timestamp=_parse_timestamp(token_transfer_json['timestamp']),
-            tzkt_token_id=token_json['id'],
-            contract_address=contract_json.get('address'),
-            contract_alias=contract_json.get('alias'),
-            token_id=token_json.get('tokenId'),
-            standard=TokenStandard(standard) if standard else None,
-            metadata=metadata if isinstance(metadata, dict) else {},
-            from_alias=from_json.get('alias'),
-            from_address=from_json.get('address'),
-            to_alias=to_json.get('alias'),
-            to_address=to_json.get('address'),
-            amount=token_transfer_json.get('amount'),
-            tzkt_transaction_id=token_transfer_json.get('transactionId'),
-            tzkt_origination_id=token_transfer_json.get('originationId'),
-            tzkt_migration_id=token_transfer_json.get('migrationId'),
-        )
-
-    @classmethod
-    def convert_event(cls, event_json: dict[str, Any]) -> EventData:
-        """Convert raw event message from WS/REST into dataclass"""
-        return EventData(
-            id=event_json['id'],
-            level=event_json['level'],
-            timestamp=_parse_timestamp(event_json['timestamp']),
-            tag=event_json['tag'],
-            payload=event_json.get('payload'),
-            contract_address=event_json['contract']['address'],
-            contract_alias=event_json['contract'].get('alias'),
-            contract_code_hash=event_json['codeHash'],
-            transaction_id=event_json.get('transactionId'),
-        )
-
-
-def _parse_timestamp(timestamp: str) -> datetime:
-    return datetime.fromisoformat(timestamp[:-1]).replace(tzinfo=timezone.utc)
```

### Comparing `dipdup-6.5.9/src/dipdup/dipdup.py` & `dipdup-7.0.0rc1/src/dipdup/dipdup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,89 @@
 import asyncio
 import logging
+import time
 from asyncio import CancelledError
 from asyncio import Event
 from asyncio import Task
 from asyncio import create_task
 from asyncio import gather
+from collections import defaultdict
 from collections import deque
 from contextlib import AsyncExitStack
+from contextlib import asynccontextmanager
 from contextlib import suppress
 from copy import copy
 from typing import Any
+from typing import AsyncIterator
 from typing import Awaitable
-from typing import Dict
-from typing import Optional
 
 from tortoise.exceptions import OperationalError
 
-from dipdup.codegen import CodeGenerator
-from dipdup.config import ContractConfig
-from dipdup.config import DatasourceConfigU
+from dipdup import env
+from dipdup.codegen import generate_environments
 from dipdup.config import DipDupConfig
 from dipdup.config import IndexTemplateConfig
 from dipdup.config import PostgresDatabaseConfig
 from dipdup.config import SqliteDatabaseConfig
-from dipdup.config import event_hooks
-from dipdup.context import CallbackManager
+from dipdup.config import system_hooks
+from dipdup.config.evm import EvmContractConfig
+from dipdup.config.tezos import TezosContractConfig
 from dipdup.context import DipDupContext
 from dipdup.context import MetadataCursor
-from dipdup.context import pending_indexes
-from dipdup.datasources.datasource import Datasource
-from dipdup.datasources.datasource import IndexDatasource
-from dipdup.datasources.factory import DatasourceFactory
-from dipdup.datasources.tzkt.datasource import TzktDatasource
-from dipdup.enums import IndexStatus
-from dipdup.enums import MessageType
-from dipdup.enums import ReindexingReason
+from dipdup.database import generate_schema
+from dipdup.database import get_connection
+from dipdup.database import get_schema_hash
+from dipdup.database import preload_cached_models
+from dipdup.database import tortoise_wrapper
+from dipdup.datasources import Datasource
+from dipdup.datasources import IndexDatasource
+from dipdup.datasources import create_datasource
+from dipdup.datasources.evm_node import EvmNodeDatasource
+from dipdup.datasources.tezos_tzkt import TzktDatasource
 from dipdup.exceptions import ConfigInitializationException
-from dipdup.exceptions import DipDupException
 from dipdup.exceptions import FrameworkException
 from dipdup.hasura import HasuraGateway
 from dipdup.index import Index
-from dipdup.indexes.big_map.index import BigMapIndex
-from dipdup.indexes.event.index import EventIndex
-from dipdup.indexes.head.index import HeadIndex
-from dipdup.indexes.operation.index import OperationIndex
-from dipdup.indexes.operation.index import extract_operation_subgroups
-from dipdup.indexes.token_transfer.index import TokenTransferIndex
-from dipdup.models import BigMapData
+from dipdup.indexes.evm_subsquid_events.index import SubsquidEventsIndex
+from dipdup.indexes.tezos_tzkt_big_maps.index import TzktBigMapsIndex
+from dipdup.indexes.tezos_tzkt_events.index import TzktEventsIndex
+from dipdup.indexes.tezos_tzkt_head.index import TzktHeadIndex
+from dipdup.indexes.tezos_tzkt_operations.index import TzktOperationsIndex
+from dipdup.indexes.tezos_tzkt_operations.index import extract_operation_subgroups
+from dipdup.indexes.tezos_tzkt_token_transfers.index import TzktTokenTransfersIndex
 from dipdup.models import Contract
-from dipdup.models import EventData
+from dipdup.models import ContractKind
 from dipdup.models import Head
-from dipdup.models import HeadBlockData
 from dipdup.models import Index as IndexState
-from dipdup.models import OperationData
+from dipdup.models import IndexStatus
+from dipdup.models import MessageType
+from dipdup.models import ReindexingReason
 from dipdup.models import Schema
-from dipdup.models import TokenTransferData
+from dipdup.models.evm_node import EvmNodeHeadData
+from dipdup.models.evm_node import EvmNodeLogData
+from dipdup.models.evm_node import EvmNodeSyncingData
+from dipdup.models.tezos_tzkt import TzktBigMapData
+from dipdup.models.tezos_tzkt import TzktEventData
+from dipdup.models.tezos_tzkt import TzktHeadBlockData
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktTokenTransferData
+from dipdup.package import DipDupPackage
+from dipdup.performance import MetricsLevel
+from dipdup.performance import metrics
 from dipdup.prometheus import Metrics
 from dipdup.scheduler import SchedulerManager
 from dipdup.transactions import TransactionManager
-from dipdup.utils.database import generate_schema
-from dipdup.utils.database import get_connection
-from dipdup.utils.database import get_schema_hash
-from dipdup.utils.database import tortoise_wrapper
 
 
 class IndexDispatcher:
     def __init__(self, ctx: DipDupContext) -> None:
         self._ctx = ctx
 
-        self._logger = logging.getLogger('dipdup')
-        self._indexes: Dict[str, Index[Any, Any, Any]] = {}
+        self._logger = logging.getLogger(__name__)
+        self._indexes: dict[str, Index[Any, Any, Any]] = {}
 
         self._entrypoint_filter: set[str | None] = set()
         self._address_filter: set[str] = set()
         self._code_hash_filter: set[int] = set()
 
     async def run(
         self,
@@ -84,79 +94,123 @@
         self._logger.info('Starting index dispatcher')
         await self._subscribe_to_datasource_events()
         await self._load_index_state()
 
         on_synchronized_fired = False
 
         for index in self._indexes.values():
-            if isinstance(index, OperationIndex):
+            if isinstance(index, TzktOperationsIndex):
                 await self._apply_filters(index)
 
         while True:
             if not spawn_datasources_event.is_set():
-                if (self._every_index_is(IndexStatus.REALTIME) or early_realtime) and not self._ctx.config.oneshot:
+                if (self._every_index_is(IndexStatus.realtime) or early_realtime) and not self._ctx.config.oneshot:
                     spawn_datasources_event.set()
 
             if spawn_datasources_event.is_set():
-                index_datasources = {i.datasource for i in self._indexes.values()}
-                for datasource in index_datasources:
+                for datasource in self._ctx.datasources.values():
+                    if not isinstance(datasource, IndexDatasource):
+                        continue
                     await datasource.subscribe()
 
             tasks: deque[Awaitable[bool]] = deque()
             for name, index in copy(self._indexes).items():
-                if index.state.status == IndexStatus.ONESHOT:
+                if index.state.status == IndexStatus.disabled:
                     del self._indexes[name]
                     continue
 
                 tasks.append(index.process())
 
             await gather(*tasks)
 
             indexes_spawned = False
-            while pending_indexes:
-                index = pending_indexes.popleft()
+            while self._ctx._pending_indexes:
+                index = self._ctx._pending_indexes.popleft()
                 self._indexes[index._config.name] = index
                 indexes_spawned = True
 
-                if isinstance(index, OperationIndex):
+                if isinstance(index, TzktOperationsIndex):
                     await self._apply_filters(index)
 
-            if not indexes_spawned and (not self._indexes or self._every_index_is(IndexStatus.ONESHOT)):
+            if not indexes_spawned and (not self._indexes or self._every_index_is(IndexStatus.disabled)):
                 self._logger.info('No indexes left, exiting')
                 break
 
-            if self._every_index_is(IndexStatus.REALTIME) and not indexes_spawned:
+            if self._every_index_is(IndexStatus.realtime) and not indexes_spawned:
                 if not on_synchronized_fired:
                     on_synchronized_fired = True
                     await self._ctx.fire_hook('on_synchronized')
+                    metrics and metrics.set('synchronized_at', time.time())
 
                 if not start_scheduler_event.is_set():
                     start_scheduler_event.set()
             else:
                 # NOTE: Fire `on_synchronized` hook when indexes will reach realtime state again
                 on_synchronized_fired = False
 
             # TODO: Replace with asyncio.Event
             await asyncio.sleep(1)
 
-    async def _update_metrics(self, update_interval: float) -> None:
+    # TODO: Use ctx.metrics
+    async def _prometheus_loop(self, update_interval: float) -> None:
         while True:
             await asyncio.sleep(update_interval)
 
             active, synced, realtime = 0, 0, 0
-            for index in tuple(self._indexes.values()) + tuple(pending_indexes):
+            for index in tuple(self._indexes.values()) + tuple(self._ctx._pending_indexes):
                 active += 1
                 if index.synchronized:
                     synced += 1
                 if index.realtime:
                     realtime += 1
 
             Metrics.set_indexes_count(active, synced, realtime)
 
-    async def _apply_filters(self, index: OperationIndex) -> None:
+    async def _metrics_loop(self, update_interval: float) -> None:
+        started_at = time.time()
+        initial_levels: defaultdict[str, int] = defaultdict(int)
+        previous_levels: defaultdict[str, int] = defaultdict(int)
+        metrics.set('started_at', started_at)
+
+        while True:
+            await asyncio.sleep(update_interval)
+            if not self._indexes:
+                continue
+
+            levels_indexed, levels_total, levels_interval = 0, 0, 0
+            for index in self._indexes.values():
+                initial_level = initial_levels[index.name]
+                if not initial_level:
+                    initial_levels[index.name] |= index.state.level
+                    continue
+
+                levels_interval += index.state.level - previous_levels[index.name]
+                levels_indexed += index.state.level - initial_level
+                levels_total += index.get_sync_level() - initial_level
+
+                previous_levels[index.name] = index.state.level
+
+            current_speed = levels_interval / update_interval
+            average_speed = levels_indexed / (time.time() - started_at)
+            time_passed = (time.time() - started_at) / 60
+            time_left, progress = 0.0, 0.0
+            if average_speed:
+                time_left = (levels_total - levels_indexed) / average_speed / 60
+            if levels_total:
+                progress = levels_indexed / levels_total
+
+            metrics.set('levels_indexed', levels_indexed)
+            metrics.set('levels_total', levels_total)
+            metrics.set('current_speed', current_speed)
+            metrics.set('average_speed', average_speed)
+            metrics.set('time_passed', time_passed)
+            metrics.set('time_left', time_left)
+            metrics.set('progress', progress)
+
+    async def _apply_filters(self, index: TzktOperationsIndex) -> None:
         entrypoints, addresses, code_hashes = await index.get_filters()
         self._entrypoint_filter.update(entrypoints)
         self._address_filter.update(addresses)
         self._code_hash_filter.update(code_hashes)
 
     def _every_index_is(self, status: IndexStatus) -> bool:
         if not self._indexes:
@@ -167,29 +221,37 @@
 
     async def _fetch_contracts(self) -> None:
         """Add contracts spawned from context to config"""
         contracts = await Contract.filter().all()
         self._logger.info('%s contracts fetched from database', len(contracts))
 
         for contract in contracts:
-            # FIXME: No `code_hash` field in the database
-            if ':' in contract.address:
-                address, code_hash = contract.address.split(':')
-            else:
-                address, code_hash = contract.address, None
+            if contract.name in self._ctx.config.contracts:
+                continue
 
-            if contract.name not in self._ctx.config.contracts:
-                contract_config = ContractConfig(
-                    address=address or None,
-                    code_hash=code_hash or None,
+            contract_config: TezosContractConfig | EvmContractConfig
+            if contract.kind == ContractKind.TEZOS:
+                contract_config = TezosContractConfig(
+                    kind='tezos',
+                    address=contract.address,
+                    code_hash=contract.code_hash,
+                    typename=contract.typename,
+                )
+            elif contract.kind == ContractKind.EVM:
+                contract_config = EvmContractConfig(
+                    kind='evm',
+                    address=contract.address,
                     typename=contract.typename,
                 )
-                self._ctx.config.contracts[contract.name] = contract_config
+            else:
+                raise NotImplementedError(contract.kind)
+
+            self._ctx.config.contracts[contract.name] = contract_config
 
-        self._ctx.config.initialize(skip_imports=True)
+        self._ctx.config.initialize()
 
     async def _load_index_state(self) -> None:
         if self._indexes:
             raise FrameworkException('Index states are already loaded')
 
         await self._fetch_contracts()
         self._logger.info('%s indexes found in database', await IndexState.all().count())
@@ -234,77 +296,110 @@
 
         # FIXME: Outdated optimization
         tasks = (create_task(_process(index_state)) for index_state in await IndexState.all())
         await gather(*tasks)
 
     async def _subscribe_to_datasource_events(self) -> None:
         for datasource in self._ctx.datasources.values():
-            if not isinstance(datasource, IndexDatasource):
-                continue
-            datasource.call_on_head(self._on_head)
-            datasource.call_on_operations(self._on_operations)
-            datasource.call_on_token_transfers(self._on_token_transfers)
-            datasource.call_on_big_maps(self._on_big_maps)
-            datasource.call_on_events(self._on_events)
-            datasource.call_on_rollback(self._on_rollback)
+            if isinstance(datasource, TzktDatasource):
+                datasource.call_on_head(self._on_tzkt_head)
+                datasource.call_on_operations(self._on_tzkt_operations)
+                datasource.call_on_token_transfers(self._on_tzkt_token_transfers)
+                datasource.call_on_big_maps(self._on_tzkt_big_maps)
+                datasource.call_on_events(self._on_tzkt_events)
+                datasource.call_on_rollback(self._on_rollback)
+            elif isinstance(datasource, EvmNodeDatasource):
+                datasource.call_on_head(self._on_evm_node_head)
+                datasource.call_on_logs(self._on_evm_node_logs)
+                datasource.call_on_syncing(self._on_evm_node_syncing)
 
-    async def _on_head(self, datasource: IndexDatasource, head: HeadBlockData) -> None:
+    async def _on_tzkt_head(self, datasource: TzktDatasource, head: TzktHeadBlockData) -> None:
         # NOTE: Do not await query results, it may block Websocket loop. We do not use Head anyway.
         asyncio.ensure_future(
             Head.update_or_create(
                 name=datasource.name,
                 defaults={
                     'level': head.level,
                     'hash': head.hash,
                     'timestamp': head.timestamp,
                 },
             ),
         )
         if Metrics.enabled:
             Metrics.set_datasource_head_updated(datasource.name)
         for index in self._indexes.values():
-            if isinstance(index, HeadIndex) and index.datasource == datasource:
+            if isinstance(index, TzktHeadIndex) and index.datasource == datasource:
                 index.push_head(head)
 
-    async def _on_operations(self, datasource: IndexDatasource, operations: tuple[OperationData, ...]) -> None:
+    async def _on_evm_node_head(self, datasource: EvmNodeDatasource, head: EvmNodeHeadData) -> None:
+        # NOTE: Do not await query results, it may block Websocket loop. We do not use Head anyway.
+        asyncio.ensure_future(
+            Head.update_or_create(
+                name=datasource.name,
+                defaults={
+                    'level': int(head.number, 16),
+                    'hash': head.hash,
+                    'timestamp': int(head.timestamp, 16),
+                },
+            ),
+        )
+        if Metrics.enabled:
+            Metrics.set_datasource_head_updated(datasource.name)
+
+    async def _on_evm_node_logs(self, datasource: EvmNodeDatasource, logs: EvmNodeLogData) -> None:
+        for index in self._indexes.values():
+            if not isinstance(index, SubsquidEventsIndex):
+                continue
+            if datasource not in index.node_datasources:
+                continue
+            index.push_realtime_message(logs)
+
+    async def _on_evm_node_syncing(self, datasource: EvmNodeDatasource, syncing: EvmNodeSyncingData) -> None:
+        raise NotImplementedError
+
+    async def _on_tzkt_operations(self, datasource: TzktDatasource, operations: tuple[TzktOperationData, ...]) -> None:
         operation_subgroups = tuple(
             extract_operation_subgroups(
                 operations,
                 addresses=self._address_filter,
                 entrypoints=self._entrypoint_filter,
                 code_hashes=self._code_hash_filter,
             )
         )
 
         if not operation_subgroups:
             return
 
         for index in self._indexes.values():
-            if isinstance(index, OperationIndex) and index.datasource == datasource:
+            if isinstance(index, TzktOperationsIndex) and index.datasource == datasource:
                 index.push_operations(operation_subgroups)
 
-    async def _on_token_transfers(
-        self, datasource: IndexDatasource, token_transfers: tuple[TokenTransferData, ...]
+    async def _on_tzkt_token_transfers(
+        self, datasource: TzktDatasource, token_transfers: tuple[TzktTokenTransferData, ...]
     ) -> None:
         for index in self._indexes.values():
-            if isinstance(index, TokenTransferIndex) and index.datasource == datasource:
+            if isinstance(index, TzktTokenTransfersIndex) and index.datasource == datasource:
                 index.push_token_transfers(token_transfers)
 
-    async def _on_big_maps(self, datasource: IndexDatasource, big_maps: tuple[BigMapData, ...]) -> None:
+    async def _on_tzkt_big_maps(self, datasource: TzktDatasource, big_maps: tuple[TzktBigMapData, ...]) -> None:
         for index in self._indexes.values():
-            if isinstance(index, BigMapIndex) and index.datasource == datasource:
+            if isinstance(index, TzktBigMapsIndex) and index.datasource == datasource:
                 index.push_big_maps(big_maps)
 
-    async def _on_events(self, datasource: IndexDatasource, events: tuple[EventData, ...]) -> None:
+    async def _on_tzkt_events(self, datasource: TzktDatasource, events: tuple[TzktEventData, ...]) -> None:
         for index in self._indexes.values():
-            if isinstance(index, EventIndex) and index.datasource == datasource:
+            if isinstance(index, TzktEventsIndex) and index.datasource == datasource:
                 index.push_events(events)
 
     async def _on_rollback(
-        self, datasource: IndexDatasource, type_: MessageType, from_level: int, to_level: int
+        self,
+        datasource: IndexDatasource[Any],
+        type_: MessageType,
+        from_level: int,
+        to_level: int,
     ) -> None:
         """Call `on_index_rollback` hook for each index that is affected by rollback"""
         if from_level <= to_level:
             raise FrameworkException(f'Attempt to rollback forward: {from_level} -> {to_level}')
 
         channel = f'{datasource.name}:{type_.value}'
         self._logger.info('Channel `%s` has rolled back: %s -> %s', channel, from_level, to_level)
@@ -345,137 +440,149 @@
 
 class DipDup:
     """Main indexer class.
 
     Spawns datasources, registers indexes, passes handler callbacks to executor"""
 
     def __init__(self, config: DipDupConfig) -> None:
-        self._logger = logging.getLogger('dipdup')
+        self._logger = logging.getLogger(__name__)
         self._config = config
-        self._datasources: Dict[str, Datasource] = {}
-        self._datasources_by_config: Dict[DatasourceConfigU, Datasource] = {}
-        self._callbacks: CallbackManager = CallbackManager(self._config.package)
+        self._datasources: dict[str, Datasource[Any]] = {}
         self._transactions: TransactionManager = TransactionManager(
             depth=self._config.advanced.rollback_depth,
             immune_tables=self._config.database.immune_tables,
         )
         self._ctx = DipDupContext(
             config=self._config,
+            package=DipDupPackage(config.package_path),
             datasources=self._datasources,
-            callbacks=self._callbacks,
             transactions=self._transactions,
         )
-        self._codegen = CodeGenerator(self._config, self._datasources_by_config)
-        self._schema: Optional[Schema] = None
+        self._schema: Schema | None = None
+        self._api: Any | None = None
 
     @property
     def schema(self) -> Schema:
         if self._schema is None:
-            raise DipDupException('Schema is not initialized')
+            raise FrameworkException('Schema is not initialized')
         return self._schema
 
     @classmethod
     async def create_dummy(
         cls,
         config: DipDupConfig,
         stack: AsyncExitStack,
         in_memory: bool = False,
     ) -> 'DipDup':
         """Create a dummy DipDup instance for testing purposes.
 
         Only basic initialization is performed:
 
           - Create datasources without spawning them
-          - Register event hooks
+          - Register system hooks
           - Initialize Tortoise ORM and create schema
 
         You need to enter `AsyncExitStack` context manager prior to calling this method.
         """
         if in_memory:
             config.database = SqliteDatabaseConfig(
                 kind='sqlite',
                 path=':memory:',
             )
-        config.initialize(skip_imports=True)
+        config.advanced.rollback_depth = 2
+        config.initialize()
 
         dipdup = DipDup(config)
         await dipdup._create_datasources()
         await dipdup._set_up_database(stack)
         await dipdup._set_up_hooks(set())
         await dipdup._initialize_schema()
         await dipdup._set_up_transactions(stack)
 
         return dipdup
 
     async def init(self, overwrite_types: bool = False, keep_schemas: bool = False) -> None:
         """Create new or update existing dipdup project"""
+        from dipdup.codegen.evm_subsquid import SubsquidCodeGenerator
+        from dipdup.codegen.tezos_tzkt import TzktCodeGenerator
+
         await self._create_datasources()
 
         async with AsyncExitStack() as stack:
             for datasource in self._datasources.values():
                 await stack.enter_async_context(datasource)
 
-            await self._codegen.init(overwrite_types, keep_schemas)
+            package = DipDupPackage(
+                root=self._config.package_path,
+                debug=keep_schemas,
+            )
+
+            for codegen_cls in (TzktCodeGenerator, SubsquidCodeGenerator):
+                codegen = codegen_cls(self._config, package, self._datasources)
+                await codegen.init(force=overwrite_types)
+
+            await generate_environments(self._config, package)
 
     async def run(self) -> None:
         """Run indexing process"""
-        advanced_config = self._config.advanced
+        # NOTE: DipDup is initialized layer by layer adding tasks to the loop and entering contexts.
+        # NOTE: Order matters. But usually you can skip some layers if you don't need them.
+        advanced = self._config.advanced
         tasks: set[Task[None]] = set()
         async with AsyncExitStack() as stack:
+            await self._set_up_metrics(stack)
+
             stack.enter_context(suppress(KeyboardInterrupt, CancelledError))
             await self._set_up_database(stack)
             await self._set_up_transactions(stack)
             await self._set_up_datasources(stack)
             await self._set_up_hooks(tasks, run=not self._config.oneshot)
             await self._set_up_prometheus()
+            await self._set_up_api(stack)
 
             await self._initialize_schema()
             await self._initialize_datasources()
 
             hasura_gateway = await self._set_up_hasura(stack)
             if hasura_gateway:
                 await hasura_gateway.configure()
 
-            if advanced_config.metadata_interface:
-                await MetadataCursor.initialize()
+            await MetadataCursor.initialize()
 
             if self._config.oneshot:
                 start_scheduler_event = Event()
                 spawn_datasources_event = Event()
 
                 if self._config.jobs:
                     self._logger.warning('Running in oneshot mode; `jobs` are ignored')
             else:
                 start_scheduler_event = await self._set_up_scheduler(tasks)
                 spawn_datasources_event = await self._spawn_datasources(tasks)
 
-                if not advanced_config.postpone_jobs:
+                if not advanced.postpone_jobs:
                     start_scheduler_event.set()
 
                 tasks.add(create_task(self._transactions.cleanup_loop()))
 
-            spawn_index_tasks = (create_task(self._ctx._spawn_index(name)) for name in self._config.indexes)
-            await gather(*spawn_index_tasks)
+            for name in self._config.indexes:
+                await self._ctx._spawn_index(name)
 
             await self._set_up_index_dispatcher(
-                tasks, spawn_datasources_event, start_scheduler_event, advanced_config.early_realtime
+                tasks=tasks,
+                spawn_datasources_event=spawn_datasources_event,
+                start_scheduler_event=start_scheduler_event,
+                early_realtime=advanced.early_realtime,
             )
 
             await gather(*tasks)
 
     async def _create_datasources(self) -> None:
-        datasource: Datasource
-        for name, datasource_config in self._config.datasources.items():
-            if name in self._datasources:
-                continue
-
-            datasource = DatasourceFactory.build(name, self._config)
-
-            self._datasources[name] = datasource
-            self._datasources_by_config[datasource_config] = datasource
+        for name, config in self._config.datasources.items():
+            if name not in self._datasources:
+                self._datasources[name] = create_datasource(config)
 
     async def _initialize_schema(self) -> None:
         self._logger.info('Initializing database schema')
         schema_name = self._config.schema_name
         conn = get_connection()
 
         # NOTE: Try to fetch existing schema, but don't fail yet
@@ -517,40 +624,69 @@
 
         await self._ctx.fire_hook('on_restart')
 
     async def _set_up_transactions(self, stack: AsyncExitStack) -> None:
         await stack.enter_async_context(self._transactions.register())
 
     async def _set_up_database(self, stack: AsyncExitStack) -> None:
+        self._logger.info('Setting up database')
+        database_config = self._config.database
+        if isinstance(database_config, SqliteDatabaseConfig) and database_config.path == ':memory:':
+            self._logger.warning('Using in-memory SQLite database; data will be lost on restart')
+
         await stack.enter_async_context(
             tortoise_wrapper(
                 url=self._config.database.connection_string,
                 models=self._config.package,
                 timeout=self._config.database.connection_timeout,
                 decimal_precision=self._config.advanced.decimal_precision,
+                unsafe_sqlite=self._config.advanced.unsafe_sqlite,
             )
         )
+        await preload_cached_models(self._config.package)
 
     async def _set_up_hooks(self, tasks: set[Task[None]], run: bool = False) -> None:
-        for event_hook_config in event_hooks.values():
-            self._callbacks.register_hook(event_hook_config)
+        for system_hook_config in system_hooks.values():
+            self._ctx.register_hook(system_hook_config)
 
         for hook_config in self._config.hooks.values():
-            self._callbacks.register_hook(hook_config)
+            self._ctx.register_hook(hook_config)
 
         if run:
-            tasks.add(create_task(self._callbacks.run()))
+            tasks.add(create_task(self._ctx._hooks_loop()))
 
     async def _set_up_prometheus(self) -> None:
         if self._config.prometheus:
             from prometheus_client import start_http_server
 
             Metrics.enabled = True
             start_http_server(self._config.prometheus.port, self._config.prometheus.host)
 
+    async def _set_up_api(self, stack: AsyncExitStack) -> None:
+        api_config = self._config.advanced.api
+        if not api_config or env.TEST or env.CI:
+            return
+
+        from aiohttp import web
+
+        from dipdup.api import create_api
+
+        api = await create_api()
+        runner = web.AppRunner(api)
+        await runner.setup()
+        site = web.TCPSite(runner, api_config.host, api_config.port)
+
+        @asynccontextmanager
+        async def _api_wrapper() -> AsyncIterator[None]:
+            await site.start()
+            yield
+            await site.stop()
+
+        await stack.enter_async_context(_api_wrapper())
+
     async def _set_up_hasura(self, stack: AsyncExitStack) -> HasuraGateway | None:
         if not self._config.hasura:
             return None
 
         if not isinstance(self._config.database, PostgresDatabaseConfig):
             raise FrameworkException('PostgresDatabaseConfig expected; check earlier')
 
@@ -565,38 +701,17 @@
     async def _set_up_datasources(self, stack: AsyncExitStack) -> None:
         await self._create_datasources()
         for datasource in self._datasources.values():
             await stack.enter_async_context(datasource)
 
     async def _initialize_datasources(self) -> None:
         for datasource in self._datasources.values():
-            if not isinstance(datasource, TzktDatasource):
-                continue
-
-            head_block = await datasource.get_head_block()
-            datasource.set_network(head_block.chain)
-            datasource.set_sync_level(
-                subscription=None,
-                level=head_block.level,
-            )
-
-            db_head = await Head.filter(name=datasource.name).first()
-            if not db_head:
+            if not isinstance(datasource, IndexDatasource):
                 continue
-
-            # NOTE: Ensure that no reorgs happened while we were offline
-            actual_head = await datasource.get_block(db_head.level)
-            if db_head.hash != actual_head.hash:
-                await self._ctx.reindex(
-                    ReindexingReason.rollback,
-                    datasource=datasource.name,
-                    level=db_head.level,
-                    stored_block_hash=db_head.hash,
-                    actual_block_hash=actual_head.hash,
-                )
+            await datasource.initialize()
 
     async def _set_up_index_dispatcher(
         self,
         tasks: set[Task[None]],
         spawn_datasources_event: Event,
         start_scheduler_event: Event,
         early_realtime: bool,
@@ -607,16 +722,19 @@
                 index_dispatcher.run(
                     spawn_datasources_event,
                     start_scheduler_event,
                     early_realtime,
                 )
             )
         )
+        # FIXME: Initialize with metrics
         if prometheus_config := self._ctx.config.prometheus:
-            tasks.add(create_task(index_dispatcher._update_metrics(prometheus_config.update_interval)))
+            tasks.add(create_task(index_dispatcher._prometheus_loop(prometheus_config.update_interval)))
+        if not self._ctx.config.oneshot:
+            tasks.add(create_task(index_dispatcher._metrics_loop(1)))
 
     async def _spawn_datasources(self, tasks: set[Task[None]]) -> Event:
         event = Event()
 
         async def _event_wrapper() -> None:
             self._logger.info('Waiting for indexes to synchronize before spawning datasources')
             await event.wait()
@@ -636,7 +754,13 @@
         tasks.add(run_task)
 
         # NOTE: Register jobs
         for job_config in self._config.jobs.values():
             scheduler.add_job(self._ctx, job_config)
 
         return event
+
+    async def _set_up_metrics(self, stack: AsyncExitStack) -> None:
+        level = self._config.advanced.metrics
+        metrics.set_level(level)
+        if level == MetricsLevel.full:
+            await stack.enter_async_context(metrics.with_pprofile(self._config.package))
```

### Comparing `dipdup-6.5.9/src/dipdup/env.py` & `dipdup-7.0.0rc1/src/dipdup/env.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 import importlib
+import importlib.util
 import platform
 from contextlib import suppress
 from os import environ as env
 from pathlib import Path
-from typing import cast
 
 
 def get_package_path(package: str) -> Path:
     """Absolute path to the indexer package, existing or default"""
-    global PACKAGE_PATH
 
     # NOTE: Integration tests run in isolated environment
     if TEST:
-        set_package_path(Path.cwd() / package)
+        return Path.cwd() / package
 
-    if PACKAGE_PATH:
-        return PACKAGE_PATH
+    # NOTE: If cwd is a package, use it
+    if Path('pyproject.toml').exists() and Path.cwd().name == package:
+        return Path.cwd()
 
     # NOTE: Detect existing package in current environment
     with suppress(ImportError):
         module = importlib.import_module(package)
         if module.__file__ is None:
-            raise RuntimeError(f'`{module.__name__}` package has no `__file__` attribute')
-        set_package_path(Path(module.__file__).parent)
-        return cast(Path, PACKAGE_PATH)
-
-    # NOTE: Create a new package; try src/<package> layout first.
-    if Path('src').is_dir():
-        set_package_path(Path('src', package))
-    else:
-        set_package_path(Path(package))
+            raise ImportError(f'`{module.__name__}` package has no `__file__` attribute')
+        return Path(module.__file__).parent
 
-    return cast(Path, PACKAGE_PATH)
+    # NOTE: Create a new package
+    return Path.cwd() / package
 
 
 def get(key: str, default: str | None = None) -> str | None:
     return env.get(key, default)
 
 
 def get_bool(key: str, default: bool = False) -> bool:
@@ -56,25 +50,17 @@
 def set_test() -> None:
     global TEST, REPLAY_PATH
     TEST = True
     REPLAY_PATH = str(Path(__file__).parent.parent.parent / 'tests' / 'replays')
     env['DIPDUP_REPLAY_PATH'] = REPLAY_PATH
 
 
-def set_package_path(path: Path) -> None:
-    global PACKAGE_PATH
-    PACKAGE_PATH = path
-    env['DIPDUP_PACKAGE_PATH'] = str(path)
-
-
 if get('CI') == 'true':
     env['DIPDUP_CI'] = '1'
 if platform.system() == 'Linux' and Path('/.dockerenv').exists():
     env['DIPDUP_DOCKER'] = '1'
 
-TEST = get_bool('DIPDUP_TEST')
 CI = get_bool('DIPDUP_CI')
 DOCKER = get_bool('DIPDUP_DOCKER')
 NEXT = get_bool('DIPDUP_NEXT')
-DOCKER_IMAGE = get('DIPDUP_DOCKER_IMAGE')
-PACKAGE_PATH = get_path('DIPDUP_PACKAGE_PATH')
 REPLAY_PATH = get_path('DIPDUP_REPLAY_PATH')
+TEST = get_bool('DIPDUP_TEST')
```

### Comparing `dipdup-6.5.9/src/dipdup/exceptions.py` & `dipdup-7.0.0rc1/src/dipdup/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import textwrap
 from abc import ABC
 from abc import abstractmethod
 from dataclasses import dataclass
 from dataclasses import field
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Type
 
-from tortoise.models import Model
+if TYPE_CHECKING:
+    from tortoise.models import Model
 
-from dipdup.enums import ReindexingReason
+    from dipdup.models import ReindexingReason  # noqa: E402
 
 tab = ('_' * 80) + '\n\n'
 
 
 def unindent(text: str) -> str:
     """Remove indentation from text"""
     return textwrap.dedent(text).strip()
@@ -77,15 +79,15 @@
 
     def _help(self) -> str:
         return f"""
             `{self.datasource}` datasource returned an error.
             
             {self.msg}
 
-            See https://docs.dipdup.io/advanced/datasources
+            See https://docs.dipdup.io/getting-started/datasources
         """
 
 
 @dataclass(repr=False)
 class InvalidRequestError(Error):
     """API returned an unexpected response"""
 
@@ -108,82 +110,59 @@
 
     msg: str
 
     def _help(self) -> str:
         return f"""
             {self.msg}
 
-            See https://docs.dipdup.io/config
+            See https://docs.dipdup.io/getting-started/config
         """
 
 
 @dataclass(repr=False)
 class InvalidModelsError(Error):
     """Can't initialize database, `models.py` module is invalid"""
 
     msg: str
-    model: Type[Model]
+    model: Type['Model']
     field: Optional[str] = None
 
     def _help(self) -> str:
         return f"""
             {self.msg}
 
               model: `{self.model._meta._model.__name__}`
               table: `{self.model._meta.db_table}`
               field: `{self.field or ''}`
 
-            See https://docs.dipdup.io/getting-started/defining-models
-            See https://docs.dipdup.io/config/database
-            See https://docs.dipdup.io/advanced/internal-models
-        """
-
-
-@dataclass(repr=False)
-class DatabaseEngineError(Error):
-    """Some of the features are not supported with the current database engine"""
-
-    msg: str
-    kind: str
-    required: str
-
-    def _help(self) -> str:
-        return f"""
-            {self.msg}
-
-              database: `{self.kind}`
-              required: `{self.required}`
-
-            See https://docs.dipdup.io/deployment/database-engines
-            See https://docs.dipdup.io/advanced/sql
-            See https://docs.dipdup.io/config/database
+            See https://docs.dipdup.io/getting-started/models
         """
 
 
 @dataclass(repr=False)
 class ReindexingRequiredError(Error):
     """Unable to continue indexing with existing database"""
 
-    reason: ReindexingReason
+    reason: 'ReindexingReason'
     context: Dict[str, Any] = field(default_factory=dict)
 
     def _help(self) -> str:
         # FIXME: Indentation hell
         prefix = '\n' + ' ' * 14
         context = prefix.join(f'{k}: {v}' for k, v in self.context.items())
         if context:
             context = '{prefix}{context}\n'.format(prefix=prefix, context=context)
 
         return """
             Reindexing required! Reason: {reason}.
               {context}
             You may want to backup database before proceeding. After that perform one of the following actions:
 
-              * Eliminate the cause of reindexing and run `dipdup schema approve`.
-              * Drop database and start indexing from scratch with `dipdup schema wipe` command.
+              - Eliminate the cause of reindexing and run `dipdup schema approve`.
+              - Drop database and start indexing from scratch with `dipdup schema wipe` command.
 
             See https://docs.dipdup.io/advanced/reindexing for more information.
         """.format(
             reason=self.reason.value,
             context=context,
         )
 
@@ -196,16 +175,16 @@
 
     def _help(self) -> str:
         return f"""
             Project initialization required! Reason: {self.message}.
 
             Perform the following actions:
 
-              * Run `dipdup init`.
-              * Review and commit changes.
+              - Run `dipdup init`.
+              - Review and commit changes.
         """
 
 
 @dataclass(repr=False)
 class ProjectImportError(Error):
     """Can't import type or callback from the project package"""
 
@@ -301,18 +280,18 @@
         return f"""
             `{self.name}` {self.kind} callback was called with an argument of invalid type.
 
               argument: `{self.arg}`
               type: {self.type_}
               expected type: {self.expected_type}
 
-            Make sure to set correct typenames in config and run `dipdup init --overwrite-types` to regenerate typeclasses.
+            Make sure to set correct typenames in config and run `dipdup init --force` to regenerate typeclasses.
 
-            See https://docs.dipdup.io/getting-started/project-structure
-            See https://docs.dipdup.io/cli-reference#init
+            See https://docs.dipdup.io/getting-started/package
+            See https://docs.dipdup.io/references/cli#init
         """
 
 
 @dataclass(repr=False)
 class HasuraError(Error):
     """Failed to configure Hasura instance"""
 
@@ -322,35 +301,15 @@
         return f"""
             Failed to configure Hasura:
 
               {self.msg}
 
             If it's `400 Bad Request`, check out Hasura logs for more information.
 
-            See https://docs.dipdup.io/graphql/
-            See https://docs.dipdup.io/config/hasura
-            See https://docs.dipdup.io/cli-reference#dipdup-hasura-configure
-        """
-
-
-@dataclass(repr=False)
-class FeatureAvailabilityError(Error):
-    """Requested feature is not supported in the current environment"""
-
-    feature: str
-    reason: str
-
-    def _help(self) -> str:
-        return f"""
-            Feature `{self.feature}` is not available in the current environment.
-
-            {self.reason}
-
-            See https://docs.dipdup.io/installation
-            See https://docs.dipdup.io/advanced/docker
+            See https://docs.dipdup.io/graphql/hasura
         """
 
 
 @dataclass(repr=False)
 class UnsupportedAPIError(Error):
     """Datasource instance runs an unsupported software version"""
 
@@ -360,12 +319,7 @@
 
     def _help(self) -> str:
         return f"""
             `{self.host}` API version is not supported by `{self.datasource}` datasource.
 
             {self.reason}
         """
-
-
-# TODO: Remove in 7.0
-DipDupException = FrameworkException
-DipDupError = Error
```

### Comparing `dipdup-6.5.9/src/dipdup/hasura.py` & `dipdup-7.0.0rc1/src/dipdup/hasura.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 from typing import Union
 from typing import cast
 
 import orjson
 from aiohttp import ClientResponseError
 from humps import main as humps
 from pydantic.dataclasses import dataclass
-from tortoise import fields
 
 from dipdup import env
+from dipdup import fields
 from dipdup.config import DEFAULT_POSTGRES_SCHEMA
 from dipdup.config import HasuraConfig
-from dipdup.config import HTTPConfig
+from dipdup.config import HttpConfig
 from dipdup.config import PostgresDatabaseConfig
-from dipdup.config import ResolvedHTTPConfig
+from dipdup.config import ResolvedHttpConfig
+from dipdup.database import get_connection
+from dipdup.database import iter_models
 from dipdup.exceptions import ConfigurationError
 from dipdup.exceptions import FrameworkException
 from dipdup.exceptions import HasuraError
 from dipdup.exceptions import UnsupportedAPIError
 from dipdup.http import HTTPGateway
 from dipdup.models import Schema
 from dipdup.utils import iter_files
 from dipdup.utils import pascal_to_snake
-from dipdup.utils.database import get_connection
-from dipdup.utils.database import iter_models
 
 vulnerable_versions = {
     # NOTE: See https://github.com/hasura/graphql-engine/security/advisories/GHSA-c9rw-rw2f-mj4x
     # NOTE: See https://github.com/hasura/graphql-engine/security/advisories/GHSA-g7mj-g7f4-hgrg
     'v2.21.0-beta': 'v2.21.0-beta.1',
     'v2.15.1': 'v2.15.2',
     'v2.15.0': 'v2.15.2',
@@ -102,34 +102,35 @@
 
     @property
     def root(self) -> str:
         return humps.decamelize(self.name)
 
 
 class HasuraGateway(HTTPGateway):
-    _default_http_config = HTTPConfig(
+    _default_http_config = HttpConfig(
         # NOTE: Fail fast; most Hasura errors are 500's that won't fix by themselves.
         # NOTE: Does not apply to initial healthcheck
         retry_sleep=1,
         retry_multiplier=1.1,
         retry_count=3,
+        alias='hasura',
     )
 
     def __init__(
         self,
         package: str,
         hasura_config: HasuraConfig,
         database_config: PostgresDatabaseConfig,
-        http_config: HTTPConfig | None = None,
+        http_config: HttpConfig | None = None,
     ) -> None:
         super().__init__(
             hasura_config.url,
-            ResolvedHTTPConfig.create(self._default_http_config, http_config),
+            ResolvedHttpConfig.create(self._default_http_config, http_config),
         )
-        self._logger = logging.getLogger('dipdup.hasura')
+        self._logger = logging.getLogger(__name__)
         self._package = package
         self._hasura_config = hasura_config
         self._database_config = database_config
 
     async def configure(self, force: bool = False) -> None:
         """Generate Hasura metadata and apply to instance with credentials from `hasura` config section."""
         # TODO: Validate during config parsing
@@ -240,15 +241,18 @@
             )
 
         # NOTE: See https://github.com/hasura/graphql-engine/security/advisories/GHSA-g7mj-g7f4-hgrg
         if version in vulnerable_versions:
             raise UnsupportedAPIError(
                 self.url,
                 'hasura',
-                f'A critical vulnerability has been discovered in {version}!\n    Update to {vulnerable_versions[version]} or the latest stable version immediately.',
+                (
+                    f'A critical vulnerability has been discovered in {version}!\n    Update to'
+                    f' {vulnerable_versions[version]} or the latest stable version immediately.'
+                ),
             )
 
         self._logger.info('Connected to Hasura %s', version)
 
     async def _create_source(self) -> dict[str, Any]:
         self._logger.info(f'Adding source `{self._hasura_config.source}`')
         return await self._hasura_request(
@@ -268,20 +272,22 @@
                     'replace_configuration': True,
                 },
             },
         )
 
     async def _fetch_metadata(self) -> dict[str, Any]:
         self._logger.info('Fetching existing metadata')
-        return await self._hasura_request(
-            endpoint='metadata',
-            json={
-                'type': 'export_metadata',
-                'args': {},
-            },
+        return dict(
+            await self._hasura_request(
+                endpoint='metadata',
+                json={
+                    'type': 'export_metadata',
+                    'args': {},
+                },
+            )
         )
 
     def _hash_metadata(self, metadata: dict[str, Any]) -> str:
         return hashlib.sha256(orjson.dumps(metadata)).hexdigest()
 
     async def _replace_metadata(self, metadata: dict[str, Any]) -> None:
         self._logger.info('Replacing metadata')
@@ -315,16 +321,17 @@
 
     async def _get_views(self) -> list[str]:
         conn = get_connection()
         views = [
             row[0]
             for row in (
                 await conn.execute_query(
-                    f"SELECT table_name FROM information_schema.views WHERE table_schema = '{self._database_config.schema_name}' UNION "
-                    f"SELECT matviewname as table_name FROM pg_matviews WHERE schemaname = '{self._database_config.schema_name}'"
+                    "SELECT table_name FROM information_schema.views WHERE table_schema ="
+                    f" '{self._database_config.schema_name}' UNION SELECT matviewname as table_name FROM pg_matviews"
+                    f" WHERE schemaname = '{self._database_config.schema_name}'"
                 )
             )[1]
         ]
         self._logger.info('Found %s regular and materialized views', len(views))
         return views
 
     def _iterate_graphql_queries(self) -> Iterator[tuple[str, str]]:
@@ -544,25 +551,17 @@
             raise ConfigurationError(f'Table `{table}` has no column `{filter}`') from e
 
         query_arg = f'${filter_field.name}: {filter_field.type}!'
         query_filter = filter_field.name + ': $' + filter_field.name
         query_fields = ' '.join(f.name for f in fields)
         return {
             'name': name,
-            'query': 'query '
-            + name
-            + ' ('
-            + query_arg
-            + ') {'
-            + table
-            + '('
-            + query_filter
-            + ') {'
-            + query_fields
-            + '}}',
+            'query': (
+                'query ' + name + ' (' + query_arg + ') {' + table + '(' + query_filter + ') {' + query_fields + '}}'
+            ),
         }
 
     def _format_rest_head_status_query(self) -> dict[str, Any]:
         name = 'dipdup_head_status'
         if self._hasura_config.camel_case:
             name = humps.camelize(name)
```

### Comparing `dipdup-6.5.9/src/dipdup/http.py` & `dipdup-7.0.0rc1/src/dipdup/http.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 import asyncio
 import hashlib
 import logging
 import platform
 import sys
+import time
 from contextlib import AbstractAsyncContextManager
 from contextlib import suppress
 from http import HTTPStatus
 from json import JSONDecodeError
 from pathlib import Path
 from typing import Any
+from typing import Literal
 from typing import Mapping
 from typing import Optional
 from typing import cast
+from typing import overload
 from urllib.parse import urlsplit
 from urllib.parse import urlunsplit
 
 import aiohttp
 import aiohttp.test_utils
 import orjson
 from aiolimiter import AsyncLimiter
 
 from dipdup import __version__
-from dipdup.config import ResolvedHTTPConfig
+from dipdup.config import ResolvedHttpConfig
 from dipdup.exceptions import FrameworkException
 from dipdup.exceptions import InvalidRequestError
+from dipdup.performance import metrics
 from dipdup.prometheus import Metrics
+from dipdup.utils import json_dumps
 
-exceptions_to_retry = (
+safe_exceptions = (
+    asyncio.TimeoutError,
     aiohttp.ClientConnectionError,
     aiohttp.ClientConnectorError,
     aiohttp.ClientResponseError,
     aiohttp.ClientPayloadError,
-    # NOTE: aiohttp doesn't reraise it
-    asyncio.TimeoutError,
 )
 
 
 class HTTPGateway(AbstractAsyncContextManager[None]):
     """Base class for datasources which connect to remote HTTP endpoints"""
 
-    def __init__(self, url: str, http_config: ResolvedHTTPConfig) -> None:
+    def __init__(self, url: str, http_config: ResolvedHttpConfig) -> None:
         self._http_config = http_config
         self._http = _HTTPGateway(url, self._http_config)
 
     async def __aenter__(self) -> None:
         """Create underlying aiohttp session"""
         await self._http.__aenter__()
 
@@ -72,18 +76,19 @@
 
 
 class _HTTPGateway(AbstractAsyncContextManager[None]):
     """Wrapper for aiohttp HTTP requests.
 
     Covers caching, retrying failed requests and ratelimiting"""
 
-    def __init__(self, url: str, config: ResolvedHTTPConfig) -> None:
-        self._logger = logging.getLogger('dipdup.http')
+    def __init__(self, url: str, config: ResolvedHttpConfig) -> None:
+        self._logger = logging.getLogger(__name__)
         parsed_url = urlsplit(url)
         self._url = urlunsplit((parsed_url.scheme, parsed_url.netloc, '', '', ''))
+        self._alias = config.alias or parsed_url.netloc
         self._path = parsed_url.path
         self._config = config
         self._user_agent_args: tuple[str, ...] = ()
         self._user_agent: Optional[str] = None
         self._ratelimiter = (
             AsyncLimiter(max_rate=config.ratelimit_rate, time_period=config.ratelimit_period)
             if config.ratelimit_rate and config.ratelimit_period
@@ -91,15 +96,15 @@
         )
         self.__session: Optional[aiohttp.ClientSession] = None
 
     async def __aenter__(self) -> None:
         """Create underlying aiohttp session"""
         self.__session = aiohttp.ClientSession(
             base_url=self._url,
-            json_serialize=lambda *a, **kw: orjson.dumps(*a, **kw).decode(),
+            json_serialize=lambda *a, **kw: json_dumps(*a, **kw).decode(),
             connector=aiohttp.TCPConnector(limit=self._config.connection_limit),
             timeout=aiohttp.ClientTimeout(total=self._config.connection_timeout),
         )
 
     async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: Any) -> None:
         """Close underlying aiohttp session"""
         self._logger.debug('Closing gateway session (%s)', self._url)
@@ -147,15 +152,15 @@
             try:
                 return await self._request(
                     method=method,
                     url=url,
                     weight=weight,
                     **kwargs,
                 )
-            except exceptions_to_retry as e:
+            except safe_exceptions as e:
                 if self._config.retry_count and attempt - 1 == self._config.retry_count:
                     raise e
 
                 ratelimit_sleep: float | None = None
                 if isinstance(e, aiohttp.ClientResponseError):
                     if Metrics.enabled:
                         Metrics.set_http_error(self._url, e.status)
@@ -173,46 +178,85 @@
                 self._logger.warning('HTTP request attempt %s/%s failed: %s', attempt, retry_count_str, e)
                 self._logger.info('Waiting %s seconds before retry', ratelimit_sleep or retry_sleep)
                 await asyncio.sleep(ratelimit_sleep or retry_sleep)
                 attempt += 1
                 if not ratelimit_sleep:
                     retry_sleep *= self._config.retry_multiplier
 
+    # FIXME: Temporary overload for Subsquid; move to public method
+    @overload
+    async def _request(
+        self,
+        method: str,
+        url: str,
+        weight: int,
+        raw: Literal[True],
+        **kwargs: Any,
+    ) -> aiohttp.ClientResponse:
+        ...
+
+    @overload
+    async def _request(
+        self,
+        method: str,
+        url: str,
+        weight: int,
+        raw: Literal[False],
+        **kwargs: Any,
+    ) -> Any:
+        ...
+
     async def _request(
         self,
         method: str,
         url: str,
         weight: int = 1,
+        raw: bool = False,
         **kwargs: Any,
     ) -> Any:
         """Wrapped aiohttp call with preconfigured headers and ratelimiting"""
-        url = f"{self._path.rstrip('/')}/{url}"
+        metrics and metrics.inc(f'{self._alias}:requests_total', 1.0)
+        if not url:
+            url = self._path
+        elif url.startswith('http'):
+            url = url.replace(self._url, '').rstrip('/')
+        else:
+            url = f"{self._path.rstrip('/')}/{url}"
+
         headers = kwargs.pop('headers', {})
         headers['User-Agent'] = self.user_agent
 
         params = kwargs.get('params', {})
         params_string = '&'.join(f'{k}={v}' for k, v in params.items())
         request_string = f'{self._url}{url}?{params_string}'.rstrip('?')
         self._logger.debug('Calling `%s`', request_string)
 
         if self._ratelimiter:
             await self._ratelimiter.acquire(weight)
 
+        started_at = time.time()
+
         async with self._session.request(
             method=method,
             url=url,
             headers=headers,
             raise_for_status=True,
             **kwargs,
         ) as response:
+            await response.read()
+            metrics and metrics.inc(f'{self._alias}:time_in_requests', (time.time() - started_at) / 60)
+            if raw:
+                return response
+
+            # NOTE: Use raw=True if fail on 204 is not a desired behavior
             if response.status == HTTPStatus.NO_CONTENT:
                 raise InvalidRequestError('204 No Content', request_string)
-            with suppress(JSONDecodeError, aiohttp.ContentTypeError):
-                return await response.json(loads=orjson.loads)
-            return await response.read()
+            with suppress(JSONDecodeError):
+                return orjson.loads(response._body)
+            return response._body
 
     async def _replay_request(
         self,
         method: str,
         url: str,
         weight: int = 1,
         **kwargs: Any,
@@ -238,15 +282,15 @@
             return content
 
         response = await self._retry_request(method, url, weight, **kwargs)
         replay_path.touch(exist_ok=True)
         if isinstance(response, bytes):
             replay_path.write_bytes(response)
         else:
-            replay_path.write_bytes(orjson.dumps(response))
+            replay_path.write_bytes(json_dumps(response))
 
         return response
 
     async def request(
         self,
         method: str,
         url: str,
```

### Comparing `dipdup-6.5.9/src/dipdup/index.py` & `dipdup-7.0.0rc1/src/dipdup/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,54 +4,53 @@
 from contextlib import ExitStack
 from typing import Any
 from typing import Generic
 from typing import TypeVar
 from typing import cast
 
 import dipdup.models as models
-from dipdup.config import HeadIndexConfig
 from dipdup.config import ResolvedIndexConfigU
 from dipdup.context import DipDupContext
-from dipdup.context import rolled_back_indexes
-from dipdup.datasources.datasource import IndexDatasource
-from dipdup.enums import IndexStatus
-from dipdup.enums import MessageType
+from dipdup.datasources import IndexDatasource
 from dipdup.exceptions import FrameworkException
+from dipdup.models import IndexStatus
+from dipdup.performance import queues
 from dipdup.prometheus import Metrics
 from dipdup.utils import FormattedLogger
 
 IndexConfigT = TypeVar('IndexConfigT', bound=ResolvedIndexConfigU)
 IndexQueueItemT = TypeVar('IndexQueueItemT', bound=Any)
-IndexDatasourceT = TypeVar('IndexDatasourceT', bound=IndexDatasource)
+IndexDatasourceT = TypeVar('IndexDatasourceT', bound=IndexDatasource[Any])
 
 
 class Index(ABC, Generic[IndexConfigT, IndexQueueItemT, IndexDatasourceT]):
     """Base class for index implementations
 
     Provides common interface for managing index state and switching between sync and realtime modes.
     """
 
-    message_type: MessageType
+    message_type: Any
 
-    def __init_subclass__(cls, message_type: MessageType) -> None:
+    def __init_subclass__(cls, message_type: Any) -> None:
         cls.message_type = message_type
         return super().__init_subclass__()
 
     def __init__(
         self,
         ctx: DipDupContext,
         config: IndexConfigT,
         datasource: IndexDatasourceT,
     ) -> None:
         self._ctx = ctx
         self._config = config
         self._datasource = datasource
         self._queue: deque[IndexQueueItemT] = deque()
+        queues.add_queue(self._queue, f'index_realtime:{config.name}')
 
-        self._logger = FormattedLogger('dipdup.index', fmt=f'{config.name}: ' + '{}')
+        self._logger = FormattedLogger(__name__, fmt=f'{config.name}: ' + '{}')
         self._state: models.Index | None = None
 
     def push_realtime_message(self, message: IndexQueueItemT) -> None:
         """Push message to the queue"""
         self._queue.append(message)
 
         if Metrics.enabled:
@@ -79,23 +78,24 @@
     def state(self) -> models.Index:
         if self._state is None:
             raise FrameworkException('Index state is not initialized')
         return self._state
 
     @property
     def synchronized(self) -> bool:
-        return self.state.status == IndexStatus.REALTIME
+        return self.state.status == IndexStatus.realtime
 
     @property
     def realtime(self) -> bool:
-        return self.state.status == IndexStatus.REALTIME and not self._queue
+        return self.state.status == IndexStatus.realtime and not self._queue
 
     def get_sync_level(self) -> int:
         """Get level index needs to be synchronized to depending on its subscription status"""
-        sync_levels = {self.datasource.get_sync_level(s) for s in self._config.subscriptions}
+        subs = self._config.get_subscriptions()
+        sync_levels = {self.datasource.get_sync_level(s) for s in subs}
         if not sync_levels:
             raise FrameworkException('Initialize config before starting `IndexDispatcher`')
         if None in sync_levels:
             raise FrameworkException('Call `set_sync_level` before starting `IndexDispatcher`')
         # NOTE: Multiple sync levels means index with new subscriptions was added in runtime.
         # NOTE: Choose the highest level; outdated realtime messages will be dropped from the queue anyway.
         return max(cast(set[int], sync_levels))
@@ -105,15 +105,15 @@
             raise FrameworkException('Index state is already initialized')
 
         if state:
             self._state = state
             return
 
         index_level = 0
-        if not isinstance(self._config, HeadIndexConfig) and self._config.first_level:
+        if self._config.first_level:
             # NOTE: Be careful there: index has not reached the first level yet
             index_level = self._config.first_level - 1
 
         self._state, _ = await models.Index.get_or_create(
             name=self._config.name,
             type=self._config.kind,
             defaults={
@@ -121,23 +121,23 @@
                 'config_hash': self._config.hash(),
                 'template': self._config.parent.name if self._config.parent else None,
                 'template_values': self._config.template_values,
             },
         )
 
     async def process(self) -> bool:
-        if self.state.status == IndexStatus.ONESHOT:
+        if self.state.status == IndexStatus.disabled:
             raise FrameworkException('Index is in oneshot state and cannot be processed')
 
-        if self.name in rolled_back_indexes:
+        if self.name in self._ctx._rolled_back_indexes:
             await self.state.refresh_from_db(('level',))
-            rolled_back_indexes.remove(self.name)
+            self._ctx._rolled_back_indexes.remove(self.name)
 
         last_level = self._config.last_level
-        if last_level and not isinstance(self._config, HeadIndexConfig):
+        if last_level:
             with ExitStack() as stack:
                 if Metrics.enabled:
                     stack.enter_context(Metrics.measure_total_sync_duration())
                 await self._synchronize(last_level)
                 await self._enter_disabled_state(last_level)
                 return True
 
@@ -168,31 +168,32 @@
 
         if index_level == head_level:
             return None
         if index_level > head_level:
             raise FrameworkException(f'Attempt to synchronize index from level {index_level} to level {head_level}')
 
         self._logger.info('Synchronizing index to level %s', head_level)
-        await self._update_state(status=IndexStatus.SYNCING, level=index_level)
+        await self._update_state(status=IndexStatus.syncing, level=index_level)
         return index_level
 
     async def _exit_sync_state(self, head_level: int) -> None:
         self._logger.info('Index is synchronized to level %s', head_level)
         if Metrics.enabled:
             Metrics.set_levels_to_sync(self._config.name, 0)
-        await self._update_state(status=IndexStatus.REALTIME, level=head_level)
+        await self._update_state(status=IndexStatus.realtime, level=head_level)
 
     async def _enter_disabled_state(self, last_level: int) -> None:
         self._logger.info('Index is synchronized to level %s', last_level)
         if Metrics.enabled:
             Metrics.set_levels_to_sync(self._config.name, 0)
-        await self._update_state(status=IndexStatus.ONESHOT, level=last_level)
+        await self._update_state(status=IndexStatus.disabled, level=last_level)
 
     async def _update_state(
         self,
         status: IndexStatus | None = None,
         level: int | None = None,
     ) -> None:
         state = self.state
+        self._logger.debug('Status %s (was %s) at %s (was %s)', status, state.status, level, state.level)
         state.status = status or state.status
         state.level = level or state.level
         await state.save()
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/big_map/index.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from contextlib import ExitStack
 from datetime import datetime
 from typing import Any
 
-from dipdup.config import BigMapHandlerConfig
-from dipdup.config import BigMapIndexConfig
-from dipdup.datasources.tzkt.datasource import TzktDatasource
-from dipdup.enums import MessageType
-from dipdup.enums import SkipHistory
+from dipdup.config.tezos_tzkt_big_maps import TzktBigMapsHandlerConfig
+from dipdup.config.tezos_tzkt_big_maps import TzktBigMapsIndexConfig
+from dipdup.datasources.tezos_tzkt import TzktDatasource
 from dipdup.exceptions import ConfigInitializationException
 from dipdup.exceptions import ConfigurationError
 from dipdup.exceptions import FrameworkException
 from dipdup.index import Index
-from dipdup.indexes.big_map.fetcher import BigMapFetcher
-from dipdup.indexes.big_map.fetcher import get_big_map_pairs
-from dipdup.indexes.big_map.matcher import match_big_maps
-from dipdup.models import BigMapAction
-from dipdup.models import BigMapData
-from dipdup.models import BigMapDiff
+from dipdup.indexes.tezos_tzkt_big_maps.fetcher import BigMapFetcher
+from dipdup.indexes.tezos_tzkt_big_maps.fetcher import get_big_map_pairs
+from dipdup.indexes.tezos_tzkt_big_maps.matcher import match_big_maps
+from dipdup.models import SkipHistory
+from dipdup.models.tezos_tzkt import TzktBigMapAction
+from dipdup.models.tezos_tzkt import TzktBigMapData
+from dipdup.models.tezos_tzkt import TzktBigMapDiff
+from dipdup.models.tezos_tzkt import TzktMessageType
 from dipdup.prometheus import Metrics
 
-BigMapQueueItem = tuple[BigMapData, ...]
+BigMapQueueItem = tuple[TzktBigMapData, ...]
 
 
-class BigMapIndex(
-    Index[BigMapIndexConfig, BigMapQueueItem, TzktDatasource],
-    message_type=MessageType.big_map,
+class TzktBigMapsIndex(
+    Index[TzktBigMapsIndexConfig, BigMapQueueItem, TzktDatasource],
+    message_type=TzktMessageType.big_map,
 ):
     def push_big_maps(self, big_maps: BigMapQueueItem) -> None:
         """Push big map diffs to queue"""
         self.push_realtime_message(big_maps)
 
     async def _process_queue(self) -> None:
         """Process WebSocket queue"""
@@ -90,75 +90,75 @@
         for address, path in big_map_pairs:
             async for contract_big_maps in self._datasource.iter_contract_big_maps(address):
                 for contract_big_map in contract_big_maps:
                     if contract_big_map['path'] == path:
                         big_map_ids.add((int(contract_big_map['ptr']), address, path))
 
         # NOTE: Do not use `_process_level_big_maps` here; we want to maintain transaction manually.
-        async with self._ctx._transactions.in_transaction(head_level, head_level, self.name):
+        async with self._ctx.transactions.in_transaction(head_level, head_level, self.name):
             for big_map_id, address, path in big_map_ids:
                 async for big_map_keys in self._datasource.iter_big_map(big_map_id, head_level):
                     big_map_data = tuple(
-                        BigMapData(
+                        TzktBigMapData(
                             id=big_map_key['id'],
                             level=head_level,
                             operation_id=head_level,
                             timestamp=datetime.now(),
                             bigmap=big_map_id,
                             contract_address=address,
                             path=path,
-                            action=BigMapAction.ADD_KEY,
+                            action=TzktBigMapAction.ADD_KEY,
                             active=big_map_key['active'],
                             key=big_map_key['key'],
                             value=big_map_key['value'],
                         )
                         for big_map_key in big_map_keys
                     )
-                    matched_handlers = match_big_maps(self._config.handlers, big_map_data)
+                    matched_handlers = match_big_maps(self._ctx.package, self._config.handlers, big_map_data)
                     for handler_config, big_map_diff in matched_handlers:
                         await self._call_matched_handler(handler_config, big_map_diff)
 
             await self._update_state(level=head_level)
 
     async def _process_level_big_maps(
         self,
-        big_maps: tuple[BigMapData, ...],
+        big_maps: tuple[TzktBigMapData, ...],
         sync_level: int,
     ) -> None:
         if not big_maps:
             return
 
         batch_level = big_maps[0].level
         index_level = self.state.level
         if batch_level <= index_level:
             raise FrameworkException(f'Batch level is lower than index level: {batch_level} <= {index_level}')
 
         self._logger.debug('Processing big map diffs of level %s', batch_level)
-        matched_handlers = match_big_maps(self._config.handlers, big_maps)
+        matched_handlers = match_big_maps(self._ctx.package, self._config.handlers, big_maps)
 
         if Metrics.enabled:
             Metrics.set_index_handlers_matched(len(matched_handlers))
 
         # NOTE: We still need to bump index level but don't care if it will be done in existing transaction
         if not matched_handlers:
             await self._update_state(level=batch_level)
             return
 
-        async with self._ctx._transactions.in_transaction(batch_level, sync_level, self.name):
+        async with self._ctx.transactions.in_transaction(batch_level, sync_level, self.name):
             for handler_config, big_map_diff in matched_handlers:
                 await self._call_matched_handler(handler_config, big_map_diff)
             await self._update_state(level=batch_level)
 
     async def _call_matched_handler(
-        self, handler_config: BigMapHandlerConfig, big_map_diff: BigMapDiff[Any, Any]
+        self, handler_config: TzktBigMapsHandlerConfig, big_map_diff: TzktBigMapDiff[Any, Any]
     ) -> None:
         if not handler_config.parent:
             raise ConfigInitializationException
 
-        await self._ctx._fire_handler(
+        await self._ctx.fire_handler(
             handler_config.callback,
             handler_config.parent.name,
             self.datasource,
             # NOTE: missing `operation_id` field in API to identify operation
             None,
             big_map_diff,
         )
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/big_map/matcher.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_big_maps/matcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,75 @@
 import logging
 from collections import deque
 from typing import Any
 from typing import Iterable
 
-from dipdup.config import BigMapHandlerConfig
-from dipdup.models import BigMapData
-from dipdup.models import BigMapDiff
-from dipdup.utils.codegen import parse_object
+from pydantic import BaseModel
+
+from dipdup.codegen.tezos_tzkt import get_big_map_key_type
+from dipdup.codegen.tezos_tzkt import get_big_map_value_type
+from dipdup.config.tezos_tzkt_big_maps import TzktBigMapsHandlerConfig
+from dipdup.models.tezos_tzkt import TzktBigMapData
+from dipdup.models.tezos_tzkt import TzktBigMapDiff
+from dipdup.package import DipDupPackage
+from dipdup.utils import parse_object
 
 _logger = logging.getLogger('dipdup.matcher')
 
-MatchedBigMapsT = tuple[BigMapHandlerConfig, BigMapDiff[Any, Any]]
+MatchedBigMapsT = tuple[TzktBigMapsHandlerConfig, TzktBigMapDiff[Any, Any]]
 
 
 def prepare_big_map_handler_args(
-    handler_config: BigMapHandlerConfig,
-    matched_big_map: BigMapData,
-) -> BigMapDiff[Any, Any]:
+    package: DipDupPackage,
+    handler_config: TzktBigMapsHandlerConfig,
+    matched_big_map: TzktBigMapData,
+) -> TzktBigMapDiff[Any, Any]:
     """Prepare handler arguments, parse key and value. Schedule callback in executor."""
-    _logger.info('%s: `%s` handler matched!', matched_big_map.operation_id, handler_config.callback)
+    _logger.debug('%s: `%s` handler matched!', matched_big_map.operation_id, handler_config.callback)
+
+    key: BaseModel | None = None
+    value: BaseModel | None = None
 
-    if matched_big_map.action.has_key:
-        type_ = handler_config.key_type_cls
+    if matched_big_map.action.has_key and matched_big_map.key is not None:
+        type_ = get_big_map_key_type(package, handler_config.contract.module_name, handler_config.path)
         key = parse_object(type_, matched_big_map.key) if type_ else None
-    else:
-        key = None
 
-    if matched_big_map.action.has_value:
-        type_ = handler_config.value_type_cls
+    if matched_big_map.action.has_value and matched_big_map.value is not None:
+        type_ = get_big_map_value_type(package, handler_config.contract.module_name, handler_config.path)
         value = parse_object(type_, matched_big_map.value) if type_ else None
-    else:
-        value = None
 
-    return BigMapDiff(
+    return TzktBigMapDiff(
         data=matched_big_map,
         action=matched_big_map.action,
         key=key,
         value=value,
     )
 
 
 def match_big_map(
-    handler_config: BigMapHandlerConfig,
-    big_map: BigMapData,
+    handler_config: TzktBigMapsHandlerConfig,
+    big_map: TzktBigMapData,
 ) -> bool:
     """Match single big map diff with pattern"""
     if handler_config.path != big_map.path:
         return False
     if handler_config.contract.address != big_map.contract_address:
         return False
     return True
 
 
 def match_big_maps(
-    handlers: Iterable[BigMapHandlerConfig],
-    big_maps: Iterable[BigMapData],
+    package: DipDupPackage,
+    handlers: Iterable[TzktBigMapsHandlerConfig],
+    big_maps: Iterable[TzktBigMapData],
 ) -> deque[MatchedBigMapsT]:
     """Try to match big map diffs with all index handlers."""
     matched_handlers: deque[MatchedBigMapsT] = deque()
 
     for handler_config in handlers:
         for big_map in big_maps:
             big_map_matched = match_big_map(handler_config, big_map)
             if big_map_matched:
-                arg = prepare_big_map_handler_args(handler_config, big_map)
+                arg = prepare_big_map_handler_args(package, handler_config, big_map)
                 matched_handlers.append((handler_config, arg))
 
     return matched_handlers
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/event/fetcher.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/fetcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from __future__ import annotations
 
 import logging
 from typing import AsyncGenerator
 
-from dipdup.datasources.tzkt.datasource import TzktDatasource
+from dipdup.datasources.tezos_tzkt import TzktDatasource
 from dipdup.fetcher import DataFetcher
-from dipdup.fetcher import yield_by_level
-from dipdup.models import EventData
+from dipdup.fetcher import readahead_by_level
+from dipdup.models.tezos_tzkt import TzktEventData
 
 
-class EventFetcher(DataFetcher[EventData]):
+class EventFetcher(DataFetcher[TzktEventData]):
     """Fetches contract events from REST API, merges them and yields by level."""
 
+    _datasource: TzktDatasource
+
     def __init__(
         self,
-        datasource: 'TzktDatasource',
+        datasource: TzktDatasource,
         first_level: int,
         last_level: int,
         event_addresses: set[str],
         event_tags: set[str],
     ) -> None:
-        self._logger = logging.getLogger('dipdup.tzkt')
+        self._logger = logging.getLogger('dipdup.fetcher')
         self._datasource = datasource
         self._first_level = first_level
         self._last_level = last_level
         self._event_addresses = event_addresses
         self._event_tags = event_tags
 
-    async def fetch_by_level(self) -> AsyncGenerator[tuple[int, tuple[EventData, ...]], None]:
+    async def fetch_by_level(self) -> AsyncGenerator[tuple[int, tuple[TzktEventData, ...]], None]:
         """Iterate over events fetched fetched from REST.
 
-        Resulting data is splitted by level, deduped, sorted and ready to be processed by EventIndex.
+        Resulting data is splitted by level, deduped, sorted and ready to be processed by TzktEventsIndex.
         """
         event_iter = self._datasource.iter_events(
             self._event_addresses,
             self._event_tags,
             self._first_level,
             self._last_level,
         )
-        async for level, batch in yield_by_level(event_iter):
+        async for level, batch in readahead_by_level(event_iter, limit=5_000):
             yield level, batch
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/event/index.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_events/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from contextlib import ExitStack
 from typing import Any
 
-from dipdup.config import EventHandlerConfig
-from dipdup.config import EventHandlerConfigU
-from dipdup.config import EventIndexConfig
-from dipdup.datasources.tzkt.datasource import TzktDatasource
-from dipdup.enums import MessageType
+from dipdup.config.tezos_tzkt_events import TzktEventsHandlerConfig
+from dipdup.config.tezos_tzkt_events import TzktEventsHandlerConfigU
+from dipdup.config.tezos_tzkt_events import TzktEventsIndexConfig
+from dipdup.datasources.tezos_tzkt import TzktDatasource
 from dipdup.exceptions import ConfigInitializationException
 from dipdup.exceptions import FrameworkException
 from dipdup.index import Index
-from dipdup.indexes.event.fetcher import EventFetcher
-from dipdup.indexes.event.matcher import match_events
-from dipdup.models import Event
-from dipdup.models import EventData
-from dipdup.models import UnknownEvent
+from dipdup.indexes.tezos_tzkt_events.fetcher import EventFetcher
+from dipdup.indexes.tezos_tzkt_events.matcher import match_events
+from dipdup.models.tezos_tzkt import TzktEvent
+from dipdup.models.tezos_tzkt import TzktEventData
+from dipdup.models.tezos_tzkt import TzktMessageType
+from dipdup.models.tezos_tzkt import TzktUnknownEvent
 from dipdup.prometheus import Metrics
 
-EventQueueItem = tuple[EventData, ...]
+EventQueueItem = tuple[TzktEventData, ...]
 
 
-class EventIndex(
-    Index[EventIndexConfig, EventQueueItem, TzktDatasource],
-    message_type=MessageType.event,
+class TzktEventsIndex(
+    Index[TzktEventsIndexConfig, EventQueueItem, TzktDatasource],
+    message_type=TzktMessageType.event,
 ):
     def push_events(self, events: EventQueueItem) -> None:
         self.push_realtime_message(events)
 
     async def _process_queue(self) -> None:
         """Process WebSocket queue"""
         if self._queue:
@@ -70,51 +70,51 @@
                     stack.enter_context(Metrics.measure_level_sync_duration())
                 await self._process_level_events(events, sync_level)
 
         await self._exit_sync_state(sync_level)
 
     async def _process_level_events(
         self,
-        events: tuple[EventData, ...],
+        events: tuple[TzktEventData, ...],
         sync_level: int,
     ) -> None:
         if not events:
             return
 
         batch_level = events[0].level
         index_level = self.state.level
         if batch_level <= index_level:
             raise FrameworkException(f'Batch level is lower than index level: {batch_level} <= {index_level}')
 
         self._logger.debug('Processing contract events of level %s', batch_level)
-        matched_handlers = match_events(self._config.handlers, events)
+        matched_handlers = match_events(self._ctx.package, self._config.handlers, events)
 
         if Metrics.enabled:
             Metrics.set_index_handlers_matched(len(matched_handlers))
 
         # NOTE: We still need to bump index level but don't care if it will be done in existing transaction
         if not matched_handlers:
             await self._update_state(level=batch_level)
             return
 
-        async with self._ctx._transactions.in_transaction(batch_level, sync_level, self.name):
+        async with self._ctx.transactions.in_transaction(batch_level, sync_level, self.name):
             for handler_config, event in matched_handlers:
                 await self._call_matched_handler(handler_config, event)
             await self._update_state(level=batch_level)
 
     async def _call_matched_handler(
-        self, handler_config: EventHandlerConfigU, event: Event[Any] | UnknownEvent
+        self, handler_config: TzktEventsHandlerConfigU, event: TzktEvent[Any] | TzktUnknownEvent
     ) -> None:
-        if isinstance(handler_config, EventHandlerConfig) != isinstance(event, Event):
+        if isinstance(handler_config, TzktEventsHandlerConfig) != isinstance(event, TzktEvent):
             raise FrameworkException(f'Invalid handler config and event types: {handler_config}, {event}')
 
         if not handler_config.parent:
             raise ConfigInitializationException
 
-        await self._ctx._fire_handler(
+        await self._ctx.fire_handler(
             handler_config.callback,
             handler_config.parent.name,
             self.datasource,
             str(event.data.transaction_id),
             event,
         )
 
@@ -125,10 +125,10 @@
             addresses.add(handler_config.contract.get_address())
         return addresses
 
     def _get_event_tags(self) -> set[str]:
         """Get tags to fetch events during initial synchronization"""
         paths = set()
         for handler_config in self._config.handlers:
-            if isinstance(handler_config, EventHandlerConfig):
+            if isinstance(handler_config, TzktEventsHandlerConfig):
                 paths.add(handler_config.tag)
         return paths
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/head/index.py` & `dipdup-7.0.0rc1/tests/test_dipdup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,81 @@
-from dipdup.config import HeadHandlerConfig
-from dipdup.config import HeadIndexConfig
-from dipdup.datasources.tzkt.datasource import TzktDatasource
-from dipdup.enums import IndexStatus
-from dipdup.enums import MessageType
-from dipdup.exceptions import ConfigInitializationException
-from dipdup.exceptions import FrameworkException
-from dipdup.index import Index
-from dipdup.models import HeadBlockData
-
-HeadQueueItem = HeadBlockData
-
-
-class HeadIndex(
-    Index[HeadIndexConfig, HeadQueueItem, TzktDatasource],
-    message_type=MessageType.head,
-):
-    def push_head(self, events: HeadQueueItem) -> None:
-        self.push_realtime_message(events)
-
-    async def _synchronize(self, sync_level: int) -> None:
-        self._logger.info('Setting index level to %s and moving on', sync_level)
-        await self._update_state(status=IndexStatus.REALTIME, level=sync_level)
-
-    async def _process_queue(self) -> None:
-        while self._queue:
-            head = self._queue.popleft()
-            message_level = head.level
-            if message_level <= self.state.level:
-                self._logger.debug('Skipping outdated message: %s <= %s', message_level, self.state.level)
-                continue
-
-            self._logger.debug('Processing head realtime message, %s left in queue', len(self._queue))
-
-            batch_level = head.level
-            index_level = self.state.level
-            if batch_level <= index_level:
-                raise FrameworkException(f'Batch level is lower than index level: {batch_level} <= {index_level}')
-
-            async with self._ctx._transactions.in_transaction(batch_level, message_level, self.name):
-                self._logger.debug('Processing head info of level %s', batch_level)
-                for handler_config in self._config.handlers:
-                    await self._call_matched_handler(handler_config, head)
-                await self._update_state(level=batch_level)
-
-    async def _call_matched_handler(self, handler_config: HeadHandlerConfig, head: HeadBlockData) -> None:
-        if not handler_config.parent:
-            raise ConfigInitializationException
-
-        await self._ctx._fire_handler(
-            handler_config.callback,
-            handler_config.parent.name,
-            self.datasource,
-            head.hash,
-            head,
-        )
+from contextlib import AsyncExitStack
+from datetime import datetime
+from pathlib import Path
+
+import pytest
+from pytz import UTC
+
+from dipdup.config import DipDupConfig
+from dipdup.dipdup import DipDup
+from dipdup.dipdup import IndexDispatcher
+from dipdup.exceptions import ReindexingRequiredError
+from dipdup.models import Index
+from dipdup.models import IndexStatus
+from dipdup.models import IndexType
+
+
+async def _create_index(hash_: str) -> None:
+    await Index.create(
+        level=1365000,
+        name='hen_mainnet',
+        template=None,
+        config_hash=hash_,
+        created_at=datetime(2021, 10, 8, 18, 43, 35, 744412, tzinfo=UTC),
+        template_values={},
+        status=IndexStatus.new,
+        updated_at=datetime(2021, 10, 8, 18, 43, 35, 744449, tzinfo=UTC),
+        type=IndexType.tezos_tzkt_operations,
+    )
+
+
+async def spawn_index(dispatcher: IndexDispatcher, name: str) -> None:
+    await dispatcher._ctx._spawn_index(name)
+    dispatcher._indexes[name] = dispatcher._ctx._pending_indexes.pop()
+
+
+class IndexStateTest:
+    def __init__(self) -> None:
+        name = 'demo_nft_marketplace.yml'
+        config_path = Path(__file__).parent / 'configs' / name
+        self.config = DipDupConfig.load([config_path])
+        self.config.initialize()
+
+        self.new_hash = '98858ec743f2c84ef9505ccefa2235fc6bb9e9b209b14b2028dd4650eaf96756'
+
+    async def test_first_run(self) -> None:
+        async with AsyncExitStack() as stack:
+            # Arrange
+            dipdup = await DipDup.create_dummy(self.config, stack, in_memory=True)
+            dispatcher = IndexDispatcher(dipdup._ctx)
+
+            # Act
+            await spawn_index(dispatcher, 'hen_mainnet')
+
+            # Assert
+            index = await Index.filter().get()
+            assert index.config_hash == self.new_hash
+
+    async def test_new_hash(self) -> None:
+        async with AsyncExitStack() as stack:
+            # Arrange
+            dipdup = await DipDup.create_dummy(self.config, stack, in_memory=True)
+            dispatcher = IndexDispatcher(dipdup._ctx)
+            await _create_index(self.new_hash)
+
+            # Act
+            await dispatcher._load_index_state()
+
+            # Assert
+            index = await Index.filter().get()
+            assert index.config_hash == self.new_hash
+
+    async def test_invalid_hash(self) -> None:
+        async with AsyncExitStack() as stack:
+            # Arrange
+            dipdup = await DipDup.create_dummy(self.config, stack, in_memory=True)
+            dispatcher = IndexDispatcher(dipdup._ctx)
+            await _create_index('hehehe')
+
+            # Act, Assert
+            with pytest.raises(ReindexingRequiredError):
+                await dispatcher._load_index_state()
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/operation/fetcher.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/fetcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,52 +2,53 @@
 
 import logging
 from collections import defaultdict
 from collections import deque
 from typing import Any
 from typing import AsyncIterator
 
-from dipdup.config import OperationHandlerOriginationPatternConfig as OriginationPatternConfig
-from dipdup.config import OperationHandlerTransactionPatternConfig as TransactionPatternConfig
-from dipdup.config import OperationIndexConfig
-from dipdup.config import OperationUnfilteredIndexConfig
-from dipdup.datasources.tzkt.datasource import TzktDatasource
-from dipdup.enums import OperationType
+from dipdup.config.tezos_tzkt_operations import OperationsHandlerOriginationPatternConfig as OriginationPatternConfig
+from dipdup.config.tezos_tzkt_operations import OperationsHandlerTransactionPatternConfig as TransactionPatternConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsIndexConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsUnfilteredIndexConfig
+from dipdup.datasources.tezos_tzkt import TzktDatasource
 from dipdup.exceptions import FrameworkException
 from dipdup.fetcher import DataFetcher
 from dipdup.fetcher import FetcherChannel
-from dipdup.models import OperationData
+from dipdup.fetcher import readahead_by_level
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktOperationType
 
 _logger = logging.getLogger('dipdup.fetcher')
 
 
-def dedup_operations(operations: tuple[OperationData, ...]) -> tuple[OperationData, ...]:
+def dedup_operations(operations: tuple[TzktOperationData, ...]) -> tuple[TzktOperationData, ...]:
     """Merge and sort operations fetched from multiple endpoints"""
     return tuple(
         sorted(
             (({op.id: op for op in operations}).values()),
             key=lambda op: op.id,
         )
     )
 
 
-def get_operations_head(operations: tuple[OperationData, ...]) -> int:
+def get_operations_head(operations: tuple[TzktOperationData, ...]) -> int:
     """Get latest block level (head) of sorted operations batch"""
     for i in range(len(operations) - 1)[::-1]:
         if operations[i].level != operations[i + 1].level:
             return operations[i].level
     return operations[0].level
 
 
 async def get_transaction_filters(
-    config: OperationIndexConfig,
+    config: TzktOperationsIndexConfig,
     datasource: TzktDatasource,
 ) -> tuple[set[str], set[int]]:
     """Get addresses to fetch transactions from during initial synchronization"""
-    if OperationType.transaction not in config.types:
+    if TzktOperationType.transaction not in config.types:
         return set(), set()
 
     code_hash: int | str | None
     addresses: set[str] = set()
     hashes: set[int] = set()
 
     # NOTE: Don't try to guess contracts from handlers if set implicitly
@@ -87,58 +88,56 @@
                     hashes.add(code_hash)
 
     _logger.info(f'Fetching transactions from {len(addresses)} addresses and {len(hashes)} code hashes')
     return addresses, hashes
 
 
 async def get_origination_filters(
-    config: OperationIndexConfig,
+    config: TzktOperationsIndexConfig,
     datasource: TzktDatasource,
 ) -> tuple[set[str], set[int]]:
     """Get addresses to fetch origination from during initial synchronization"""
-    if OperationType.origination not in config.types:
+    if TzktOperationType.origination not in config.types:
         return set(), set()
 
     addresses: set[str] = set()
     hashes: set[int] = set()
 
     for handler_config in config.handlers:
         for pattern_config in handler_config.pattern:
             if not isinstance(pattern_config, OriginationPatternConfig):
                 continue
 
-            # TODO: Remove in 7.0
-            if pattern_config.similar_to:
-                raise FrameworkException('originated_contract` alias, should be replaced in __init__')
-
             if pattern_config.originated_contract:
                 if address := pattern_config.originated_contract.address:
                     addresses.add(address)
                 if code_hash := pattern_config.originated_contract.code_hash:
                     if isinstance(code_hash, str):
                         code_hash, _ = await datasource.get_contract_hashes(code_hash)
                         pattern_config.originated_contract.code_hash = code_hash
                     hashes.add(code_hash)
 
             if pattern_config.source:
                 _logger.warning(
-                    "`source.address` filter significantly hurts indexing performance and doesn't support strict typing. "
-                    'Consider using `originated_contract.code_hash` instead'
+                    "`source.address` filter significantly hurts indexing performance and doesn't support strict"
+                    " typing. Consider using `originated_contract.code_hash` instead"
                 )
                 if address := pattern_config.source.address:
                     async for batch in datasource.iter_originated_contracts(address):
-                        addresses.update(batch)
+                        addresses.update(item['address'] for item in batch)
                 if code_hash := pattern_config.source.code_hash:
                     raise FrameworkException('Invalid transaction filter `source.code_hash`')
 
     _logger.info(f'Fetching originations from {len(addresses)} addresses and {len(hashes)} code hashes')
     return addresses, hashes
 
 
-class OriginationAddressFetcherChannel(FetcherChannel[OperationData, str]):
+class OriginationAddressFetcherChannel(FetcherChannel[TzktOperationData, str]):
+    _datasource: TzktDatasource
+
     async def fetch(self) -> None:
         if not self._filter:
             self._head = self._last_level
             self._offset = self._last_level
             return
 
         # FIXME: No pagination because of URL length limit workaround
@@ -151,15 +150,17 @@
         for op in originations:
             self._buffer[op.level].append(op)
 
         self._head = self._last_level
         self._offset = self._last_level
 
 
-class OriginationHashFetcherChannel(FetcherChannel[OperationData, int]):
+class OriginationHashFetcherChannel(FetcherChannel[TzktOperationData, int]):
+    _datasource: TzktDatasource
+
     async def fetch(self) -> None:
         if not self._filter:
             self._head = self._last_level
             self._offset = self._last_level
             return
 
         originations = await self._datasource.get_originations(
@@ -175,44 +176,52 @@
         if len(originations) < self._datasource.request_limit:
             self._head = self._last_level
         else:
             self._offset = originations[-1].id
             self._head = get_operations_head(originations)
 
 
-class MigrationOriginationFetcherChannel(FetcherChannel[OperationData, None]):
+class MigrationOriginationFetcherChannel(FetcherChannel[TzktOperationData, None]):
+    _datasource: TzktDatasource
+
     async def fetch(self) -> None:
         if self._filter:
             raise FrameworkException("Migration origination fetcher channel doesn't support filters")
 
         originations = await self._datasource.get_migration_originations(
             first_level=self._first_level,
             last_level=self._last_level,
             offset=self._offset,
         )
 
         for op in originations:
             if op.originated_contract_address:
                 code_hash, type_hash = await self._datasource.get_contract_hashes(op.originated_contract_address)
-                op.originated_contract_code_hash = code_hash
-                op.originated_contract_type_hash = type_hash
+                op_dict = op.__dict__
+                op_dict.update(
+                    originated_contract_code_hash=code_hash,
+                    originated_contract_type_hash=type_hash,
+                )
+                op = TzktOperationData(**op_dict)
 
             self._buffer[op.level].append(op)
 
         if len(originations) < self._datasource.request_limit:
             self._head = self._last_level
         else:
             self._offset = originations[-1].id
             self._head = get_operations_head(originations)
 
 
-class TransactionAddressFetcherChannel(FetcherChannel[OperationData, str]):
+class TransactionAddressFetcherChannel(FetcherChannel[TzktOperationData, str]):
+    _datasource: TzktDatasource
+
     def __init__(
         self,
-        buffer: defaultdict[int, deque[OperationData]],
+        buffer: defaultdict[int, deque[TzktOperationData]],
         filter: set[str],
         first_level: int,
         last_level: int,
         datasource: TzktDatasource,
         field: str,
     ) -> None:
         super().__init__(buffer, filter, first_level, last_level, datasource)
@@ -240,18 +249,20 @@
         if len(transactions) < self._datasource.request_limit:
             self._head = self._last_level
         else:
             self._offset = transactions[-1].id
             self._head = get_operations_head(transactions)
 
 
-class TransactionHashFetcherChannel(FetcherChannel[OperationData, int]):
+class TransactionHashFetcherChannel(FetcherChannel[TzktOperationData, int]):
+    _datasource: TzktDatasource
+
     def __init__(
         self,
-        buffer: defaultdict[int, deque[OperationData]],
+        buffer: defaultdict[int, deque[TzktOperationData]],
         filter: set[int],
         first_level: int,
         last_level: int,
         datasource: TzktDatasource,
         field: str,
     ) -> None:
         super().__init__(buffer, filter, first_level, last_level, datasource)
@@ -278,36 +289,38 @@
         if len(transactions) < self._datasource.request_limit:
             self._head = self._last_level
         else:
             self._offset = transactions[-1].id
             self._head = get_operations_head(transactions)
 
 
-class OperationUnfilteredFetcherChannel(FetcherChannel[OperationData, None]):
+class OperationUnfilteredFetcherChannel(FetcherChannel[TzktOperationData, None]):
+    _datasource: TzktDatasource
+
     def __init__(
         self,
-        buffer: defaultdict[int, deque[OperationData]],
+        buffer: defaultdict[int, deque[TzktOperationData]],
         first_level: int,
         last_level: int,
         datasource: TzktDatasource,
-        type: OperationType,
+        type: TzktOperationType,
     ) -> None:
         super().__init__(buffer, set(), first_level, last_level, datasource)
         self._type = type
 
     async def fetch(self) -> None:
-        if self._type == OperationType.origination:
+        if self._type == TzktOperationType.origination:
             operations = await self._datasource.get_originations(
                 addresses=None,
                 code_hashes=None,
                 first_level=self._first_level,
                 last_level=self._last_level,
                 offset=self._offset,
             )
-        elif self._type == OperationType.transaction:
+        elif self._type == TzktOperationType.transaction:
             operations = await self._datasource.get_transactions(
                 field='',
                 addresses=None,
                 code_hashes=None,
                 first_level=self._first_level,
                 last_level=self._last_level,
                 offset=self._offset,
@@ -321,15 +334,15 @@
         if len(operations) < self._datasource.request_limit:
             self._head = self._last_level
         else:
             self._offset = operations[-1].id
             self._head = get_operations_head(operations)
 
 
-class OperationFetcher(DataFetcher[OperationData]):
+class OperationFetcher(DataFetcher[TzktOperationData]):
     """Fetches operations from multiple REST API endpoints, merges them and yields by level.
 
     Offet of every endpoint is tracked separately.
     """
 
     def __init__(
         self,
@@ -348,15 +361,15 @@
         self._origination_addresses = origination_addresses
         self._origination_hashes = origination_hashes
         self._migration_originations = migration_originations
 
     @classmethod
     async def create(
         cls,
-        config: OperationIndexConfig,
+        config: TzktOperationsIndexConfig,
         datasource: TzktDatasource,
         first_level: int,
         last_level: int,
     ) -> OperationFetcher:
         transaction_addresses, transaction_hashes = await get_transaction_filters(config, datasource)
         origination_addresses, origination_hashes = await get_origination_filters(config, datasource)
 
@@ -364,29 +377,29 @@
             datasource=datasource,
             first_level=first_level,
             last_level=last_level,
             transaction_addresses=transaction_addresses,
             transaction_hashes=transaction_hashes,
             origination_addresses=origination_addresses,
             origination_hashes=origination_hashes,
-            migration_originations=OperationType.migration in config.types,
+            migration_originations=TzktOperationType.migration in config.types,
         )
 
-    async def fetch_by_level(self) -> AsyncIterator[tuple[int, tuple[OperationData, ...]]]:
+    async def fetch_by_level(self) -> AsyncIterator[tuple[int, tuple[TzktOperationData, ...]]]:
         """Iterate over operations fetched with multiple REST requests with different filters.
 
-        Resulting data is splitted by level, deduped, sorted and ready to be processed by OperationIndex.
+        Resulting data is splitted by level, deduped, sorted and ready to be processed by TzktOperationsIndex.
         """
         channel_kwargs = {
             'buffer': self._buffer,
             'datasource': self._datasource,
             'first_level': self._first_level,
             'last_level': self._last_level,
         }
-        channels: tuple[FetcherChannel[OperationData, Any], ...] = (
+        channels: tuple[FetcherChannel[TzktOperationData, Any], ...] = (
             TransactionAddressFetcherChannel(
                 filter=self._transaction_addresses,
                 field='sender',
                 **channel_kwargs,  # type: ignore[arg-type]
             ),
             TransactionAddressFetcherChannel(
                 filter=self._transaction_addresses,
@@ -409,36 +422,43 @@
             ),
             OriginationHashFetcherChannel(
                 filter=self._origination_hashes,
                 **channel_kwargs,  # type: ignore[arg-type]
             ),
         )
 
-        while True:
-            min_channel = sorted(channels, key=lambda x: x.head)[0]
-            await min_channel.fetch()
-
-            # NOTE: It's a different channel now, but with greater head level
-            min_channel = sorted(channels, key=lambda x: x.head)[0]
-            min_head = min_channel.head
-
-            while self._head <= min_head:
-                if self._head in self._buffer:
-                    operations = self._buffer.pop(self._head)
-                    yield self._head, dedup_operations(tuple(operations))
-                self._head += 1
-
-            if all(c.fetched for c in channels):
-                break
-
-        if self._buffer:
-            raise FrameworkException('Operations left in queue')
+        async def _merged_iter(
+            channels: tuple[FetcherChannel[TzktOperationData, Any], ...]
+        ) -> AsyncIterator[tuple[TzktOperationData, ...]]:
+            while True:
+                min_channel = sorted(channels, key=lambda x: x.head)[0]
+                await min_channel.fetch()
+
+                # NOTE: It's a different channel now, but with greater head level
+                min_channel = sorted(channels, key=lambda x: x.head)[0]
+                min_head = min_channel.head
+
+                while self._head <= min_head:
+                    if self._head in self._buffer:
+                        operations = self._buffer.pop(self._head)
+                        yield dedup_operations(tuple(operations))
+                    self._head += 1
+
+                if all(c.fetched for c in channels):
+                    break
+
+            if self._buffer:
+                raise FrameworkException('Operations left in queue')
+
+        event_iter = _merged_iter(channels)
+        async for level, operations in readahead_by_level(event_iter, limit=5_000):
+            yield level, operations
 
 
-class OperationUnfilteredFetcher(DataFetcher[OperationData]):
+class OperationUnfilteredFetcher(DataFetcher[TzktOperationData]):
     def __init__(
         self,
         datasource: TzktDatasource,
         first_level: int,
         last_level: int,
         transactions: bool,
         originations: bool,
@@ -448,51 +468,51 @@
         self._transactions = transactions
         self._originations = originations
         self._migration_originations = migration_originations
 
     @classmethod
     async def create(
         cls,
-        config: OperationUnfilteredIndexConfig,
+        config: TzktOperationsUnfilteredIndexConfig,
         datasource: TzktDatasource,
         first_level: int,
         last_level: int,
     ) -> OperationUnfilteredFetcher:
         return OperationUnfilteredFetcher(
             datasource=datasource,
             first_level=first_level,
             last_level=last_level,
-            transactions=OperationType.transaction in config.types,
-            originations=OperationType.origination in config.types,
-            migration_originations=OperationType.migration in config.types,
+            transactions=TzktOperationType.transaction in config.types,
+            originations=TzktOperationType.origination in config.types,
+            migration_originations=TzktOperationType.migration in config.types,
         )
 
-    async def fetch_by_level(self) -> AsyncIterator[tuple[int, tuple[OperationData, ...]]]:
+    async def fetch_by_level(self) -> AsyncIterator[tuple[int, tuple[TzktOperationData, ...]]]:
         """Iterate over operations fetched with multiple REST requests with different filters.
 
-        Resulting data is splitted by level, deduped, sorted and ready to be processed by OperationIndex.
+        Resulting data is splitted by level, deduped, sorted and ready to be processed by TzktOperationsIndex.
         """
         channel_kwargs = {
             'buffer': self._buffer,
             'datasource': self._datasource,
             'first_level': self._first_level,
             'last_level': self._last_level,
         }
-        channels: tuple[FetcherChannel[OperationData, Any], ...] = ()
+        channels: tuple[FetcherChannel[TzktOperationData, Any], ...] = ()
         if self._transactions:
             channels += (
                 OperationUnfilteredFetcherChannel(
-                    type=OperationType.transaction,
+                    type=TzktOperationType.transaction,
                     **channel_kwargs,  # type: ignore[arg-type]
                 ),
             )
         if self._originations:
             channels += (
                 OperationUnfilteredFetcherChannel(
-                    type=OperationType.origination,
+                    type=TzktOperationType.origination,
                     **channel_kwargs,  # type: ignore[arg-type]
                 ),
             )
         if self._migration_originations:
             channels += (
                 MigrationOriginationFetcherChannel(
                     filter=set(),
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/operation/index.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,115 +2,107 @@
 from collections import defaultdict
 from collections import deque
 from contextlib import ExitStack
 from typing import Iterable
 from typing import Iterator
 from typing import Sequence
 
-from dipdup.config import OperationHandlerConfig
-from dipdup.config import OperationHandlerConfigU
-from dipdup.config import OperationHandlerOriginationPatternConfig as OriginationPatternConfig
-from dipdup.config import OperationHandlerTransactionPatternConfig as TransactionPatternConfig
-from dipdup.config import OperationIndexConfig
-from dipdup.config import OperationIndexConfigU
-from dipdup.config import OperationUnfilteredIndexConfig
+from dipdup.config.tezos_tzkt_operations import OperationsHandlerOriginationPatternConfig as OriginationPatternConfig
+from dipdup.config.tezos_tzkt_operations import OperationsHandlerTransactionPatternConfig as TransactionPatternConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsHandlerConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsHandlerConfigU
+from dipdup.config.tezos_tzkt_operations import TzktOperationsIndexConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsIndexConfigU
+from dipdup.config.tezos_tzkt_operations import TzktOperationsUnfilteredIndexConfig
 from dipdup.context import DipDupContext
-from dipdup.datasources.tzkt.datasource import TzktDatasource
-from dipdup.enums import MessageType
+from dipdup.datasources.tezos_tzkt import TzktDatasource
 from dipdup.exceptions import ConfigInitializationException
 from dipdup.exceptions import FrameworkException
 from dipdup.index import Index
-from dipdup.indexes.operation.fetcher import OperationFetcher
-from dipdup.indexes.operation.fetcher import OperationUnfilteredFetcher
-from dipdup.indexes.operation.matcher import MatchedOperationsT
-from dipdup.indexes.operation.matcher import OperationHandlerArgumentU
-from dipdup.indexes.operation.matcher import OperationSubgroup
-from dipdup.indexes.operation.matcher import match_operation_subgroup
-from dipdup.indexes.operation.matcher import match_operation_unfiltered_subgroup
-from dipdup.models import OperationData
+from dipdup.indexes.tezos_tzkt_operations.fetcher import OperationFetcher
+from dipdup.indexes.tezos_tzkt_operations.fetcher import OperationUnfilteredFetcher
+from dipdup.indexes.tezos_tzkt_operations.matcher import MatchedOperationsT
+from dipdup.indexes.tezos_tzkt_operations.matcher import OperationsHandlerArgumentU
+from dipdup.indexes.tezos_tzkt_operations.matcher import OperationSubgroup
+from dipdup.indexes.tezos_tzkt_operations.matcher import match_operation_subgroup
+from dipdup.indexes.tezos_tzkt_operations.matcher import match_operation_unfiltered_subgroup
+from dipdup.models.tezos_tzkt import TzktMessageType
+from dipdup.models.tezos_tzkt import TzktOperationData
 from dipdup.prometheus import Metrics
 
 _logger = logging.getLogger('dipdup.matcher')
 
 OperationQueueItem = tuple[OperationSubgroup, ...]
 
 
-def entrypoint_filter(handlers: tuple[OperationHandlerConfig, ...]) -> set[str | None]:
+def entrypoint_filter(handlers: tuple[TzktOperationsHandlerConfig, ...]) -> set[str | None]:
     """Set of entrypoints to filter operations with before an actual matching"""
     entrypoints = set()
     for handler_config in handlers:
         for pattern_config in handler_config.pattern:
             if not isinstance(pattern_config, TransactionPatternConfig):
                 continue
             entrypoints.add(pattern_config.entrypoint)
 
     return entrypoints
 
 
-def address_filter(handlers: tuple[OperationHandlerConfig, ...]) -> set[str]:
+def address_filter(handlers: tuple[TzktOperationsHandlerConfig, ...]) -> set[str]:
     """Set of addresses (any field) to filter operations with before an actual matching"""
     addresses = set()
     for handler_config in handlers:
         for pattern_config in handler_config.pattern:
             if isinstance(pattern_config, TransactionPatternConfig):
                 if pattern_config.source:
                     if address := pattern_config.source.address:
                         addresses.add(address)
                 if pattern_config.destination:
                     if address := pattern_config.destination.address:
                         addresses.add(address)
             elif isinstance(pattern_config, OriginationPatternConfig):
-                # TODO: Remove in 7.0
-                if pattern_config.similar_to:
-                    raise FrameworkException('originated_contract` alias, should be replaced in __init__')
-
                 if pattern_config.originated_contract:
                     if address := pattern_config.originated_contract.address:
                         addresses.add(address)
 
     return addresses
 
 
-def code_hash_filter(handlers: tuple[OperationHandlerConfig, ...]) -> set[int | str]:
+def code_hash_filter(handlers: tuple[TzktOperationsHandlerConfig, ...]) -> set[int | str]:
     """Set of code hashes to filter operations with before an actual matching"""
     code_hashes = set()
     for handler_config in handlers:
         for pattern_config in handler_config.pattern:
             if isinstance(pattern_config, TransactionPatternConfig):
                 if pattern_config.source:
                     if code_hash := pattern_config.source.code_hash:
                         code_hashes.add(code_hash)
                 if pattern_config.destination:
                     if code_hash := pattern_config.destination.code_hash:
                         code_hashes.add(code_hash)
             elif isinstance(pattern_config, OriginationPatternConfig):
-                # TODO: Remove in 7.0
-                if pattern_config.similar_to:
-                    raise FrameworkException('originated_contract` alias, should be replaced in __init__')
-
                 if pattern_config.source:
                     if code_hash := pattern_config.source.code_hash:
                         raise FrameworkException('`source.code_hash` is not supported for origination patterns')
 
                 if pattern_config.originated_contract:
                     if code_hash := pattern_config.originated_contract.code_hash:
                         code_hashes.add(code_hash)
 
     return code_hashes
 
 
 def extract_operation_subgroups(
-    operations: Iterable[OperationData],
+    operations: Iterable[TzktOperationData],
     addresses: set[str],
     entrypoints: set[str | None],
     code_hashes: set[int],
 ) -> Iterator[OperationSubgroup]:
     filtered: int = 0
     levels: set[int] = set()
-    operation_subgroups: defaultdict[tuple[str, int], deque[OperationData]] = defaultdict(deque)
+    operation_subgroups: defaultdict[tuple[str, int], deque[TzktOperationData]] = defaultdict(deque)
 
     _operation_index = -1
     for _operation_index, op in enumerate(operations):
         # NOTE: Filtering out operations that are not part of any index
         if op.type == 'transaction':
             if entrypoints and op.entrypoint not in entrypoints:
                 filtered += 1
@@ -145,34 +137,34 @@
             hash=hash_,
             counter=counter,
             operations=tuple(operations),
             entrypoints=entrypoints,
         )
 
 
-class OperationIndex(
-    Index[OperationIndexConfigU, OperationQueueItem, TzktDatasource],
-    message_type=MessageType.operation,
+class TzktOperationsIndex(
+    Index[TzktOperationsIndexConfigU, OperationQueueItem, TzktDatasource],
+    message_type=TzktMessageType.operation,
 ):
     def __init__(
         self,
         ctx: DipDupContext,
-        config: OperationIndexConfigU,
+        config: TzktOperationsIndexConfigU,
         datasource: TzktDatasource,
     ) -> None:
         super().__init__(ctx, config, datasource)
         self._entrypoint_filter: set[str | None] = set()
         self._address_filter: set[str] = set()
         self._code_hash_filter: set[int] = set()
 
     def push_operations(self, operation_subgroups: OperationQueueItem) -> None:
         self.push_realtime_message(operation_subgroups)
 
     async def get_filters(self) -> tuple[set[str | None], set[str], set[int]]:
-        if isinstance(self._config, OperationUnfilteredIndexConfig):
+        if isinstance(self._config, TzktOperationsUnfilteredIndexConfig):
             return set(), set(), set()
 
         if self._entrypoint_filter or self._address_filter or self._code_hash_filter:
             return self._entrypoint_filter, self._address_filter, self._code_hash_filter
 
         for code_hash in code_hash_filter(self._config.handlers):
             if not isinstance(code_hash, int):
@@ -219,22 +211,22 @@
         if index_level is None:
             return
 
         first_level = index_level + 1
         self._logger.info('Fetching operations from level %s to %s', first_level, sync_level)
 
         fetcher: OperationFetcher | OperationUnfilteredFetcher
-        if isinstance(self._config, OperationIndexConfig):
+        if isinstance(self._config, TzktOperationsIndexConfig):
             fetcher = await OperationFetcher.create(
                 self._config,
                 self._datasource,
                 first_level,
                 sync_level,
             )
-        elif isinstance(self._config, OperationUnfilteredIndexConfig):
+        elif isinstance(self._config, TzktOperationsUnfilteredIndexConfig):
             fetcher = await OperationUnfilteredFetcher.create(
                 self._config,
                 self._datasource,
                 first_level,
                 sync_level,
             )
 
@@ -247,15 +239,15 @@
                     operations,
                     entrypoints=self._entrypoint_filter,
                     addresses=self._address_filter,
                     code_hashes=self._code_hash_filter,
                 )
             )
             if operation_subgroups:
-                self._logger.info('Processing operations of level %s', level)
+                self._logger.debug('Processing operations of level %s', level)
                 with ExitStack() as stack:
                     if Metrics.enabled:
                         stack.enter_context(Metrics.measure_level_sync_duration())
                     await self._process_level_operations(operation_subgroups, sync_level)
 
         await self._exit_sync_state(sync_level)
 
@@ -271,56 +263,57 @@
         index_level = self.state.level
         if batch_level <= index_level:
             raise FrameworkException(f'Batch level is lower than index level: {batch_level} <= {index_level}')
 
         self._logger.debug('Processing %s operation subgroups of level %s', len(operation_subgroups), batch_level)
         matched_handlers: deque[MatchedOperationsT] = deque()
         for operation_subgroup in operation_subgroups:
-            if isinstance(self._config, OperationUnfilteredIndexConfig):
+            if isinstance(self._config, TzktOperationsUnfilteredIndexConfig):
                 subgroup_handlers = match_operation_unfiltered_subgroup(
                     index=self._config,
                     operation_subgroup=operation_subgroup,
                 )
             else:
                 subgroup_handlers = match_operation_subgroup(
+                    self._ctx.package,
                     handlers=self._config.handlers,
                     operation_subgroup=operation_subgroup,
                     alt=self._ctx.config.advanced.alt_operation_matcher,
                 )
 
             if subgroup_handlers:
-                self._logger.info(
+                self._logger.debug(
                     '%s: `%s` handler matched!',
                     operation_subgroup.hash,
                     subgroup_handlers[0][1].callback,
                 )
             matched_handlers += subgroup_handlers
 
         if Metrics.enabled:
             Metrics.set_index_handlers_matched(len(matched_handlers))
 
         # NOTE: We still need to bump index level but don't care if it will be done in existing transaction
         if not matched_handlers:
             await self._update_state(level=batch_level)
             return
 
-        async with self._ctx._transactions.in_transaction(batch_level, sync_level, self.name):
+        async with self._ctx.transactions.in_transaction(batch_level, sync_level, self.name):
             for operation_subgroup, handler_config, args in matched_handlers:
                 await self._call_matched_handler(handler_config, operation_subgroup, args)
             await self._update_state(level=batch_level)
 
     async def _call_matched_handler(
         self,
-        handler_config: OperationHandlerConfigU,
+        handler_config: TzktOperationsHandlerConfigU,
         operation_subgroup: OperationSubgroup,
-        args: Sequence[OperationHandlerArgumentU],
+        args: Sequence[OperationsHandlerArgumentU],
     ) -> None:
         if not handler_config.parent:
             raise ConfigInitializationException
 
-        await self._ctx._fire_handler(
+        await self._ctx.fire_handler(
             handler_config.callback,
             handler_config.parent.name,
             self.datasource,
             operation_subgroup.hash + ': {}',
             *args,
         )
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/operation/matcher.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_operations/matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,98 +1,103 @@
 import logging
 from collections import deque
 from typing import Any
 from typing import Iterable
 
 from pydantic.dataclasses import dataclass
 
-from dipdup.config import OperationHandlerConfig
-from dipdup.config import OperationHandlerConfigU
-from dipdup.config import OperationHandlerOriginationPatternConfig as OriginationPatternConfig
-from dipdup.config import OperationHandlerTransactionPatternConfig as TransactionPatternConfig
-from dipdup.config import OperationUnfilteredIndexConfig
-from dipdup.datasources.tzkt.models import deserialize_storage
-from dipdup.enums import OperationType
+from dipdup.codegen.tezos_tzkt import get_parameter_type
+from dipdup.codegen.tezos_tzkt import get_storage_type
+from dipdup.config.tezos_tzkt_operations import OperationsHandlerOriginationPatternConfig as OriginationPatternConfig
+from dipdup.config.tezos_tzkt_operations import OperationsHandlerTransactionPatternConfig as TransactionPatternConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsHandlerConfig
+from dipdup.config.tezos_tzkt_operations import TzktOperationsHandlerConfigU
+from dipdup.config.tezos_tzkt_operations import TzktOperationsUnfilteredIndexConfig
 from dipdup.exceptions import FrameworkException
-from dipdup.models import OperationData
-from dipdup.models import Origination
-from dipdup.models import Transaction
-from dipdup.utils.codegen import parse_object
+from dipdup.indexes.tezos_tzkt_operations.parser import deserialize_storage
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktOperationType
+from dipdup.models.tezos_tzkt import TzktOrigination
+from dipdup.models.tezos_tzkt import TzktTransaction
+from dipdup.package import DipDupPackage
+from dipdup.utils import parse_object
 
 _logger = logging.getLogger('dipdup.matcher')
 
 
 @dataclass(frozen=True)
 class OperationSubgroup:
     """Operations of a single contract call"""
 
     hash: str
     counter: int
-    operations: tuple[OperationData, ...]
+    operations: tuple[TzktOperationData, ...]
     entrypoints: set[str | None]
 
 
-OperationHandlerArgumentU = Transaction | Origination | OperationData | None
-MatchedOperationsT = tuple[OperationSubgroup, OperationHandlerConfigU, deque[OperationHandlerArgumentU]]
+OperationsHandlerArgumentU = TzktTransaction | TzktOrigination | TzktOperationData | None
+MatchedOperationsT = tuple[OperationSubgroup, TzktOperationsHandlerConfigU, deque[OperationsHandlerArgumentU]]
 
 
 def prepare_operation_handler_args(
-    handler_config: OperationHandlerConfig,
-    matched_operations: deque[OperationData | None],
-) -> deque[OperationHandlerArgumentU]:
+    package: DipDupPackage,
+    handler_config: TzktOperationsHandlerConfig,
+    matched_operations: deque[TzktOperationData | None],
+) -> deque[OperationsHandlerArgumentU]:
     """Prepare handler arguments, parse parameter and storage."""
-    args: deque[OperationHandlerArgumentU] = deque()
+    args: deque[OperationsHandlerArgumentU] = deque()
     for pattern_config, operation_data in zip(handler_config.pattern, matched_operations):
         if operation_data is None:
             args.append(None)
 
         elif isinstance(pattern_config, TransactionPatternConfig):
-            if not pattern_config.entrypoint:
+            if not pattern_config.typed_contract or not pattern_config.entrypoint:
                 args.append(operation_data)
                 continue
 
-            type_ = pattern_config.parameter_type_cls
+            if not operation_data.parameter_json:
+                raise FrameworkException('Transaction parameter is empty')
+            typename = pattern_config.typed_contract.module_name
+            type_ = get_parameter_type(package, typename, pattern_config.entrypoint)
             parameter = parse_object(type_, operation_data.parameter_json) if type_ else None
 
-            storage_type = pattern_config.storage_type_cls
-            storage = deserialize_storage(operation_data, storage_type)
+            storage_type = get_storage_type(package, typename)
+            operation_data, storage = deserialize_storage(operation_data, storage_type)
 
-            typed_transaction: Transaction[Any, Any] = Transaction(
+            typed_transaction: TzktTransaction[Any, Any] = TzktTransaction(
                 data=operation_data,
                 parameter=parameter,
                 storage=storage,
             )
             args.append(typed_transaction)
 
         elif isinstance(pattern_config, OriginationPatternConfig):
-            if pattern_config.originated_contract or pattern_config.similar_to:
-                pass
-            # NOTE: `source` is always untyped
-            else:
+            if not pattern_config.typed_contract:
                 args.append(operation_data)
                 continue
 
-            storage_type = pattern_config.storage_type_cls
-            storage = deserialize_storage(operation_data, storage_type)
+            typename = pattern_config.typed_contract.module_name
+            storage_type = get_storage_type(package, typename)
+            operation_data, storage = deserialize_storage(operation_data, storage_type)
 
-            typed_origination = Origination(
+            typed_origination = TzktOrigination(
                 data=operation_data,
                 storage=storage,
             )
             args.append(typed_origination)
 
         else:
             raise NotImplementedError
 
     return args
 
 
 def match_transaction(
     pattern_config: TransactionPatternConfig,
-    operation: OperationData,
+    operation: TzktOperationData,
 ) -> bool:
     """Match a single transaction with pattern"""
     if entrypoint := pattern_config.entrypoint:
         if entrypoint != operation.entrypoint:
             return False
     if destination := pattern_config.destination:
         if destination.address not in (operation.target_address, None):
@@ -106,15 +111,15 @@
             return False
 
     return True
 
 
 def match_origination(
     pattern_config: OriginationPatternConfig,
-    operation: OperationData,
+    operation: TzktOperationData,
 ) -> bool:
     if source := pattern_config.source:
         if source.address not in (operation.sender_address, None):
             return False
         if source.code_hash:
             raise FrameworkException('Invalid origination filter `source.code_hash`')
 
@@ -124,39 +129,40 @@
         if originated_contract.code_hash not in (operation.originated_contract_code_hash, None):
             return False
 
     return True
 
 
 def match_operation_unfiltered_subgroup(
-    index: OperationUnfilteredIndexConfig,
+    index: TzktOperationsUnfilteredIndexConfig,
     operation_subgroup: OperationSubgroup,
 ) -> deque[MatchedOperationsT]:
     matched_handlers: deque[MatchedOperationsT] = deque()
 
     for operation in operation_subgroup.operations:
-        if OperationType[operation.type] in index.types:
+        if TzktOperationType[operation.type] in index.types:
             matched_handlers.append((operation_subgroup, index.handler_config, deque([operation])))
 
     return matched_handlers
 
 
 def match_operation_subgroup(
-    handlers: Iterable[OperationHandlerConfig],
+    package: DipDupPackage,
+    handlers: Iterable[TzktOperationsHandlerConfig],
     operation_subgroup: OperationSubgroup,
     alt: bool = False,
 ) -> deque[MatchedOperationsT]:
     """Try to match operation subgroup with all index handlers."""
     matched_handlers: deque[MatchedOperationsT] = deque()
     operations = operation_subgroup.operations
 
     for handler_config in handlers:
         subgroup_index = 0
         pattern_index = 0
-        matched_operations: deque[OperationData | None] = deque()
+        matched_operations: deque[TzktOperationData | None] = deque()
 
         # TODO: Ensure complex cases work, e.g. when optional argument is followed by required one
         while subgroup_index < len(operations):
             operation = operations[subgroup_index]
             pattern_config = handler_config.pattern[pattern_index]
 
             matched = False
@@ -176,39 +182,39 @@
             elif pattern_config.optional:
                 matched_operations.append(None)
                 pattern_index += 1
             else:
                 subgroup_index += 1
 
             if pattern_index == len(handler_config.pattern):
-                _logger.info('%s: `%s` handler matched!', operation_subgroup.hash, handler_config.callback)
+                _logger.debug('%s: `%s` handler matched!', operation_subgroup.hash, handler_config.callback)
 
-                args = prepare_operation_handler_args(handler_config, matched_operations)
+                args = prepare_operation_handler_args(package, handler_config, matched_operations)
                 matched_handlers.append((operation_subgroup, handler_config, args))
 
                 matched_operations.clear()
                 pattern_index = 0
 
         if len(matched_operations) >= sum(0 if x.optional else 1 for x in handler_config.pattern):
-            _logger.info('%s: `%s` handler matched!', operation_subgroup.hash, handler_config.callback)
+            _logger.debug('%s: `%s` handler matched!', operation_subgroup.hash, handler_config.callback)
 
-            args = prepare_operation_handler_args(handler_config, matched_operations)
+            args = prepare_operation_handler_args(package, handler_config, matched_operations)
             matched_handlers.append((operation_subgroup, handler_config, args))
 
     if not (alt and len(matched_handlers) in (0, 1)):
         return matched_handlers
 
-    # NOTE: Below is a secret algorithm for very special cases
+    # NOTE: Alternative algorithm. Sort matched handlers by the internal incremental TzKT id of the last operation in matched pattern.
     index_list = list(range(len(matched_handlers)))
     id_list = []
     for handler in matched_handlers:
         transaction = handler[2][-1]
-        if isinstance(transaction, OperationData):
+        if isinstance(transaction, TzktOperationData):
             id_list.append(transaction.id)
-        elif isinstance(transaction, Transaction):
+        elif isinstance(transaction, TzktTransaction):
             id_list.append(transaction.data.id)
         else:
             raise FrameworkException('Type of the first handler argument is unknown')
 
     sorted_index_list = [x for _, x in sorted(zip(id_list, index_list))]
     if index_list == sorted_index_list:
         return matched_handlers
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/token_transfer/fetcher.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/fetcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 from __future__ import annotations
 
 import logging
 from typing import AsyncIterator
 
-from dipdup.datasources.tzkt.datasource import TzktDatasource
+from dipdup.datasources.tezos_tzkt import TzktDatasource
 from dipdup.fetcher import DataFetcher
-from dipdup.fetcher import yield_by_level
-from dipdup.models import TokenTransferData
+from dipdup.fetcher import readahead_by_level
+from dipdup.models.tezos_tzkt import TzktTokenTransferData
 
 
-class TokenTransferFetcher(DataFetcher[TokenTransferData]):
+class TokenTransferFetcher(DataFetcher[TzktTokenTransferData]):
+    _datasource: TzktDatasource
+
     def __init__(
         self,
         datasource: TzktDatasource,
         token_addresses: set[str],
         token_ids: set[int],
         from_addresses: set[str],
         to_addresses: set[str],
         first_level: int,
         last_level: int,
     ) -> None:
         super().__init__(datasource, first_level, last_level)
-        self._logger = logging.getLogger('dipdup.tzkt')
+        self._logger = logging.getLogger('dipdup.fetcher')
         self._token_addresses = token_addresses
         self._token_ids = token_ids
         self._from_addresses = from_addresses
         self._to_addresses = to_addresses
 
-    async def fetch_by_level(self) -> AsyncIterator[tuple[int, tuple[TokenTransferData, ...]]]:
+    async def fetch_by_level(self) -> AsyncIterator[tuple[int, tuple[TzktTokenTransferData, ...]]]:
         token_transfer_iter = self._datasource.iter_token_transfers(
             self._token_addresses,
             self._token_ids,
             self._from_addresses,
             self._to_addresses,
             self._first_level,
             self._last_level,
         )
-        async for level, batch in yield_by_level(token_transfer_iter):
+        async for level, batch in readahead_by_level(token_transfer_iter, limit=5_000):
             yield level, batch
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/token_transfer/index.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from contextlib import ExitStack
 
-from dipdup.config import TokenTransferHandlerConfig
-from dipdup.config import TokenTransferIndexConfig
-from dipdup.datasources.tzkt.datasource import TzktDatasource
-from dipdup.enums import MessageType
+from dipdup.config.tezos_tzkt_token_transfers import TzktTokenTransfersHandlerConfig
+from dipdup.config.tezos_tzkt_token_transfers import TzktTokenTransfersIndexConfig
+from dipdup.datasources.tezos_tzkt import TzktDatasource
 from dipdup.exceptions import ConfigInitializationException
 from dipdup.exceptions import FrameworkException
 from dipdup.index import Index
-from dipdup.indexes.token_transfer.fetcher import TokenTransferFetcher
-from dipdup.indexes.token_transfer.matcher import match_token_transfers
-from dipdup.models import TokenTransferData
+from dipdup.indexes.tezos_tzkt_token_transfers.fetcher import TokenTransferFetcher
+from dipdup.indexes.tezos_tzkt_token_transfers.matcher import match_token_transfers
+from dipdup.models.tezos_tzkt import TzktMessageType
+from dipdup.models.tezos_tzkt import TzktTokenTransferData
 from dipdup.prometheus import Metrics
 
-TokenTransferQueueItem = tuple[TokenTransferData, ...]
+TokenTransferQueueItem = tuple[TzktTokenTransferData, ...]
 
 
-class TokenTransferIndex(
-    Index[TokenTransferIndexConfig, TokenTransferQueueItem, TzktDatasource],
-    message_type=MessageType.token_transfer,
+class TzktTokenTransfersIndex(
+    Index[TzktTokenTransfersIndexConfig, TokenTransferQueueItem, TzktDatasource],
+    message_type=TzktMessageType.token_transfer,
 ):
     def push_token_transfers(self, token_transfers: TokenTransferQueueItem) -> None:
         self.push_realtime_message(token_transfers)
 
     def _create_fetcher(self, first_level: int, last_level: int) -> TokenTransferFetcher:
         token_addresses: set[str] = set()
         token_ids: set[int] = set()
@@ -64,15 +64,15 @@
                     stack.enter_context(Metrics.measure_level_sync_duration())
                 await self._process_level_token_transfers(token_transfers, sync_level)
 
         await self._exit_sync_state(sync_level)
 
     async def _process_level_token_transfers(
         self,
-        token_transfers: tuple[TokenTransferData, ...],
+        token_transfers: tuple[TzktTokenTransferData, ...],
         sync_level: int,
     ) -> None:
         if not token_transfers:
             return
 
         batch_level = token_transfers[0].level
         index_level = self.state.level
@@ -86,26 +86,26 @@
             Metrics.set_index_handlers_matched(len(matched_handlers))
 
         # NOTE: We still need to bump index level but don't care if it will be done in existing transaction
         if not matched_handlers:
             await self._update_state(level=batch_level)
             return
 
-        async with self._ctx._transactions.in_transaction(batch_level, sync_level, self.name):
+        async with self._ctx.transactions.in_transaction(batch_level, sync_level, self.name):
             for handler_config, token_transfer in matched_handlers:
                 await self._call_matched_handler(handler_config, token_transfer)
             await self._update_state(level=batch_level)
 
     async def _call_matched_handler(
-        self, handler_config: TokenTransferHandlerConfig, token_transfer: TokenTransferData
+        self, handler_config: TzktTokenTransfersHandlerConfig, token_transfer: TzktTokenTransferData
     ) -> None:
         if not handler_config.parent:
             raise ConfigInitializationException
 
-        await self._ctx._fire_handler(
+        await self._ctx.fire_handler(
             handler_config.callback,
             handler_config.parent.name,
             self.datasource,
             # NOTE: missing `operation_id` field in API to identify operation
             None,
             token_transfer,
         )
```

### Comparing `dipdup-6.5.9/src/dipdup/indexes/token_transfer/matcher.py` & `dipdup-7.0.0rc1/src/dipdup/indexes/tezos_tzkt_token_transfers/matcher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 from collections import deque
 from typing import Iterable
 
-from dipdup.config import TokenTransferHandlerConfig
-from dipdup.models import TokenTransferData
+from dipdup.config.tezos_tzkt_token_transfers import TzktTokenTransfersHandlerConfig
+from dipdup.models.tezos_tzkt import TzktTokenTransferData
 
 _logger = logging.getLogger('dipdup.matcher')
 
-MatchedTokenTransfersT = tuple[TokenTransferHandlerConfig, TokenTransferData]
+MatchedTokenTransfersT = tuple[TzktTokenTransfersHandlerConfig, TzktTokenTransferData]
 
 
 def match_token_transfer(
-    handler_config: TokenTransferHandlerConfig,
-    token_transfer: TokenTransferData,
+    handler_config: TzktTokenTransfersHandlerConfig,
+    token_transfer: TzktTokenTransferData,
 ) -> bool:
     """Match single token transfer with pattern"""
     if handler_config.contract:
         if handler_config.contract.address != token_transfer.contract_address:
             return False
     if handler_config.token_id is not None:
         if handler_config.token_id != token_transfer.token_id:
@@ -27,25 +27,22 @@
     if handler_config.to:
         if handler_config.to.address != token_transfer.to_address:
             return False
     return True
 
 
 def match_token_transfers(
-    handlers: Iterable[TokenTransferHandlerConfig], token_transfers: Iterable[TokenTransferData]
+    handlers: Iterable[TzktTokenTransfersHandlerConfig], token_transfers: Iterable[TzktTokenTransferData]
 ) -> deque[MatchedTokenTransfersT]:
     """Try to match token transfers with all index handlers."""
 
     matched_handlers: deque[MatchedTokenTransfersT] = deque()
 
     for token_transfer in token_transfers:
         for handler_config in handlers:
             token_transfer_matched = match_token_transfer(handler_config, token_transfer)
-            if token_transfer_matched:
-                _logger.info(
-                    '%s: `%s` handler matched!',
-                    token_transfer.level,
-                    handler_config.callback,
-                )
-                matched_handlers.append((handler_config, token_transfer))
+            if not token_transfer_matched:
+                continue
+            _logger.debug('%s: `%s` handler matched!', token_transfer.level, handler_config.callback)
+            matched_handlers.append((handler_config, token_transfer))
 
     return matched_handlers
```

### Comparing `dipdup-6.5.9/src/dipdup/install.py` & `dipdup-7.0.0rc1/src/dipdup/install.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 """This script (un)installs DipDup and its dependencies with pipx.
 
 WARNING: No imports allowed here except stdlib! Otherwise, `curl | python` magic will break.
-And no pre-3.10 code too. Just to print nice colored "not supported" message instead of crashing.
+And no 3.11-only code too. Just to print nice colored "not supported" message instead of crashing.
 
 Some functions are importable to use in `dipdup.cli`.
 This script is also available as `dipdup-install` or `python -m dipdup.install`.
 """
 import argparse
 import os
 import subprocess
 import sys
 from pathlib import Path
-from shutil import rmtree
 from shutil import which
 from typing import Any
 from typing import Dict
 from typing import NoReturn
 from typing import Optional
 from typing import Set
+from typing import cast
 
 GITHUB = 'https://github.com/dipdup-io/dipdup.git'
 WHICH_CMDS = (
-    'python3',
+    'bash',
+    'python3.11',
     'pipx',
     'dipdup',
     'datamodel-codegen',
-    'poetry',
+    'pdm',
     'pyvenv',
     'pyenv',
 )
 
+WELCOME_ASCII = """\0
+        ____   _         ____              
+       / __ \ (_)____   / __ \ __  __ ____ 
+      / / / // // __ \ / / / // / / // __ \\
+     / /_/ // // /_/ // /_/ // /_/ // /_/ /
+    /_____//_// .___//_____/ \__,_// .___/ 
+             /_/                  /_/      
+"""
+EPILOG = """\0
+Documentation:         https://docs.dipdup.io
+GitHub:                https://github.com/dipdup-io/dipdup
+Discord:               https://discord.gg/NbANhqCJHA
+"""
+
 
 class Colors:
     """ANSI color codes"""
 
     BLUE = '\033[34m'
     GREEN = '\033[92m'
     YELLOW = '\033[93m'
@@ -51,203 +66,220 @@
 
 
 def done(msg: str) -> NoReturn:
     echo(msg, color=Colors.GREEN)
     sys.exit(0)
 
 
-def ask(msg: str, default: bool, quiet: bool) -> bool:
-    msg += ' [Y/n]' if default else ' [y/N]'
-    echo(msg, Colors.YELLOW)
-
-    if quiet:
-        return default
-    if default:
-        return input().lower() not in ('n', 'no')
-    else:
-        return input().lower() in ('y', 'yes')
-
-
 # NOTE: DipDup has `tabulate` dep, don't use this one elsewhere
 def _tab(text: str, indent: int = 20) -> str:
     return text + ' ' * (indent - len(text))
 
 
 class DipDupEnvironment:
-    def __init__(self, quiet: bool = False) -> None:
+    def __init__(self) -> None:
         self._os = os.uname().sysname
         self._arch = os.uname().machine
-        self._quiet = quiet
         self._commands: Dict[str, Optional[str]] = {}
         self._pipx_packages: Set[str] = set()
 
     def refresh(self) -> None:
-        if not self._quiet and not self._commands:
-            print()
-            print(_tab('OS:') + self._os)
-            print(_tab('Arch:') + self._arch)
-            print(_tab('Python:') + sys.version)
-            print(_tab('PATH:') + os.environ['PATH'])
-            print()
-
         for command in WHICH_CMDS:
             old, new = self._commands.get(command), which(command)
             if old == new:
                 continue
             self._commands[command] = new
-            self._quiet or print(_tab(command) + (new or ''))
 
+    def print(self) -> None:
+        print()
+        print(WELCOME_ASCII)
+        print(EPILOG)
+        print()
+        print(_tab('OS:') + f'{self._os} ({self._arch})')
+        print(_tab('Python:') + sys.version)
+        print(_tab('PATH:') + os.environ['PATH'])
+        print(_tab('PYTHONPATH:') + os.environ.get('PYTHONPATH', ''))
         print()
+        for command, path in self._commands.items():
+            print(_tab(f'{command}:') + (path or ''))
+        print(_tab('pipx packages:') + ', '.join(self._pipx_packages) + '\n')
 
     def refresh_pipx(self) -> None:
         """Get installed pipx packages"""
         self.ensure_pipx()
         pipx_packages_raw = self.run_cmd('pipx', 'list', '--short', capture_output=True).stdout
         self._pipx_packages = {p.split()[0].decode() for p in pipx_packages_raw.splitlines()}
-        self._quiet or print(_tab('pipx packages:') + ', '.join(self._pipx_packages) + '\n')
-
-    def check(self) -> None:
-        if not sys.version.startswith('3.10'):
-            fail('DipDup requires Python 3.10')
 
+    def prepare(self) -> None:
         # NOTE: Show warning if user is root
         if os.geteuid() == 0:
             echo('WARNING: Running as root, this is not generally recommended', Colors.YELLOW)
 
         # NOTE: Show warning if user is in virtualenv
         if sys.base_prefix != sys.prefix:
             echo('WARNING: Running in virtualenv, this script affects only current user', Colors.YELLOW)
 
         self.refresh()
         self.refresh_pipx()
 
-        if self._commands.get('pyenv'):
-            echo('WARNING: pyenv is installed, this may cause issues', Colors.YELLOW)
-
     def run_cmd(self, cmd: str, *args: Any, **kwargs: Any) -> subprocess.CompletedProcess[bytes]:
         """Run command safely (relatively lol)"""
         if (found_cmd := self._commands.get(cmd)) is None:
             fail(f'Command not found: {cmd}')
         args = (found_cmd,) + tuple(a for a in args if a)
         try:
             return subprocess.run(
                 args,
                 **kwargs,
                 check=True,
             )
         except subprocess.CalledProcessError as e:
-            self._quiet or fail(f'{cmd} failed: {e.cmd} {e.returncode}')
-            raise
+            fail(f'{cmd} failed: {e.cmd} {e.returncode}')
 
     def ensure_pipx(self) -> None:
+        if not sys.version.startswith('3.11'):
+            fail('DipDup requires Python 3.11')
+
         """Ensure pipx is installed for current user"""
         if self._commands.get('pipx'):
             return
 
-        if sys.prefix != sys.base_prefix:
-            fail("pipx can't be installed in virtualenv, run `deactivate` and try again")
-
         echo('Installing pipx')
-        self.run_cmd('python3', '-m', 'pip', 'install', '--user', '-q', 'pipx')
-        self.run_cmd('python3', '-m', 'pipx', 'ensurepath')
-        os.environ['PATH'] = os.environ['PATH'] + ':' + str(Path.home() / '.local' / 'bin')
-        os.execv(sys.executable, [sys.executable] + sys.argv)
+        if sys.base_prefix != sys.prefix:
+            self.run_cmd('python3.11', '-m', 'pip', 'install', '-q', 'pipx')
+        else:
+            self.run_cmd('python3.11', '-m', 'pip', 'install', '--user', '-q', 'pipx')
+        self.run_cmd('python3.11', '-m', 'pipx', 'ensurepath')
+        pipx_path = str(Path.home() / '.local' / 'bin')
+        os.environ['PATH'] = pipx_path + os.pathsep + os.environ['PATH']
+        self._commands['pipx'] = which('pipx')
 
 
 def install(
     quiet: bool,
     force: bool,
+    version: str | None,
     ref: str | None,
     path: str | None,
 ) -> None:
     """Install DipDup and its dependencies with pipx"""
     if ref and path:
         fail('Specify either ref or path, not both')
 
+    if not any((version, ref, path)):
+        # FIXME: Temporary, remove when 7.0.0 is released
+        version = '7.0.0rc1'
+
     env = DipDupEnvironment()
-    env.check()
+    env.prepare()
+    if not quiet:
+        env.print()
 
     force_str = '--force' if force else ''
     pipx_packages = env._pipx_packages
     pipx_dipdup = 'dipdup' in pipx_packages
     pipx_datamodel_codegen = 'datamodel-code-generator' in pipx_packages
-    pipx_poetry = 'poetry' in pipx_packages
+    pipx_pdm = 'pdm' in pipx_packages
+
+    python_inter_pipx = cast(str, which('python3.11'))
+    if 'pyenv' in python_inter_pipx:
+        python_inter_pipx = (
+            subprocess.run(['pyenv', 'which', 'python3.11'], capture_output=True, text=True)
+            .stdout.strip()
+            .split('\n')[0]
+        )
 
-    if pipx_dipdup:
+    if pipx_dipdup and not force:
         echo('Updating DipDup')
         env.run_cmd('pipx', 'upgrade', 'dipdup', force_str)
     else:
         if path:
             echo(f'Installing DipDup from `{path}`')
-            env.run_cmd('pipx', 'install', path, force_str)
+            env.run_cmd('pipx', 'install', '--python', python_inter_pipx, path, force_str)
         elif ref:
-            echo(f'Installing DipDup from `{ref}`')
-            env.run_cmd('pipx', 'install', f'git+{GITHUB}@{ref}', force_str)
+            url = f'git+{GITHUB}@{ref}'
+            echo(f'Installing DipDup from `{url}`')
+            env.run_cmd('pipx', 'install', '--python', python_inter_pipx, url, force_str)
         else:
             echo('Installing DipDup from PyPI')
-            env.run_cmd('pipx', 'install', 'dipdup', force_str)
+            pkg = 'dipdup' if not version else f'dipdup=={version}'
+            env.run_cmd('pipx', 'install', '--python', python_inter_pipx, pkg, force_str)
 
     if pipx_datamodel_codegen:
         env.run_cmd('pipx', 'upgrade', 'datamodel-code-generator', force_str)
     else:
-        env.run_cmd('pipx', 'install', 'datamodel-code-generator', force_str)
+        env.run_cmd('pipx', 'install', '--python', python_inter_pipx, 'datamodel-code-generator', force_str)
 
-    if (legacy_poetry := Path(Path.home(), '.poetry')).exists():
-        rmtree(legacy_poetry, ignore_errors=True)
-        env.run_cmd('pipx', 'install', 'poetry', force_str)
-    elif pipx_poetry:
-        echo('Updating Poetry')
-        env.run_cmd('pipx', 'upgrade', 'poetry', force_str)
-    elif ask('Install poetry? Optional for `dipdup new` command', True, quiet):
-        echo('Installing poetry')
-        env.run_cmd('pipx', 'install', 'poetry', force_str)
-        env._commands['poetry'] = which('poetry')
-        pipx_poetry = True
+    if pipx_pdm:
+        echo('Updating PDM')
+        env.run_cmd('pipx', 'upgrade', 'pdm', force_str)
+    elif quiet or ask('Install PDM? (recommended)', True):
+        echo('Installing PDM')
+        env.run_cmd('pipx', 'install', '--python', python_inter_pipx, 'pdm', force_str)
+        env._commands['pdm'] = which('pdm')
+        pipx_pdm = True
 
     done(
-        'Done! DipDup is ready to use.\nRun `dipdup new` to create a new project or `dipdup` to see all available commands.'
+        'Done! DipDup is ready to use.\nRun `dipdup new` to create a new project or `dipdup` to see all available'
+        ' commands.'
     )
 
 
+def ask(question: str, default: bool) -> bool:
+    """Ask user a yes/no question"""
+    while True:
+        answer = input(question + (' [Y/n] ' if default else ' [y/N] ')).lower().strip()
+        if not answer:
+            return default
+        return answer in ('n', 'no') if default else answer in ('y', 'yes')
+
+
 def uninstall(quiet: bool) -> NoReturn:
     """Uninstall DipDup and its dependencies with pipx"""
     env = DipDupEnvironment()
-    env.check()
-
-    pipx_packages = env._pipx_packages
+    env.prepare()
+    if not quiet:
+        env.print()
+
+    packages = (
+        ('dipdup', True),
+        ('datamodel-code-generator', False),
+        ('pdm', False),
+    )
+    for package, default in packages:
+        if package not in env._pipx_packages:
+            continue
+        if not quiet and not ask(f'Uninstall {package}?', default):
+            continue
 
-    if 'dipdup' in pipx_packages:
-        echo('Uninstalling DipDup')
-        env.run_cmd('pipx', 'uninstall', 'dipdup')
-
-    if 'datamodel-code-generator' in pipx_packages:
-        if ask('Uninstall datamodel-code-generator?', True, quiet):
-            echo('Uninstalling datamodel-code-generator')
-            env.run_cmd('pipx', 'uninstall', 'datamodel-code-generator')
+        echo(f'Uninstalling {package}')
+        env.run_cmd('pipx', 'uninstall', package)
 
     done('Done! DipDup is uninstalled.')
 
 
 def cli() -> None:
     echo('Welcome to DipDup installer')
 
     parser = argparse.ArgumentParser()
     parser.add_argument('-q', '--quiet', action='store_true', help='Use default answers for all questions')
     parser.add_argument('-f', '--force', action='store_true', help='Force reinstall')
+    parser.add_argument('-v', '--version', help='Install DipDup from a specific version')
     parser.add_argument('-r', '--ref', help='Install DipDup from a specific git ref')
     parser.add_argument('-p', '--path', help='Install DipDup from a local path')
     parser.add_argument('-u', '--uninstall', action='store_true', help='Uninstall DipDup')
     args = parser.parse_args()
 
     if args.uninstall:
         uninstall(args.quiet)
     else:
         install(
             quiet=args.quiet,
             force=args.force,
+            version=args.version.strip() if args.version else None,
             ref=args.ref.strip() if args.ref else None,
             path=args.path.strip() if args.path else None,
         )
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `dipdup-6.5.9/src/dipdup/models.py` & `dipdup-7.0.0rc1/src/dipdup/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,296 +1,119 @@
+from __future__ import annotations
+
 import logging
-from collections import defaultdict
 from collections import deque
+from contextlib import suppress
 from copy import copy
-from dataclasses import field
 from datetime import date
 from datetime import datetime
 from datetime import time
 from decimal import Decimal
 from enum import Enum
-from functools import cache
 from typing import Any
-from typing import DefaultDict
-from typing import Dict
-from typing import Generic
 from typing import Iterable
-from typing import List
-from typing import Optional
-from typing import Set
-from typing import Type
 from typing import TypeVar
 from typing import cast
 
-from pydantic import BaseModel
+import tortoise
+import tortoise.queryset
 from pydantic.dataclasses import dataclass
-from tortoise import fields
 from tortoise.backends.base.client import BaseDBAsyncClient
+from tortoise.exceptions import OperationalError
 from tortoise.expressions import Q
 from tortoise.fields import relational
 from tortoise.models import MODEL
 from tortoise.models import Model as TortoiseModel
 from tortoise.queryset import BulkCreateQuery as TortoiseBulkCreateQuery
 from tortoise.queryset import BulkUpdateQuery as TortoiseBulkUpdateQuery
 from tortoise.queryset import DeleteQuery as TortoiseDeleteQuery
 from tortoise.queryset import QuerySet as TortoiseQuerySet
 from tortoise.queryset import UpdateQuery as TortoiseUpdateQuery
 
-from dipdup.enums import IndexStatus
-from dipdup.enums import IndexType
-from dipdup.enums import ReindexingReason
-from dipdup.enums import TokenStandard
+from dipdup import fields
 from dipdup.exceptions import FrameworkException
-from dipdup.utils import json_dumps_decimals
-
-ParameterType = TypeVar('ParameterType', bound=BaseModel)
-StorageType = TypeVar('StorageType', bound=BaseModel)
-KeyType = TypeVar('KeyType', bound=BaseModel)
-ValueType = TypeVar('ValueType', bound=BaseModel)
-EventType = TypeVar('EventType', bound=BaseModel)
-
+from dipdup.performance import caches
+from dipdup.utils import json_dumps_plain
 
 _logger = logging.getLogger(__name__)
 
-# ===> Dataclasses
-
-
-@dataclass
-class OperationData:
-    """Basic structure for operations from TzKT response"""
-
-    type: str
-    id: int
-    level: int
-    timestamp: datetime
-    hash: str
-    counter: int
-    sender_address: Optional[str]
-    target_address: Optional[str]
-    initiator_address: Optional[str]
-    amount: Optional[int]
-    status: str
-    has_internals: Optional[bool]
-    storage: Any
-    diffs: tuple[Dict[str, Any], ...] = field(default_factory=tuple)
-    block: Optional[str] = None
-    sender_alias: Optional[str] = None
-    nonce: Optional[int] = None
-    target_alias: Optional[str] = None
-    initiator_alias: Optional[str] = None
-    entrypoint: Optional[str] = None
-    parameter_json: Optional[Any] = None
-    originated_contract_address: Optional[str] = None
-    originated_contract_alias: Optional[str] = None
-    originated_contract_type_hash: Optional[int] = None
-    originated_contract_code_hash: Optional[int] = None
-    originated_contract_tzips: Optional[tuple[str, ...]] = None
-    delegate_address: Optional[str] = None
-    delegate_alias: Optional[str] = None
-    target_code_hash: Optional[int] = None
-    sender_code_hash: Optional[int] = None
-
-
-@dataclass
-class Transaction(Generic[ParameterType, StorageType]):
-    """Wrapper for matched transaction with typed data passed to the handler"""
-
-    data: OperationData
-    parameter: ParameterType
-    storage: StorageType
-
-
-@dataclass
-class Origination(Generic[StorageType]):
-    """Wrapper for matched origination with typed data passed to the handler"""
-
-    data: OperationData
-    storage: StorageType
-
-
-class BigMapAction(Enum):
-    """Mapping for action in TzKT response"""
-
-    ALLOCATE = 'allocate'
-    ADD_KEY = 'add_key'
-    UPDATE_KEY = 'update_key'
-    REMOVE_KEY = 'remove_key'
-    REMOVE = 'remove'
 
-    @property
-    def has_key(self) -> bool:
-        return self in (BigMapAction.ADD_KEY, BigMapAction.UPDATE_KEY, BigMapAction.REMOVE_KEY)
+# NOTE: Skip expensive copy() calls on each queryset update. Doesn't affect us. Definitely will be in Kleinmann officially.
+tortoise.queryset.QuerySet._clone = lambda self: self  # type: ignore[method-assign]
 
-    @property
-    def has_value(self) -> bool:
-        return self in (BigMapAction.ADD_KEY, BigMapAction.UPDATE_KEY)
 
+class IndexType(Enum):
+    """Enum for `dipdup.models.Index`"""
 
-@dataclass
-class BigMapData:
-    """Basic structure for big map diffs from TzKT response"""
+    tezos_tzkt_operations = 'tezos.tzkt.operations'
+    tezos_tzkt_operations_unfiltered = 'tezos.tzkt.operations_unfiltered'
+    tezos_tzkt_big_maps = 'tezos.tzkt.big_maps'
+    tezos_tzkt_head = 'tezos.tzkt.head'
+    tezos_tzkt_token_transfers = 'tezos.tzkt.token_transfers'
+    tezos_tzkt_events = 'tezos.tzkt.events'
+    evm_subsquid_operations = 'evm.subsquid.operations'
+    evm_subsquid_events = 'evm.subsquid.events'
 
-    id: int
-    level: int
-    operation_id: int
-    timestamp: datetime
-    bigmap: int
-    contract_address: str
-    path: str
-    action: BigMapAction
-    active: bool
-    key: Optional[Any] = None
-    value: Optional[Any] = None
 
+class MessageType:
+    value: str
 
-@dataclass
-class BigMapDiff(Generic[KeyType, ValueType]):
-    """Wrapper for matched big map diff with typed data passed to the handler"""
 
-    action: BigMapAction
-    data: BigMapData
-    key: Optional[KeyType]
-    value: Optional[ValueType]
+class IndexStatus(Enum):
+    new = 'new'
+    syncing = 'syncing'
+    realtime = 'realtime'
+    disabled = 'disabled'
+    failed = 'failed'
 
 
-@dataclass
-class BlockData:
-    """Basic structure for blocks received from TzKT REST API"""
+# NOTE: Used as a key in config, must inherit from str
+class ReindexingReason(str, Enum):
+    """Reason that caused reindexing"""
 
-    level: int
-    hash: str
-    timestamp: datetime
-    proto: int
-    validations: int
-    deposit: int
-    reward: int
-    fees: int
-    nonce_revealed: bool
-    priority: Optional[int] = None
-    baker_address: Optional[str] = None
-    baker_alias: Optional[str] = None
+    manual = 'manual'
+    migration = 'migration'
+    rollback = 'rollback'
+    config_modified = 'config_modified'
+    schema_modified = 'schema_modified'
 
 
-@dataclass
-class HeadBlockData:
-    """Basic structure for head block received from TzKT SignalR API"""
+class ReindexingAction(Enum):
+    """Action that should be performed on reindexing"""
 
-    chain: str
-    chain_id: str
-    cycle: int
-    level: int
-    hash: str
-    protocol: str
-    next_protocol: str
-    timestamp: datetime
-    voting_epoch: int
-    voting_period: int
-    known_level: int
-    last_sync: datetime
-    synced: bool
-    quote_level: int
-    quote_btc: Decimal
-    quote_eur: Decimal
-    quote_usd: Decimal
-    quote_cny: Decimal
-    quote_jpy: Decimal
-    quote_krw: Decimal
-    quote_eth: Decimal
-    quote_gbp: Decimal
+    exception = 'exception'
+    wipe = 'wipe'
+    ignore = 'ignore'
 
 
-@dataclass
-class QuoteData:
-    """Basic structure for quotes received from TzKT REST API"""
+class SkipHistory(Enum):
+    """Whether to skip indexing operation history and use only current state"""
 
-    level: int
-    timestamp: datetime
-    btc: Decimal
-    eur: Decimal
-    usd: Decimal
-    cny: Decimal
-    jpy: Decimal
-    krw: Decimal
-    eth: Decimal
-    gbp: Decimal
-
-
-@dataclass
-class TokenTransferData:
-    """Basic structure for token transver received from TzKT SignalR API"""
-
-    id: int
-    level: int
-    timestamp: datetime
-    tzkt_token_id: int
-    contract_address: Optional[str] = None
-    contract_alias: Optional[str] = None
-    token_id: Optional[int] = None
-    standard: Optional[TokenStandard] = None
-    metadata: Optional[Dict[str, Any]] = None
-    from_alias: Optional[str] = None
-    from_address: Optional[str] = None
-    to_alias: Optional[str] = None
-    to_address: Optional[str] = None
-    amount: Optional[int] = None
-    tzkt_transaction_id: Optional[int] = None
-    tzkt_origination_id: Optional[int] = None
-    tzkt_migration_id: Optional[int] = None
-
-
-@dataclass
-class EventData:
-    """Basic structure for events received from TzKT REST API"""
-
-    id: int
-    level: int
-    timestamp: datetime
-    tag: str
-    payload: Any | None
-    contract_address: str
-    contract_alias: Optional[str] = None
-    contract_code_hash: Optional[int] = None
-    transaction_id: Optional[int] = None
-
-
-@dataclass
-class Event(Generic[EventType]):
-    data: EventData
-    payload: EventType
-
-
-@dataclass
-class UnknownEvent:
-    data: EventData
-    payload: Any | None
-
-
-# ===> Model Versioning
-
-
-versioned_fields: DefaultDict[str, Set[str]] = defaultdict(set)
+    never = 'never'
+    once = 'once'
+    always = 'always'
 
 
 @dataclass
 class VersionedTransaction:
     """Metadata of currently opened versioned transaction."""
 
     level: int
     index: str
-    immune_tables: Set[str]
+    immune_tables: set[str]
 
 
 # NOTE: Overwritten by TransactionManager.register()
-def get_transaction() -> Optional[VersionedTransaction]:
+def get_transaction() -> VersionedTransaction | None:
     """Get metadata of currently opened versioned transaction if any"""
     raise FrameworkException('TransactionManager is not registered')
 
 
 # NOTE: Overwritten by TransactionManager.register()
-def get_pending_updates() -> deque['ModelUpdate']:
+def get_pending_updates() -> deque[ModelUpdate]:
     """Get pending model updates queue"""
     raise FrameworkException('TransactionManager is not registered')
 
 
 class ModelUpdateAction(Enum):
     """Mapping for actions in model update"""
 
@@ -298,30 +121,30 @@
     UPDATE = 'UPDATE'
     DELETE = 'DELETE'
 
 
 class ModelUpdate(TortoiseModel):
     """Model update created within versioned transactions"""
 
-    model_name = fields.CharField(256)
-    model_pk = fields.CharField(256)
+    model_name = fields.TextField()
+    model_pk = fields.TextField()
     level = fields.IntField()
-    index = fields.CharField(256)
+    index = fields.TextField()
 
-    action = fields.CharEnumField(ModelUpdateAction)
-    data: Dict[str, Any] = fields.JSONField(encoder=json_dumps_decimals, null=True)
+    action = fields.EnumField(ModelUpdateAction)
+    data: dict[str, Any] = fields.JSONField(encoder=json_dumps_plain, null=True)
 
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True)
 
     class Meta:
         table = 'dipdup_model_update'
 
     @classmethod
-    def from_model(cls, model: 'Model', action: ModelUpdateAction) -> Optional['ModelUpdate']:
+    def from_model(cls, model: 'Model', action: ModelUpdateAction) -> 'ModelUpdate' | None:
         """Create model update from model instance if necessary"""
         if not (transaction := get_transaction()):
             return None
         if model._meta.db_table in transaction.immune_tables:
             return None
 
         if action == ModelUpdateAction.INSERT:
@@ -348,15 +171,15 @@
             self.model_name,
             self.model_pk,
             self.action.value,
             data,
         )
         return self
 
-    async def revert(self, model: Type[TortoiseModel]) -> None:
+    async def revert(self, model: type[TortoiseModel]) -> None:
         """Revert a single model update"""
         data = copy(self.data)
         # NOTE: Deserialize non-JSON types
         if data:
             for key, field_ in model._meta.fields_map.items():
                 # NOTE: Restore deleted models with old PK
                 if field_.pk and self.action == ModelUpdateAction.DELETE:
@@ -395,22 +218,22 @@
 
         await self.delete()
 
 
 class UpdateQuery(TortoiseUpdateQuery):
     def __init__(
         self,
-        model: Type[TortoiseModel],
-        update_kwargs: Dict[str, Any],
+        model: type[TortoiseModel],
+        update_kwargs: dict[str, Any],
         db: BaseDBAsyncClient,
-        q_objects: List[Q],
-        annotations: Dict[str, Any],
-        custom_filters: Dict[str, Dict[str, Any]],
-        limit: Optional[int],
-        orderings: List[tuple[str, str]],
+        q_objects: list[Q],
+        annotations: dict[str, Any],
+        custom_filters: dict[str, dict[str, Any]],
+        limit: int | None,
+        orderings: list[tuple[str, str]],
         filter_queryset: TortoiseQuerySet,  # type: ignore[type-arg]
     ) -> None:
         super().__init__(
             model,
             update_kwargs,
             db,
             q_objects,
@@ -435,21 +258,21 @@
 
         return await super()._execute()
 
 
 class DeleteQuery(TortoiseDeleteQuery):
     def __init__(
         self,
-        model: Type[TortoiseModel],
+        model: type[TortoiseModel],
         db: BaseDBAsyncClient,
-        q_objects: List[Q],
-        annotations: Dict[str, Any],
-        custom_filters: Dict[str, Dict[str, Any]],
-        limit: Optional[int],
-        orderings: List[tuple[str, str]],
+        q_objects: list[Q],
+        annotations: dict[str, Any],
+        custom_filters: dict[str, dict[str, Any]],
+        limit: int | None,
+        orderings: list[tuple[str, str]],
         filter_queryset: TortoiseQuerySet,  # type: ignore[type-arg]
     ) -> None:
         super().__init__(model, db, q_objects, annotations, custom_filters, limit, orderings)
         self.filter_queryset = filter_queryset
 
     async def _execute(self) -> int:
         _logger.debug('Prefetching query models: %s', self.filter_queryset)
@@ -472,15 +295,15 @@
             ):
                 get_pending_updates().append(update)
 
         return await super()._execute()
 
 
 class BulkCreateQuery(TortoiseBulkCreateQuery):
-    async def _execute(self) -> List[MODEL]:
+    async def _execute(self) -> list[MODEL]:
         for model in self.objects:
             if update := ModelUpdate.from_model(
                 cast(Model, model),
                 ModelUpdateAction.INSERT,
             ):
                 get_pending_updates().append(update)
 
@@ -514,30 +337,37 @@
             custom_filters=self._custom_filters,
             limit=self._limit,
             orderings=self._orderings,
             filter_queryset=self,
         )
 
 
-@cache
-def get_versioned_fields(model: Type['Model']) -> Set[str]:
-    field_names: Set[str] = set()
+# NOTE: Don't register cache; plain dict is faster
+_versioned_fields: dict[type['Model'], frozenset[str]] = {}
+
+
+def get_versioned_fields(model: type['Model']) -> frozenset[str]:
+    if model in _versioned_fields:
+        return _versioned_fields[model]
+
+    field_names: set[str] = set()
     field_keys = model._meta.db_fields.union(model._meta.fk_fields)
 
     for key, field_ in model._meta.fields_map.items():
         if key not in field_keys:
             continue
         if field_.pk:
             continue
         elif isinstance(field_, relational.ForeignKeyFieldInstance):
             field_names.add(f'{key}_id')
         else:
             field_names.add(key)
 
-    return field_names
+    _versioned_fields[model] = frozenset(field_names)
+    return frozenset(field_names)
 
 
 class Model(TortoiseModel):
     """Base class for DipDup project models"""
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
@@ -546,46 +376,46 @@
     @classmethod
     def _init_from_db(cls, **kwargs: Any) -> 'Model':
         model = super()._init_from_db(**kwargs)
         model._original_versioned_data = model.versioned_data
         return model
 
     @property
-    def original_versioned_data(self) -> Dict[str, Any]:
+    def original_versioned_data(self) -> dict[str, Any]:
         """Get versioned data of the model at the time of creation"""
         return self._original_versioned_data
 
     @property
-    def versioned_data(self) -> Dict[str, Any]:
+    def versioned_data(self) -> dict[str, Any]:
         """Get versioned data of the model at the current time"""
         return {name: getattr(self, name) for name in get_versioned_fields(self.__class__)}
 
     @property
-    def versioned_data_diff(self) -> Dict[str, Any]:
+    def versioned_data_diff(self) -> dict[str, Any]:
         """Get versioned data of the model changed since creation"""
         data = {}
         for key, value in self.original_versioned_data.items():
             if value != self.versioned_data[key]:
                 data[key] = value
         return data
 
     # NOTE: Do not touch docstrings below this line to preserve Tortoise ones
     async def delete(
         self,
-        using_db: Optional[BaseDBAsyncClient] = None,
+        using_db: BaseDBAsyncClient | None = None,
     ) -> None:
         await super().delete(using_db=using_db)
 
         if update := ModelUpdate.from_model(self, ModelUpdateAction.DELETE):
             get_pending_updates().append(update)
 
     async def save(
         self,
-        using_db: Optional[BaseDBAsyncClient] = None,
-        update_fields: Optional[Iterable[str]] = None,
+        using_db: BaseDBAsyncClient | None = None,
+        update_fields: Iterable[str] | None = None,
         force_create: bool = False,
         force_update: bool = False,
     ) -> None:
         action = ModelUpdateAction.UPDATE if self._saved_in_db else ModelUpdateAction.INSERT
         await super().save(
             using_db=using_db,
             update_fields=update_fields,
@@ -598,33 +428,33 @@
 
     @classmethod
     def filter(cls, *args: Any, **kwargs: Any) -> TortoiseQuerySet:  # type: ignore[type-arg]
         return QuerySet(cls).filter(*args, **kwargs)
 
     @classmethod
     async def create(
-        cls: Type['ModelT'],
-        using_db: Optional[BaseDBAsyncClient] = None,
+        cls: type['ModelT'],
+        using_db: BaseDBAsyncClient | None = None,
         **kwargs: Any,
     ) -> 'ModelT':
         instance = cls(**kwargs)
         instance._saved_in_db = False
         db = using_db or cls._choose_db(True)
         await instance.save(using_db=db, force_create=True)
         return instance
 
     @classmethod
     def bulk_create(
-        cls: Type['Model'],
+        cls: type['Model'],
         objects: Iterable['Model'],
-        batch_size: Optional[int] = None,
+        batch_size: int | None = None,
         ignore_conflicts: bool = False,
-        update_fields: Optional[Iterable[str]] = None,
-        on_conflict: Optional[Iterable[str]] = None,
-        using_db: Optional[BaseDBAsyncClient] = None,
+        update_fields: Iterable[str] | None = None,
+        on_conflict: Iterable[str] | None = None,
+        using_db: BaseDBAsyncClient | None = None,
     ) -> BulkCreateQuery:
         if ignore_conflicts and update_fields:
             raise ValueError(
                 'ignore_conflicts and update_fields are mutually exclusive.',
             )
         if not ignore_conflicts:
             if (update_fields and not on_conflict) or (on_conflict and not update_fields):
@@ -638,19 +468,19 @@
             ignore_conflicts=ignore_conflicts,
             update_fields=update_fields,
             on_conflict=on_conflict,
         )
 
     @classmethod
     def bulk_update(
-        cls: Type['Model'],
+        cls: type['Model'],
         objects: Iterable['Model'],
         fields: Iterable[str],
-        batch_size: Optional[int] = None,
-        using_db: Optional[BaseDBAsyncClient] = None,
+        batch_size: int | None = None,
+        using_db: BaseDBAsyncClient | None = None,
     ) -> BulkUpdateQuery:
         if any(obj.pk is None for obj in objects):
             raise ValueError('All bulk_update() objects must have a primary key set.')
 
         self = QuerySet(cls)
         return BulkUpdateQuery(
             db=self._db,
@@ -665,98 +495,159 @@
             batch_size=batch_size,
         )
 
     class Meta:
         abstract = True
 
 
+class CachedModel(Model):
+    @classmethod
+    async def preload(cls) -> None:
+        # NOTE: Table can be missing
+        with suppress(OperationalError):
+            async for model in cls.all():
+                model.cache()
+
+    @classmethod
+    async def cached_get(
+        cls: type['ModelT'],
+        pk: int | str,
+    ) -> 'ModelT':
+        cls_cache = caches._model[cls.__name__]
+
+        if pk not in cls_cache:
+            cls_cache[pk] = await cls.get(pk=pk)
+        return cls_cache[pk]  # type: ignore[return-value]
+
+    @classmethod
+    async def cached_get_or_none(
+        cls: type['ModelT'],
+        pk: int | str,
+    ) -> 'ModelT' | None:
+        cls_cache = caches._model[cls.__name__]
+
+        if pk not in cls_cache:
+            cls_cache[pk] = await cls.get_or_none(pk=pk)  # type: ignore[assignment]
+        return cls_cache[pk]  # type: ignore[return-value]
+
+    def cache(self) -> None:
+        cls_cache = caches._model[self.__class__.__name__]
+        if self.pk is None:
+            raise FrameworkException('Cannot cache model without PK')
+        if self.pk in cls_cache:
+            raise FrameworkException(f'Model {self} is already cached')
+        cls_cache[self.pk] = self
+
+    class Meta:
+        abstract = True
+
+
 ModelT = TypeVar('ModelT', bound=Model)
 
 
 # ===> Built-in Models (not versioned)
 
 
 class Schema(TortoiseModel):
-    name = fields.CharField(256, pk=True)
-    hash = fields.CharField(256)
-    reindex = fields.CharEnumField(ReindexingReason, max_length=40, null=True)
+    name = fields.TextField(pk=True)
+    hash = fields.TextField(null=True)
+    reindex = fields.EnumField(ReindexingReason, null=True)
 
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True)
 
     class Meta:
         table = 'dipdup_schema'
 
 
 class Head(TortoiseModel):
-    name = fields.CharField(256, pk=True)
+    name = fields.TextField(pk=True)
     level = fields.IntField()
-    hash = fields.CharField(64)
+    hash = fields.TextField(null=True)
     timestamp = fields.DatetimeField()
 
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True)
 
     class Meta:
         table = 'dipdup_head'
 
 
 class Index(TortoiseModel):
-    name = fields.CharField(256, pk=True)
-    type = fields.CharEnumField(IndexType)
-    status = fields.CharEnumField(IndexStatus, default=IndexStatus.NEW)
-
-    config_hash = fields.CharField(256)
-    template = fields.CharField(256, null=True)
-    template_values: Dict[str, Any] = fields.JSONField(null=True)
+    name = fields.TextField(pk=True)
+    type = fields.EnumField(IndexType)
+    status = fields.EnumField(IndexStatus, default=IndexStatus.new)
+
+    config_hash = fields.TextField(null=True)
+    template = fields.TextField(null=True)
+    template_values: dict[str, Any] = fields.JSONField(encoder=json_dumps_plain, null=True)
 
     level = fields.IntField(default=0)
 
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True)
 
     class Meta:
         table = 'dipdup_index'
 
 
+class ContractKind(Enum):
+    """Mapping for contract kind in"""
+
+    TEZOS = 'tezos'
+    EVM = 'evm'
+
+
 class Contract(TortoiseModel):
-    name = fields.CharField(256, pk=True)
-    address = fields.CharField(256)
-    # TODO: Add `code_hash` field
-    typename = fields.CharField(256, null=True)
+    name = fields.TextField(pk=True)
+    address = fields.TextField(null=True)
+    code_hash = fields.BigIntField(null=True)
+    typename = fields.TextField(null=True)
+    kind = fields.EnumField(ContractKind)
 
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True)
 
     class Meta:
         table = 'dipdup_contract'
 
 
+class Meta(TortoiseModel):
+    key = fields.TextField(pk=True)
+    value = fields.JSONField(encoder=json_dumps_plain, null=True)
+
+    created_at = fields.DatetimeField(auto_now_add=True)
+    updated_at = fields.DatetimeField(auto_now=True)
+
+    class Meta:
+        table = 'dipdup_meta'
+
+
 # ===> Built-in Models (versioned)
 
 
 class ContractMetadata(Model):
-    network = fields.CharField(51)
-    contract = fields.CharField(36)
-    metadata = fields.JSONField()
+    network = fields.TextField()
+    contract = fields.TextField()
+    metadata = fields.JSONField(encoder=json_dumps_plain, null=True)
     update_id = fields.IntField()
 
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True)
 
     class Meta:
         table = 'dipdup_contract_metadata'
         unique_together = ('network', 'contract')
 
 
 class TokenMetadata(Model):
-    network = fields.CharField(51)
-    contract = fields.CharField(36)
+    network = fields.TextField()
+    contract = fields.TextField()
     token_id = fields.TextField()
-    metadata = fields.JSONField()
+    metadata = fields.JSONField(encoder=json_dumps_plain, null=True)
     update_id = fields.IntField()
 
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True)
 
     class Meta:
         table = 'dipdup_token_metadata'
```

### Comparing `dipdup-6.5.9/src/dipdup/project.py` & `dipdup-7.0.0rc1/src/dipdup/config/tezos_tzkt_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,346 +1,364 @@
-import logging
-from pathlib import Path
-from types import NoneType
-from typing import Any
-
-import asyncclick as cl
-import orjson as json
-from pydantic import BaseModel
-from pydantic import Field
-from tabulate import tabulate
+from __future__ import annotations
 
-from dipdup import __version__
+from dataclasses import field
+from typing import Any
+from typing import Iterator
+from typing import Literal
+from typing import cast
+
+from pydantic.dataclasses import dataclass
+
+from dipdup.config import CodegenMixin
+from dipdup.config import ContractConfig
+from dipdup.config import HandlerConfig
+from dipdup.config.tezos import TezosContractConfig
+from dipdup.config.tezos_tzkt import TzktDatasourceConfig
+from dipdup.config.tezos_tzkt import TzktIndexConfig
+from dipdup.exceptions import ConfigInitializationException
 from dipdup.exceptions import ConfigurationError
-from dipdup.utils.codegen import load_template
-from dipdup.utils.codegen import write
-
-_logger = logging.getLogger('dipdup.project')
+from dipdup.models.tezos_tzkt import OriginationSubscription
+from dipdup.models.tezos_tzkt import TransactionSubscription
+from dipdup.models.tezos_tzkt import TzktOperationType
+from dipdup.subscriptions import Subscription
+from dipdup.utils import pascal_to_snake
+from dipdup.utils import snake_to_pascal
+
+
+@dataclass
+class SubgroupIndexMixin:
+    """`subgroup_index` field to track index of operation in group
 
+    :param subgroup_index:
+    """
 
-DEMO_PROJECTS = (
-    ('demo_domains', 'Tezos Domains name service'),
-    ('demo_big_maps', 'Indexing specific big maps'),
-    ('demo_events', 'Processing contract events'),
-    ('demo_head', 'Processing head block metadata'),
-    ('demo_nft_marketplace', 'hic at nunc NFT marketplace'),
-    ('demo_dex', 'Quipuswap DEX balances and liquidity'),
-    ('demo_factories', 'Example of spawning indexes in runtime'),
-    ('demo_dao', 'Homebase DAO registry'),
-    ('demo_token', 'TzBTC FA1.2 token operations'),
-    ('demo_token_transfers', 'TzBTC FA1.2 token transfers'),
-    ('demo_auction', 'TzColors NFT marketplace'),
-    ('demo_raw', 'Process raw operations without filtering and strict typing (experimental)'),
-    ('blank', 'Empty config for a fresh start'),
-    # TODO: demo_jobs
-    # TODO: demo_backup
-    # TODO: demo_sql
-)
-
-
-class Question(BaseModel):
-    type: type = str
-    name: str
-    description: str
-    default: Any
+    def __post_init_post_parse__(self) -> None:
+        self._subgroup_index: int | None = None
 
     @property
-    def text(self) -> str:
-        return f'{self.name} [{self.default}]'
-
-    def prompt(self) -> Any:
-        try:
-            value = cl.prompt(
-                text=self.text,
-                default=self.default,
-                type=self.type,
-                show_default=False,
+    def subgroup_index(self) -> int:
+        if self._subgroup_index is None:
+            raise ConfigInitializationException
+        return self._subgroup_index
+
+    @subgroup_index.setter
+    def subgroup_index(self, value: int) -> None:
+        self._subgroup_index = value
+
+
+class PatternConfig(CodegenMixin):
+    """Base class for pattern config items.
+
+    Contains methods for import and method signature generation during handler callbacks codegen.
+    """
+
+    @classmethod
+    def format_storage_import(
+        cls,
+        package: str,
+        module_name: str,
+    ) -> tuple[str, str]:
+        storage_cls = f'{snake_to_pascal(module_name)}Storage'
+        return f'{package}.types.{module_name}.tezos_storage', storage_cls
+
+    @classmethod
+    def format_parameter_import(
+        cls,
+        package: str,
+        module_name: str,
+        entrypoint: str,
+        alias: str | None,
+    ) -> tuple[str, str]:
+        entrypoint = entrypoint.lstrip('_')
+        parameter_module = pascal_to_snake(entrypoint)
+        parameter_cls = f'{snake_to_pascal(entrypoint)}Parameter'
+        if alias:
+            parameter_cls += f' as {snake_to_pascal(alias)}Parameter'
+
+        return f'{package}.types.{module_name}.tezos_parameters.{parameter_module}', parameter_cls
+
+    @classmethod
+    def format_untyped_operation_import(cls) -> tuple[str, str]:
+        return 'dipdup.models.tezos_tzkt', 'TzktOperationData'
+
+    @classmethod
+    def format_origination_argument(
+        cls,
+        module_name: str,
+        optional: bool,
+        alias: str | None,
+    ) -> tuple[str, str]:
+        arg_name = pascal_to_snake(alias or f'{module_name}_origination')
+        storage_cls = f'{snake_to_pascal(module_name)}Storage'
+        if optional:
+            return arg_name, f'TzktOrigination[{storage_cls}] | None'
+        return arg_name, f'TzktOrigination[{storage_cls}]'
+
+    @classmethod
+    def format_operation_argument(
+        cls,
+        module_name: str,
+        entrypoint: str,
+        optional: bool,
+        alias: str | None,
+    ) -> tuple[str, str]:
+        arg_name = alias or entrypoint
+        entrypoint = entrypoint.lstrip('_')
+        parameter_cls = f'{snake_to_pascal(arg_name)}Parameter'
+        storage_cls = f'{snake_to_pascal(module_name)}Storage'
+        if optional:
+            return pascal_to_snake(arg_name), f'TzktTransaction[{parameter_cls}, {storage_cls}] | None'
+        return pascal_to_snake(arg_name), f'TzktTransaction[{parameter_cls}, {storage_cls}]'
+
+    @classmethod
+    def format_untyped_operation_argument(
+        cls,
+        type_: str,
+        subgroup_index: int,
+        optional: bool,
+        alias: str | None,
+    ) -> tuple[str, str]:
+        arg_name = pascal_to_snake(alias or f'{type_}_{subgroup_index}')
+        if optional:
+            return arg_name, 'TzktOperationData | None'
+        return arg_name, 'TzktOperationData'
+
+
+@dataclass
+class OperationsHandlerTransactionPatternConfig(PatternConfig, SubgroupIndexMixin):
+    """Operation handler pattern config
+
+    :param type: always 'transaction'
+    :param source: Match operations by source contract alias
+    :param destination: Match operations by destination contract alias
+    :param entrypoint: Match operations by contract entrypoint
+    :param optional: Whether can operation be missing in operation group
+    :param alias: Alias for transaction (helps to avoid duplicates)
+    """
+
+    type: Literal['transaction'] = 'transaction'
+    source: TezosContractConfig | None = None
+    destination: TezosContractConfig | None = None
+    entrypoint: str | None = None
+    optional: bool = False
+    alias: str | None = None
+
+    def __post_init_post_parse__(self) -> None:
+        SubgroupIndexMixin.__post_init_post_parse__(self)
+
+    def iter_imports(self, package: str) -> Iterator[tuple[str, str]]:
+        if self.typed_contract:
+            module_name = self.typed_contract.module_name
+            yield 'dipdup.models.tezos_tzkt', 'TzktTransaction'
+            yield self.format_parameter_import(
+                package,
+                module_name,
+                cast(str, self.entrypoint),
+                self.alias,
+            )
+            yield self.format_storage_import(package, module_name)
+        else:
+            yield self.format_untyped_operation_import()
+
+    def iter_arguments(self) -> Iterator[tuple[str, str]]:
+        if self.typed_contract:
+            module_name = self.typed_contract.module_name
+            yield self.format_operation_argument(
+                module_name,
+                cast(str, self.entrypoint),
+                self.optional,
+                self.alias,
+            )
+        else:
+            yield self.format_untyped_operation_argument(
+                'transaction',
+                self.subgroup_index,
+                self.optional,
+                self.alias,
             )
-            print('\n')
-            return value
-        except cl.Abort:
-            cl.echo('\nAborted')
-            quit(0)
-
-    class Config:
-        frozen = True
-
-
-class NotifyQuestion(Question):
-    type = NoneType
-
-    def prompt(self) -> Any:
-        cl.secho('\n' + self.description + '\n', fg='yellow')
-        return self.default
-
-
-class InputQuestion(Question):
-    type = str
-    default: str
-
-    def prompt(self) -> str:
-        cl.secho(f'=> {self.description}', fg='blue')
-        return str(super().prompt())
-
-
-class BooleanQuestion(Question):
-    type = bool
-    default: bool
-
-    @property
-    def text(self) -> str:
-        return f'{self.name} [{self.default and "Y/n" or "y/N"}]'
-
-    def prompt(self) -> bool:
-        cl.secho(f'=> {self.description}', fg='blue')
-        return bool(super().prompt())
-
-
-class ChoiceQuestion(Question):
-    type = int
-    default: int
-    choices: tuple[str, ...]
-    comments: tuple[str, ...]
 
     @property
-    def default_choice(self) -> str:
-        return self.choices[self.default]
+    def typed_contract(self) -> TezosContractConfig | None:
+        if self.entrypoint and self.destination:
+            return self.destination
+        return None
+
+
+@dataclass
+class OperationsHandlerOriginationPatternConfig(PatternConfig, SubgroupIndexMixin):
+    """Origination handler pattern config
+
+    :param type: always 'origination'
+    :param source: Match operations by source contract alias
+    :param originated_contract: Match origination of exact contract
+    :param optional: Whether can operation be missing in operation group
+    :param strict: Match operations by storage only or by the whole code
+    :param alias: Alias for transaction (helps to avoid duplicates)
+    """
+
+    type: Literal['origination'] = 'origination'
+    source: TezosContractConfig | None = None
+    originated_contract: TezosContractConfig | None = None
+    optional: bool = False
+    strict: bool = False
+    alias: str | None = None
+
+    def iter_imports(self, package: str) -> Iterator[tuple[str, str]]:
+        if self.typed_contract:
+            module_name = self.typed_contract.module_name
+            yield 'dipdup.models.tezos_tzkt', 'TzktOrigination'
+            yield self.format_storage_import(package, module_name)
+        else:
+            yield 'dipdup.models.tezos_tzkt', 'TzktOperationData'
+
+    def iter_arguments(self) -> Iterator[tuple[str, str]]:
+        if self.typed_contract:
+            yield self.format_origination_argument(
+                self.typed_contract.module_name,
+                self.optional,
+                self.alias,
+            )
+        else:
+            yield self.format_untyped_operation_argument(
+                'origination',
+                self.subgroup_index,
+                self.optional,
+                self.alias,
+            )
 
     @property
-    def text(self) -> str:
-        return f'{self.name} [{self.default_choice}]'
-
-    def prompt(self) -> str:
-        rows = [f'{i})' for i in range(len(self.choices))]
-        table = tabulate(
-            zip(rows, self.choices, self.comments),
-            colalign=('right', 'left', 'left'),
-        )
-        cl.secho(f'=> {self.description}', fg='blue')
-        cl.echo(table)
-        return str(self.choices[super().prompt()])
-
-
-class JinjaAnswers(dict[str, Any]):
-    def __init__(self, *args: str, **kwargs: Any) -> None:
-        super().__init__(*args, **kwargs)
-        self['dipdup_version'] = __version__.split('.')[0]
-
-    def __getattr__(self, item: str) -> Any:
-        return self[item]
-
-
-class Project(BaseModel):
-    path: Path
-    description: str
-    questions: tuple[Question, ...]
-    answers: JinjaAnswers = Field(default_factory=JinjaAnswers)
-
-    def verify(self) -> None:
-        for question in self.questions:
-            if not self.answers.get(question.name):
-                raise ConfigurationError(f'Question {question.name} is not answered')
-
-    def reset(self) -> None:
-        self.answers = JinjaAnswers()
-
-    def run(self, quiet: bool, replay: str | None) -> None:
-        if not self.questions:
-            raise ConfigurationError('No questions defined')
-
-        if replay:
-            with open(replay, 'rb') as f:
-                self.answers = JinjaAnswers(json.loads(f.read()))
-
-        for question in self.questions:
-            if question.name in self.answers:
-                _logger.info('Skipping question `%s`', question.name)
-                continue
-
-            if quiet:
-                value = question.choices[question.default] if isinstance(question, ChoiceQuestion) else question.default
-                cl.echo(f'{question.name}: using default value `{value}`')
+    def typed_contract(self) -> TezosContractConfig | None:
+        if self.originated_contract:
+            return self.originated_contract
+        return None
+
+
+@dataclass
+class TzktOperationsIndexConfig(TzktIndexConfig):
+    """Operation index config
+
+    :param kind: always `tezos.tzkt.operations`
+    :param datasource: Alias of index datasource in `datasources` section
+    :param handlers: List of indexer handlers
+    :param types: Types of transaction to fetch
+    :param contracts: Aliases of contracts being indexed in `contracts` section
+    :param first_level: Level to start indexing from
+    :param last_level: Level to stop indexing at
+    """
+
+    kind: Literal['tezos.tzkt.operations']
+    datasource: TzktDatasourceConfig
+    handlers: tuple[TzktOperationsHandlerConfig, ...]
+    contracts: list[TezosContractConfig] = field(default_factory=list)
+    types: tuple[TzktOperationType, ...] = (TzktOperationType.transaction,)
+
+    first_level: int = 0
+    last_level: int = 0
+
+    def get_subscriptions(self) -> set[Subscription]:
+        subs = super().get_subscriptions()
+        if TzktOperationType.transaction in self.types:
+            if self.datasource.merge_subscriptions:
+                subs.add(TransactionSubscription())
             else:
-                value = question.prompt()
-
-            self.answers[question.name] = value
+                for contract_config in self.contracts:
+                    if not isinstance(contract_config, ContractConfig):
+                        raise ConfigInitializationException
+                    subs.add(TransactionSubscription(address=contract_config.address))
+        if TzktOperationType.origination in self.types:
+            subs.add(OriginationSubscription())
+        return subs
+
+    @classmethod
+    def strip(cls, config_dict: dict[str, Any]) -> None:
+        super().strip(config_dict)
+        for handler in config_dict['handlers']:
+            for item in handler['pattern']:
+                item.pop('alias', None)
+
+
+# FIXME: Reversed for new Pydantic. Why?
+OperationsHandlerPatternConfigU = OperationsHandlerTransactionPatternConfig | OperationsHandlerOriginationPatternConfig
+
+
+@dataclass
+class TzktOperationsHandlerConfig(HandlerConfig):
+    """Operation handler config
+
+    :param callback: Callback name
+    :param pattern: Filters to match operation groups
+    """
+
+    pattern: tuple[OperationsHandlerPatternConfigU, ...]
+
+    def iter_imports(self, package: str) -> Iterator[tuple[str, str]]:
+        yield 'dipdup.context', 'HandlerContext'
+        for pattern in self.pattern:
+            yield from pattern.iter_imports(package)
+
+    def iter_arguments(self) -> Iterator[tuple[str, str]]:
+        yield 'ctx', 'HandlerContext'
+
+        arg_names: set[str] = set()
+        for pattern in self.pattern:
+            arg, arg_type = next(pattern.iter_arguments())
+            if arg in arg_names:
+                raise ConfigurationError(
+                    (
+                        'Pattern item is not unique. Set `alias` field to avoid duplicates.\n\n              handler:'
+                        f' `{self.callback}`\n              entrypoint: `{arg}`'
+                    ),
+                )
+            arg_names.add(arg)
+            yield arg, arg_type
+
+
+@dataclass
+class OperationUnfilteredHandlerConfig(HandlerConfig):
+    """Handler of unfiltered operation index
+
+    :param callback: Callback name
+    """
+
+    def iter_imports(self, package: str) -> Iterator[tuple[str, str]]:
+        yield 'dipdup.context', 'HandlerContext'
+        yield 'dipdup.models.tezos_tzkt', 'TzktOperationData'
+        yield package, 'models as models'
+
+    def iter_arguments(self) -> Iterator[tuple[str, str]]:
+        yield 'ctx', 'HandlerContext'
+        yield 'operation', 'TzktOperationData'
+
+
+@dataclass
+class TzktOperationsUnfilteredIndexConfig(TzktIndexConfig):
+    """Operation index config
+
+    :param kind: always `tezos.tzkt.operations_unfiltered`
+    :param datasource: Alias of index datasource in `datasources` section
+    :param callback: Callback name
+    :param types: Types of transaction to fetch
+
+    :param first_level: Level to start indexing from
+    :param last_level: Level to stop indexing at
+    """
+
+    kind: Literal['tezos.tzkt.operations_unfiltered']
+    datasource: TzktDatasourceConfig
+    callback: str
+    types: tuple[TzktOperationType, ...] = (TzktOperationType.transaction,)
+
+    first_level: int = 0
+    last_level: int = 0
+
+    def __post_init_post_parse__(self) -> None:
+        super().__post_init_post_parse__()
+        self.handler_config = OperationUnfilteredHandlerConfig(callback=self.callback)
+
+    def get_subscriptions(self) -> set[Subscription]:
+        subs = super().get_subscriptions()
+        subs.add(TransactionSubscription())
+        return subs
 
-    def write_cookiecutter_json(self, path: Path) -> None:
-        values = {k: v for k, v in self.answers.items() if not k.startswith('_')}
-        path.write_bytes(
-            json.dumps(
-                values,
-                option=json.OPT_INDENT_2,
-            )
-        )
 
-    def _render(self, template_path: Path, output_path: Path, force: bool) -> None:
-        if output_path.exists() and not force:
-            _logger.warning('File `%s` already exists, skipping', output_path)
-
-        _logger.info('Generating `%s`', output_path)
-        template = load_template(template_path)
-        content = template.render(cookiecutter=self.answers)
-        write(output_path, content, overwrite=force)
-
-    def render(self, force: bool = False) -> None:
-        from jinja2 import Template
-
-        project_path = Path(__file__).parent / 'projects' / self.path
-        project_paths = project_path.glob('**/*.j2')
-
-        for path in project_paths:
-            template_path = path.relative_to(Path(__file__).parent)
-            output_path = Path(
-                self.answers['project_name'],
-                *path.relative_to(project_path).parts,
-                # NOTE: Remove ".j2" from extension
-            ).with_suffix(path.suffix[:-3])
-            output_path = Path(Template(str(output_path)).render(cookiecutter=self.answers))
-            self._render(template_path, output_path, force)
-
-    def get_defaults(self) -> dict[str, Any]:
-        return {
-            question.name: question.choices[question.default]
-            if isinstance(question, ChoiceQuestion)
-            else question.default
-            for question in self.questions
-        }
-
-
-class BaseProject(Project):
-    # FIXME: Replace defaults with fields
-    path = Path('base')
-    description = 'Default DipDup project, ex. cookiecutter template'
-    questions: tuple[Question, ...] = (
-        NotifyQuestion(
-            name='_welcome',
-            default=None,
-            description=(
-                'Welcome to DipDup! This command will help you to create a new project.\n'
-                'You can abort at any time by pressing Ctrl+C. Press Enter to use default value.\n'
-                "Let's start with some basic questions."
-            ),
-        ),
-        ChoiceQuestion(
-            name='template',
-            description=('Choose config template depending on the type of your project (DEX, NFT marketplace etc.)\n'),
-            default=7,
-            choices=tuple(p[0] for p in DEMO_PROJECTS),
-            comments=tuple(p[1] for p in DEMO_PROJECTS),
-        ),
-        InputQuestion(
-            name='project_name',
-            description='Enter project name',
-            default='dipdup-indexer',
-        ),
-        InputQuestion(
-            name='package',
-            description='Enter Python package name',
-            default='dipdup_indexer',
-        ),
-        InputQuestion(
-            name='version',
-            description='Enter project version',
-            default='0.0.1',
-        ),
-        InputQuestion(
-            name='description',
-            description='Enter project description',
-            default='My shiny new indexer based on DipDup',
-        ),
-        InputQuestion(
-            name='license',
-            description=('Enter project license\n' 'DipDup itself is MIT-licensed.'),
-            default='MIT',
-        ),
-        InputQuestion(
-            name='author',
-            description=('Enter project author\n' 'You can add more later in pyproject.toml.'),
-            default='John Smith <john_smith@localhost.lan>',
-        ),
-        NotifyQuestion(
-            name='_versions',
-            default=None,
-            description='Now choose versions of software you want to use.',
-        ),
-        ChoiceQuestion(
-            name='postgresql_image',
-            description=('Choose PostgreSQL version\n' 'Try TimescaleDB when working with time series.'),
-            default=0,
-            choices=(
-                'postgres:14',
-                'timescale/timescaledb:latest-pg14',
-                'timescale/timescaledb-ha:pg14-latest',
-            ),
-            comments=(
-                'PostgreSQL',
-                'TimescaleDB',
-                'TimescaleDB HA (more extensions)',
-            ),
-        ),
-        ChoiceQuestion(
-            name='hasura_image',
-            description=(
-                'Choose Hasura version\n'
-                'Test new releases before using in production; new versions may break compatibility.'
-            ),
-            default=0,
-            choices=(
-                'hasura/graphql-engine:v2.29.0',
-                'hasura/graphql-engine:v2.29.0',
-            ),
-            comments=(
-                'stable',
-                'beta',
-            ),
-        ),
-        NotifyQuestion(
-            name='_other',
-            default=None,
-            description='Miscellaneous tunables; leave default values if unsure',
-        ),
-        BooleanQuestion(
-            name='crash_reporting',
-            description='Enable crash reporting?\n' 'It helps us a lot to improve DipDup 🙏',
-            default=False,
-        ),
-        ChoiceQuestion(
-            name='linters',
-            description=(
-                'Choose tools to lint and test your code\n' 'You can always add more later in pyproject.toml.'
-            ),
-            default=0,
-            choices=(
-                'default',
-                'none',
-            ),
-            comments=(
-                'Classic set: black, isort, ruff, mypy, pytest',
-                'None',
-            ),
-        ),
-        InputQuestion(
-            name='line_length',
-            description=('Enter maximum line length\n' 'Used by linters.'),
-            default='120',
-        ),
-    )
-
-    def render(self, force: bool = False) -> None:
-        super().render(force)
-
-        # NOTE: Config and handlers
-        Project(
-            path=self.answers['template'],
-            description='',
-            questions=(),
-            answers=self.answers,
-        ).render(force)
-
-        # NOTE: Linters and stuff
-        Project(
-            path='linters_' + self.answers['linters'],
-            description='',
-            questions=(),
-            answers=self.answers,
-        ).render(force)
+TzktOperationsHandlerConfigU = TzktOperationsHandlerConfig | OperationUnfilteredHandlerConfig
+TzktOperationsIndexConfigU = TzktOperationsIndexConfig | TzktOperationsUnfilteredIndexConfig
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/base/docker-compose.swarm.yml.j2` & `dipdup-7.0.0rc1/src/demo_auction/deploy/compose.swarm.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-version: "3.8"
+name: demo_auction
 
 services:
   dipdup:
-    image: ${DOCKER_REGISTRY:-ghcr.io}/dipdup-io/dipdup:${TAG:-master}
+    image: ${IMAGE:-ghcr.io/dipdup-io/dipdup}:${TAG:-7}
     depends_on:
       - db
       - hasura
-    command: ["-c", "dipdup.yml", "-c", "dipdup.prod.yml", "run"]
-    environment:
-      - "POSTGRES_USER=dipdup"
-      - "POSTGRES_PASSWORD=changeme"
-      - "POSTGRES_DB=dipdup"
-      - "HASURA_SECRET=changeme"
+    command: ["-c", "dipdup.yaml", "-c", "configs/dipdup.swarm.yaml", "run"]
+    env_file: .env
     networks:
       - dipdup-private
       - prometheus-private
     deploy:
       mode: replicated
       replicas: ${INDEXER_ENABLED:-1}
       labels:
@@ -28,46 +24,46 @@
       driver: "json-file"
       options:
         max-size: "10m"
         max-file: "10"
         tag: "\{\{.Name\}\}.\{\{.ImageID\}\}"
 
   db:
-    image: {{ cookiecutter.postgresql_image }}
+    image: postgres:15
     volumes:
       - db:/var/lib/postgresql/data
+    env_file: .env
     environment: 
       - POSTGRES_USER=dipdup
       - POSTGRES_DB=dipdup
-      - POSTGRES_PASSWORD=${POSTGRES_PASSWORD:-changeme}
+      - POSTGRES_PASSWORD=${POSTGRES_PASSWORD}
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U postgres"]
       interval: 10s
       timeout: 5s
       retries: 5
     networks:
       - dipdup-private
     deploy:
       mode: replicated
       replicas: 1
       placement: *placement
     logging: *logging
 
   hasura:
-    image: {{ cookiecutter.hasura_image }}
+    image: hasura/graphql-engine:v2.30.0
     depends_on:
       - db
     environment:
-      - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD:-changeme}@db:5432
+      - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@demo_auction_db:5432/dipdup
+      - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=false
-      - HASURA_GRAPHQL_ENABLED_LOG_TYPES=startup, http-log, websocket-log, query-log
       - HASURA_GRAPHQL_LOG_LEVEL=warn
       - HASURA_GRAPHQL_ENABLE_TELEMETRY=false
-      - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_UNAUTHORIZED_ROLE=user
       - HASURA_GRAPHQL_STRINGIFY_NUMERIC_TYPES=true
     networks:
       - dipdup-private
       - traefik-public
     deploy:
       mode: replicated
@@ -80,15 +76,14 @@
         - "traefik.http.routers.${SERVICE}-console.rule=Host(`${SERVICE}.${SWARM_ROOT_DOMAIN}`)"
         - traefik.http.routers.${SERVICE}-console.entrypoints=https
         - traefik.http.middlewares.${SERVICE}-console.headers.customrequestheaders.X-Hasura-Admin-Secret=${HASURA_SECRET}
         - traefik.http.routers.${SERVICE}-console.middlewares=authelia@docker,${SERVICE}-console
       placement: *placement
     logging: *logging
 
-
 volumes:
   db:
 
 networks:
   dipdup-private:
   traefik-public:
     external: true
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/base/docker-compose.yml.j2` & `dipdup-7.0.0rc1/src/demo_nft_marketplace/deploy/compose.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,54 @@
-version: "3.8"
+name: demo_nft_marketplace
 
 services:
   dipdup:
-    build: .
-    depends_on:
-      - db
-    command: ["-c", "dipdup.yml", "-c", "dipdup.prod.yml", "run"]
+    build:
+      context: ..
+      dockerfile: deploy/Dockerfile
     restart: always
-    environment:
-      - POSTGRES_PASSWORD=${POSTGRES_PASSWORD:-changeme}
-      - ADMIN_SECRET=${ADMIN_SECRET:-changeme}
+    env_file: .env
     ports:
-      - 127.0.0.1:9000:9000
+      - 46339
+      - 9000
+    command: ["-c", "dipdup.yaml", "-c", "configs/dipdup.compose.yaml", "run"]
+    depends_on:
+      - db
+      - hasura
 
   db:
-    image: {{ cookiecutter.postgresql_image }}
+    image: postgres:15
     ports:
-      - 127.0.0.1:5432:5432
+      - 5432
     volumes:
       - db:/var/lib/postgresql/data
     restart: always
+    env_file: .env
     environment:
       - POSTGRES_USER=dipdup
       - POSTGRES_DB=dipdup
-      - POSTGRES_PASSWORD=${POSTGRES_PASSWORD:-changeme}
+      - POSTGRES_PASSWORD=${POSTGRES_PASSWORD}
     healthcheck:
       test: ["CMD-SHELL", "pg_isready -U dipdup"]
       interval: 10s
       timeout: 5s
       retries: 5
 
   hasura:
-    image: {{ cookiecutter.hasura_image }}
+    image: hasura/graphql-engine:v2.30.0
     ports:
-      - 127.0.0.1:8080:8080
+      - 8080
     depends_on:
       - db
     restart: always
     environment:
-      - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD:-changeme}@db:5432
+      - HASURA_GRAPHQL_DATABASE_URL=postgres://dipdup:${POSTGRES_PASSWORD}@db:5432/dipdup
+      - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET}
       - HASURA_GRAPHQL_ENABLE_CONSOLE=true
       - HASURA_GRAPHQL_DEV_MODE=true
-      - HASURA_GRAPHQL_ENABLED_LOG_TYPES=startup, http-log, webhook-log, websocket-log, query-log
-      - HASURA_GRAPHQL_ADMIN_SECRET=${HASURA_SECRET:-changeme}
+      - HASURA_GRAPHQL_LOG_LEVEL=info
+      - HASURA_GRAPHQL_ENABLE_TELEMETRY=false
       - HASURA_GRAPHQL_UNAUTHORIZED_ROLE=user
       - HASURA_GRAPHQL_STRINGIFY_NUMERIC_TYPES=true
 
 volumes:
-  db:
+  db:
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_auction/dipdup.yml.j2` & `dipdup-7.0.0rc1/src/demo_auction/dipdup.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,71 @@
-00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 312e  spec_version: 1.
-00000010: 320a 7061 636b 6167 653a 207b 7b20 636f  2.package: {{ co
-00000020: 6f6b 6965 6375 7474 6572 2e70 6163 6b61  okiecutter.packa
-00000030: 6765 207d 7d0a 0a64 6174 6162 6173 653a  ge }}..database:
-00000040: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000050: 2020 7061 7468 3a20 7b7b 2063 6f6f 6b69    path: {{ cooki
-00000060: 6563 7574 7465 722e 7072 6f6a 6563 745f  ecutter.project_
-00000070: 6e61 6d65 207d 7d2e 7371 6c69 7465 330a  name }}.sqlite3.
-00000080: 0a63 6f6e 7472 6163 7473 3a0a 2020 747a  .contracts:.  tz
-00000090: 636f 6c6f 7273 5f6d 696e 7465 723a 0a20  colors_minter:. 
-000000a0: 2020 2061 6464 7265 7373 3a20 4b54 3146     address: KT1F
-000000b0: 7961 4471 694d 5157 6737 4578 6f37 5655  yaDqiMQWg7Exo7VU
-000000c0: 6958 4167 5a62 6432 6b43 7a6f 3364 3473  iXAgZbd2kCzo3d4s
-000000d0: 0a20 2020 2074 7970 656e 616d 653a 2074  .    typename: t
-000000e0: 7a63 6f6c 6f72 735f 6d69 6e74 6572 0a20  zcolors_minter. 
-000000f0: 2074 7a63 6f6c 6f72 735f 6175 6374 696f   tzcolors_auctio
-00000100: 6e3a 0a20 2020 2061 6464 7265 7373 3a20  n:.    address: 
-00000110: 4b54 3143 7065 5351 4b64 6b68 5769 3470  KT1CpeSQKdkhWi4p
-00000120: 696e 5963 7365 4346 4b6d 4468 7335 4d37  inYcseCFKmDhs5M7
-00000130: 3442 6b55 0a20 2020 2074 7970 656e 616d  4BkU.    typenam
-00000140: 653a 2074 7a63 6f6c 6f72 735f 6175 6374  e: tzcolors_auct
-00000150: 696f 6e0a 0a64 6174 6173 6f75 7263 6573  ion..datasources
-00000160: 3a0a 2020 747a 6b74 3a0a 2020 2020 6b69  :.  tzkt:.    ki
-00000170: 6e64 3a20 747a 6b74 0a20 2020 2075 726c  nd: tzkt.    url
-00000180: 3a20 247b 545a 4b54 5f55 524c 3a2d 6874  : ${TZKT_URL:-ht
-00000190: 7470 733a 2f2f 6170 692e 747a 6b74 2e69  tps://api.tzkt.i
-000001a0: 6f7d 0a0a 7465 6d70 6c61 7465 733a 0a20  o}..templates:. 
-000001b0: 2061 7563 7469 6f6e 3a0a 2020 2020 6b69   auction:.    ki
-000001c0: 6e64 3a20 6f70 6572 6174 696f 6e0a 2020  nd: operation.  
-000001d0: 2020 6461 7461 736f 7572 6365 3a20 3c64    datasource: <d
-000001e0: 6174 6173 6f75 7263 653e 0a20 2020 2063  atasource>.    c
-000001f0: 6f6e 7472 6163 7473 3a0a 2020 2020 2020  ontracts:.      
-00000200: 2d20 3c61 7563 7469 6f6e 3e0a 2020 2020  - <auction>.    
-00000210: 6861 6e64 6c65 7273 3a0a 2020 2020 2020  handlers:.      
-00000220: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f63  - callback: on_c
-00000230: 7265 6174 655f 6175 6374 696f 6e0a 2020  reate_auction.  
-00000240: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
-00000250: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-00000260: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000270: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00000280: 7469 6f6e 3a20 3c61 7563 7469 6f6e 3e0a  tion: <auction>.
-00000290: 2020 2020 2020 2020 2020 2020 656e 7472              entr
-000002a0: 7970 6f69 6e74 3a20 6372 6561 7465 5f61  ypoint: create_a
-000002b0: 7563 7469 6f6e 0a20 2020 2020 202d 2063  uction.      - c
-000002c0: 616c 6c62 6163 6b3a 206f 6e5f 6269 640a  allback: on_bid.
-000002d0: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-000002e0: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-000002f0: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000300: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00000310: 6e61 7469 6f6e 3a20 3c61 7563 7469 6f6e  nation: <auction
-00000320: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
-00000330: 7472 7970 6f69 6e74 3a20 6269 640a 2020  trypoint: bid.  
-00000340: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
-00000350: 6f6e 5f77 6974 6864 7261 770a 2020 2020  on_withdraw.    
-00000360: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
-00000370: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
-00000380: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
-00000390: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-000003a0: 6f6e 3a20 3c61 7563 7469 6f6e 3e0a 2020  on: <auction>.  
-000003b0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
-000003c0: 6f69 6e74 3a20 7769 7468 6472 6177 0a0a  oint: withdraw..
-000003d0: 696e 6465 7865 733a 0a20 2074 7a63 6f6c  indexes:.  tzcol
-000003e0: 6f72 733a 0a20 2020 2074 656d 706c 6174  ors:.    templat
-000003f0: 653a 2061 7563 7469 6f6e 0a20 2020 2076  e: auction.    v
-00000400: 616c 7565 733a 0a20 2020 2020 2064 6174  alues:.      dat
-00000410: 6173 6f75 7263 653a 2074 7a6b 740a 2020  asource: tzkt.  
-00000420: 2020 2020 6d69 6e74 6572 3a20 747a 636f      minter: tzco
-00000430: 6c6f 7273 5f6d 696e 7465 720a 2020 2020  lors_minter.    
-00000440: 2020 6175 6374 696f 6e3a 2074 7a63 6f6c    auction: tzcol
-00000450: 6f72 735f 6175 6374 696f 6e0a            ors_auction.
+00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
+00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
+00000020: 6175 6374 696f 6e0a 0a64 6174 6162 6173  auction..databas
+00000030: 653a 0a20 206b 696e 643a 2073 716c 6974  e:.  kind: sqlit
+00000040: 650a 2020 7061 7468 3a20 6465 6d6f 5f61  e.  path: demo_a
+00000050: 7563 7469 6f6e 2e73 716c 6974 6533 0a0a  uction.sqlite3..
+00000060: 636f 6e74 7261 6374 733a 0a20 2074 7a63  contracts:.  tzc
+00000070: 6f6c 6f72 735f 6d69 6e74 6572 3a0a 2020  olors_minter:.  
+00000080: 2020 6b69 6e64 3a20 7465 7a6f 730a 2020    kind: tezos.  
+00000090: 2020 6164 6472 6573 733a 204b 5431 4679    address: KT1Fy
+000000a0: 6144 7169 4d51 5767 3745 786f 3756 5569  aDqiMQWg7Exo7VUi
+000000b0: 5841 675a 6264 326b 437a 6f33 6434 730a  XAgZbd2kCzo3d4s.
+000000c0: 2020 2020 7479 7065 6e61 6d65 3a20 747a      typename: tz
+000000d0: 636f 6c6f 7273 5f6d 696e 7465 720a 2020  colors_minter.  
+000000e0: 747a 636f 6c6f 7273 5f61 7563 7469 6f6e  tzcolors_auction
+000000f0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+00000100: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
+00000110: 5431 4370 6553 514b 646b 6857 6934 7069  T1CpeSQKdkhWi4pi
+00000120: 6e59 6373 6543 464b 6d44 6873 354d 3734  nYcseCFKmDhs5M74
+00000130: 426b 550a 2020 2020 7479 7065 6e61 6d65  BkU.    typename
+00000140: 3a20 747a 636f 6c6f 7273 5f61 7563 7469  : tzcolors_aucti
+00000150: 6f6e 0a0a 6461 7461 736f 7572 6365 733a  on..datasources:
+00000160: 0a20 2074 7a6b 743a 0a20 2020 206b 696e  .  tzkt:.    kin
+00000170: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
+00000180: 2020 7572 6c3a 2024 7b54 5a4b 545f 5552    url: ${TZKT_UR
+00000190: 4c3a 2d68 7474 7073 3a2f 2f61 7069 2e74  L:-https://api.t
+000001a0: 7a6b 742e 696f 7d0a 0a74 656d 706c 6174  zkt.io}..templat
+000001b0: 6573 3a0a 2020 6175 6374 696f 6e3a 0a20  es:.  auction:. 
+000001c0: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
+000001d0: 7a6b 742e 6f70 6572 6174 696f 6e73 0a20  zkt.operations. 
+000001e0: 2020 2064 6174 6173 6f75 7263 653a 203c     datasource: <
+000001f0: 6461 7461 736f 7572 6365 3e0a 2020 2020  datasource>.    
+00000200: 636f 6e74 7261 6374 733a 0a20 2020 2020  contracts:.     
+00000210: 202d 203c 6175 6374 696f 6e3e 0a20 2020   - <auction>.   
+00000220: 2068 616e 646c 6572 733a 0a20 2020 2020   handlers:.     
+00000230: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+00000240: 6372 6561 7465 5f61 7563 7469 6f6e 0a20  create_auction. 
+00000250: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
+00000260: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+00000270: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
+00000280: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+00000290: 6174 696f 6e3a 203c 6175 6374 696f 6e3e  ation: <auction>
+000002a0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+000002b0: 7279 706f 696e 743a 2063 7265 6174 655f  rypoint: create_
+000002c0: 6175 6374 696f 6e0a 2020 2020 2020 2d20  auction.      - 
+000002d0: 6361 6c6c 6261 636b 3a20 6f6e 5f62 6964  callback: on_bid
+000002e0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+000002f0: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
+00000300: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+00000310: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000320: 696e 6174 696f 6e3a 203c 6175 6374 696f  ination: <auctio
+00000330: 6e3e 0a20 2020 2020 2020 2020 2020 2065  n>.            e
+00000340: 6e74 7279 706f 696e 743a 2062 6964 0a20  ntrypoint: bid. 
+00000350: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
+00000360: 206f 6e5f 7769 7468 6472 6177 0a20 2020   on_withdraw.   
+00000370: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
+00000380: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
+00000390: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
+000003a0: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+000003b0: 696f 6e3a 203c 6175 6374 696f 6e3e 0a20  ion: <auction>. 
+000003c0: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
+000003d0: 706f 696e 743a 2077 6974 6864 7261 770a  point: withdraw.
+000003e0: 0a69 6e64 6578 6573 3a0a 2020 747a 636f  .indexes:.  tzco
+000003f0: 6c6f 7273 3a0a 2020 2020 7465 6d70 6c61  lors:.    templa
+00000400: 7465 3a20 6175 6374 696f 6e0a 2020 2020  te: auction.    
+00000410: 7661 6c75 6573 3a0a 2020 2020 2020 6461  values:.      da
+00000420: 7461 736f 7572 6365 3a20 747a 6b74 0a20  tasource: tzkt. 
+00000430: 2020 2020 206d 696e 7465 723a 2074 7a63       minter: tzc
+00000440: 6f6c 6f72 735f 6d69 6e74 6572 0a20 2020  olors_minter.   
+00000450: 2020 2061 7563 7469 6f6e 3a20 747a 636f     auction: tzco
+00000460: 6c6f 7273 5f61 7563 7469 6f6e            lors_auction
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_bid.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_bid.py.j2`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.tzcolors_auction.parameter.bid import BidParameter
-from {{cookiecutter.package}}.types.tzcolors_auction.storage import TzcolorsAuctionStorage
+import {{project.package}}.models as models
+from {{project.package}}.types.tzcolors_auction.tezos_parameters.bid import BidParameter
+from {{project.package}}.types.tzcolors_auction.tezos_storage import TzcolorsAuctionStorage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_bid(
     ctx: HandlerContext,
-    bid: Transaction[BidParameter, TzcolorsAuctionStorage],
+    bid: TzktTransaction[BidParameter, TzcolorsAuctionStorage],
 ) -> None:
     assert bid.data.amount is not None
 
     auction = await models.Auction.filter(
         id=bid.parameter.__root__,
     ).get()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/handlers/on_create_auction.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/handlers/on_create_auction.py.j2`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.tzcolors_auction.parameter.create_auction import CreateAuctionParameter
-from {{cookiecutter.package}}.types.tzcolors_auction.storage import TzcolorsAuctionStorage
+import {{project.package}}.models as models
+from {{project.package}}.types.tzcolors_auction.tezos_parameters.create_auction import CreateAuctionParameter
+from {{project.package}}.types.tzcolors_auction.tezos_storage import TzcolorsAuctionStorage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_create_auction(
     ctx: HandlerContext,
-    create_auction: Transaction[CreateAuctionParameter, TzcolorsAuctionStorage],
+    create_auction: TzktTransaction[CreateAuctionParameter, TzcolorsAuctionStorage],
 ) -> None:
     holder, _ = await models.User.get_or_create(address=create_auction.data.sender_address)
 
     token, _ = await models.Token.get_or_create(
         id=create_auction.parameter.token_id,
         address=create_auction.parameter.token_address,
         defaults={
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_auction/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-7.0.0rc1/src/demo_auction/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 from enum import IntEnum
 
-from tortoise.fields.relational import ForeignKeyFieldInstance
-from tortoise import fields
-
+from dipdup import fields
 from dipdup.models import Model
 
 
 class AuctionStatus(IntEnum):
     ACTIVE = 0
     FINISHED = 1
 
 
 class User(Model):
-    address = fields.CharField(36, pk=True)
+    address = fields.TextField(pk=True)
 
 
 class Token(Model):
     id = fields.BigIntField(pk=True)
-    address = fields.CharField(36)
+    address = fields.TextField()
     amount = fields.BigIntField()
     level = fields.BigIntField()
     timestamp = fields.DatetimeField()
-    holder: ForeignKeyFieldInstance[User] = fields.ForeignKeyField('models.User', 'tokens')
+    holder: fields.ForeignKeyField[User] = fields.ForeignKeyField('models.User', 'tokens')
 
     token_id: int
 
 
 class Auction(Model):
     id = fields.BigIntField(pk=True)
-    token: ForeignKeyFieldInstance[Token] = fields.ForeignKeyField('models.Token', 'auctions')
+    token: fields.ForeignKeyField[Token] = fields.ForeignKeyField('models.Token', 'auctions')
     bid_amount = fields.BigIntField()
-    bidder: ForeignKeyFieldInstance[User] = fields.ForeignKeyField('models.User', 'winning_auctions')
-    seller: ForeignKeyFieldInstance[User] = fields.ForeignKeyField('models.User', 'created_auctions')
+    bidder: fields.ForeignKeyField[User] = fields.ForeignKeyField('models.User', 'winning_auctions')
+    seller: fields.ForeignKeyField[User] = fields.ForeignKeyField('models.User', 'created_auctions')
     end_timestamp = fields.DatetimeField()
     status = fields.IntEnumField(AuctionStatus)
     level = fields.BigIntField()
     timestamp = fields.DatetimeField()
 
     token_id: int
 
 
 class Bid(Model):
     id = fields.BigIntField(pk=True)
-    auction: ForeignKeyFieldInstance[Auction] = fields.ForeignKeyField('models.Auction', 'bids')
+    auction: fields.ForeignKeyField[Auction] = fields.ForeignKeyField('models.Auction', 'bids')
     bid_amount = fields.BigIntField()
-    bidder: ForeignKeyFieldInstance[User] = fields.ForeignKeyField('models.User', 'bids')
+    bidder: fields.ForeignKeyField[User] = fields.ForeignKeyField('models.User', 'bids')
     level = fields.BigIntField()
-    timestamp = fields.DatetimeField()
+    timestamp = fields.DatetimeField()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_big_maps/dipdup.yml.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/dipdup.yaml.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,58 @@
-00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 312e  spec_version: 1.
-00000010: 320a 7061 636b 6167 653a 207b 7b20 636f  2.package: {{ co
-00000020: 6f6b 6965 6375 7474 6572 2e70 6163 6b61  okiecutter.packa
-00000030: 6765 207d 7d0a 0a64 6174 6162 6173 653a  ge }}..database:
-00000040: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000050: 2020 7061 7468 3a20 7b7b 2063 6f6f 6b69    path: {{ cooki
-00000060: 6563 7574 7465 722e 7072 6f6a 6563 745f  ecutter.project_
-00000070: 6e61 6d65 207d 7d2e 7371 6c69 7465 330a  name }}.sqlite3.
-00000080: 0a63 6f6e 7472 6163 7473 3a0a 2020 6d61  .contracts:.  ma
-00000090: 696e 6e65 745f 6e61 6d65 5f72 6567 6973  innet_name_regis
-000000a0: 7472 793a 0a20 2020 2061 6464 7265 7373  try:.    address
-000000b0: 3a20 4b54 3147 425a 6d53 786d 6e4b 4a58  : KT1GBZmSxmnKJX
-000000c0: 474d 644d 4c62 7567 5066 4c79 5550 6d75  GMdMLbugPfLyUPmu
-000000d0: 4c53 4d77 4b53 0a20 2020 2074 7970 656e  LSMwKS.    typen
-000000e0: 616d 653a 206e 616d 655f 7265 6769 7374  ame: name_regist
-000000f0: 7279 0a0a 6461 7461 736f 7572 6365 733a  ry..datasources:
-00000100: 0a20 2074 7a6b 745f 6d61 696e 6e65 743a  .  tzkt_mainnet:
-00000110: 0a20 2020 206b 696e 643a 2074 7a6b 740a  .    kind: tzkt.
-00000120: 2020 2020 7572 6c3a 2024 7b54 5a4b 545f      url: ${TZKT_
-00000130: 5552 4c3a 2d68 7474 7073 3a2f 2f61 7069  URL:-https://api
-00000140: 2e74 7a6b 742e 696f 7d0a 0a74 656d 706c  .tzkt.io}..templ
-00000150: 6174 6573 3a0a 2020 6269 675f 6d61 7073  ates:.  big_maps
-00000160: 3a0a 2020 2020 6b69 6e64 3a20 6269 675f  :.    kind: big_
-00000170: 6d61 700a 2020 2020 6461 7461 736f 7572  map.    datasour
-00000180: 6365 3a20 3c64 6174 6173 6f75 7263 653e  ce: <datasource>
-00000190: 0a20 2020 2073 6b69 705f 6869 7374 6f72  .    skip_histor
-000001a0: 793a 206f 6e63 650a 2020 2020 6861 6e64  y: once.    hand
-000001b0: 6c65 7273 3a0a 2020 2020 2020 2d20 6361  lers:.      - ca
-000001c0: 6c6c 6261 636b 3a20 6f6e 5f75 7064 6174  llback: on_updat
-000001d0: 655f 7265 636f 7264 730a 2020 2020 2020  e_records.      
-000001e0: 2020 636f 6e74 7261 6374 3a20 3c6e 616d    contract: <nam
-000001f0: 655f 7265 6769 7374 7279 3e0a 2020 2020  e_registry>.    
-00000200: 2020 2020 7061 7468 3a20 7374 6f72 652e      path: store.
-00000210: 7265 636f 7264 730a 2020 2020 2020 2d20  records.      - 
-00000220: 6361 6c6c 6261 636b 3a20 6f6e 5f75 7064  callback: on_upd
-00000230: 6174 655f 6578 7069 7279 5f6d 6170 0a20  ate_expiry_map. 
-00000240: 2020 2020 2020 2063 6f6e 7472 6163 743a         contract:
-00000250: 203c 6e61 6d65 5f72 6567 6973 7472 793e   <name_registry>
-00000260: 0a20 2020 2020 2020 2070 6174 683a 2073  .        path: s
-00000270: 746f 7265 2e65 7870 6972 795f 6d61 700a  tore.expiry_map.
-00000280: 0a69 6e64 6578 6573 3a0a 2020 6269 675f  .indexes:.  big_
-00000290: 6d61 7073 5f6d 6169 6e6e 6574 3a0a 2020  maps_mainnet:.  
-000002a0: 2020 7465 6d70 6c61 7465 3a20 6269 675f    template: big_
-000002b0: 6d61 7073 0a20 2020 2076 616c 7565 733a  maps.    values:
-000002c0: 0a20 2020 2020 2064 6174 6173 6f75 7263  .      datasourc
-000002d0: 653a 2074 7a6b 745f 6d61 696e 6e65 740a  e: tzkt_mainnet.
-000002e0: 2020 2020 2020 6e61 6d65 5f72 6567 6973        name_regis
-000002f0: 7472 793a 206d 6169 6e6e 6574 5f6e 616d  try: mainnet_nam
-00000300: 655f 7265 6769 7374 7279 0a              e_registry.
+00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
+00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
+00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
+00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
+00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
+00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
+00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
+00000070: 0a0a 636f 6e74 7261 6374 733a 0a20 206d  ..contracts:.  m
+00000080: 6169 6e6e 6574 5f6e 616d 655f 7265 6769  ainnet_name_regi
+00000090: 7374 7279 3a0a 2020 2020 6b69 6e64 3a20  stry:.    kind: 
+000000a0: 7465 7a6f 730a 2020 2020 6164 6472 6573  tezos.    addres
+000000b0: 733a 204b 5431 4742 5a6d 5378 6d6e 4b4a  s: KT1GBZmSxmnKJ
+000000c0: 5847 4d64 4d4c 6275 6750 664c 7955 506d  XGMdMLbugPfLyUPm
+000000d0: 754c 534d 774b 530a 2020 2020 7479 7065  uLSMwKS.    type
+000000e0: 6e61 6d65 3a20 6e61 6d65 5f72 6567 6973  name: name_regis
+000000f0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
+00000100: 3a0a 2020 747a 6b74 5f6d 6169 6e6e 6574  :.  tzkt_mainnet
+00000110: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+00000120: 732e 747a 6b74 0a20 2020 2075 726c 3a20  s.tzkt.    url: 
+00000130: 247b 545a 4b54 5f55 524c 3a2d 6874 7470  ${TZKT_URL:-http
+00000140: 733a 2f2f 6170 692e 747a 6b74 2e69 6f7d  s://api.tzkt.io}
+00000150: 0a0a 7465 6d70 6c61 7465 733a 0a20 2064  ..templates:.  d
+00000160: 6f6d 6169 6e73 3a0a 2020 2020 6b69 6e64  omains:.    kind
+00000170: 3a20 7465 7a6f 732e 747a 6b74 2e6f 7065  : tezos.tzkt.ope
+00000180: 7261 7469 6f6e 730a 2020 2020 6461 7461  rations.    data
+00000190: 736f 7572 6365 3a20 3c64 6174 6173 6f75  source: <datasou
+000001a0: 7263 653e 0a20 2020 2063 6f6e 7472 6163  rce>.    contrac
+000001b0: 7473 3a0a 2020 2020 2020 2d20 3c6e 616d  ts:.      - <nam
+000001c0: 655f 7265 6769 7374 7279 3e0a 2020 2020  e_registry>.    
+000001d0: 6861 6e64 6c65 7273 3a0a 2020 2020 2020  handlers:.      
+000001e0: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f61  - callback: on_a
+000001f0: 646d 696e 5f75 7064 6174 650a 2020 2020  dmin_update.    
+00000200: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
+00000210: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
+00000220: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
+00000230: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
+00000240: 6f6e 3a20 3c6e 616d 655f 7265 6769 7374  on: <name_regist
+00000250: 7279 3e0a 2020 2020 2020 2020 2020 2020  ry>.            
+00000260: 656e 7472 7970 6f69 6e74 3a20 6164 6d69  entrypoint: admi
+00000270: 6e5f 7570 6461 7465 0a20 2020 2020 202d  n_update.      -
+00000280: 2063 616c 6c62 6163 6b3a 206f 6e5f 6578   callback: on_ex
+00000290: 6563 7574 650a 2020 2020 2020 2020 7061  ecute.        pa
+000002a0: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
+000002b0: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
+000002c0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+000002d0: 2064 6573 7469 6e61 7469 6f6e 3a20 3c6e   destination: <n
+000002e0: 616d 655f 7265 6769 7374 7279 3e0a 2020  ame_registry>.  
+000002f0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
+00000300: 6f69 6e74 3a20 6578 6563 7574 650a 0a69  oint: execute..i
+00000310: 6e64 6578 6573 3a0a 2020 646f 6d61 696e  ndexes:.  domain
+00000320: 735f 6d61 696e 6e65 743a 0a20 2020 2074  s_mainnet:.    t
+00000330: 656d 706c 6174 653a 2064 6f6d 6169 6e73  emplate: domains
+00000340: 0a20 2020 2076 616c 7565 733a 0a20 2020  .    values:.   
+00000350: 2020 2064 6174 6173 6f75 7263 653a 2074     datasource: t
+00000360: 7a6b 745f 6d61 696e 6e65 740a 2020 2020  zkt_mainnet.    
+00000370: 2020 6e61 6d65 5f72 6567 6973 7472 793a    name_registry:
+00000380: 206d 6169 6e6e 6574 5f6e 616d 655f 7265   mainnet_name_re
+00000390: 6769 7374 7279 0a                        gistry.
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_expiry_map.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/handlers/on_update_expiry_map.py.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.name_registry.big_map.store_expiry_map_key import StoreExpiryMapKey
-from {{cookiecutter.package}}.types.name_registry.big_map.store_expiry_map_value import StoreExpiryMapValue
+import {{project.package}}.models as models
+from {{project.package}}.types.name_registry.tezos_big_maps.store_expiry_map_key import StoreExpiryMapKey
+from {{project.package}}.types.name_registry.tezos_big_maps.store_expiry_map_value import StoreExpiryMapValue
 from dipdup.context import HandlerContext
-from dipdup.models import BigMapDiff
+from dipdup.models.tezos_tzkt import TzktBigMapDiff
 
 
 async def on_update_expiry_map(
     ctx: HandlerContext,
-    store_expiry_map: BigMapDiff[StoreExpiryMapKey, StoreExpiryMapValue],
+    store_expiry_map: TzktBigMapDiff[StoreExpiryMapKey, StoreExpiryMapValue],
 ) -> None:
     if not store_expiry_map.action.has_value:
         return
     assert store_expiry_map.key
     assert store_expiry_map.value
 
     timestamp = store_expiry_map.value.__root__
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_big_maps/src/{{cookiecutter.package}}/handlers/on_update_records.py.j2` & `dipdup-7.0.0rc1/src/demo_big_maps/handlers/on_update_records.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.name_registry.big_map.store_records_key import StoreRecordsKey
-from {{cookiecutter.package}}.types.name_registry.big_map.store_records_value import StoreRecordsValue
+import demo_big_maps.models as models
+from demo_big_maps.types.name_registry.tezos_big_maps.store_records_key import StoreRecordsKey
+from demo_big_maps.types.name_registry.tezos_big_maps.store_records_value import StoreRecordsValue
 from dipdup.context import HandlerContext
-from dipdup.models import BigMapDiff
+from dipdup.models.tezos_tzkt import TzktBigMapDiff
 
 
 async def on_update_records(
     ctx: HandlerContext,
-    store_records: BigMapDiff[StoreRecordsKey, StoreRecordsValue],
+    store_records: TzktBigMapDiff[StoreRecordsKey, StoreRecordsValue],
 ) -> None:
     if not store_records.action.has_value:
         return
     assert store_records.key
     assert store_records.value
 
     record_name = bytes.fromhex(store_records.key.__root__).decode()
     record_path = record_name.split('.')
     ctx.logger.info('Processing `%s`', record_name)
 
-    if len(record_path) != int(store_records.value.level):
-        ctx.logger.error('Invalid record `%s`: expected %s chunks, got %s', record_name, store_records.value.level, len(record_path))
+    level = store_records.value.level
+    if len(record_path) != int(level):
+        ctx.logger.error('`%s`: expected %s chunks, got %s', record_name, level, len(record_path))
         return
 
-    if store_records.value.level == "1":
+    if level == '1':
         await models.TLD.update_or_create(id=record_name, defaults={'owner': store_records.value.owner})
     else:
-        if store_records.value.level == "2":
+        if level == '2':
+            token_id = int(store_records.value.tzip12_token_id) if store_records.value.tzip12_token_id else None
             await models.Domain.update_or_create(
                 id=record_name,
                 defaults={
                     'tld_id': record_path[-1],
                     'owner': store_records.value.owner,
-                    'token_id': int(store_records.value.tzip12_token_id) if store_records.value.tzip12_token_id else None,
+                    'token_id': token_id,
                 },
             )
 
         await models.Record.update_or_create(
             id=record_name,
-            defaults={'domain_id': '.'.join(record_path[-2:]), 'address': store_records.value.address},
-        )
+            defaults={'domain_id': '.'.join(record_path[-2:]), 'address': store_records.value.address,},
+        )
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dao/dipdup.yml.j2` & `dipdup-7.0.0rc1/src/demo_factories/dipdup.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 312e  spec_version: 1.
-00000010: 320a 7061 636b 6167 653a 207b 7b20 636f  2.package: {{ co
-00000020: 6f6b 6965 6375 7474 6572 2e70 6163 6b61  okiecutter.packa
-00000030: 6765 207d 7d0a 0a64 6174 6162 6173 653a  ge }}..database:
-00000040: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000050: 2020 7061 7468 3a20 7b7b 2063 6f6f 6b69    path: {{ cooki
-00000060: 6563 7574 7465 722e 7072 6f6a 6563 745f  ecutter.project_
-00000070: 6e61 6d65 207d 7d2e 7371 6c69 7465 330a  name }}.sqlite3.
-00000080: 0a63 6f6e 7472 6163 7473 3a0a 2020 7265  .contracts:.  re
-00000090: 6769 7374 7279 3a0a 2020 2020 636f 6465  gistry:.    code
-000000a0: 5f68 6173 683a 204b 5431 3943 4633 4b4b  _hash: KT19CF3KK
-000000b0: 7276 6457 3737 7474 466f 6d43 7569 6e32  rvdW77ttFomCuin2
-000000c0: 6b34 7541 566b 7279 5971 680a 2020 2020  k4uAVkryYqh.    
-000000d0: 7479 7065 6e61 6d65 3a20 7265 6769 7374  typename: regist
-000000e0: 7279 0a0a 6461 7461 736f 7572 6365 733a  ry..datasources:
-000000f0: 0a20 2074 7a6b 743a 0a20 2020 206b 696e  .  tzkt:.    kin
-00000100: 643a 2074 7a6b 740a 2020 2020 7572 6c3a  d: tzkt.    url:
-00000110: 2024 7b54 5a4b 545f 5552 4c3a 2d68 7474   ${TZKT_URL:-htt
-00000120: 7073 3a2f 2f61 7069 2e74 7a6b 742e 696f  ps://api.tzkt.io
-00000130: 7d0a 0a69 6e64 6578 6573 3a0a 2020 7265  }..indexes:.  re
-00000140: 6769 7374 7279 5f64 616f 3a0a 2020 2020  gistry_dao:.    
-00000150: 6b69 6e64 3a20 6f70 6572 6174 696f 6e0a  kind: operation.
-00000160: 2020 2020 6461 7461 736f 7572 6365 3a20      datasource: 
-00000170: 747a 6b74 0a20 2020 2074 7970 6573 3a0a  tzkt.    types:.
-00000180: 2020 2020 2020 2d20 7472 616e 7361 6374        - transact
-00000190: 696f 6e0a 2020 2020 2020 2d20 6f72 6967  ion.      - orig
-000001a0: 696e 6174 696f 6e0a 2020 2020 6861 6e64  ination.    hand
-000001b0: 6c65 7273 3a0a 2020 2020 2020 2d20 6361  lers:.      - ca
-000001c0: 6c6c 6261 636b 3a20 6f6e 5f6f 7269 6769  llback: on_origi
-000001d0: 6e61 7469 6f6e 0a20 2020 2020 2020 2070  nation.        p
-000001e0: 6174 7465 726e 3a0a 2020 2020 2020 2020  attern:.        
-000001f0: 2020 2d20 7479 7065 3a20 6f72 6967 696e    - type: origin
-00000200: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
-00000210: 2020 6f72 6967 696e 6174 6564 5f63 6f6e    originated_con
-00000220: 7472 6163 743a 2072 6567 6973 7472 790a  tract: registry.
-00000230: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
-00000240: 3a20 6f6e 5f70 726f 706f 7365 0a20 2020  : on_propose.   
-00000250: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
-00000260: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
-00000270: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
-00000280: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
-00000290: 696f 6e3a 2072 6567 6973 7472 790a 2020  ion: registry.  
-000002a0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
-000002b0: 6f69 6e74 3a20 7072 6f70 6f73 650a       oint: propose.
+00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
+00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
+00000020: 6661 6374 6f72 6965 730a 0a64 6174 6162  factories..datab
+00000030: 6173 653a 0a20 206b 696e 643a 2073 716c  ase:.  kind: sql
+00000040: 6974 650a 2020 7061 7468 3a20 6465 6d6f  ite.  path: demo
+00000050: 5f66 6163 746f 7269 6573 2e73 716c 6974  _factories.sqlit
+00000060: 6533 0a0a 636f 6e74 7261 6374 733a 0a20  e3..contracts:. 
+00000070: 2072 6567 6973 7472 793a 0a20 2020 206b   registry:.    k
+00000080: 696e 643a 2074 657a 6f73 0a20 2020 2061  ind: tezos.    a
+00000090: 6464 7265 7373 3a20 4b54 3139 4346 334b  ddress: KT19CF3K
+000000a0: 4b72 7664 5737 3774 7446 6f6d 4375 696e  KrvdW77ttFomCuin
+000000b0: 326b 3475 4156 6b72 7959 7168 0a20 2020  2k4uAVkryYqh.   
+000000c0: 2074 7970 656e 616d 653a 2072 6567 6973   typename: regis
+000000d0: 7472 790a 0a64 6174 6173 6f75 7263 6573  try..datasources
+000000e0: 3a0a 2020 747a 6b74 3a0a 2020 2020 6b69  :.  tzkt:.    ki
+000000f0: 6e64 3a20 7465 7a6f 732e 747a 6b74 0a20  nd: tezos.tzkt. 
+00000100: 2020 2075 726c 3a20 247b 545a 4b54 5f55     url: ${TZKT_U
+00000110: 524c 3a2d 6874 7470 733a 2f2f 6170 692e  RL:-https://api.
+00000120: 747a 6b74 2e69 6f7d 0a0a 696e 6465 7865  tzkt.io}..indexe
+00000130: 733a 0a20 2072 6567 6973 7472 795f 6461  s:.  registry_da
+00000140: 6f3a 0a20 2020 206b 696e 643a 2074 657a  o:.    kind: tez
+00000150: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
+00000160: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
+00000170: 653a 2074 7a6b 740a 2020 2020 7479 7065  e: tzkt.    type
+00000180: 733a 0a20 2020 2020 202d 2074 7261 6e73  s:.      - trans
+00000190: 6163 7469 6f6e 0a20 2020 2020 202d 206f  action.      - o
+000001a0: 7269 6769 6e61 7469 6f6e 0a20 2020 2068  rigination.    h
+000001b0: 616e 646c 6572 733a 0a20 2020 2020 202d  andlers:.      -
+000001c0: 2063 616c 6c62 6163 6b3a 206f 6e5f 6f72   callback: on_or
+000001d0: 6967 696e 6174 696f 6e0a 2020 2020 2020  igination.      
+000001e0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
+000001f0: 2020 2020 202d 2074 7970 653a 206f 7269       - type: ori
+00000200: 6769 6e61 7469 6f6e 0a20 2020 2020 2020  gination.       
+00000210: 2020 2020 206f 7269 6769 6e61 7465 645f       originated_
+00000220: 636f 6e74 7261 6374 3a20 7265 6769 7374  contract: regist
+00000230: 7279 0a20 2020 2020 202d 2063 616c 6c62  ry.      - callb
+00000240: 6163 6b3a 206f 6e5f 7072 6f70 6f73 650a  ack: on_propose.
+00000250: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
+00000260: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
+00000270: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
+00000280: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+00000290: 6e61 7469 6f6e 3a20 7265 6769 7374 7279  nation: registry
+000002a0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+000002b0: 7279 706f 696e 743a 2070 726f 706f 7365  rypoint: propose
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_dao/handlers/on_propose.py.j2`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.registry.parameter.propose import ProposeParameter
-from {{cookiecutter.package}}.types.registry.storage import RegistryStorage
+import {{project.package}}.models as models
+from {{project.package}}.types.registry.tezos_parameters.propose import ProposeParameter
+from {{project.package}}.types.registry.tezos_storage import RegistryStorage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_propose(
     ctx: HandlerContext,
-    propose: Transaction[ProposeParameter, RegistryStorage],
+    propose: TzktTransaction[ProposeParameter, RegistryStorage],
 ) -> None:
     dao = await models.DAO.get(address=propose.data.target_address)
     await models.Proposal(dao=dao).save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dao/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/models/__init__.py.j2`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,45 @@
-from tortoise.fields.relational import ForeignKeyFieldInstance
-from tortoise import fields
+from enum import IntEnum
 
-from dipdup.models import Model
-
-
-class DAO(Model):
-    address = fields.CharField(36, pk=True)
 
+from dipdup import fields
 
-class User(Model):
-    address = fields.CharField(36, pk=True)
-    balance = fields.IntField()
-
-
-class Proposal(Model):
-    id = fields.IntField(pk=True)
-    dao: ForeignKeyFieldInstance[DAO] = fields.ForeignKeyField('models.DAO', 'proposals')
-    # upvotes = fields.IntField(default=0)
-    # downvotes = fields.IntField(default=0)
-    # start_date = fields.DatetimeField()
-    # metadata = fields.JSONField()
-    # proposer = fields.ForeignKeyField('models.Address', 'proposals')
+from dipdup.models import Model
 
 
-class Vote(Model):
-    id = fields.IntField(pk=True)
-    proposal: ForeignKeyFieldInstance[Proposal] = fields.ForeignKeyField('models.Proposal', 'votes')
-    amount = fields.IntField()
+class SwapStatus(IntEnum):
+    ACTIVE = 0
+    FINISHED = 1
+    CANCELED = 2
+
+
+class Holder(Model):
+    address = fields.TextField(pk=True)
+
+
+class Token(Model):
+    id = fields.BigIntField(pk=True)
+    creator: fields.ForeignKeyField[Holder] = fields.ForeignKeyField('models.Holder', 'tokens')
+    supply = fields.BigIntField()
+    level = fields.BigIntField()
+    timestamp = fields.DatetimeField()
+
+
+class Swap(Model):
+    id = fields.BigIntField(pk=True)
+    creator: fields.ForeignKeyField[Holder] = fields.ForeignKeyField('models.Holder', 'swaps')
+    price = fields.BigIntField()
+    amount = fields.BigIntField()
+    amount_left = fields.BigIntField()
+    level = fields.BigIntField()
+    status = fields.IntEnumField(SwapStatus)
+    timestamp = fields.DatetimeField()
+
+
+class Trade(Model):
+    id = fields.BigIntField(pk=True)
+    swap: fields.ForeignKeyField[Swap] = fields.ForeignKeyField('models.Swap', 'trades')
+    seller: fields.ForeignKeyField[Holder] = fields.ForeignKeyField('models.Holder', 'sales')
+    buyer: fields.ForeignKeyField[Holder] = fields.ForeignKeyField('models.Holder', 'purchases')
+    amount = fields.BigIntField()
+    level = fields.BigIntField()
+    timestamp = fields.DatetimeField()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/dipdup.yml.j2` & `dipdup-7.0.0rc1/tests/configs/demo_dex.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,305 +1,317 @@
-00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 312e  spec_version: 1.
-00000010: 320a 7061 636b 6167 653a 207b 7b20 636f  2.package: {{ co
-00000020: 6f6b 6965 6375 7474 6572 2e70 6163 6b61  okiecutter.packa
-00000030: 6765 207d 7d0a 0a64 6174 6162 6173 653a  ge }}..database:
-00000040: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000050: 2020 7061 7468 3a20 7b7b 2063 6f6f 6b69    path: {{ cooki
-00000060: 6563 7574 7465 722e 7072 6f6a 6563 745f  ecutter.project_
-00000070: 6e61 6d65 207d 7d2e 7371 6c69 7465 330a  name }}.sqlite3.
-00000080: 0a63 6f6e 7472 6163 7473 3a0a 2020 6b75  .contracts:.  ku
-00000090: 7364 5f64 6578 5f6d 6169 6e6e 6574 3a0a  sd_dex_mainnet:.
-000000a0: 2020 2020 6164 6472 6573 733a 204b 5431      address: KT1
-000000b0: 4b34 4577 5470 6276 594e 3961 674a 646a  K4EwTpbvYN9agJdj
-000000c0: 7079 4a6d 345a 5a64 6870 554e 4b42 3346  pyJm4ZZdhpUNKB3F
-000000d0: 360a 2020 2020 7479 7065 6e61 6d65 3a20  6.    typename: 
-000000e0: 7175 6970 755f 6661 3132 0a20 206b 7573  quipu_fa12.  kus
-000000f0: 645f 746f 6b65 6e5f 6d61 696e 6e65 743a  d_token_mainnet:
-00000100: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
-00000110: 314b 3967 4352 6761 4c52 464b 5445 7259  1K9gCRgaLRFKTErY
-00000120: 7431 7756 7841 3346 7262 3946 6a61 736a  t1wVxA3Frb9Fjasj
-00000130: 5456 0a20 2020 2074 7970 656e 616d 653a  TV.    typename:
-00000140: 2066 6131 325f 746f 6b65 6e0a 2020 6864   fa12_token.  hd
-00000150: 616f 5f64 6578 5f6d 6169 6e6e 6574 3a0a  ao_dex_mainnet:.
-00000160: 2020 2020 6164 6472 6573 733a 204b 5431      address: KT1
-00000170: 5178 4c71 756b 7966 6f68 5056 356b 506b  QxLqukyfohPV5kPk
-00000180: 7739 3752 7336 6377 3144 4444 7659 6762  w97Rs6cw1DDDvYgb
-00000190: 420a 2020 2020 7479 7065 6e61 6d65 3a20  B.    typename: 
-000001a0: 7175 6970 755f 6661 320a 2020 6864 616f  quipu_fa2.  hdao
-000001b0: 5f74 6f6b 656e 5f6d 6169 6e6e 6574 3a0a  _token_mainnet:.
-000001c0: 2020 2020 6164 6472 6573 733a 204b 5431      address: KT1
-000001d0: 4146 4132 6d77 4e55 4d4e 6434 5373 756a  AFA2mwNUMNd4Ssuj
-000001e0: 4531 5959 7032 3976 6438 425a 656a 794b  E1YYp29vd8BZejyK
-000001f0: 570a 2020 2020 7479 7065 6e61 6d65 3a20  W.    typename: 
-00000200: 6661 325f 746f 6b65 6e0a 0a64 6174 6173  fa2_token..datas
-00000210: 6f75 7263 6573 3a0a 2020 747a 6b74 5f6d  ources:.  tzkt_m
-00000220: 6169 6e6e 6574 3a0a 2020 2020 6b69 6e64  ainnet:.    kind
-00000230: 3a20 747a 6b74 0a20 2020 2075 726c 3a20  : tzkt.    url: 
-00000240: 6874 7470 733a 2f2f 6170 692e 747a 6b74  https://api.tzkt
-00000250: 2e69 6f0a 0a61 6476 616e 6365 643a 0a20  .io..advanced:. 
-00000260: 2065 6172 6c79 5f72 6561 6c74 696d 653a   early_realtime:
-00000270: 2054 7275 650a 0a74 656d 706c 6174 6573   True..templates
-00000280: 3a0a 2020 7175 6970 7573 7761 705f 6661  :.  quipuswap_fa
-00000290: 3132 3a0a 2020 2020 6b69 6e64 3a20 6f70  12:.    kind: op
-000002a0: 6572 6174 696f 6e0a 2020 2020 6461 7461  eration.    data
-000002b0: 736f 7572 6365 3a20 747a 6b74 5f6d 6169  source: tzkt_mai
-000002c0: 6e6e 6574 0a20 2020 2063 6f6e 7472 6163  nnet.    contrac
-000002d0: 7473 3a0a 2020 2020 2020 2d20 3c64 6578  ts:.      - <dex
-000002e0: 5f63 6f6e 7472 6163 743e 0a20 2020 2074  _contract>.    t
-000002f0: 7970 6573 3a0a 2020 2020 2020 2d20 7472  ypes:.      - tr
-00000300: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-00000310: 2d20 6f72 6967 696e 6174 696f 6e0a 2020  - origination.  
-00000320: 2020 6861 6e64 6c65 7273 3a0a 2020 2020    handlers:.    
-00000330: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-00000340: 5f66 6131 325f 6f72 6967 696e 6174 696f  _fa12_originatio
-00000350: 6e0a 2020 2020 2020 2020 7061 7474 6572  n.        patter
-00000360: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
-00000370: 7970 653a 206f 7269 6769 6e61 7469 6f6e  ype: origination
-00000380: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
-00000390: 6769 6e61 7465 645f 636f 6e74 7261 6374  ginated_contract
-000003a0: 3a20 3c64 6578 5f63 6f6e 7472 6163 743e  : <dex_contract>
-000003b0: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
-000003c0: 6b3a 206f 6e5f 6661 3132 5f74 6f6b 656e  k: on_fa12_token
-000003d0: 5f74 6f5f 7465 7a0a 2020 2020 2020 2020  _to_tez.        
-000003e0: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
-000003f0: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
-00000400: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
-00000410: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
-00000420: 3c64 6578 5f63 6f6e 7472 6163 743e 0a20  <dex_contract>. 
-00000430: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
-00000440: 706f 696e 743a 2074 6f6b 656e 546f 5465  point: tokenToTe
-00000450: 7a50 6179 6d65 6e74 0a20 2020 2020 2020  zPayment.       
-00000460: 2020 202d 2074 7970 653a 2074 7261 6e73     - type: trans
-00000470: 6163 7469 6f6e 0a20 2020 2020 2020 2020  action.         
-00000480: 2020 2064 6573 7469 6e61 7469 6f6e 3a20     destination: 
-00000490: 3c74 6f6b 656e 5f63 6f6e 7472 6163 743e  <token_contract>
-000004a0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-000004b0: 7279 706f 696e 743a 2074 7261 6e73 6665  rypoint: transfe
-000004c0: 720a 2020 2020 2020 2020 2020 2d20 7479  r.          - ty
-000004d0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-000004e0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-000004f0: 6365 3a20 3c64 6578 5f63 6f6e 7472 6163  ce: <dex_contrac
-00000500: 743e 0a20 2020 2020 202d 2063 616c 6c62  t>.      - callb
-00000510: 6163 6b3a 206f 6e5f 6661 3132 5f74 657a  ack: on_fa12_tez
-00000520: 5f74 6f5f 746f 6b65 6e0a 2020 2020 2020  _to_token.      
-00000530: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-00000540: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00000550: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-00000560: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-00000570: 3a20 3c64 6578 5f63 6f6e 7472 6163 743e  : <dex_contract>
-00000580: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-00000590: 7279 706f 696e 743a 2074 657a 546f 546f  rypoint: tezToTo
-000005a0: 6b65 6e50 6179 6d65 6e74 0a20 2020 2020  kenPayment.     
-000005b0: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-000005c0: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-000005d0: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-000005e0: 3a20 3c74 6f6b 656e 5f63 6f6e 7472 6163  : <token_contrac
-000005f0: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
-00000600: 6e74 7279 706f 696e 743a 2074 7261 6e73  ntrypoint: trans
-00000610: 6665 720a 2020 2020 2020 2d20 6361 6c6c  fer.      - call
-00000620: 6261 636b 3a20 6f6e 5f66 6131 325f 696e  back: on_fa12_in
-00000630: 7665 7374 5f6c 6971 7569 6469 7479 0a20  vest_liquidity. 
-00000640: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-00000650: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-00000660: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-00000670: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00000680: 6174 696f 6e3a 203c 6465 785f 636f 6e74  ation: <dex_cont
-00000690: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
-000006a0: 2020 656e 7472 7970 6f69 6e74 3a20 696e    entrypoint: in
-000006b0: 7665 7374 4c69 7175 6964 6974 790a 2020  vestLiquidity.  
-000006c0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
-000006d0: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
-000006e0: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
-000006f0: 696f 6e3a 203c 746f 6b65 6e5f 636f 6e74  ion: <token_cont
-00000700: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
-00000710: 2020 656e 7472 7970 6f69 6e74 3a20 7472    entrypoint: tr
-00000720: 616e 7366 6572 0a20 2020 2020 202d 2063  ansfer.      - c
-00000730: 616c 6c62 6163 6b3a 206f 6e5f 6661 3132  allback: on_fa12
-00000740: 5f74 7261 6e73 6665 720a 2020 2020 2020  _transfer.      
-00000750: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
-00000760: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
-00000770: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
-00000780: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
-00000790: 3a20 3c64 6578 5f63 6f6e 7472 6163 743e  : <dex_contract>
-000007a0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-000007b0: 7279 706f 696e 743a 2074 7261 6e73 6665  rypoint: transfe
-000007c0: 720a 2020 2020 2020 2d20 6361 6c6c 6261  r.      - callba
-000007d0: 636b 3a20 6f6e 5f66 6131 325f 6469 7665  ck: on_fa12_dive
-000007e0: 7374 5f6c 6971 7569 6469 7479 0a20 2020  st_liquidity.   
-000007f0: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
-00000800: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
-00000810: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
-00000820: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
-00000830: 696f 6e3a 203c 6465 785f 636f 6e74 7261  ion: <dex_contra
-00000840: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00000850: 656e 7472 7970 6f69 6e74 3a20 6469 7665  entrypoint: dive
-00000860: 7374 4c69 7175 6964 6974 790a 2020 2020  stLiquidity.    
-00000870: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-00000880: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-00000890: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-000008a0: 6e3a 203c 746f 6b65 6e5f 636f 6e74 7261  n: <token_contra
-000008b0: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-000008c0: 656e 7472 7970 6f69 6e74 3a20 7472 616e  entrypoint: tran
-000008d0: 7366 6572 0a20 2020 2020 2020 2020 202d  sfer.          -
-000008e0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
-000008f0: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
-00000900: 6f75 7263 653a 203c 6465 785f 636f 6e74  ource: <dex_cont
-00000910: 7261 6374 3e0a 2020 2020 2020 2d20 6361  ract>.      - ca
-00000920: 6c6c 6261 636b 3a20 6f6e 5f66 6131 325f  llback: on_fa12_
-00000930: 7769 7468 6472 6177 5f70 726f 6669 740a  withdraw_profit.
-00000940: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
-00000950: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
-00000960: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
-00000970: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-00000980: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
-00000990: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-000009a0: 2020 2065 6e74 7279 706f 696e 743a 2077     entrypoint: w
-000009b0: 6974 6864 7261 7750 726f 6669 740a 2020  ithdrawProfit.  
-000009c0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
-000009d0: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
-000009e0: 2020 2020 2020 2020 736f 7572 6365 3a20          source: 
-000009f0: 3c64 6578 5f63 6f6e 7472 6163 743e 0a20  <dex_contract>. 
-00000a00: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00000a10: 6e61 6c3a 2054 7275 650a 0a20 2071 7569  nal: True..  qui
-00000a20: 7075 7377 6170 5f66 6132 3a0a 2020 2020  puswap_fa2:.    
-00000a30: 6b69 6e64 3a20 6f70 6572 6174 696f 6e0a  kind: operation.
-00000a40: 2020 2020 6461 7461 736f 7572 6365 3a20      datasource: 
-00000a50: 747a 6b74 5f6d 6169 6e6e 6574 0a20 2020  tzkt_mainnet.   
-00000a60: 2063 6f6e 7472 6163 7473 3a0a 2020 2020   contracts:.    
-00000a70: 2020 2d20 3c64 6578 5f63 6f6e 7472 6163    - <dex_contrac
-00000a80: 743e 0a20 2020 2074 7970 6573 3a0a 2020  t>.    types:.  
-00000a90: 2020 2020 2d20 7472 616e 7361 6374 696f      - transactio
-00000aa0: 6e0a 2020 2020 2020 2d20 6f72 6967 696e  n.      - origin
-00000ab0: 6174 696f 6e0a 2020 2020 6861 6e64 6c65  ation.    handle
-00000ac0: 7273 3a0a 2020 2020 2020 2d20 6361 6c6c  rs:.      - call
-00000ad0: 6261 636b 3a20 6f6e 5f66 6132 5f6f 7269  back: on_fa2_ori
-00000ae0: 6769 6e61 7469 6f6e 0a20 2020 2020 2020  gination.       
-00000af0: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
-00000b00: 2020 2020 2d20 7479 7065 3a20 6f72 6967      - type: orig
-00000b10: 696e 6174 696f 6e0a 2020 2020 2020 2020  ination.        
-00000b20: 2020 2020 6f72 6967 696e 6174 6564 5f63      originated_c
-00000b30: 6f6e 7472 6163 743a 203c 6465 785f 636f  ontract: <dex_co
-00000b40: 6e74 7261 6374 3e0a 2020 2020 2020 2d20  ntract>.      - 
-00000b50: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6132  callback: on_fa2
-00000b60: 5f74 6f6b 656e 5f74 6f5f 7465 7a0a 2020  _token_to_tez.  
-00000b70: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
-00000b80: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-00000b90: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000ba0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00000bb0: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
-00000bc0: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
-00000bd0: 2065 6e74 7279 706f 696e 743a 2074 6f6b   entrypoint: tok
-00000be0: 656e 546f 5465 7a50 6179 6d65 6e74 0a20  enToTezPayment. 
-00000bf0: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-00000c00: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00000c10: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00000c20: 7469 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e  tion: <token_con
-00000c30: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
-00000c40: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
-00000c50: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
-00000c60: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
-00000c70: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00000c80: 2020 736f 7572 6365 3a20 3c64 6578 5f63    source: <dex_c
-00000c90: 6f6e 7472 6163 743e 0a20 2020 2020 202d  ontract>.      -
-00000ca0: 2063 616c 6c62 6163 6b3a 206f 6e5f 6661   callback: on_fa
-00000cb0: 325f 7465 7a5f 746f 5f74 6f6b 656e 0a20  2_tez_to_token. 
-00000cc0: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-00000cd0: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-00000ce0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-00000cf0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00000d00: 6174 696f 6e3a 203c 6465 785f 636f 6e74  ation: <dex_cont
-00000d10: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
-00000d20: 2020 656e 7472 7970 6f69 6e74 3a20 7465    entrypoint: te
-00000d30: 7a54 6f54 6f6b 656e 5061 796d 656e 740a  zToTokenPayment.
-00000d40: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-00000d50: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-00000d60: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00000d70: 6174 696f 6e3a 203c 746f 6b65 6e5f 636f  ation: <token_co
-00000d80: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
-00000d90: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
-00000da0: 7472 616e 7366 6572 0a20 2020 2020 202d  transfer.      -
-00000db0: 2063 616c 6c62 6163 6b3a 206f 6e5f 6661   callback: on_fa
-00000dc0: 325f 696e 7665 7374 5f6c 6971 7569 6469  2_invest_liquidi
-00000dd0: 7479 0a20 2020 2020 2020 2070 6174 7465  ty.        patte
-00000de0: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
-00000df0: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
-00000e00: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
-00000e10: 7374 696e 6174 696f 6e3a 203c 6465 785f  stination: <dex_
-00000e20: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
-00000e30: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-00000e40: 3a20 696e 7665 7374 4c69 7175 6964 6974  : investLiquidit
-00000e50: 790a 2020 2020 2020 2020 2020 2d20 7479  y.          - ty
-00000e60: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00000e70: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00000e80: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
-00000e90: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
-00000ea0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-00000eb0: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
-00000ec0: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
-00000ed0: 6661 325f 7472 616e 7366 6572 0a20 2020  fa2_transfer.   
-00000ee0: 2020 2020 2070 6174 7465 726e 3a0a 2020       pattern:.  
-00000ef0: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
-00000f00: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
-00000f10: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
-00000f20: 696f 6e3a 203c 6465 785f 636f 6e74 7261  ion: <dex_contra
-00000f30: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-00000f40: 656e 7472 7970 6f69 6e74 3a20 7472 616e  entrypoint: tran
-00000f50: 7366 6572 0a20 2020 2020 202d 2063 616c  sfer.      - cal
-00000f60: 6c62 6163 6b3a 206f 6e5f 6661 325f 6469  lback: on_fa2_di
-00000f70: 7665 7374 5f6c 6971 7569 6469 7479 0a20  vest_liquidity. 
-00000f80: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
-00000f90: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
-00000fa0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
-00000fb0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
-00000fc0: 6174 696f 6e3a 203c 6465 785f 636f 6e74  ation: <dex_cont
-00000fd0: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
-00000fe0: 2020 656e 7472 7970 6f69 6e74 3a20 6469    entrypoint: di
-00000ff0: 7665 7374 4c69 7175 6964 6974 790a 2020  vestLiquidity.  
-00001000: 2020 2020 2020 2020 2d20 7479 7065 3a20          - type: 
-00001010: 7472 616e 7361 6374 696f 6e0a 2020 2020  transaction.    
-00001020: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
-00001030: 696f 6e3a 203c 746f 6b65 6e5f 636f 6e74  ion: <token_cont
-00001040: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
-00001050: 2020 656e 7472 7970 6f69 6e74 3a20 7472    entrypoint: tr
-00001060: 616e 7366 6572 0a20 2020 2020 2020 2020  ansfer.         
-00001070: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-00001080: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00001090: 2073 6f75 7263 653a 203c 6465 785f 636f   source: <dex_co
-000010a0: 6e74 7261 6374 3e0a 2020 2020 2020 2d20  ntract>.      - 
-000010b0: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6132  callback: on_fa2
-000010c0: 5f77 6974 6864 7261 775f 7072 6f66 6974  _withdraw_profit
-000010d0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-000010e0: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
-000010f0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-00001100: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00001110: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
-00001120: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
-00001130: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
-00001140: 7769 7468 6472 6177 5072 6f66 6974 0a20  withdrawProfit. 
-00001150: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-00001160: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
-00001170: 2020 2020 2020 2020 2073 6f75 7263 653a           source:
-00001180: 203c 6465 785f 636f 6e74 7261 6374 3e0a   <dex_contract>.
-00001190: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-000011a0: 6f6e 616c 3a20 5472 7565 0a0a 696e 6465  onal: True..inde
-000011b0: 7865 733a 0a20 206b 7573 645f 6d61 696e  xes:.  kusd_main
-000011c0: 6e65 743a 0a20 2020 2074 656d 706c 6174  net:.    templat
-000011d0: 653a 2071 7569 7075 7377 6170 5f66 6131  e: quipuswap_fa1
-000011e0: 320a 2020 2020 7661 6c75 6573 3a0a 2020  2.    values:.  
-000011f0: 2020 2020 6465 785f 636f 6e74 7261 6374      dex_contract
-00001200: 3a20 6b75 7364 5f64 6578 5f6d 6169 6e6e  : kusd_dex_mainn
-00001210: 6574 0a20 2020 2020 2074 6f6b 656e 5f63  et.      token_c
-00001220: 6f6e 7472 6163 743a 206b 7573 645f 746f  ontract: kusd_to
-00001230: 6b65 6e5f 6d61 696e 6e65 740a 2020 2020  ken_mainnet.    
-00001240: 2020 7379 6d62 6f6c 3a20 6b55 5344 0a20    symbol: kUSD. 
-00001250: 2020 2020 2064 6563 696d 616c 733a 2031       decimals: 1
-00001260: 380a 0a20 2068 6461 6f5f 6d61 696e 6e65  8..  hdao_mainne
-00001270: 743a 0a20 2020 2074 656d 706c 6174 653a  t:.    template:
-00001280: 2071 7569 7075 7377 6170 5f66 6132 0a20   quipuswap_fa2. 
-00001290: 2020 2076 616c 7565 733a 0a20 2020 2020     values:.     
-000012a0: 2064 6578 5f63 6f6e 7472 6163 743a 2068   dex_contract: h
-000012b0: 6461 6f5f 6465 785f 6d61 696e 6e65 740a  dao_dex_mainnet.
-000012c0: 2020 2020 2020 746f 6b65 6e5f 636f 6e74        token_cont
-000012d0: 7261 6374 3a20 6864 616f 5f74 6f6b 656e  ract: hdao_token
-000012e0: 5f6d 6169 6e6e 6574 0a20 2020 2020 2073  _mainnet.      s
-000012f0: 796d 626f 6c3a 2068 4441 4f0a 2020 2020  ymbol: hDAO.    
-00001300: 2020 6465 6369 6d61 6c73 3a20 360a         decimals: 6.
+00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
+00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
+00000020: 6465 780a 0a64 6174 6162 6173 653a 0a20  dex..database:. 
+00000030: 206b 696e 643a 2073 716c 6974 650a 2020   kind: sqlite.  
+00000040: 7061 7468 3a20 6462 2e73 716c 6974 6533  path: db.sqlite3
+00000050: 0a0a 636f 6e74 7261 6374 733a 0a20 206b  ..contracts:.  k
+00000060: 7573 645f 6465 785f 6d61 696e 6e65 743a  usd_dex_mainnet:
+00000070: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+00000080: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
+00000090: 314b 3445 7754 7062 7659 4e39 6167 4a64  1K4EwTpbvYN9agJd
+000000a0: 6a70 794a 6d34 5a5a 6468 7055 4e4b 4233  jpyJm4ZZdhpUNKB3
+000000b0: 4636 0a20 2020 2074 7970 656e 616d 653a  F6.    typename:
+000000c0: 2071 7569 7075 5f66 6131 320a 2020 6b75   quipu_fa12.  ku
+000000d0: 7364 5f74 6f6b 656e 5f6d 6169 6e6e 6574  sd_token_mainnet
+000000e0: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+000000f0: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
+00000100: 5431 4b39 6743 5267 614c 5246 4b54 4572  T1K9gCRgaLRFKTEr
+00000110: 5974 3177 5678 4133 4672 6239 466a 6173  Yt1wVxA3Frb9Fjas
+00000120: 6a54 560a 2020 2020 7479 7065 6e61 6d65  jTV.    typename
+00000130: 3a20 6661 3132 5f74 6f6b 656e 0a20 2068  : fa12_token.  h
+00000140: 6461 6f5f 6465 785f 6d61 696e 6e65 743a  dao_dex_mainnet:
+00000150: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+00000160: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
+00000170: 3151 784c 7175 6b79 666f 6850 5635 6b50  1QxLqukyfohPV5kP
+00000180: 6b77 3937 5273 3663 7731 4444 4476 5967  kw97Rs6cw1DDDvYg
+00000190: 6242 0a20 2020 2074 7970 656e 616d 653a  bB.    typename:
+000001a0: 2071 7569 7075 5f66 6132 0a20 2068 6461   quipu_fa2.  hda
+000001b0: 6f5f 746f 6b65 6e5f 6d61 696e 6e65 743a  o_token_mainnet:
+000001c0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+000001d0: 0a20 2020 2061 6464 7265 7373 3a20 4b54  .    address: KT
+000001e0: 3141 4641 326d 774e 554d 4e64 3453 7375  1AFA2mwNUMNd4Ssu
+000001f0: 6a45 3159 5970 3239 7664 3842 5a65 6a79  jE1YYp29vd8BZejy
+00000200: 4b57 0a20 2020 2074 7970 656e 616d 653a  KW.    typename:
+00000210: 2066 6132 5f74 6f6b 656e 0a0a 6461 7461   fa2_token..data
+00000220: 736f 7572 6365 733a 0a20 2074 7a6b 745f  sources:.  tzkt_
+00000230: 6d61 696e 6e65 743a 0a20 2020 206b 696e  mainnet:.    kin
+00000240: 643a 2074 657a 6f73 2e74 7a6b 740a 2020  d: tezos.tzkt.  
+00000250: 2020 7572 6c3a 2068 7474 7073 3a2f 2f61    url: https://a
+00000260: 7069 2e74 7a6b 742e 696f 0a20 2020 2068  pi.tzkt.io.    h
+00000270: 7474 703a 0a20 2020 2020 2072 6570 6c61  ttp:.      repla
+00000280: 795f 7061 7468 3a20 247b 4449 5044 5550  y_path: ${DIPDUP
+00000290: 5f52 4550 4c41 595f 5041 5448 3a2d 7d0a  _REPLAY_PATH:-}.
+000002a0: 0a74 656d 706c 6174 6573 3a0a 2020 7175  .templates:.  qu
+000002b0: 6970 7573 7761 705f 6661 3132 3a0a 2020  ipuswap_fa12:.  
+000002c0: 2020 6b69 6e64 3a20 7465 7a6f 732e 747a    kind: tezos.tz
+000002d0: 6b74 2e6f 7065 7261 7469 6f6e 730a 2020  kt.operations.  
+000002e0: 2020 6461 7461 736f 7572 6365 3a20 747a    datasource: tz
+000002f0: 6b74 5f6d 6169 6e6e 6574 0a20 2020 2063  kt_mainnet.    c
+00000300: 6f6e 7472 6163 7473 3a0a 2020 2020 2020  ontracts:.      
+00000310: 2d20 3c64 6578 5f63 6f6e 7472 6163 743e  - <dex_contract>
+00000320: 0a20 2020 2074 7970 6573 3a0a 2020 2020  .    types:.    
+00000330: 2020 2d20 7472 616e 7361 6374 696f 6e0a    - transaction.
+00000340: 2020 2020 2020 2d20 6f72 6967 696e 6174        - originat
+00000350: 696f 6e0a 2020 2020 6861 6e64 6c65 7273  ion.    handlers
+00000360: 3a0a 2020 2020 2020 2d20 6361 6c6c 6261  :.      - callba
+00000370: 636b 3a20 6f6e 5f66 6131 325f 6f72 6967  ck: on_fa12_orig
+00000380: 696e 6174 696f 6e0a 2020 2020 2020 2020  ination.        
+00000390: 7061 7474 6572 6e3a 0a20 2020 2020 2020  pattern:.       
+000003a0: 2020 202d 2074 7970 653a 206f 7269 6769     - type: origi
+000003b0: 6e61 7469 6f6e 0a20 2020 2020 2020 2020  nation.         
+000003c0: 2020 206f 7269 6769 6e61 7465 645f 636f     originated_co
+000003d0: 6e74 7261 6374 3a20 3c64 6578 5f63 6f6e  ntract: <dex_con
+000003e0: 7472 6163 743e 0a20 2020 2020 202d 2063  tract>.      - c
+000003f0: 616c 6c62 6163 6b3a 206f 6e5f 6661 3132  allback: on_fa12
+00000400: 5f74 6f6b 656e 5f74 6f5f 7465 7a0a 2020  _token_to_tez.  
+00000410: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000420: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+00000430: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+00000440: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+00000450: 7469 6f6e 3a20 3c64 6578 5f63 6f6e 7472  tion: <dex_contr
+00000460: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+00000470: 2065 6e74 7279 706f 696e 743a 2074 6f6b   entrypoint: tok
+00000480: 656e 546f 5465 7a50 6179 6d65 6e74 0a20  enToTezPayment. 
+00000490: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+000004a0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+000004b0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+000004c0: 7469 6f6e 3a20 3c74 6f6b 656e 5f63 6f6e  tion: <token_con
+000004d0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+000004e0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
+000004f0: 7261 6e73 6665 720a 2020 2020 2020 2020  ransfer.        
+00000500: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
+00000510: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+00000520: 2020 736f 7572 6365 3a20 3c64 6578 5f63    source: <dex_c
+00000530: 6f6e 7472 6163 743e 0a20 2020 2020 202d  ontract>.      -
+00000540: 2063 616c 6c62 6163 6b3a 206f 6e5f 6661   callback: on_fa
+00000550: 3132 5f74 657a 5f74 6f5f 746f 6b65 6e0a  12_tez_to_token.
+00000560: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
+00000570: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
+00000580: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
+00000590: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+000005a0: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
+000005b0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+000005c0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
+000005d0: 657a 546f 546f 6b65 6e50 6179 6d65 6e74  ezToTokenPayment
+000005e0: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
+000005f0: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
+00000600: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+00000610: 6e61 7469 6f6e 3a20 3c74 6f6b 656e 5f63  nation: <token_c
+00000620: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
+00000630: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
+00000640: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
+00000650: 2d20 6361 6c6c 6261 636b 3a20 6f6e 5f66  - callback: on_f
+00000660: 6131 325f 696e 7665 7374 5f6c 6971 7569  a12_invest_liqui
+00000670: 6469 7479 0a20 2020 2020 2020 2070 6174  dity.        pat
+00000680: 7465 726e 3a0a 2020 2020 2020 2020 2020  tern:.          
+00000690: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
+000006a0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000006b0: 6465 7374 696e 6174 696f 6e3a 203c 6465  destination: <de
+000006c0: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
+000006d0: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+000006e0: 6e74 3a20 696e 7665 7374 4c69 7175 6964  nt: investLiquid
+000006f0: 6974 790a 2020 2020 2020 2020 2020 2d20  ity.          - 
+00000700: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00000710: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000720: 7374 696e 6174 696f 6e3a 203c 746f 6b65  stination: <toke
+00000730: 6e5f 636f 6e74 7261 6374 3e0a 2020 2020  n_contract>.    
+00000740: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+00000750: 6e74 3a20 7472 616e 7366 6572 0a20 2020  nt: transfer.   
+00000760: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
+00000770: 6e5f 6661 3132 5f74 7261 6e73 6665 720a  n_fa12_transfer.
+00000780: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
+00000790: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
+000007a0: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
+000007b0: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+000007c0: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
+000007d0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+000007e0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
+000007f0: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
+00000800: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6131  callback: on_fa1
+00000810: 325f 6469 7665 7374 5f6c 6971 7569 6469  2_divest_liquidi
+00000820: 7479 0a20 2020 2020 2020 2070 6174 7465  ty.        patte
+00000830: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
+00000840: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00000850: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
+00000860: 7374 696e 6174 696f 6e3a 203c 6465 785f  stination: <dex_
+00000870: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+00000880: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+00000890: 3a20 6469 7665 7374 4c69 7175 6964 6974  : divestLiquidit
+000008a0: 790a 2020 2020 2020 2020 2020 2d20 7479  y.          - ty
+000008b0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+000008c0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+000008d0: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
+000008e0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+000008f0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+00000900: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
+00000910: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+00000920: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+00000930: 2020 2020 2073 6f75 7263 653a 203c 6465       source: <de
+00000940: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
+00000950: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
+00000960: 5f66 6131 325f 7769 7468 6472 6177 5f70  _fa12_withdraw_p
+00000970: 726f 6669 740a 2020 2020 2020 2020 7061  rofit.        pa
+00000980: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
+00000990: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
+000009a0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+000009b0: 2064 6573 7469 6e61 7469 6f6e 3a20 3c64   destination: <d
+000009c0: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
+000009d0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+000009e0: 696e 743a 2077 6974 6864 7261 7750 726f  int: withdrawPro
+000009f0: 6669 740a 2020 2020 2020 2020 2020 2d20  fit.          - 
+00000a00: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
+00000a10: 6e0a 2020 2020 2020 2020 2020 2020 736f  n.            so
+00000a20: 7572 6365 3a20 3c64 6578 5f63 6f6e 7472  urce: <dex_contr
+00000a30: 6163 743e 0a20 2020 2020 2020 2020 2020  act>.           
+00000a40: 206f 7074 696f 6e61 6c3a 2054 7275 650a   optional: True.
+00000a50: 2020 2020 6669 7273 745f 6c65 7665 6c3a      first_level:
+00000a60: 2031 3430 3735 3238 0a20 2020 206c 6173   1407528.    las
+00000a70: 745f 6c65 7665 6c3a 2031 3433 3736 3130  t_level: 1437610
+00000a80: 0a0a 2020 7175 6970 7573 7761 705f 6661  ..  quipuswap_fa
+00000a90: 323a 0a20 2020 206b 696e 643a 2074 657a  2:.    kind: tez
+00000aa0: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
+00000ab0: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
+00000ac0: 653a 2074 7a6b 745f 6d61 696e 6e65 740a  e: tzkt_mainnet.
+00000ad0: 2020 2020 636f 6e74 7261 6374 733a 0a20      contracts:. 
+00000ae0: 2020 2020 202d 203c 6465 785f 636f 6e74       - <dex_cont
+00000af0: 7261 6374 3e0a 2020 2020 7479 7065 733a  ract>.    types:
+00000b00: 0a20 2020 2020 202d 2074 7261 6e73 6163  .      - transac
+00000b10: 7469 6f6e 0a20 2020 2020 202d 206f 7269  tion.      - ori
+00000b20: 6769 6e61 7469 6f6e 0a20 2020 2068 616e  gination.    han
+00000b30: 646c 6572 733a 0a20 2020 2020 202d 2063  dlers:.      - c
+00000b40: 616c 6c62 6163 6b3a 206f 6e5f 6661 325f  allback: on_fa2_
+00000b50: 6f72 6967 696e 6174 696f 6e0a 2020 2020  origination.    
+00000b60: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
+00000b70: 2020 2020 2020 202d 2074 7970 653a 206f         - type: o
+00000b80: 7269 6769 6e61 7469 6f6e 0a20 2020 2020  rigination.     
+00000b90: 2020 2020 2020 206f 7269 6769 6e61 7465         originate
+00000ba0: 645f 636f 6e74 7261 6374 3a20 3c64 6578  d_contract: <dex
+00000bb0: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
+00000bc0: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+00000bd0: 6661 325f 746f 6b65 6e5f 746f 5f74 657a  fa2_token_to_tez
+00000be0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
+00000bf0: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
+00000c00: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+00000c10: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000c20: 696e 6174 696f 6e3a 203c 6465 785f 636f  ination: <dex_co
+00000c30: 6e74 7261 6374 3e0a 2020 2020 2020 2020  ntract>.        
+00000c40: 2020 2020 656e 7472 7970 6f69 6e74 3a20      entrypoint: 
+00000c50: 746f 6b65 6e54 6f54 657a 5061 796d 656e  tokenToTezPaymen
+00000c60: 740a 2020 2020 2020 2020 2020 2d20 7479  t.          - ty
+00000c70: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+00000c80: 2020 2020 2020 2020 2020 2020 6465 7374              dest
+00000c90: 696e 6174 696f 6e3a 203c 746f 6b65 6e5f  ination: <token_
+00000ca0: 636f 6e74 7261 6374 3e0a 2020 2020 2020  contract>.      
+00000cb0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
+00000cc0: 3a20 7472 616e 7366 6572 0a20 2020 2020  : transfer.     
+00000cd0: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+00000ce0: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+00000cf0: 2020 2020 2073 6f75 7263 653a 203c 6465       source: <de
+00000d00: 785f 636f 6e74 7261 6374 3e0a 2020 2020  x_contract>.    
+00000d10: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
+00000d20: 5f66 6132 5f74 657a 5f74 6f5f 746f 6b65  _fa2_tez_to_toke
+00000d30: 6e0a 2020 2020 2020 2020 7061 7474 6572  n.        patter
+00000d40: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
+00000d50: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
+00000d60: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00000d70: 7469 6e61 7469 6f6e 3a20 3c64 6578 5f63  tination: <dex_c
+00000d80: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
+00000d90: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
+00000da0: 2074 657a 546f 546f 6b65 6e50 6179 6d65   tezToTokenPayme
+00000db0: 6e74 0a20 2020 2020 2020 2020 202d 2074  nt.          - t
+00000dc0: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
+00000dd0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00000de0: 7469 6e61 7469 6f6e 3a20 3c74 6f6b 656e  tination: <token
+00000df0: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
+00000e00: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
+00000e10: 743a 2074 7261 6e73 6665 720a 2020 2020  t: transfer.    
+00000e20: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
+00000e30: 5f66 6132 5f69 6e76 6573 745f 6c69 7175  _fa2_invest_liqu
+00000e40: 6964 6974 790a 2020 2020 2020 2020 7061  idity.        pa
+00000e50: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
+00000e60: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
+00000e70: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00000e80: 2064 6573 7469 6e61 7469 6f6e 3a20 3c64   destination: <d
+00000e90: 6578 5f63 6f6e 7472 6163 743e 0a20 2020  ex_contract>.   
+00000ea0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+00000eb0: 696e 743a 2069 6e76 6573 744c 6971 7569  int: investLiqui
+00000ec0: 6469 7479 0a20 2020 2020 2020 2020 202d  dity.          -
+00000ed0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
+00000ee0: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
+00000ef0: 6573 7469 6e61 7469 6f6e 3a20 3c74 6f6b  estination: <tok
+00000f00: 656e 5f63 6f6e 7472 6163 743e 0a20 2020  en_contract>.   
+00000f10: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+00000f20: 696e 743a 2074 7261 6e73 6665 720a 2020  int: transfer.  
+00000f30: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
+00000f40: 6f6e 5f66 6132 5f74 7261 6e73 6665 720a  on_fa2_transfer.
+00000f50: 2020 2020 2020 2020 7061 7474 6572 6e3a          pattern:
+00000f60: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
+00000f70: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
+00000f80: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+00000f90: 6e61 7469 6f6e 3a20 3c64 6578 5f63 6f6e  nation: <dex_con
+00000fa0: 7472 6163 743e 0a20 2020 2020 2020 2020  tract>.         
+00000fb0: 2020 2065 6e74 7279 706f 696e 743a 2074     entrypoint: t
+00000fc0: 7261 6e73 6665 720a 2020 2020 2020 2d20  ransfer.      - 
+00000fd0: 6361 6c6c 6261 636b 3a20 6f6e 5f66 6132  callback: on_fa2
+00000fe0: 5f64 6976 6573 745f 6c69 7175 6964 6974  _divest_liquidit
+00000ff0: 790a 2020 2020 2020 2020 7061 7474 6572  y.        patter
+00001000: 6e3a 0a20 2020 2020 2020 2020 202d 2074  n:.          - t
+00001010: 7970 653a 2074 7261 6e73 6163 7469 6f6e  ype: transaction
+00001020: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00001030: 7469 6e61 7469 6f6e 3a20 3c64 6578 5f63  tination: <dex_c
+00001040: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
+00001050: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
+00001060: 2064 6976 6573 744c 6971 7569 6469 7479   divestLiquidity
+00001070: 0a20 2020 2020 2020 2020 202d 2074 7970  .          - typ
+00001080: 653a 2074 7261 6e73 6163 7469 6f6e 0a20  e: transaction. 
+00001090: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+000010a0: 6e61 7469 6f6e 3a20 3c74 6f6b 656e 5f63  nation: <token_c
+000010b0: 6f6e 7472 6163 743e 0a20 2020 2020 2020  ontract>.       
+000010c0: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
+000010d0: 2074 7261 6e73 6665 720a 2020 2020 2020   transfer.      
+000010e0: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+000010f0: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+00001100: 2020 2020 736f 7572 6365 3a20 3c64 6578      source: <dex
+00001110: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
+00001120: 202d 2063 616c 6c62 6163 6b3a 206f 6e5f   - callback: on_
+00001130: 6661 325f 7769 7468 6472 6177 5f70 726f  fa2_withdraw_pro
+00001140: 6669 740a 2020 2020 2020 2020 7061 7474  fit.        patt
+00001150: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
+00001160: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
+00001170: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
+00001180: 6573 7469 6e61 7469 6f6e 3a20 3c64 6578  estination: <dex
+00001190: 5f63 6f6e 7472 6163 743e 0a20 2020 2020  _contract>.     
+000011a0: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
+000011b0: 743a 2077 6974 6864 7261 7750 726f 6669  t: withdrawProfi
+000011c0: 740a 2020 2020 2020 2020 2020 2d20 7479  t.          - ty
+000011d0: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
+000011e0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
+000011f0: 6365 3a20 3c64 6578 5f63 6f6e 7472 6163  ce: <dex_contrac
+00001200: 743e 0a20 2020 2020 2020 2020 2020 206f  t>.            o
+00001210: 7074 696f 6e61 6c3a 2054 7275 650a 2020  ptional: True.  
+00001220: 2020 6669 7273 745f 6c65 7665 6c3a 2031    first_level: 1
+00001230: 3430 3735 3238 0a20 2020 206c 6173 745f  407528.    last_
+00001240: 6c65 7665 6c3a 2031 3434 3431 3333 0a0a  level: 1444133..
+00001250: 696e 6465 7865 733a 0a20 206b 7573 645f  indexes:.  kusd_
+00001260: 6d61 696e 6e65 743a 0a20 2020 2074 656d  mainnet:.    tem
+00001270: 706c 6174 653a 2071 7569 7075 7377 6170  plate: quipuswap
+00001280: 5f66 6131 320a 2020 2020 7661 6c75 6573  _fa12.    values
+00001290: 3a0a 2020 2020 2020 6465 785f 636f 6e74  :.      dex_cont
+000012a0: 7261 6374 3a20 6b75 7364 5f64 6578 5f6d  ract: kusd_dex_m
+000012b0: 6169 6e6e 6574 0a20 2020 2020 2074 6f6b  ainnet.      tok
+000012c0: 656e 5f63 6f6e 7472 6163 743a 206b 7573  en_contract: kus
+000012d0: 645f 746f 6b65 6e5f 6d61 696e 6e65 740a  d_token_mainnet.
+000012e0: 2020 2020 2020 7379 6d62 6f6c 3a20 6b55        symbol: kU
+000012f0: 5344 0a20 2020 2020 2064 6563 696d 616c  SD.      decimal
+00001300: 733a 2031 380a 0a20 2068 6461 6f5f 6d61  s: 18..  hdao_ma
+00001310: 696e 6e65 743a 0a20 2020 2074 656d 706c  innet:.    templ
+00001320: 6174 653a 2071 7569 7075 7377 6170 5f66  ate: quipuswap_f
+00001330: 6132 0a20 2020 2076 616c 7565 733a 0a20  a2.    values:. 
+00001340: 2020 2020 2064 6578 5f63 6f6e 7472 6163       dex_contrac
+00001350: 743a 2068 6461 6f5f 6465 785f 6d61 696e  t: hdao_dex_main
+00001360: 6e65 740a 2020 2020 2020 746f 6b65 6e5f  net.      token_
+00001370: 636f 6e74 7261 6374 3a20 6864 616f 5f74  contract: hdao_t
+00001380: 6f6b 656e 5f6d 6169 6e6e 6574 0a20 2020  oken_mainnet.   
+00001390: 2020 2073 796d 626f 6c3a 2068 4441 4f0a     symbol: hDAO.
+000013a0: 2020 2020 2020 6465 6369 6d61 6c73 3a20        decimals: 
+000013b0: 360a 0a6c 6f67 6769 6e67 3a20 5741 524e  6..logging: WARN
+000013c0: 0a                                       .
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_divest_liquidity.py.j2` & `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_divest_liquidity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from decimal import Decimal
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.fa12_token.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.fa12_token.storage import Fa12TokenStorage
-from {{cookiecutter.package}}.types.quipu_fa12.parameter.divest_liquidity import DivestLiquidityParameter
-from {{cookiecutter.package}}.types.quipu_fa12.storage import QuipuFa12Storage
+import demo_dex.models as models
+from demo_dex.types.fa12_token.tezos_parameters.transfer import TransferParameter
+from demo_dex.types.fa12_token.tezos_storage import Fa12TokenStorage
+from demo_dex.types.quipu_fa12.tezos_parameters.divest_liquidity import DivestLiquidityParameter
+from demo_dex.types.quipu_fa12.tezos_storage import QuipuFa12Storage
 from dipdup.context import HandlerContext
-from dipdup.models import OperationData
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa12_divest_liquidity(
     ctx: HandlerContext,
-    divest_liquidity: Transaction[DivestLiquidityParameter, QuipuFa12Storage],
-    transfer: Transaction[TransferParameter, Fa12TokenStorage],
-    transaction_1: OperationData,
+    divest_liquidity: TzktTransaction[DivestLiquidityParameter, QuipuFa12Storage],
+    transfer: TzktTransaction[TransferParameter, Fa12TokenStorage],
+    transaction_1: TzktOperationData,
 ) -> None:
     storage = divest_liquidity.storage
 
     decimals = int(ctx.template_values['decimals'])
     symbol = ctx.template_values['symbol']
     trader = divest_liquidity.data.sender_address
 
@@ -39,8 +39,8 @@
     price = tez_pool / token_pool
     share_px = (tez_qty + price * token_qty) / shares_qty
 
     position.realized_pl += shares_qty * (share_px - position.avg_share_px)
     position.shares_qty -= shares_qty
     assert position.shares_qty >= 0, divest_liquidity.data.hash
 
-    await position.save()
+    await position.save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_invest_liquidity.py.j2` & `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_invest_liquidity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from decimal import Decimal
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.fa12_token.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.fa12_token.storage import Fa12TokenStorage
-from {{cookiecutter.package}}.types.quipu_fa12.parameter.invest_liquidity import InvestLiquidityParameter
-from {{cookiecutter.package}}.types.quipu_fa12.storage import QuipuFa12Storage
+import demo_dex.models as models
+from demo_dex.types.fa2_token.tezos_parameters.transfer import TransferParameter
+from demo_dex.types.fa2_token.tezos_storage import Fa2TokenStorage
+from demo_dex.types.quipu_fa2.tezos_parameters.invest_liquidity import InvestLiquidityParameter
+from demo_dex.types.quipu_fa2.tezos_storage import QuipuFa2Storage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
-async def on_fa12_invest_liquidity(
+async def on_fa2_invest_liquidity(
     ctx: HandlerContext,
-    invest_liquidity: Transaction[InvestLiquidityParameter, QuipuFa12Storage],
-    transfer: Transaction[TransferParameter, Fa12TokenStorage],
+    invest_liquidity: TzktTransaction[InvestLiquidityParameter, QuipuFa2Storage],
+    transfer: TzktTransaction[TransferParameter, Fa2TokenStorage],
 ) -> None:
     storage = invest_liquidity.storage
 
     decimals = int(ctx.template_values['decimals'])
     symbol = ctx.template_values['symbol']
     trader = invest_liquidity.data.sender_address
 
     assert trader is not None
 
     position, _ = await models.Position.get_or_create(trader=trader, symbol=symbol)
 
     assert invest_liquidity.data.amount is not None
     tez_qty = Decimal(invest_liquidity.data.amount) / (10**6)
-    token_qty = Decimal(transfer.parameter.value) / (10**decimals)
+    token_qty = sum(Decimal(tx.amount) for tx in transfer.parameter.__root__[0].txs) / (10**decimals)
     new_shares_qty = int(storage.storage.ledger[trader].balance) + int(storage.storage.ledger[trader].frozen_balance)
 
     price = (Decimal(storage.storage.tez_pool) / (10**6)) / (Decimal(storage.storage.token_pool) / (10**decimals))
     value = tez_qty + price * token_qty
     share_px = value / (new_shares_qty - position.shares_qty)
     assert share_px > 0, invest_liquidity.data.hash
 
     position.avg_share_px = (position.shares_qty * position.avg_share_px + value) / new_shares_qty
     position.shares_qty = new_shares_qty
 
-    await position.save()
+    await position.save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_origination.py.j2` & `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_origination.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.quipu_fa12.storage import QuipuFa12Storage
+import demo_dex.models as models
+from demo_dex.types.quipu_fa12.tezos_storage import QuipuFa12Storage
 from dipdup.context import HandlerContext
-from dipdup.models import Origination
+from dipdup.models.tezos_tzkt import TzktOrigination
 
 
 async def on_fa12_origination(
     ctx: HandlerContext,
-    quipu_fa12_origination: Origination[QuipuFa12Storage],
+    quipu_fa12_origination: TzktOrigination[QuipuFa12Storage],
 ) -> None:
     symbol = ctx.template_values['symbol']
 
     for address, value in quipu_fa12_origination.storage.storage.ledger.items():
         shares_qty = value.balance
-        await models.Position(trader=address, symbol=symbol, shares_qty=shares_qty).save()
+        await models.Position(trader=address, symbol=symbol, shares_qty=shares_qty).save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_tez_to_token.py.j2` & `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_tez_to_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from decimal import Decimal
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.fa12_token.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.fa12_token.storage import Fa12TokenStorage
-from {{cookiecutter.package}}.types.quipu_fa12.parameter.tez_to_token_payment import TezToTokenPaymentParameter
-from {{cookiecutter.package}}.types.quipu_fa12.storage import QuipuFa12Storage
+import demo_dex.models as models
+from demo_dex.types.fa12_token.tezos_parameters.transfer import TransferParameter
+from demo_dex.types.fa12_token.tezos_storage import Fa12TokenStorage
+from demo_dex.types.quipu_fa12.tezos_parameters.tez_to_token_payment import TezToTokenPaymentParameter
+from demo_dex.types.quipu_fa12.tezos_storage import QuipuFa12Storage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa12_tez_to_token(
     ctx: HandlerContext,
-    tez_to_token_payment: Transaction[TezToTokenPaymentParameter, QuipuFa12Storage],
-    transfer: Transaction[TransferParameter, Fa12TokenStorage],
+    tez_to_token_payment: TzktTransaction[TezToTokenPaymentParameter, QuipuFa12Storage],
+    transfer: TzktTransaction[TransferParameter, Fa12TokenStorage],
 ) -> None:
     decimals = int(ctx.template_values['decimals'])
     symbol = ctx.template_values['symbol']
     trader = tez_to_token_payment.data.sender_address
 
     min_token_quantity = Decimal(tez_to_token_payment.parameter.min_out) / (10**decimals)
     token_quantity = Decimal(transfer.parameter.value) / (10**decimals)
@@ -30,8 +30,8 @@
         side=models.TradeSide.BUY,
         quantity=token_quantity,
         price=token_quantity / tez_quantity,
         slippage=(1 - (min_token_quantity / token_quantity)).quantize(Decimal('0.000001')),
         level=transfer.data.level,
         timestamp=transfer.data.timestamp,
     )
-    await trade.save()
+    await trade.save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_token_to_tez.py.j2` & `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa12_token_to_tez.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from decimal import Decimal
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.fa12_token.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.fa12_token.storage import Fa12TokenStorage
-from {{cookiecutter.package}}.types.quipu_fa12.parameter.token_to_tez_payment import TokenToTezPaymentParameter
-from {{cookiecutter.package}}.types.quipu_fa12.storage import QuipuFa12Storage
+import demo_dex.models as models
+from demo_dex.types.fa12_token.tezos_parameters.transfer import TransferParameter
+from demo_dex.types.fa12_token.tezos_storage import Fa12TokenStorage
+from demo_dex.types.quipu_fa12.tezos_parameters.token_to_tez_payment import TokenToTezPaymentParameter
+from demo_dex.types.quipu_fa12.tezos_storage import QuipuFa12Storage
 from dipdup.context import HandlerContext
-from dipdup.models import OperationData
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa12_token_to_tez(
     ctx: HandlerContext,
-    token_to_tez_payment: Transaction[TokenToTezPaymentParameter, QuipuFa12Storage],
-    transfer: Transaction[TransferParameter, Fa12TokenStorage],
-    transaction_0: OperationData,
+    token_to_tez_payment: TzktTransaction[TokenToTezPaymentParameter, QuipuFa12Storage],
+    transfer: TzktTransaction[TransferParameter, Fa12TokenStorage],
+    transaction_0: TzktOperationData,
 ) -> None:
     decimals = int(ctx.template_values['decimals'])
     symbol = ctx.template_values['symbol']
     trader = token_to_tez_payment.data.sender_address
 
     min_tez_quantity = Decimal(token_to_tez_payment.parameter.min_out) / (10**6)
     token_quantity = Decimal(token_to_tez_payment.parameter.amount) / (10**decimals)
@@ -32,8 +32,8 @@
         side=models.TradeSide.SELL,
         quantity=token_quantity,
         price=token_quantity / tez_quantity,
         slippage=(1 - (min_tez_quantity / tez_quantity)).quantize(Decimal('0.000001')),
         level=transfer.data.level,
         timestamp=transfer.data.timestamp,
     )
-    await trade.save()
+    await trade.save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_transfer.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_transfer.py.j2`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.quipu_fa12.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.quipu_fa12.storage import QuipuFa12Storage
+import {{project.package}}.models as models
+from {{project.package}}.types.quipu_fa12.tezos_parameters.transfer import TransferParameter
+from {{project.package}}.types.quipu_fa12.tezos_storage import QuipuFa12Storage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa12_transfer(
     ctx: HandlerContext,
-    transfer: Transaction[TransferParameter, QuipuFa12Storage],
+    transfer: TzktTransaction[TransferParameter, QuipuFa12Storage],
 ) -> None:
     symbol = ctx.template_values['symbol']
     from_address = transfer.parameter.from_
     to_address = transfer.parameter.to
     value = int(transfer.parameter.value)
 
     from_position, _ = await models.Position.get_or_create(trader=from_address, symbol=symbol)
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa12_withdraw_profit.py.j2` & `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_withdraw_profit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from decimal import Decimal
 from typing import Optional
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.quipu_fa12.parameter.withdraw_profit import WithdrawProfitParameter
-from {{cookiecutter.package}}.types.quipu_fa12.storage import QuipuFa12Storage
+import demo_dex.models as models
+from demo_dex.types.quipu_fa2.tezos_parameters.withdraw_profit import WithdrawProfitParameter
+from demo_dex.types.quipu_fa2.tezos_storage import QuipuFa2Storage
 from dipdup.context import HandlerContext
-from dipdup.models import OperationData
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
-async def on_fa12_withdraw_profit(
+async def on_fa2_withdraw_profit(
     ctx: HandlerContext,
-    withdraw_profit: Transaction[WithdrawProfitParameter, QuipuFa12Storage],
-    transaction_0: Optional[OperationData] = None,
+    withdraw_profit: TzktTransaction[WithdrawProfitParameter, QuipuFa2Storage],
+    transaction_0: Optional[TzktOperationData] = None,
 ) -> None:
     symbol = ctx.template_values['symbol']
     trader = withdraw_profit.data.sender_address
 
     position, _ = await models.Position.get_or_create(trader=trader, symbol=symbol)
+
     if transaction_0:
         assert transaction_0.amount is not None
         position.realized_pl += Decimal(transaction_0.amount) / (10**6)
 
-        await position.save()
+        await position.save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_divest_liquidity.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_divest_liquidity.py.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from decimal import Decimal
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.fa2_token.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.fa2_token.storage import Fa2TokenStorage
-from {{cookiecutter.package}}.types.quipu_fa2.parameter.divest_liquidity import DivestLiquidityParameter
-from {{cookiecutter.package}}.types.quipu_fa2.storage import QuipuFa2Storage
+import {{project.package}}.models as models
+from {{project.package}}.types.fa2_token.tezos_parameters.transfer import TransferParameter
+from {{project.package}}.types.fa2_token.tezos_storage import Fa2TokenStorage
+from {{project.package}}.types.quipu_fa2.tezos_parameters.divest_liquidity import DivestLiquidityParameter
+from {{project.package}}.types.quipu_fa2.tezos_storage import QuipuFa2Storage
 from dipdup.context import HandlerContext
-from dipdup.models import OperationData
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa2_divest_liquidity(
     ctx: HandlerContext,
-    divest_liquidity: Transaction[DivestLiquidityParameter, QuipuFa2Storage],
-    transfer: Transaction[TransferParameter, Fa2TokenStorage],
-    transaction_1: OperationData,
+    divest_liquidity: TzktTransaction[DivestLiquidityParameter, QuipuFa2Storage],
+    transfer: TzktTransaction[TransferParameter, Fa2TokenStorage],
+    transaction_1: TzktOperationData,
 ) -> None:
     storage = divest_liquidity.storage
 
     decimals = int(ctx.template_values['decimals'])
     symbol = ctx.template_values['symbol']
     trader = divest_liquidity.data.sender_address
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_invest_liquidity.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_invest_liquidity.py.j2`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from decimal import Decimal
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.fa2_token.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.fa2_token.storage import Fa2TokenStorage
-from {{cookiecutter.package}}.types.quipu_fa2.parameter.invest_liquidity import InvestLiquidityParameter
-from {{cookiecutter.package}}.types.quipu_fa2.storage import QuipuFa2Storage
+import {{project.package}}.models as models
+from {{project.package}}.types.fa2_token.tezos_parameters.transfer import TransferParameter
+from {{project.package}}.types.fa2_token.tezos_storage import Fa2TokenStorage
+from {{project.package}}.types.quipu_fa2.tezos_parameters.invest_liquidity import InvestLiquidityParameter
+from {{project.package}}.types.quipu_fa2.tezos_storage import QuipuFa2Storage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa2_invest_liquidity(
     ctx: HandlerContext,
-    invest_liquidity: Transaction[InvestLiquidityParameter, QuipuFa2Storage],
-    transfer: Transaction[TransferParameter, Fa2TokenStorage],
+    invest_liquidity: TzktTransaction[InvestLiquidityParameter, QuipuFa2Storage],
+    transfer: TzktTransaction[TransferParameter, Fa2TokenStorage],
 ) -> None:
     storage = invest_liquidity.storage
 
     decimals = int(ctx.template_values['decimals'])
     symbol = ctx.template_values['symbol']
     trader = invest_liquidity.data.sender_address
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_origination.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa12_origination.py.j2`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.quipu_fa2.storage import QuipuFa2Storage
+import {{project.package}}.models as models
+from {{project.package}}.types.quipu_fa12.tezos_storage import QuipuFa12Storage
 from dipdup.context import HandlerContext
-from dipdup.models import Origination
+from dipdup.models.tezos_tzkt import TzktOrigination
 
 
-async def on_fa2_origination(
+async def on_fa12_origination(
     ctx: HandlerContext,
-    quipu_fa2_origination: Origination[QuipuFa2Storage],
+    quipu_fa12_origination: TzktOrigination[QuipuFa12Storage],
 ) -> None:
     symbol = ctx.template_values['symbol']
 
-    for address, value in quipu_fa2_origination.storage.storage.ledger.items():
+    for address, value in quipu_fa12_origination.storage.storage.ledger.items():
         shares_qty = value.balance
         await models.Position(trader=address, symbol=symbol, shares_qty=shares_qty).save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_tez_to_token.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_tez_to_token.py.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from decimal import Decimal
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.fa2_token.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.fa2_token.storage import Fa2TokenStorage
-from {{cookiecutter.package}}.types.quipu_fa2.parameter.tez_to_token_payment import TezToTokenPaymentParameter
-from {{cookiecutter.package}}.types.quipu_fa2.storage import QuipuFa2Storage
+import {{project.package}}.models as models
+from {{project.package}}.types.fa2_token.tezos_parameters.transfer import TransferParameter
+from {{project.package}}.types.fa2_token.tezos_storage import Fa2TokenStorage
+from {{project.package}}.types.quipu_fa2.tezos_parameters.tez_to_token_payment import TezToTokenPaymentParameter
+from {{project.package}}.types.quipu_fa2.tezos_storage import QuipuFa2Storage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa2_tez_to_token(
     ctx: HandlerContext,
-    tez_to_token_payment: Transaction[TezToTokenPaymentParameter, QuipuFa2Storage],
-    transfer: Transaction[TransferParameter, Fa2TokenStorage],
+    tez_to_token_payment: TzktTransaction[TezToTokenPaymentParameter, QuipuFa2Storage],
+    transfer: TzktTransaction[TransferParameter, Fa2TokenStorage],
 ) -> None:
     decimals = int(ctx.template_values['decimals'])
     symbol = ctx.template_values['symbol']
     trader = tez_to_token_payment.data.sender_address
 
     min_token_quantity = Decimal(tez_to_token_payment.parameter.min_out) / (10**decimals)
     assert tez_to_token_payment.data.amount is not None
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_token_to_tez.py.j2` & `dipdup-7.0.0rc1/src/demo_dex/handlers/on_fa2_token_to_tez.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from decimal import Decimal
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.fa2_token.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.fa2_token.storage import Fa2TokenStorage
-from {{cookiecutter.package}}.types.quipu_fa2.parameter.token_to_tez_payment import TokenToTezPaymentParameter
-from {{cookiecutter.package}}.types.quipu_fa2.storage import QuipuFa2Storage
+import demo_dex.models as models
+from demo_dex.types.fa2_token.tezos_parameters.transfer import TransferParameter
+from demo_dex.types.fa2_token.tezos_storage import Fa2TokenStorage
+from demo_dex.types.quipu_fa2.tezos_parameters.token_to_tez_payment import TokenToTezPaymentParameter
+from demo_dex.types.quipu_fa2.tezos_storage import QuipuFa2Storage
 from dipdup.context import HandlerContext
-from dipdup.models import OperationData
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa2_token_to_tez(
     ctx: HandlerContext,
-    token_to_tez_payment: Transaction[TokenToTezPaymentParameter, QuipuFa2Storage],
-    transfer: Transaction[TransferParameter, Fa2TokenStorage],
-    transaction_0: OperationData,
+    token_to_tez_payment: TzktTransaction[TokenToTezPaymentParameter, QuipuFa2Storage],
+    transfer: TzktTransaction[TransferParameter, Fa2TokenStorage],
+    transaction_0: TzktOperationData,
 ) -> None:
     decimals = int(ctx.template_values['decimals'])
     symbol = ctx.template_values['symbol']
     trader = token_to_tez_payment.data.sender_address
 
     min_tez_quantity = Decimal(token_to_tez_payment.parameter.min_out) / (10**decimals)
     token_quantity = Decimal(token_to_tez_payment.parameter.amount) / (10**decimals)
@@ -32,8 +32,8 @@
         side=models.TradeSide.SELL,
         quantity=token_quantity,
         price=token_quantity / tez_quantity,
         slippage=1 - (min_tez_quantity / tez_quantity),
         level=transfer.data.level,
         timestamp=transfer.data.timestamp,
     )
-    await trade.save()
+    await trade.save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_transfer.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_transfer.py.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.quipu_fa2.parameter.transfer import TransferParameter
-from {{cookiecutter.package}}.types.quipu_fa2.storage import QuipuFa2Storage
+import {{project.package}}.models as models
+from {{project.package}}.types.quipu_fa2.tezos_parameters.transfer import TransferParameter
+from {{project.package}}.types.quipu_fa2.tezos_storage import QuipuFa2Storage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa2_transfer(
     ctx: HandlerContext,
-    transfer: Transaction[TransferParameter, QuipuFa2Storage],
+    transfer: TzktTransaction[TransferParameter, QuipuFa2Storage],
 ) -> None:
     transfer_parameter = transfer.parameter.__root__[0]
 
     symbol = ctx.template_values['symbol']
     from_address = transfer_parameter.from_
     from_position, _ = await models.Position.get_or_create(trader=from_address, symbol=symbol)
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/handlers/on_fa2_withdraw_profit.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_dex/handlers/on_fa2_withdraw_profit.py.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from decimal import Decimal
 from typing import Optional
 
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.quipu_fa2.parameter.withdraw_profit import WithdrawProfitParameter
-from {{cookiecutter.package}}.types.quipu_fa2.storage import QuipuFa2Storage
+import {{project.package}}.models as models
+from {{project.package}}.types.quipu_fa2.tezos_parameters.withdraw_profit import WithdrawProfitParameter
+from {{project.package}}.types.quipu_fa2.tezos_storage import QuipuFa2Storage
 from dipdup.context import HandlerContext
-from dipdup.models import OperationData
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktOperationData
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_fa2_withdraw_profit(
     ctx: HandlerContext,
-    withdraw_profit: Transaction[WithdrawProfitParameter, QuipuFa2Storage],
-    transaction_0: Optional[OperationData] = None,
+    withdraw_profit: TzktTransaction[WithdrawProfitParameter, QuipuFa2Storage],
+    transaction_0: Optional[TzktOperationData] = None,
 ) -> None:
     symbol = ctx.template_values['symbol']
     trader = withdraw_profit.data.sender_address
 
     position, _ = await models.Position.get_or_create(trader=trader, symbol=symbol)
 
     if transaction_0:
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_dex/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-7.0.0rc1/src/demo_dex/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from enum import IntEnum
 
-from tortoise import fields
-
+from dipdup import fields
 from dipdup.models import Model
 
 
 class TradeSide(IntEnum):
     BUY = 1
     SELL = 0
 
 
 class Trade(Model):
     id = fields.IntField(pk=True)
-    symbol = fields.CharField(max_length=5)
-    trader = fields.CharField(36)
+    symbol = fields.TextField()
+    trader = fields.TextField()
     side = fields.IntEnumField(enum_type=TradeSide)
     quantity = fields.DecimalField(decimal_places=6, max_digits=20)
     price = fields.DecimalField(decimal_places=6, max_digits=20)
     slippage = fields.DecimalField(decimal_places=6, max_digits=20)
     level = fields.BigIntField()
     timestamp = fields.DatetimeField()
 
 
 class Position(Model):
     id = fields.IntField(pk=True)
-    symbol = fields.CharField(max_length=5)
-    trader = fields.CharField(36)
+    symbol = fields.TextField()
+    trader = fields.TextField()
     shares_qty = fields.BigIntField(default=0)
     avg_share_px = fields.DecimalField(decimal_places=6, max_digits=20, default=0)
-    realized_pl = fields.DecimalField(decimal_places=6, max_digits=20, default=0)
+    realized_pl = fields.DecimalField(decimal_places=6, max_digits=20, default=0)
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_domains/dipdup.yml.j2` & `dipdup-7.0.0rc1/src/demo_domains/dipdup.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 312e  spec_version: 1.
-00000010: 320a 7061 636b 6167 653a 207b 7b20 636f  2.package: {{ co
-00000020: 6f6b 6965 6375 7474 6572 2e70 6163 6b61  okiecutter.packa
-00000030: 6765 207d 7d0a 0a64 6174 6162 6173 653a  ge }}..database:
-00000040: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000050: 2020 7061 7468 3a20 7b7b 2063 6f6f 6b69    path: {{ cooki
-00000060: 6563 7574 7465 722e 7072 6f6a 6563 745f  ecutter.project_
-00000070: 6e61 6d65 207d 7d2e 7371 6c69 7465 330a  name }}.sqlite3.
-00000080: 0a63 6f6e 7472 6163 7473 3a0a 2020 6d61  .contracts:.  ma
-00000090: 696e 6e65 745f 6e61 6d65 5f72 6567 6973  innet_name_regis
-000000a0: 7472 793a 0a20 2020 2061 6464 7265 7373  try:.    address
-000000b0: 3a20 4b54 3147 425a 6d53 786d 6e4b 4a58  : KT1GBZmSxmnKJX
-000000c0: 474d 644d 4c62 7567 5066 4c79 5550 6d75  GMdMLbugPfLyUPmu
-000000d0: 4c53 4d77 4b53 0a20 2020 2074 7970 656e  LSMwKS.    typen
-000000e0: 616d 653a 206e 616d 655f 7265 6769 7374  ame: name_regist
-000000f0: 7279 0a0a 6461 7461 736f 7572 6365 733a  ry..datasources:
-00000100: 0a20 2074 7a6b 745f 6d61 696e 6e65 743a  .  tzkt_mainnet:
-00000110: 0a20 2020 206b 696e 643a 2074 7a6b 740a  .    kind: tzkt.
-00000120: 2020 2020 7572 6c3a 2024 7b54 5a4b 545f      url: ${TZKT_
-00000130: 5552 4c3a 2d68 7474 7073 3a2f 2f61 7069  URL:-https://api
-00000140: 2e74 7a6b 742e 696f 7d0a 0a74 656d 706c  .tzkt.io}..templ
-00000150: 6174 6573 3a0a 2020 646f 6d61 696e 733a  ates:.  domains:
-00000160: 0a20 2020 206b 696e 643a 206f 7065 7261  .    kind: opera
-00000170: 7469 6f6e 0a20 2020 2064 6174 6173 6f75  tion.    datasou
-00000180: 7263 653a 203c 6461 7461 736f 7572 6365  rce: <datasource
-00000190: 3e0a 2020 2020 636f 6e74 7261 6374 733a  >.    contracts:
-000001a0: 0a20 2020 2020 202d 203c 6e61 6d65 5f72  .      - <name_r
-000001b0: 6567 6973 7472 793e 0a20 2020 2068 616e  egistry>.    han
-000001c0: 646c 6572 733a 0a20 2020 2020 202d 2063  dlers:.      - c
-000001d0: 616c 6c62 6163 6b3a 206f 6e5f 6164 6d69  allback: on_admi
-000001e0: 6e5f 7570 6461 7465 0a20 2020 2020 2020  n_update.       
-000001f0: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
-00000200: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
-00000210: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
-00000220: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
-00000230: 203c 6e61 6d65 5f72 6567 6973 7472 793e   <name_registry>
-00000240: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
-00000250: 7279 706f 696e 743a 2061 646d 696e 5f75  rypoint: admin_u
-00000260: 7064 6174 650a 2020 2020 2020 2d20 6361  pdate.      - ca
-00000270: 6c6c 6261 636b 3a20 6f6e 5f65 7865 6375  llback: on_execu
-00000280: 7465 0a20 2020 2020 2020 2070 6174 7465  te.        patte
-00000290: 726e 3a0a 2020 2020 2020 2020 2020 2d20  rn:.          - 
-000002a0: 7479 7065 3a20 7472 616e 7361 6374 696f  type: transactio
-000002b0: 6e0a 2020 2020 2020 2020 2020 2020 6465  n.            de
-000002c0: 7374 696e 6174 696f 6e3a 203c 6e61 6d65  stination: <name
-000002d0: 5f72 6567 6973 7472 793e 0a20 2020 2020  _registry>.     
-000002e0: 2020 2020 2020 2065 6e74 7279 706f 696e         entrypoin
-000002f0: 743a 2065 7865 6375 7465 0a0a 696e 6465  t: execute..inde
-00000300: 7865 733a 0a20 2064 6f6d 6169 6e73 5f6d  xes:.  domains_m
-00000310: 6169 6e6e 6574 3a0a 2020 2020 7465 6d70  ainnet:.    temp
-00000320: 6c61 7465 3a20 646f 6d61 696e 730a 2020  late: domains.  
-00000330: 2020 7661 6c75 6573 3a0a 2020 2020 2020    values:.      
-00000340: 6461 7461 736f 7572 6365 3a20 747a 6b74  datasource: tzkt
-00000350: 5f6d 6169 6e6e 6574 0a20 2020 2020 206e  _mainnet.      n
-00000360: 616d 655f 7265 6769 7374 7279 3a20 6d61  ame_registry: ma
-00000370: 696e 6e65 745f 6e61 6d65 5f72 6567 6973  innet_name_regis
-00000380: 7472 790a                                try.
+00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
+00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
+00000020: 646f 6d61 696e 730a 0a64 6174 6162 6173  domains..databas
+00000030: 653a 0a20 206b 696e 643a 2073 716c 6974  e:.  kind: sqlit
+00000040: 650a 2020 7061 7468 3a20 6465 6d6f 5f64  e.  path: demo_d
+00000050: 6f6d 6169 6e73 2e73 716c 6974 6533 0a0a  omains.sqlite3..
+00000060: 636f 6e74 7261 6374 733a 0a20 206d 6169  contracts:.  mai
+00000070: 6e6e 6574 5f6e 616d 655f 7265 6769 7374  nnet_name_regist
+00000080: 7279 3a0a 2020 2020 6b69 6e64 3a20 7465  ry:.    kind: te
+00000090: 7a6f 730a 2020 2020 6164 6472 6573 733a  zos.    address:
+000000a0: 204b 5431 4742 5a6d 5378 6d6e 4b4a 5847   KT1GBZmSxmnKJXG
+000000b0: 4d64 4d4c 6275 6750 664c 7955 506d 754c  MdMLbugPfLyUPmuL
+000000c0: 534d 774b 530a 2020 2020 7479 7065 6e61  SMwKS.    typena
+000000d0: 6d65 3a20 6e61 6d65 5f72 6567 6973 7472  me: name_registr
+000000e0: 790a 0a64 6174 6173 6f75 7263 6573 3a0a  y..datasources:.
+000000f0: 2020 747a 6b74 5f6d 6169 6e6e 6574 3a0a    tzkt_mainnet:.
+00000100: 2020 2020 6b69 6e64 3a20 7465 7a6f 732e      kind: tezos.
+00000110: 747a 6b74 0a20 2020 2075 726c 3a20 247b  tzkt.    url: ${
+00000120: 545a 4b54 5f55 524c 3a2d 6874 7470 733a  TZKT_URL:-https:
+00000130: 2f2f 6170 692e 747a 6b74 2e69 6f7d 0a0a  //api.tzkt.io}..
+00000140: 7465 6d70 6c61 7465 733a 0a20 2064 6f6d  templates:.  dom
+00000150: 6169 6e73 3a0a 2020 2020 6b69 6e64 3a20  ains:.    kind: 
+00000160: 7465 7a6f 732e 747a 6b74 2e6f 7065 7261  tezos.tzkt.opera
+00000170: 7469 6f6e 730a 2020 2020 6461 7461 736f  tions.    dataso
+00000180: 7572 6365 3a20 3c64 6174 6173 6f75 7263  urce: <datasourc
+00000190: 653e 0a20 2020 2063 6f6e 7472 6163 7473  e>.    contracts
+000001a0: 3a0a 2020 2020 2020 2d20 3c6e 616d 655f  :.      - <name_
+000001b0: 7265 6769 7374 7279 3e0a 2020 2020 6861  registry>.    ha
+000001c0: 6e64 6c65 7273 3a0a 2020 2020 2020 2d20  ndlers:.      - 
+000001d0: 6361 6c6c 6261 636b 3a20 6f6e 5f61 646d  callback: on_adm
+000001e0: 696e 5f75 7064 6174 650a 2020 2020 2020  in_update.      
+000001f0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
+00000200: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+00000210: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+00000220: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+00000230: 3a20 3c6e 616d 655f 7265 6769 7374 7279  : <name_registry
+00000240: 3e0a 2020 2020 2020 2020 2020 2020 656e  >.            en
+00000250: 7472 7970 6f69 6e74 3a20 6164 6d69 6e5f  trypoint: admin_
+00000260: 7570 6461 7465 0a20 2020 2020 202d 2063  update.      - c
+00000270: 616c 6c62 6163 6b3a 206f 6e5f 6578 6563  allback: on_exec
+00000280: 7574 650a 2020 2020 2020 2020 7061 7474  ute.        patt
+00000290: 6572 6e3a 0a20 2020 2020 2020 2020 202d  ern:.          -
+000002a0: 2074 7970 653a 2074 7261 6e73 6163 7469   type: transacti
+000002b0: 6f6e 0a20 2020 2020 2020 2020 2020 2064  on.            d
+000002c0: 6573 7469 6e61 7469 6f6e 3a20 3c6e 616d  estination: <nam
+000002d0: 655f 7265 6769 7374 7279 3e0a 2020 2020  e_registry>.    
+000002e0: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+000002f0: 6e74 3a20 6578 6563 7574 650a 0a69 6e64  nt: execute..ind
+00000300: 6578 6573 3a0a 2020 646f 6d61 696e 735f  exes:.  domains_
+00000310: 6d61 696e 6e65 743a 0a20 2020 2074 656d  mainnet:.    tem
+00000320: 706c 6174 653a 2064 6f6d 6169 6e73 0a20  plate: domains. 
+00000330: 2020 2076 616c 7565 733a 0a20 2020 2020     values:.     
+00000340: 2064 6174 6173 6f75 7263 653a 2074 7a6b   datasource: tzk
+00000350: 745f 6d61 696e 6e65 740a 2020 2020 2020  t_mainnet.      
+00000360: 6e61 6d65 5f72 6567 6973 7472 793a 206d  name_registry: m
+00000370: 6169 6e6e 6574 5f6e 616d 655f 7265 6769  ainnet_name_regi
+00000380: 7374 7279                                stry
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_admin_update.py.j2` & `dipdup-7.0.0rc1/src/demo_domains/handlers/on_admin_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from {{ cookiecutter.package }}.handlers.on_storage_diff import on_storage_diff
-from {{ cookiecutter.package }}.types.name_registry.parameter.admin_update import AdminUpdateParameter
-from {{ cookiecutter.package }}.types.name_registry.storage import NameRegistryStorage
+from demo_domains.handlers.on_storage_diff import on_storage_diff
+from demo_domains.types.name_registry.tezos_parameters.admin_update import AdminUpdateParameter
+from demo_domains.types.name_registry.tezos_storage import NameRegistryStorage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_admin_update(
     ctx: HandlerContext,
-    admin_update: Transaction[AdminUpdateParameter, NameRegistryStorage],
+    admin_update: TzktTransaction[AdminUpdateParameter, NameRegistryStorage],
 ) -> None:
     storage = admin_update.storage
-    await on_storage_diff(ctx, storage)
+    await on_storage_diff(ctx, storage)
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_execute.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_admin_update.py.j2`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from {{ cookiecutter.package }}.handlers.on_storage_diff import on_storage_diff
-from {{ cookiecutter.package }}.types.name_registry.parameter.execute import ExecuteParameter
-from {{ cookiecutter.package }}.types.name_registry.storage import NameRegistryStorage
+from {{ project.package }}.handlers.on_storage_diff import on_storage_diff
+from {{ project.package }}.types.name_registry.tezos_parameters.admin_update import AdminUpdateParameter
+from {{ project.package }}.types.name_registry.tezos_storage import NameRegistryStorage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
-async def on_execute(
+async def on_admin_update(
     ctx: HandlerContext,
-    execute: Transaction[ExecuteParameter, NameRegistryStorage],
+    admin_update: TzktTransaction[AdminUpdateParameter, NameRegistryStorage],
 ) -> None:
-    storage = execute.storage
+    storage = admin_update.storage
     await on_storage_diff(ctx, storage)
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/handlers/on_storage_diff.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_domains/handlers/on_storage_diff.py.j2`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import {{ cookiecutter.package }}.models as models
-from {{ cookiecutter.package }}.types.name_registry.storage import NameRegistryStorage
+import {{ project.package }}.models as models
+from {{ project.package }}.types.name_registry.tezos_storage import NameRegistryStorage
 from dipdup.context import HandlerContext
 
 
 async def on_storage_diff(ctx: HandlerContext, storage: NameRegistryStorage) -> None:
     for name, item in storage.store.records.items():
         record_name = bytes.fromhex(name).decode()
         record_path = record_name.split('.')
         ctx.logger.info('Processing `%s`', record_name)
 
         if len(record_path) != int(item.level):
-            ctx.logger.error('Invalid record `%s`: expected %s chunks, got %s', record_name, item.level, len(record_path))
+            ctx.logger.error('`%s`: expected %s chunks, got %s', record_name, item.level, len(record_path))
             return
 
-        if item.level == "1":
+        if item.level == '1':
             await models.TLD.update_or_create(id=record_name, defaults={'owner': item.owner})
         else:
-            if item.level == "2":
+            if item.level == '2':
                 await models.Domain.update_or_create(
                     id=record_name,
                     defaults={
                         'tld_id': record_path[-1],
                         'owner': item.owner,
                         'expiry': storage.store.expiry_map.get(item.expiry_key) if item.expiry_key else None,
                         'token_id': int(item.tzip12_token_id) if item.tzip12_token_id else None,
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_domains/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_big_maps/models/__init__.py.j2`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Optional
 
-from tortoise.fields.relational import ForeignKeyFieldInstance
-from tortoise import fields
+from dipdup import fields
 
 from dipdup.models import Model
 
 
 class TLD(Model):
-    id = fields.CharField(max_length=255, pk=True)
-    owner = fields.CharField(max_length=36)
+    id = fields.TextField(pk=True)
+    owner = fields.TextField()
+
+
+class Expiry(Model):
+    id = fields.TextField(pk=True)
+    timestamp = fields.DatetimeField(null=True)
 
 
 class Domain(Model):
-    id = fields.CharField(max_length=255, pk=True)
-    tld: ForeignKeyFieldInstance[TLD] = fields.ForeignKeyField('models.TLD', 'domains')
-    expiry = fields.DatetimeField(null=True)
-    owner = fields.CharField(max_length=36)
+    id = fields.TextField(pk=True)
+    tld: fields.ForeignKeyField[TLD] = fields.ForeignKeyField('models.TLD', 'domains')
+    owner = fields.TextField()
     token_id = fields.BigIntField(null=True)
 
-    tld_id: Optional[str]
-
 
 class Record(Model):
-    id = fields.CharField(max_length=255, pk=True)
-    domain: ForeignKeyFieldInstance[Domain] = fields.ForeignKeyField('models.Domain', 'records')
-    address = fields.CharField(max_length=36, null=True)
+    id = fields.TextField(pk=True)
+    domain: fields.ForeignKeyField[Domain] = fields.ForeignKeyField('models.Domain', 'records')
+    address = fields.TextField(null=True)
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_events/dipdup.yml.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_events/dipdup.yaml.j2`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 312e  spec_version: 1.
-00000010: 320a 7061 636b 6167 653a 207b 7b20 636f  2.package: {{ co
-00000020: 6f6b 6965 6375 7474 6572 2e70 6163 6b61  okiecutter.packa
-00000030: 6765 207d 7d0a 0a64 6174 6162 6173 653a  ge }}..database:
-00000040: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000050: 2020 7061 7468 3a20 7b7b 2063 6f6f 6b69    path: {{ cooki
-00000060: 6563 7574 7465 722e 7072 6f6a 6563 745f  ecutter.project_
-00000070: 6e61 6d65 207d 7d2e 7371 6c69 7465 330a  name }}.sqlite3.
-00000080: 0a64 6174 6173 6f75 7263 6573 3a0a 2020  .datasources:.  
-00000090: 747a 6b74 3a0a 2020 2020 6b69 6e64 3a20  tzkt:.    kind: 
-000000a0: 747a 6b74 0a20 2020 2075 726c 3a20 6874  tzkt.    url: ht
-000000b0: 7470 733a 2f2f 6170 692e 6768 6f73 746e  tps://api.ghostn
-000000c0: 6574 2e74 7a6b 742e 696f 0a0a 636f 6e74  et.tzkt.io..cont
-000000d0: 7261 6374 733a 0a20 2065 7665 6e74 735f  racts:.  events_
-000000e0: 636f 6e74 7261 6374 3a0a 2020 2020 636f  contract:.    co
-000000f0: 6465 5f68 6173 683a 204b 5431 5570 3641  de_hash: KT1Up6A
-00000100: 4d65 687a 6532 5654 6474 3377 3835 7861  Mehze2VTdt3w85xa
-00000110: 5a50 7472 4557 6e31 4165 7952 330a 0a69  ZPtrEWn1AeyR3..i
-00000120: 6e64 6578 6573 3a0a 2020 6576 656e 7473  ndexes:.  events
-00000130: 3a0a 2020 2020 6b69 6e64 3a20 6576 656e  :.    kind: even
-00000140: 740a 2020 2020 6461 7461 736f 7572 6365  t.    datasource
-00000150: 3a20 747a 6b74 0a20 2020 2068 616e 646c  : tzkt.    handl
-00000160: 6572 733a 0a20 2020 2020 202d 2063 616c  ers:.      - cal
-00000170: 6c62 6163 6b3a 206f 6e5f 6d6f 7665 5f65  lback: on_move_e
-00000180: 7665 6e74 0a20 2020 2020 2020 2063 6f6e  vent.        con
-00000190: 7472 6163 743a 2065 7665 6e74 735f 636f  tract: events_co
-000001a0: 6e74 7261 6374 0a20 2020 2020 2020 2074  ntract.        t
-000001b0: 6167 3a20 6d6f 7665 0a20 2020 2020 202d  ag: move.      -
-000001c0: 2063 616c 6c62 6163 6b3a 206f 6e5f 726f   callback: on_ro
-000001d0: 6c6c 5f65 7665 6e74 0a20 2020 2020 2020  ll_event.       
-000001e0: 2063 6f6e 7472 6163 743a 2065 7665 6e74   contract: event
-000001f0: 735f 636f 6e74 7261 6374 0a20 2020 2020  s_contract.     
-00000200: 2020 2074 6167 3a20 726f 6c6c 0a20 2020     tag: roll.   
-00000210: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
-00000220: 6e5f 6f74 6865 725f 6576 656e 740a 2020  n_other_event.  
-00000230: 2020 2020 2020 636f 6e74 7261 6374 3a20        contract: 
-00000240: 6576 656e 7473 5f63 6f6e 7472 6163 740a  events_contract.
+00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
+00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
+00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
+00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
+00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
+00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
+00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
+00000070: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
+00000080: 2074 7a6b 743a 0a20 2020 206b 696e 643a   tzkt:.    kind:
+00000090: 2074 657a 6f73 2e74 7a6b 740a 2020 2020   tezos.tzkt.    
+000000a0: 7572 6c3a 2068 7474 7073 3a2f 2f61 7069  url: https://api
+000000b0: 2e67 686f 7374 6e65 742e 747a 6b74 2e69  .ghostnet.tzkt.i
+000000c0: 6f0a 0a63 6f6e 7472 6163 7473 3a0a 2020  o..contracts:.  
+000000d0: 6576 656e 7473 5f63 6f6e 7472 6163 743a  events_contract:
+000000e0: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+000000f0: 0a20 2020 2063 6f64 655f 6861 7368 3a20  .    code_hash: 
+00000100: 4b54 3155 7036 414d 6568 7a65 3256 5464  KT1Up6AMehze2VTd
+00000110: 7433 7738 3578 615a 5074 7245 576e 3141  t3w85xaZPtrEWn1A
+00000120: 6579 5233 0a0a 696e 6465 7865 733a 0a20  eyR3..indexes:. 
+00000130: 2065 7665 6e74 733a 0a20 2020 206b 696e   events:.    kin
+00000140: 643a 2074 657a 6f73 2e74 7a6b 742e 6576  d: tezos.tzkt.ev
+00000150: 656e 7473 0a20 2020 2064 6174 6173 6f75  ents.    datasou
+00000160: 7263 653a 2074 7a6b 740a 2020 2020 6861  rce: tzkt.    ha
+00000170: 6e64 6c65 7273 3a0a 2020 2020 2020 2d20  ndlers:.      - 
+00000180: 6361 6c6c 6261 636b 3a20 6f6e 5f6d 6f76  callback: on_mov
+00000190: 655f 6576 656e 740a 2020 2020 2020 2020  e_event.        
+000001a0: 636f 6e74 7261 6374 3a20 6576 656e 7473  contract: events
+000001b0: 5f63 6f6e 7472 6163 740a 2020 2020 2020  _contract.      
+000001c0: 2020 7461 673a 206d 6f76 650a 2020 2020    tag: move.    
+000001d0: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
+000001e0: 5f72 6f6c 6c5f 6576 656e 740a 2020 2020  _roll_event.    
+000001f0: 2020 2020 636f 6e74 7261 6374 3a20 6576      contract: ev
+00000200: 656e 7473 5f63 6f6e 7472 6163 740a 2020  ents_contract.  
+00000210: 2020 2020 2020 7461 673a 2072 6f6c 6c0a        tag: roll.
+00000220: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+00000230: 3a20 6f6e 5f6f 7468 6572 5f65 7665 6e74  : on_other_event
+00000240: 0a20 2020 2020 2020 2063 6f6e 7472 6163  .        contrac
+00000250: 743a 2065 7665 6e74 735f 636f 6e74 7261  t: events_contra
+00000260: 6374 0a                                  ct.
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_factories/dipdup.yml.j2` & `dipdup-7.0.0rc1/tests/configs/demo_domains.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,59 @@
-00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 312e  spec_version: 1.
-00000010: 320a 7061 636b 6167 653a 207b 7b20 636f  2.package: {{ co
-00000020: 6f6b 6965 6375 7474 6572 2e70 6163 6b61  okiecutter.packa
-00000030: 6765 207d 7d0a 0a64 6174 6162 6173 653a  ge }}..database:
-00000040: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000050: 2020 7061 7468 3a20 7b7b 2063 6f6f 6b69    path: {{ cooki
-00000060: 6563 7574 7465 722e 7072 6f6a 6563 745f  ecutter.project_
-00000070: 6e61 6d65 207d 7d2e 7371 6c69 7465 330a  name }}.sqlite3.
-00000080: 0a63 6f6e 7472 6163 7473 3a0a 2020 7265  .contracts:.  re
-00000090: 6769 7374 7279 3a0a 2020 2020 6164 6472  gistry:.    addr
-000000a0: 6573 733a 204b 5431 3943 4633 4b4b 7276  ess: KT19CF3KKrv
-000000b0: 6457 3737 7474 466f 6d43 7569 6e32 6b34  dW77ttFomCuin2k4
-000000c0: 7541 566b 7279 5971 680a 2020 2020 7479  uAVkryYqh.    ty
-000000d0: 7065 6e61 6d65 3a20 7265 6769 7374 7279  pename: registry
-000000e0: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
-000000f0: 2074 7a6b 743a 0a20 2020 206b 696e 643a   tzkt:.    kind:
-00000100: 2074 7a6b 740a 2020 2020 7572 6c3a 2024   tzkt.    url: $
-00000110: 7b54 5a4b 545f 5552 4c3a 2d68 7474 7073  {TZKT_URL:-https
-00000120: 3a2f 2f61 7069 2e74 7a6b 742e 696f 7d0a  ://api.tzkt.io}.
-00000130: 0a74 656d 706c 6174 6573 3a0a 2020 7265  .templates:.  re
-00000140: 6769 7374 7279 5f64 616f 3a0a 2020 2020  gistry_dao:.    
-00000150: 6b69 6e64 3a20 6f70 6572 6174 696f 6e0a  kind: operation.
-00000160: 2020 2020 6461 7461 736f 7572 6365 3a20      datasource: 
-00000170: 747a 6b74 0a20 2020 2074 7970 6573 3a0a  tzkt.    types:.
-00000180: 2020 2020 2020 2d20 7472 616e 7361 6374        - transact
-00000190: 696f 6e0a 2020 2020 2020 2d20 6f72 6967  ion.      - orig
-000001a0: 696e 6174 696f 6e0a 2020 2020 636f 6e74  ination.    cont
-000001b0: 7261 6374 733a 0a20 2020 2020 202d 203c  racts:.      - <
-000001c0: 636f 6e74 7261 6374 3e0a 2020 2020 6861  contract>.    ha
-000001d0: 6e64 6c65 7273 3a0a 2020 2020 2020 2d20  ndlers:.      - 
-000001e0: 6361 6c6c 6261 636b 3a20 6f6e 5f6f 7269  callback: on_ori
-000001f0: 6769 6e61 7469 6f6e 0a20 2020 2020 2020  gination.       
-00000200: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
-00000210: 2020 2020 2d20 7479 7065 3a20 6f72 6967      - type: orig
-00000220: 696e 6174 696f 6e0a 2020 2020 2020 2020  ination.        
-00000230: 2020 2020 6f72 6967 696e 6174 6564 5f63      originated_c
-00000240: 6f6e 7472 6163 743a 203c 636f 6e74 7261  ontract: <contra
-00000250: 6374 3e0a 2020 2020 2020 2d20 6361 6c6c  ct>.      - call
-00000260: 6261 636b 3a20 6f6e 5f70 726f 706f 7365  back: on_propose
-00000270: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00000280: 3a0a 2020 2020 2020 2020 2020 2d20 7479  :.          - ty
-00000290: 7065 3a20 7472 616e 7361 6374 696f 6e0a  pe: transaction.
-000002a0: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-000002b0: 696e 6174 696f 6e3a 203c 636f 6e74 7261  ination: <contra
-000002c0: 6374 3e0a 2020 2020 2020 2020 2020 2020  ct>.            
-000002d0: 656e 7472 7970 6f69 6e74 3a20 7072 6f70  entrypoint: prop
-000002e0: 6f73 650a 0a69 6e64 6578 6573 3a0a 2020  ose..indexes:.  
-000002f0: 6661 6374 6f72 793a 0a20 2020 206b 696e  factory:.    kin
-00000300: 643a 206f 7065 7261 7469 6f6e 0a20 2020  d: operation.   
-00000310: 2064 6174 6173 6f75 7263 653a 2074 7a6b   datasource: tzk
-00000320: 740a 2020 2020 7479 7065 733a 0a20 2020  t.    types:.   
-00000330: 2020 202d 206f 7269 6769 6e61 7469 6f6e     - origination
-00000340: 0a20 2020 2068 616e 646c 6572 733a 0a20  .    handlers:. 
-00000350: 2020 2020 2020 202d 2063 616c 6c62 6163         - callbac
-00000360: 6b3a 206f 6e5f 6661 6374 6f72 795f 6f72  k: on_factory_or
-00000370: 6967 696e 6174 696f 6e0a 2020 2020 2020  igination.      
-00000380: 2020 2020 7061 7474 6572 6e3a 0a20 2020      pattern:.   
-00000390: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
-000003a0: 206f 7269 6769 6e61 7469 6f6e 0a20 2020   origination.   
-000003b0: 2020 2020 2020 2020 2020 2073 696d 696c             simil
-000003c0: 6172 5f74 6f3a 2072 6567 6973 7472 790a  ar_to: registry.
+00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
+00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
+00000020: 646f 6d61 696e 730a 0a64 6174 6162 6173  domains..databas
+00000030: 653a 0a20 206b 696e 643a 2073 716c 6974  e:.  kind: sqlit
+00000040: 650a 2020 7061 7468 3a20 6462 2e73 716c  e.  path: db.sql
+00000050: 6974 6533 0a0a 636f 6e74 7261 6374 733a  ite3..contracts:
+00000060: 0a20 206e 616d 655f 7265 6769 7374 7279  .  name_registry
+00000070: 3a0a 2020 2020 6b69 6e64 3a20 7465 7a6f  :.    kind: tezo
+00000080: 730a 2020 2020 6164 6472 6573 733a 204b  s.    address: K
+00000090: 5431 4742 5a6d 5378 6d6e 4b4a 5847 4d64  T1GBZmSxmnKJXGMd
+000000a0: 4d4c 6275 6750 664c 7955 506d 754c 534d  MLbugPfLyUPmuLSM
+000000b0: 774b 530a 2020 2020 7479 7065 6e61 6d65  wKS.    typename
+000000c0: 3a20 6e61 6d65 5f72 6567 6973 7472 790a  : name_registry.
+000000d0: 0a64 6174 6173 6f75 7263 6573 3a0a 2020  .datasources:.  
+000000e0: 747a 6b74 3a0a 2020 2020 6b69 6e64 3a20  tzkt:.    kind: 
+000000f0: 7465 7a6f 732e 747a 6b74 0a20 2020 2075  tezos.tzkt.    u
+00000100: 726c 3a20 247b 545a 4b54 5f55 524c 3a2d  rl: ${TZKT_URL:-
+00000110: 6874 7470 733a 2f2f 6170 692e 747a 6b74  https://api.tzkt
+00000120: 2e69 6f7d 0a20 2020 2068 7474 703a 0a20  .io}.    http:. 
+00000130: 2020 2020 2072 6570 6c61 795f 7061 7468       replay_path
+00000140: 3a20 247b 4449 5044 5550 5f52 4550 4c41  : ${DIPDUP_REPLA
+00000150: 595f 5041 5448 3a2d 7d0a 0a74 656d 706c  Y_PATH:-}..templ
+00000160: 6174 6573 3a0a 2020 646f 6d61 696e 733a  ates:.  domains:
+00000170: 0a20 2020 206b 696e 643a 2074 657a 6f73  .    kind: tezos
+00000180: 2e74 7a6b 742e 6f70 6572 6174 696f 6e73  .tzkt.operations
+00000190: 0a20 2020 2064 6174 6173 6f75 7263 653a  .    datasource:
+000001a0: 203c 6461 7461 736f 7572 6365 3e0a 2020   <datasource>.  
+000001b0: 2020 636f 6e74 7261 6374 733a 0a20 2020    contracts:.   
+000001c0: 2020 202d 203c 6e61 6d65 5f72 6567 6973     - <name_regis
+000001d0: 7472 793e 0a20 2020 2068 616e 646c 6572  try>.    handler
+000001e0: 733a 0a20 2020 2020 202d 2063 616c 6c62  s:.      - callb
+000001f0: 6163 6b3a 206f 6e5f 6164 6d69 6e5f 7570  ack: on_admin_up
+00000200: 6461 7465 0a20 2020 2020 2020 2070 6174  date.        pat
+00000210: 7465 726e 3a0a 2020 2020 2020 2020 2020  tern:.          
+00000220: 2d20 7479 7065 3a20 7472 616e 7361 6374  - type: transact
+00000230: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00000240: 6465 7374 696e 6174 696f 6e3a 203c 6e61  destination: <na
+00000250: 6d65 5f72 6567 6973 7472 793e 0a20 2020  me_registry>.   
+00000260: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+00000270: 696e 743a 2061 646d 696e 5f75 7064 6174  int: admin_updat
+00000280: 650a 2020 2020 2020 2d20 6361 6c6c 6261  e.      - callba
+00000290: 636b 3a20 6f6e 5f65 7865 6375 7465 0a20  ck: on_execute. 
+000002a0: 2020 2020 2020 2070 6174 7465 726e 3a0a         pattern:.
+000002b0: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+000002c0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
+000002d0: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+000002e0: 6174 696f 6e3a 203c 6e61 6d65 5f72 6567  ation: <name_reg
+000002f0: 6973 7472 793e 0a20 2020 2020 2020 2020  istry>.         
+00000300: 2020 2065 6e74 7279 706f 696e 743a 2065     entrypoint: e
+00000310: 7865 6375 7465 0a20 2020 206c 6173 745f  xecute.    last_
+00000320: 6c65 7665 6c3a 2031 3435 3038 3532 0a0a  level: 1450852..
+00000330: 696e 6465 7865 733a 0a20 2064 6f6d 6169  indexes:.  domai
+00000340: 6e73 3a0a 2020 2020 7465 6d70 6c61 7465  ns:.    template
+00000350: 3a20 646f 6d61 696e 730a 2020 2020 7661  : domains.    va
+00000360: 6c75 6573 3a0a 2020 2020 2020 6461 7461  lues:.      data
+00000370: 736f 7572 6365 3a20 747a 6b74 0a20 2020  source: tzkt.   
+00000380: 2020 206e 616d 655f 7265 6769 7374 7279     name_registry
+00000390: 3a20 6e61 6d65 5f72 6567 6973 7472 790a  : name_registry.
+000003a0: 0a6c 6f67 6769 6e67 3a20 5741 524e 0a    .logging: WARN.
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/handlers/on_propose.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_factories/handlers/on_propose.py.j2`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.registry.parameter.propose import ProposeParameter
-from {{cookiecutter.package}}.types.registry.storage import RegistryStorage
+import {{project.package}}.models as models
+from {{project.package}}.types.registry.tezos_parameters.propose import ProposeParameter
+from {{project.package}}.types.registry.tezos_storage import RegistryStorage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_propose(
     ctx: HandlerContext,
-    propose: Transaction[ProposeParameter, RegistryStorage],
+    propose: TzktTransaction[ProposeParameter, RegistryStorage],
 ) -> None:
     dao = await models.DAO.get(address=propose.data.target_address)
     await models.Proposal(dao=dao).save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_factories/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-7.0.0rc1/src/demo_nft_marketplace/models/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,43 @@
-from tortoise.fields.relational import ForeignKeyFieldInstance
-from tortoise import fields
+from enum import IntEnum
 
+from dipdup import fields
 from dipdup.models import Model
 
 
-class DAO(Model):
-    address = fields.CharField(36, pk=True)
-
-
-class User(Model):
-    address = fields.CharField(36, pk=True)
-    balance = fields.IntField()
-
-
-class Proposal(Model):
-    id = fields.IntField(pk=True)
-    dao: ForeignKeyFieldInstance[DAO] = fields.ForeignKeyField('models.DAO', 'proposals')
-    # upvotes = fields.IntField(default=0)
-    # downvotes = fields.IntField(default=0)
-    # start_date = fields.DatetimeField()
-    # metadata = fields.JSONField()
-    # proposer = fields.ForeignKeyField('models.Address', 'proposals')
-
-
-class Vote(Model):
-    id = fields.IntField(pk=True)
-    proposal: ForeignKeyFieldInstance[Proposal] = fields.ForeignKeyField('models.Proposal', 'votes')
-    amount = fields.IntField()
+class SwapStatus(IntEnum):
+    ACTIVE = 0
+    FINISHED = 1
+    CANCELED = 2
+
+
+class Holder(Model):
+    address = fields.TextField(pk=True)
+
+
+class Token(Model):
+    id = fields.BigIntField(pk=True)
+    creator: fields.ForeignKeyField[Holder] = fields.ForeignKeyField('models.Holder', 'tokens')
+    supply = fields.BigIntField()
+    level = fields.BigIntField()
+    timestamp = fields.DatetimeField()
+
+
+class Swap(Model):
+    id = fields.BigIntField(pk=True)
+    creator: fields.ForeignKeyField[Holder] = fields.ForeignKeyField('models.Holder', 'swaps')
+    price = fields.BigIntField()
+    amount = fields.BigIntField()
+    amount_left = fields.BigIntField()
+    level = fields.BigIntField()
+    status = fields.IntEnumField(SwapStatus)
+    timestamp = fields.DatetimeField()
+
+
+class Trade(Model):
+    id = fields.BigIntField(pk=True)
+    swap: fields.ForeignKeyField[Swap] = fields.ForeignKeyField('models.Swap', 'trades')
+    seller: fields.ForeignKeyField[Holder] = fields.ForeignKeyField('models.Holder', 'sales')
+    buyer: fields.ForeignKeyField[Holder] = fields.ForeignKeyField('models.Holder', 'purchases')
+    amount = fields.BigIntField()
+    level = fields.BigIntField()
+    timestamp = fields.DatetimeField()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/dipdup.yml.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_nft_marketplace/dipdup.yaml.j2`

 * *Files 5% similar despite different names*

```diff
@@ -1,77 +1,80 @@
-00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 312e  spec_version: 1.
-00000010: 320a 7061 636b 6167 653a 207b 7b20 636f  2.package: {{ co
-00000020: 6f6b 6965 6375 7474 6572 2e70 6163 6b61  okiecutter.packa
-00000030: 6765 207d 7d0a 0a64 6174 6162 6173 653a  ge }}..database:
-00000040: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000050: 2020 7061 7468 3a20 7b7b 2063 6f6f 6b69    path: {{ cooki
-00000060: 6563 7574 7465 722e 7072 6f6a 6563 745f  ecutter.project_
-00000070: 6e61 6d65 207d 7d2e 7371 6c69 7465 330a  name }}.sqlite3.
-00000080: 0a64 6174 6173 6f75 7263 6573 3a0a 2020  .datasources:.  
-00000090: 747a 6b74 5f6d 6169 6e6e 6574 3a0a 2020  tzkt_mainnet:.  
-000000a0: 2020 6b69 6e64 3a20 747a 6b74 0a20 2020    kind: tzkt.   
-000000b0: 2075 726c 3a20 247b 545a 4b54 5f55 524c   url: ${TZKT_URL
-000000c0: 3a2d 6874 7470 733a 2f2f 6170 692e 747a  :-https://api.tz
-000000d0: 6b74 2e69 6f7d 0a0a 636f 6e74 7261 6374  kt.io}..contract
-000000e0: 733a 0a20 2048 454e 5f6f 626a 6b74 733a  s:.  HEN_objkts:
-000000f0: 0a20 2020 2061 6464 7265 7373 3a20 247b  .    address: ${
-00000100: 4845 4e5f 4f42 4a4b 5453 3a2d 4b54 3152  HEN_OBJKTS:-KT1R
-00000110: 4a36 5062 6a48 7077 6333 4d35 7277 3573  J6PbjHpwc3M5rw5s
-00000120: 324e 626d 6566 7762 7577 6264 7874 6f6e  2Nbmefwbuwbdxton
-00000130: 7d0a 2020 2020 7479 7065 6e61 6d65 3a20  }.    typename: 
-00000140: 6865 6e5f 6f62 6a6b 7473 0a20 2048 454e  hen_objkts.  HEN
-00000150: 5f6d 696e 7465 723a 0a20 2020 2061 6464  _minter:.    add
-00000160: 7265 7373 3a20 247b 4845 4e5f 4d49 4e54  ress: ${HEN_MINT
-00000170: 4552 3a2d 4b54 3148 6b67 3571 654e 6866  ER:-KT1Hkg5qeNhf
-00000180: 7770 4b57 3466 5876 7137 4847 5a42 397a  wpKW4fXvq7HGZB9z
-00000190: 3245 6e6d 4343 4139 7d0a 2020 2020 7479  2EnmCCA9}.    ty
-000001a0: 7065 6e61 6d65 3a20 6865 6e5f 6d69 6e74  pename: hen_mint
-000001b0: 6572 0a0a 696e 6465 7865 733a 0a20 2068  er..indexes:.  h
-000001c0: 656e 5f6d 6169 6e6e 6574 3a0a 2020 2020  en_mainnet:.    
-000001d0: 6b69 6e64 3a20 6f70 6572 6174 696f 6e0a  kind: operation.
-000001e0: 2020 2020 6461 7461 736f 7572 6365 3a20      datasource: 
-000001f0: 747a 6b74 5f6d 6169 6e6e 6574 0a20 2020  tzkt_mainnet.   
-00000200: 2063 6f6e 7472 6163 7473 3a0a 2020 2020   contracts:.    
-00000210: 2020 2d20 4845 4e5f 6d69 6e74 6572 0a20    - HEN_minter. 
-00000220: 2020 2068 616e 646c 6572 733a 0a20 2020     handlers:.   
-00000230: 2020 202d 2063 616c 6c62 6163 6b3a 206f     - callback: o
-00000240: 6e5f 6d69 6e74 0a20 2020 2020 2020 2070  n_mint.        p
-00000250: 6174 7465 726e 3a0a 2020 2020 2020 2020  attern:.        
-00000260: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
-00000270: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00000280: 2020 6465 7374 696e 6174 696f 6e3a 2048    destination: H
-00000290: 454e 5f6d 696e 7465 720a 2020 2020 2020  EN_minter.      
-000002a0: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-000002b0: 3a20 6d69 6e74 5f4f 424a 4b54 0a20 2020  : mint_OBJKT.   
-000002c0: 2020 2020 2020 202d 2074 7970 653a 2074         - type: t
-000002d0: 7261 6e73 6163 7469 6f6e 0a20 2020 2020  ransaction.     
-000002e0: 2020 2020 2020 2064 6573 7469 6e61 7469         destinati
-000002f0: 6f6e 3a20 4845 4e5f 6f62 6a6b 7473 0a20  on: HEN_objkts. 
-00000300: 2020 2020 2020 2020 2020 2065 6e74 7279             entry
-00000310: 706f 696e 743a 206d 696e 740a 2020 2020  point: mint.    
-00000320: 2020 2d20 6361 6c6c 6261 636b 3a20 6f6e    - callback: on
-00000330: 5f73 7761 700a 2020 2020 2020 2020 7061  _swap.        pa
-00000340: 7474 6572 6e3a 0a20 2020 2020 2020 2020  ttern:.         
-00000350: 202d 2074 7970 653a 2074 7261 6e73 6163   - type: transac
-00000360: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00000370: 2064 6573 7469 6e61 7469 6f6e 3a20 4845   destination: HE
-00000380: 4e5f 6d69 6e74 6572 0a20 2020 2020 2020  N_minter.       
-00000390: 2020 2020 2065 6e74 7279 706f 696e 743a       entrypoint:
-000003a0: 2073 7761 700a 2020 2020 2020 2d20 6361   swap.      - ca
-000003b0: 6c6c 6261 636b 3a20 6f6e 5f63 616e 6365  llback: on_cance
-000003c0: 6c5f 7377 6170 0a20 2020 2020 2020 2070  l_swap.        p
-000003d0: 6174 7465 726e 3a0a 2020 2020 2020 2020  attern:.        
-000003e0: 2020 2d20 7479 7065 3a20 7472 616e 7361    - type: transa
-000003f0: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
-00000400: 2020 6465 7374 696e 6174 696f 6e3a 2048    destination: H
-00000410: 454e 5f6d 696e 7465 720a 2020 2020 2020  EN_minter.      
-00000420: 2020 2020 2020 656e 7472 7970 6f69 6e74        entrypoint
-00000430: 3a20 6361 6e63 656c 5f73 7761 700a 2020  : cancel_swap.  
-00000440: 2020 2020 2d20 6361 6c6c 6261 636b 3a20      - callback: 
-00000450: 6f6e 5f63 6f6c 6c65 6374 0a20 2020 2020  on_collect.     
-00000460: 2020 2070 6174 7465 726e 3a0a 2020 2020     pattern:.    
-00000470: 2020 2020 2020 2d20 7479 7065 3a20 7472        - type: tr
-00000480: 616e 7361 6374 696f 6e0a 2020 2020 2020  ansaction.      
-00000490: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-000004a0: 6e3a 2048 454e 5f6d 696e 7465 720a 2020  n: HEN_minter.  
-000004b0: 2020 2020 2020 2020 2020 656e 7472 7970            entryp
-000004c0: 6f69 6e74 3a20 636f 6c6c 6563 740a       oint: collect.
+00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
+00000010: 300a 7061 636b 6167 653a 207b 7b20 7072  0.package: {{ pr
+00000020: 6f6a 6563 742e 7061 636b 6167 6520 7d7d  oject.package }}
+00000030: 0a0a 6461 7461 6261 7365 3a0a 2020 6b69  ..database:.  ki
+00000040: 6e64 3a20 7371 6c69 7465 0a20 2070 6174  nd: sqlite.  pat
+00000050: 683a 207b 7b20 7072 6f6a 6563 742e 7061  h: {{ project.pa
+00000060: 636b 6167 6520 7d7d 2e73 716c 6974 6533  ckage }}.sqlite3
+00000070: 0a0a 6461 7461 736f 7572 6365 733a 0a20  ..datasources:. 
+00000080: 2074 7a6b 745f 6d61 696e 6e65 743a 0a20   tzkt_mainnet:. 
+00000090: 2020 206b 696e 643a 2074 657a 6f73 2e74     kind: tezos.t
+000000a0: 7a6b 740a 2020 2020 7572 6c3a 2024 7b54  zkt.    url: ${T
+000000b0: 5a4b 545f 5552 4c3a 2d68 7474 7073 3a2f  ZKT_URL:-https:/
+000000c0: 2f61 7069 2e74 7a6b 742e 696f 7d0a 0a63  /api.tzkt.io}..c
+000000d0: 6f6e 7472 6163 7473 3a0a 2020 4845 4e5f  ontracts:.  HEN_
+000000e0: 6f62 6a6b 7473 3a0a 2020 2020 6b69 6e64  objkts:.    kind
+000000f0: 3a20 7465 7a6f 730a 2020 2020 6164 6472  : tezos.    addr
+00000100: 6573 733a 2024 7b48 454e 5f4f 424a 4b54  ess: ${HEN_OBJKT
+00000110: 533a 2d4b 5431 524a 3650 626a 4870 7763  S:-KT1RJ6PbjHpwc
+00000120: 334d 3572 7735 7332 4e62 6d65 6677 6275  3M5rw5s2Nbmefwbu
+00000130: 7762 6478 746f 6e7d 0a20 2020 2074 7970  wbdxton}.    typ
+00000140: 656e 616d 653a 2068 656e 5f6f 626a 6b74  ename: hen_objkt
+00000150: 730a 2020 4845 4e5f 6d69 6e74 6572 3a0a  s.  HEN_minter:.
+00000160: 2020 2020 6b69 6e64 3a20 7465 7a6f 730a      kind: tezos.
+00000170: 2020 2020 6164 6472 6573 733a 2024 7b48      address: ${H
+00000180: 454e 5f4d 494e 5445 523a 2d4b 5431 486b  EN_MINTER:-KT1Hk
+00000190: 6735 7165 4e68 6677 704b 5734 6658 7671  g5qeNhfwpKW4fXvq
+000001a0: 3748 475a 4239 7a32 456e 6d43 4341 397d  7HGZB9z2EnmCCA9}
+000001b0: 0a20 2020 2074 7970 656e 616d 653a 2068  .    typename: h
+000001c0: 656e 5f6d 696e 7465 720a 0a69 6e64 6578  en_minter..index
+000001d0: 6573 3a0a 2020 6865 6e5f 6d61 696e 6e65  es:.  hen_mainne
+000001e0: 743a 0a20 2020 206b 696e 643a 2074 657a  t:.    kind: tez
+000001f0: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
+00000200: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
+00000210: 653a 2074 7a6b 745f 6d61 696e 6e65 740a  e: tzkt_mainnet.
+00000220: 2020 2020 636f 6e74 7261 6374 733a 0a20      contracts:. 
+00000230: 2020 2020 202d 2048 454e 5f6d 696e 7465       - HEN_minte
+00000240: 720a 2020 2020 6861 6e64 6c65 7273 3a0a  r.    handlers:.
+00000250: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+00000260: 3a20 6f6e 5f6d 696e 740a 2020 2020 2020  : on_mint.      
+00000270: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
+00000280: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+00000290: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+000002a0: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+000002b0: 3a20 4845 4e5f 6d69 6e74 6572 0a20 2020  : HEN_minter.   
+000002c0: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+000002d0: 696e 743a 206d 696e 745f 4f42 4a4b 540a  int: mint_OBJKT.
+000002e0: 2020 2020 2020 2020 2020 2d20 7479 7065            - type
+000002f0: 3a20 7472 616e 7361 6374 696f 6e0a 2020  : transaction.  
+00000300: 2020 2020 2020 2020 2020 6465 7374 696e            destin
+00000310: 6174 696f 6e3a 2048 454e 5f6f 626a 6b74  ation: HEN_objkt
+00000320: 730a 2020 2020 2020 2020 2020 2020 656e  s.            en
+00000330: 7472 7970 6f69 6e74 3a20 6d69 6e74 0a20  trypoint: mint. 
+00000340: 2020 2020 202d 2063 616c 6c62 6163 6b3a       - callback:
+00000350: 206f 6e5f 7377 6170 0a20 2020 2020 2020   on_swap.       
+00000360: 2070 6174 7465 726e 3a0a 2020 2020 2020   pattern:.      
+00000370: 2020 2020 2d20 7479 7065 3a20 7472 616e      - type: tran
+00000380: 7361 6374 696f 6e0a 2020 2020 2020 2020  saction.        
+00000390: 2020 2020 6465 7374 696e 6174 696f 6e3a      destination:
+000003a0: 2048 454e 5f6d 696e 7465 720a 2020 2020   HEN_minter.    
+000003b0: 2020 2020 2020 2020 656e 7472 7970 6f69          entrypoi
+000003c0: 6e74 3a20 7377 6170 0a20 2020 2020 202d  nt: swap.      -
+000003d0: 2063 616c 6c62 6163 6b3a 206f 6e5f 6361   callback: on_ca
+000003e0: 6e63 656c 5f73 7761 700a 2020 2020 2020  ncel_swap.      
+000003f0: 2020 7061 7474 6572 6e3a 0a20 2020 2020    pattern:.     
+00000400: 2020 2020 202d 2074 7970 653a 2074 7261       - type: tra
+00000410: 6e73 6163 7469 6f6e 0a20 2020 2020 2020  nsaction.       
+00000420: 2020 2020 2064 6573 7469 6e61 7469 6f6e       destination
+00000430: 3a20 4845 4e5f 6d69 6e74 6572 0a20 2020  : HEN_minter.   
+00000440: 2020 2020 2020 2020 2065 6e74 7279 706f           entrypo
+00000450: 696e 743a 2063 616e 6365 6c5f 7377 6170  int: cancel_swap
+00000460: 0a20 2020 2020 202d 2063 616c 6c62 6163  .      - callbac
+00000470: 6b3a 206f 6e5f 636f 6c6c 6563 740a 2020  k: on_collect.  
+00000480: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000490: 2020 2020 2020 2020 202d 2074 7970 653a           - type:
+000004a0: 2074 7261 6e73 6163 7469 6f6e 0a20 2020   transaction.   
+000004b0: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
+000004c0: 7469 6f6e 3a20 4845 4e5f 6d69 6e74 6572  tion: HEN_minter
+000004d0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+000004e0: 7279 706f 696e 743a 2063 6f6c 6c65 6374  rypoint: collect
+000004f0: 0a                                       .
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/handlers/on_swap.py.j2` & `dipdup-7.0.0rc1/src/demo_auction/handlers/on_bid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-import {{cookiecutter.package}}.models as models
-from {{cookiecutter.package}}.types.hen_minter.parameter.swap import SwapParameter
-from {{cookiecutter.package}}.types.hen_minter.storage import HenMinterStorage
+import demo_auction.models as models
+from demo_auction.types.tzcolors_auction.tezos_parameters.bid import BidParameter
+from demo_auction.types.tzcolors_auction.tezos_storage import TzcolorsAuctionStorage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
-async def on_swap(
+async def on_bid(
     ctx: HandlerContext,
-    swap: Transaction[SwapParameter, HenMinterStorage],
+    bid: TzktTransaction[BidParameter, TzcolorsAuctionStorage],
 ) -> None:
-    holder, _ = await models.Holder.get_or_create(address=swap.data.sender_address)
-    swap_model = models.Swap(
-        id=int(swap.storage.swap_id) - 1,
-        creator=holder,
-        price=swap.parameter.xtz_per_objkt,
-        amount=swap.parameter.objkt_amount,
-        amount_left=swap.parameter.objkt_amount,
-        status=models.SwapStatus.ACTIVE,
-        level=swap.data.level,
-        timestamp=swap.data.timestamp,
-    )
-    await swap_model.save()
+    assert bid.data.amount is not None
+
+    auction = await models.Auction.filter(
+        id=bid.parameter.__root__,
+    ).get()
+
+    bidder, _ = await models.User.get_or_create(address=bid.data.sender_address)
+    await models.Bid(
+        auction=auction,
+        bidder=bidder,
+        bid_amount=bid.data.amount,
+        level=bid.data.level,
+        timestamp=bid.data.timestamp,
+    ).save()
+
+    auction.bidder = bidder
+    auction.bid_amount += bid.data.amount
+    await auction.save()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_nft_marketplace/src/{{cookiecutter.package}}/models.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_auction/models/__init__.py.j2`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 from enum import IntEnum
 
-from tortoise.fields.relational import ForeignKeyFieldInstance
-from tortoise import fields
+
+from dipdup import fields
 
 from dipdup.models import Model
 
 
-class SwapStatus(IntEnum):
+class AuctionStatus(IntEnum):
     ACTIVE = 0
     FINISHED = 1
-    CANCELED = 2
 
 
-class Holder(Model):
-    address = fields.CharField(36, pk=True)
+class User(Model):
+    address = fields.TextField(pk=True)
 
 
 class Token(Model):
     id = fields.BigIntField(pk=True)
-    creator: ForeignKeyFieldInstance[Holder] = fields.ForeignKeyField('models.Holder', 'tokens')
-    supply = fields.BigIntField()
+    address = fields.TextField()
+    amount = fields.BigIntField()
     level = fields.BigIntField()
     timestamp = fields.DatetimeField()
+    holder: fields.ForeignKeyField[User] = fields.ForeignKeyField('models.User', 'tokens')
+
+    token_id: int
 
 
-class Swap(Model):
+class Auction(Model):
     id = fields.BigIntField(pk=True)
-    creator: ForeignKeyFieldInstance[Holder] = fields.ForeignKeyField('models.Holder', 'swaps')
-    price = fields.BigIntField()
-    amount = fields.BigIntField()
-    amount_left = fields.BigIntField()
+    token: fields.ForeignKeyField[Token] = fields.ForeignKeyField('models.Token', 'auctions')
+    bid_amount = fields.BigIntField()
+    bidder: fields.ForeignKeyField[User] = fields.ForeignKeyField('models.User', 'winning_auctions')
+    seller: fields.ForeignKeyField[User] = fields.ForeignKeyField('models.User', 'created_auctions')
+    end_timestamp = fields.DatetimeField()
+    status = fields.IntEnumField(AuctionStatus)
     level = fields.BigIntField()
-    status = fields.IntEnumField(SwapStatus)
     timestamp = fields.DatetimeField()
 
+    token_id: int
+
 
-class Trade(Model):
+class Bid(Model):
     id = fields.BigIntField(pk=True)
-    swap: ForeignKeyFieldInstance[Swap] = fields.ForeignKeyField('models.Swap', 'trades')
-    seller: ForeignKeyFieldInstance[Holder] = fields.ForeignKeyField('models.Holder', 'sales')
-    buyer: ForeignKeyFieldInstance[Holder] = fields.ForeignKeyField('models.Holder', 'purchases')
-    amount = fields.BigIntField()
+    auction: fields.ForeignKeyField[Auction] = fields.ForeignKeyField('models.Auction', 'bids')
+    bid_amount = fields.BigIntField()
+    bidder: fields.ForeignKeyField[User] = fields.ForeignKeyField('models.User', 'bids')
     level = fields.BigIntField()
     timestamp = fields.DatetimeField()
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_token/dipdup.yml.j2` & `dipdup-7.0.0rc1/src/demo_token/dipdup.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 312e  spec_version: 1.
-00000010: 320a 7061 636b 6167 653a 207b 7b20 636f  2.package: {{ co
-00000020: 6f6b 6965 6375 7474 6572 2e70 6163 6b61  okiecutter.packa
-00000030: 6765 207d 7d0a 0a64 6174 6162 6173 653a  ge }}..database:
-00000040: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
-00000050: 2020 7061 7468 3a20 7b7b 2063 6f6f 6b69    path: {{ cooki
-00000060: 6563 7574 7465 722e 7072 6f6a 6563 745f  ecutter.project_
-00000070: 6e61 6d65 207d 7d2e 7371 6c69 7465 330a  name }}.sqlite3.
-00000080: 0a63 6f6e 7472 6163 7473 3a0a 2020 747a  .contracts:.  tz
-00000090: 6274 635f 6d61 696e 6e65 743a 0a20 2020  btc_mainnet:.   
-000000a0: 2061 6464 7265 7373 3a20 4b54 3150 5778   address: KT1PWx
-000000b0: 326d 6e44 7565 6f6f 6437 6645 6d66 6242  2mnDueood7fEmfbB
-000000c0: 444b 7831 4439 4241 6e6e 5869 746e 0a20  DKx1D9BAnnXitn. 
-000000d0: 2020 2074 7970 656e 616d 653a 2074 7a62     typename: tzb
-000000e0: 7463 0a0a 6461 7461 736f 7572 6365 733a  tc..datasources:
-000000f0: 0a20 2074 7a6b 745f 6d61 696e 6e65 743a  .  tzkt_mainnet:
-00000100: 0a20 2020 206b 696e 643a 2074 7a6b 740a  .    kind: tzkt.
-00000110: 2020 2020 7572 6c3a 2068 7474 7073 3a2f      url: https:/
-00000120: 2f61 7069 2e74 7a6b 742e 696f 0a0a 696e  /api.tzkt.io..in
-00000130: 6465 7865 733a 0a20 2074 7a62 7463 5f68  dexes:.  tzbtc_h
-00000140: 6f6c 6465 7273 5f6d 6169 6e6e 6574 3a0a  olders_mainnet:.
-00000150: 2020 2020 7465 6d70 6c61 7465 3a20 747a      template: tz
-00000160: 6274 635f 686f 6c64 6572 730a 2020 2020  btc_holders.    
-00000170: 7661 6c75 6573 3a0a 2020 2020 2020 636f  values:.      co
-00000180: 6e74 7261 6374 3a20 747a 6274 635f 6d61  ntract: tzbtc_ma
-00000190: 696e 6e65 740a 2020 2020 2020 6461 7461  innet.      data
-000001a0: 736f 7572 6365 3a20 747a 6b74 5f6d 6169  source: tzkt_mai
-000001b0: 6e6e 6574 0a0a 7465 6d70 6c61 7465 733a  nnet..templates:
-000001c0: 0a20 2074 7a62 7463 5f68 6f6c 6465 7273  .  tzbtc_holders
-000001d0: 3a0a 2020 2020 6b69 6e64 3a20 6f70 6572  :.    kind: oper
-000001e0: 6174 696f 6e0a 2020 2020 6461 7461 736f  ation.    dataso
-000001f0: 7572 6365 3a20 3c64 6174 6173 6f75 7263  urce: <datasourc
-00000200: 653e 0a20 2020 2063 6f6e 7472 6163 7473  e>.    contracts
-00000210: 3a0a 2020 2020 2020 2d20 3c63 6f6e 7472  :.      - <contr
-00000220: 6163 743e 0a20 2020 2068 616e 646c 6572  act>.    handler
-00000230: 733a 0a20 2020 2020 202d 2063 616c 6c62  s:.      - callb
-00000240: 6163 6b3a 206f 6e5f 7472 616e 7366 6572  ack: on_transfer
-00000250: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-00000260: 3a0a 2020 2020 2020 2020 2020 2d20 6465  :.          - de
-00000270: 7374 696e 6174 696f 6e3a 203c 636f 6e74  stination: <cont
-00000280: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
-00000290: 2020 656e 7472 7970 6f69 6e74 3a20 7472    entrypoint: tr
-000002a0: 616e 7366 6572 0a20 2020 2020 202d 2063  ansfer.      - c
-000002b0: 616c 6c62 6163 6b3a 206f 6e5f 6d69 6e74  allback: on_mint
-000002c0: 0a20 2020 2020 2020 2070 6174 7465 726e  .        pattern
-000002d0: 3a0a 2020 2020 2020 2020 2020 2d20 6465  :.          - de
-000002e0: 7374 696e 6174 696f 6e3a 203c 636f 6e74  stination: <cont
-000002f0: 7261 6374 3e0a 2020 2020 2020 2020 2020  ract>.          
-00000300: 2020 656e 7472 7970 6f69 6e74 3a20 6d69    entrypoint: mi
-00000310: 6e74 0a                                  nt.
+00000000: 7370 6563 5f76 6572 7369 6f6e 3a20 322e  spec_version: 2.
+00000010: 300a 7061 636b 6167 653a 2064 656d 6f5f  0.package: demo_
+00000020: 746f 6b65 6e0a 0a64 6174 6162 6173 653a  token..database:
+00000030: 0a20 206b 696e 643a 2073 716c 6974 650a  .  kind: sqlite.
+00000040: 2020 7061 7468 3a20 6465 6d6f 5f74 6f6b    path: demo_tok
+00000050: 656e 2e73 716c 6974 6533 0a0a 636f 6e74  en.sqlite3..cont
+00000060: 7261 6374 733a 0a20 2074 7a62 7463 5f6d  racts:.  tzbtc_m
+00000070: 6169 6e6e 6574 3a0a 2020 2020 6b69 6e64  ainnet:.    kind
+00000080: 3a20 7465 7a6f 730a 2020 2020 6164 6472  : tezos.    addr
+00000090: 6573 733a 204b 5431 5057 7832 6d6e 4475  ess: KT1PWx2mnDu
+000000a0: 656f 6f64 3766 456d 6662 4244 4b78 3144  eood7fEmfbBDKx1D
+000000b0: 3942 416e 6e58 6974 6e0a 2020 2020 7479  9BAnnXitn.    ty
+000000c0: 7065 6e61 6d65 3a20 747a 6274 630a 0a64  pename: tzbtc..d
+000000d0: 6174 6173 6f75 7263 6573 3a0a 2020 747a  atasources:.  tz
+000000e0: 6b74 5f6d 6169 6e6e 6574 3a0a 2020 2020  kt_mainnet:.    
+000000f0: 6b69 6e64 3a20 7465 7a6f 732e 747a 6b74  kind: tezos.tzkt
+00000100: 0a20 2020 2075 726c 3a20 6874 7470 733a  .    url: https:
+00000110: 2f2f 6170 692e 747a 6b74 2e69 6f0a 0a69  //api.tzkt.io..i
+00000120: 6e64 6578 6573 3a0a 2020 747a 6274 635f  ndexes:.  tzbtc_
+00000130: 686f 6c64 6572 735f 6d61 696e 6e65 743a  holders_mainnet:
+00000140: 0a20 2020 2074 656d 706c 6174 653a 2074  .    template: t
+00000150: 7a62 7463 5f68 6f6c 6465 7273 0a20 2020  zbtc_holders.   
+00000160: 2076 616c 7565 733a 0a20 2020 2020 2063   values:.      c
+00000170: 6f6e 7472 6163 743a 2074 7a62 7463 5f6d  ontract: tzbtc_m
+00000180: 6169 6e6e 6574 0a20 2020 2020 2064 6174  ainnet.      dat
+00000190: 6173 6f75 7263 653a 2074 7a6b 745f 6d61  asource: tzkt_ma
+000001a0: 696e 6e65 740a 0a74 656d 706c 6174 6573  innet..templates
+000001b0: 3a0a 2020 747a 6274 635f 686f 6c64 6572  :.  tzbtc_holder
+000001c0: 733a 0a20 2020 206b 696e 643a 2074 657a  s:.    kind: tez
+000001d0: 6f73 2e74 7a6b 742e 6f70 6572 6174 696f  os.tzkt.operatio
+000001e0: 6e73 0a20 2020 2064 6174 6173 6f75 7263  ns.    datasourc
+000001f0: 653a 203c 6461 7461 736f 7572 6365 3e0a  e: <datasource>.
+00000200: 2020 2020 636f 6e74 7261 6374 733a 0a20      contracts:. 
+00000210: 2020 2020 202d 203c 636f 6e74 7261 6374       - <contract
+00000220: 3e0a 2020 2020 6861 6e64 6c65 7273 3a0a  >.    handlers:.
+00000230: 2020 2020 2020 2d20 6361 6c6c 6261 636b        - callback
+00000240: 3a20 6f6e 5f74 7261 6e73 6665 720a 2020  : on_transfer.  
+00000250: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+00000260: 2020 2020 2020 2020 202d 2064 6573 7469           - desti
+00000270: 6e61 7469 6f6e 3a20 3c63 6f6e 7472 6163  nation: <contrac
+00000280: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
+00000290: 6e74 7279 706f 696e 743a 2074 7261 6e73  ntrypoint: trans
+000002a0: 6665 720a 2020 2020 2020 2d20 6361 6c6c  fer.      - call
+000002b0: 6261 636b 3a20 6f6e 5f6d 696e 740a 2020  back: on_mint.  
+000002c0: 2020 2020 2020 7061 7474 6572 6e3a 0a20        pattern:. 
+000002d0: 2020 2020 2020 2020 202d 2064 6573 7469           - desti
+000002e0: 6e61 7469 6f6e 3a20 3c63 6f6e 7472 6163  nation: <contrac
+000002f0: 743e 0a20 2020 2020 2020 2020 2020 2065  t>.            e
+00000300: 6e74 7279 706f 696e 743a 206d 696e 74    ntrypoint: mint
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_mint.py.j2` & `dipdup-7.0.0rc1/src/demo_token/handlers/on_mint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from decimal import Decimal
 
-from {{ cookiecutter.package }}.handlers.on_balance_update import on_balance_update
-from {{ cookiecutter.package }}.types.tzbtc.parameter.mint import MintParameter
-from {{ cookiecutter.package }}.types.tzbtc.storage import TzbtcStorage
+from demo_token.handlers.on_balance_update import on_balance_update
+from demo_token.types.tzbtc.tezos_parameters.mint import MintParameter
+from demo_token.types.tzbtc.tezos_storage import TzbtcStorage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_mint(
     ctx: HandlerContext,
-    mint: Transaction[MintParameter, TzbtcStorage],
+    mint: TzktTransaction[MintParameter, TzbtcStorage],
 ) -> None:
     amount = Decimal(mint.parameter.value) / (10**8)
     await on_balance_update(
         address=mint.parameter.to,
         balance_update=amount,
         timestamp=mint.data.timestamp,
-    )
+    )
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_token/src/{{cookiecutter.package}}/handlers/on_transfer.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_token/handlers/on_transfer.py.j2`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from decimal import Decimal
 
-from {{ cookiecutter.package }}.handlers.on_balance_update import on_balance_update
-from {{ cookiecutter.package }}.types.tzbtc.parameter.transfer import TransferParameter
-from {{ cookiecutter.package }}.types.tzbtc.storage import TzbtcStorage
+from {{ project.package }}.handlers.on_balance_update import on_balance_update
+from {{ project.package }}.types.tzbtc.tezos_parameters.transfer import TransferParameter
+from {{ project.package }}.types.tzbtc.tezos_storage import TzbtcStorage
 from dipdup.context import HandlerContext
-from dipdup.models import Transaction
+from dipdup.models.tezos_tzkt import TzktTransaction
 
 
 async def on_transfer(
     ctx: HandlerContext,
-    transfer: Transaction[TransferParameter, TzbtcStorage],
+    transfer: TzktTransaction[TransferParameter, TzbtcStorage],
 ) -> None:
     if transfer.parameter.from_ == transfer.parameter.to:
         # NOTE: Internal tzBTC transfer
         return
 
     amount = Decimal(transfer.parameter.value) / (10**8)
     await on_balance_update(
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_balance_update.py.j2` & `dipdup-7.0.0rc1/src/dipdup/projects/demo_token_transfers/handlers/on_balance_update.py.j2`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from decimal import Decimal
 from decimal import InvalidOperation
 
-import {{cookiecutter.package}}.models as models
+import {{project.package}}.models as models
 
 
 async def on_balance_update(address: str, balance_update: Decimal, timestamp: datetime) -> None:
     try:
         holder, _ = await models.Holder.get_or_create(address=address)
         holder.balance += balance_update
         holder.turnover += abs(balance_update)
```

### Comparing `dipdup-6.5.9/src/dipdup/projects/demo_token_transfers/src/{{cookiecutter.package}}/handlers/on_token_transfer.py.j2` & `dipdup-7.0.0rc1/src/demo_token_transfers/handlers/on_token_transfer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from decimal import Decimal
 from decimal import InvalidOperation
 
-from {{cookiecutter.package}}.handlers.on_balance_update import on_balance_update
+from demo_token_transfers.handlers.on_balance_update import on_balance_update
 from dipdup.context import HandlerContext
-from dipdup.models import TokenTransferData
+from dipdup.models.tezos_tzkt import TzktTokenTransferData
 
 
 async def on_token_transfer(
     ctx: HandlerContext,
-    token_transfer: TokenTransferData,
+    token_transfer: TzktTokenTransferData,
 ) -> None:
     from_, to = token_transfer.from_address, token_transfer.to_address
     if not from_ or not to or from_ == to:
         return
     try:
         amount = Decimal(token_transfer.amount or 0) / (10**8)
     except InvalidOperation:
         return
     if not amount:
         return
 
     await on_balance_update(address=from_, balance_update=-amount, timestamp=token_transfer.timestamp)
-    await on_balance_update(address=to, balance_update=amount, timestamp=token_transfer.timestamp)
+    await on_balance_update(address=to, balance_update=amount, timestamp=token_transfer.timestamp)
```

### Comparing `dipdup-6.5.9/src/dipdup/prometheus.py` & `dipdup-7.0.0rc1/src/dipdup/prometheus.py`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.9/src/dipdup/scheduler.py` & `dipdup-7.0.0rc1/src/dipdup/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import json
 import logging
 from contextlib import suppress
 from functools import partial
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Set
@@ -18,25 +17,26 @@
 
 from dipdup.config import JobConfig
 from dipdup.context import DipDupContext
 from dipdup.context import HookContext
 from dipdup.exceptions import ConfigurationError
 from dipdup.exceptions import FrameworkException
 from dipdup.utils import FormattedLogger
+from dipdup.utils import json_dumps
 
 DEFAULT_CONFIG = {
     'apscheduler.jobstores.default.class': 'apscheduler.jobstores.memory:MemoryJobStore',
     'apscheduler.executors.default.class': 'apscheduler.executors.asyncio:AsyncIOExecutor',
     'apscheduler.timezone': 'UTC',
 }
 
 
 def _verify_config(config: Dict[str, Any]) -> None:
     """Ensure that dict is a valid `apscheduler` config"""
-    json_config = json.dumps(config)
+    json_config = json_dumps(config).decode()
     if 'apscheduler.executors.pool' in json_config:
         raise ConfigurationError(
             '`apscheduler.executors.pool` is not supported. If needed, create a pool inside a regular hook.'
         )
     for key in config:
         if not key.startswith('apscheduler.'):
             raise ConfigurationError(
@@ -44,15 +44,15 @@
             )
 
 
 class SchedulerManager:
     def __init__(self, config: Optional[Dict[str, Any]] = None) -> None:
         if config:
             _verify_config(config)
-        self._logger = logging.getLogger('dipdup.jobs')
+        self._logger = logging.getLogger(__name__)
         self._scheduler = AsyncIOScheduler(config or DEFAULT_CONFIG)
         self._scheduler.add_listener(self._on_error, EVENT_JOB_ERROR)
         self._scheduler.add_listener(self._on_executed, EVENT_JOB_EXECUTED)
         self._exception: Optional[Exception] = None
         self._exception_event: asyncio.Event = asyncio.Event()
         self._daemons: Set[str] = set()
 
@@ -87,17 +87,17 @@
             ctx: DipDupContext,
             *args: Any,
             **kwargs: Any,
         ) -> None:
             nonlocal job_config, hook_config
             job_ctx = HookContext(
                 config=ctx.config,
+                package=ctx.package,
                 datasources=ctx.datasources,
-                callbacks=ctx._callbacks,
-                transactions=ctx._transactions,
+                transactions=ctx.transactions,
                 logger=logger,
                 hook_config=hook_config,
             )
             with suppress(asyncio.CancelledError):
                 await job_ctx.fire_hook(
                     hook_config.callback,
                     *args,
```

### Comparing `dipdup-6.5.9/src/dipdup/sentry.py` & `dipdup-7.0.0rc1/src/dipdup/sentry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,76 @@
 # NOTE: All imports except the basic ones are very lazy in this module. Let's keep it that way.
 import asyncio
 import hashlib
 import logging
 import platform
-import tempfile
 from contextlib import suppress
-from functools import partial
-from pathlib import Path
-from tempfile import NamedTemporaryFile
-from typing import TYPE_CHECKING
 from typing import Any
 
-import orjson
 import sentry_sdk
 import sentry_sdk.serializer
 import sentry_sdk.utils
 from sentry_sdk.integrations.aiohttp import AioHttpIntegration
 from sentry_sdk.integrations.atexit import AtexitIntegration
 from sentry_sdk.integrations.logging import LoggingIntegration
 
 from dipdup import __version__
-from dipdup import baking_bad
 from dipdup import env
-from dipdup.utils.sys import is_shutting_down
+from dipdup.config import DipDupConfig
+from dipdup.sys import is_shutting_down
 
-if TYPE_CHECKING:
-    from dipdup.config import DipDupConfig
-
-
-_logger = logging.getLogger('dipdup.sentry')
+_logger = logging.getLogger(__name__)
 
 
 async def _heartbeat() -> None:
     """Restart Sentry session every 24 hours"""
     with suppress(asyncio.CancelledError):
         while True:
             await asyncio.sleep(60 * 60 * 24)
             _logger.info('Reopening Sentry session')
             sentry_sdk.Hub.current.end_session()
             sentry_sdk.Hub.current.flush()
             sentry_sdk.Hub.current.start_session()
 
 
-def save_crashdump(error: Exception) -> str:
-    """Saves a crashdump file with Sentry error data, returns the path to the tempfile"""
+def extract_event(error: Exception) -> dict[str, Any]:
+    """Extracts Sentry event from an exception"""
     exc_info = sentry_sdk.utils.exc_info_from_error(error)
     event, _ = sentry_sdk.utils.event_from_exception(exc_info)
     event = sentry_sdk.serializer.serialize(event)
-
-    tmp_dir = Path(tempfile.gettempdir()) / 'dipdup' / 'crashdumps'
-    tmp_dir.mkdir(parents=True, exist_ok=True)
-
-    crashdump_file = NamedTemporaryFile(
-        mode='ab',
-        suffix='.json',
-        dir=tmp_dir,
-        delete=False,
-    )
-    with crashdump_file as f:
-        f.write(
-            orjson.dumps(
-                event,
-                option=orjson.OPT_INDENT_2,
-            ),
-        )
-    return crashdump_file.name
+    event.pop('_meta', None)
+    return event
 
 
 def before_send(
     event: dict[str, Any],
     hint: dict[str, Any],
-    crash_reporting: bool,
 ) -> dict[str, Any] | None:
     # NOTE: Terminated connections, cancelled tasks, etc.
     if is_shutting_down():
         return None
 
-    # NOTE: Skip some reports if Sentry DSN is not set implicitly
-    if crash_reporting:
-        if env.TEST or env.CI:
-            return None
-
-        # NOTE: User-generated events (e.g. from `ctx.logger`)
-        if not event.get('logger', 'dipdup').startswith('dipdup'):
-            return None
-
     # NOTE: Dark magic ahead. Merge `CallbackError` and its cause when possible.
     with suppress(KeyError, IndexError):
         exceptions = event['exception']['values']
         if exceptions[-1]['type'] == 'CallbackError':
             wrapper_frames = exceptions[-1]['stacktrace']['frames']
             crash_frames = exceptions[-2]['stacktrace']['frames']
             exceptions[-2]['stacktrace']['frames'] = wrapper_frames + crash_frames
             event['message'] = exceptions[-2]['value']
             del exceptions[-1]
 
     return event
 
 
 def init_sentry(config: 'DipDupConfig') -> None:
-    crash_reporting = config.advanced.crash_reporting
     dsn = config.sentry.dsn
-
     if dsn:
-        pass
-    elif crash_reporting:
-        dsn = baking_bad.SENTRY_DSN
-    else:
-        return
+        _logger.info('Sentry is enabled: %s', dsn)
 
-    _logger.info('Crash reporting is enabled: %s', dsn)
     if config.sentry.debug:
         level, event_level, attach_stacktrace = logging.DEBUG, logging.WARNING, True
     else:
         level, event_level, attach_stacktrace = logging.INFO, logging.ERROR, False
 
     integrations = [
         AioHttpIntegration(),
@@ -124,41 +81,33 @@
         # NOTE: Suppresses `atexit` notification
         AtexitIntegration(lambda _, __: None),
     ]
     package = config.package or 'dipdup'
     release = config.sentry.release or __version__
     environment = config.sentry.environment
     server_name = config.sentry.server_name
-    before_send_fn = partial(
-        before_send,
-        crash_reporting=crash_reporting,
-    )
 
     if not environment:
         if env.DOCKER:
             environment = 'docker'
         elif env.TEST:
             environment = 'tests'
         elif env.CI:
             environment = 'gha'
         else:
             environment = 'local'
 
     if not server_name:
-        if crash_reporting:
-            # NOTE: Prevent Sentry from leaking hostnames
-            server_name = 'unknown'
-        else:
-            server_name = platform.node()
+        server_name = platform.node()
 
     sentry_sdk.init(
         dsn=dsn,
         integrations=integrations,
         attach_stacktrace=attach_stacktrace,
-        before_send=before_send_fn,
+        before_send=before_send,
         release=release,
         environment=environment,
         server_name=server_name,
     )
     # NOTE: Increase __repr__ length limit
     sentry_sdk.utils.MAX_STRING_LENGTH *= 10
 
@@ -167,15 +116,14 @@
         'python': platform.python_version(),
         'os': f'{platform.system().lower()}-{platform.machine()}',
         'version': __version__,
         'package': package,
         'release': release,
         'environment': environment,
         'server_name': server_name,
-        'crash_reporting': crash_reporting,
     }
     _logger.debug('Sentry tags: %s', ', '.join(f'{k}={v}' for k, v in tags.items()))
     for tag, value in tags.items():
         sentry_sdk.set_tag(f'dipdup.{tag}', value)
 
     # NOTE: User ID allows to track release adoption. It's sent on every session,
     # NOTE: but obfuscated below, so it's not a privacy issue. However, randomly
```

### Comparing `dipdup-6.5.9/src/dipdup/sql/truncate_schema.sql` & `dipdup-7.0.0rc1/src/dipdup/sql/truncate_schema.sql`

 * *Files identical despite different names*

### Comparing `dipdup-6.5.9/src/dipdup/transactions.py` & `dipdup-7.0.0rc1/src/dipdup/transactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import asyncio
 from collections import deque
 from contextlib import asynccontextmanager
 from typing import AsyncIterator
 from typing import Optional
-from typing import Set
 
 from tortoise.transactions import in_transaction
 
 import dipdup.models
-from dipdup.utils.database import get_connection
-from dipdup.utils.database import set_connection
+from dipdup.database import get_connection
+from dipdup.database import set_connection
 
 CLEANUP_INTERVAL = 60
 
 
 class TransactionManager:
     """Manages versioned transactions"""
 
     def __init__(
         self,
-        depth: int = 2,
-        immune_tables: Optional[Set[str]] = None,
+        depth: int | None = None,
+        immune_tables: set[str] | None = None,
     ) -> None:
         self._depth = depth
         self._immune_tables = immune_tables or set()
         self._transaction: Optional[dipdup.models.VersionedTransaction] = None
         self._pending_updates: deque[dipdup.models.ModelUpdate] = deque()
 
     @asynccontextmanager
@@ -74,14 +73,16 @@
     async def _commit(self) -> None:
         """Save pending updates to DB in the same order as they were added"""
         while self._pending_updates:
             await self._pending_updates.popleft().save()
 
     async def cleanup(self) -> None:
         """Cleanup outdated model updates"""
+        if not self._depth:
+            return
         most_recent_index = await dipdup.models.Index.filter().order_by('-level').first()
         if not most_recent_index:
             return
 
         last_level = most_recent_index.level - self._depth
         await dipdup.models.ModelUpdate.filter(level__lt=last_level).delete()
```

### Comparing `dipdup-6.5.9/src/dipdup/utils/__init__.py` & `dipdup-7.0.0rc1/src/dipdup/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pkgutil
 import types
 from collections import defaultdict
 from decimal import Decimal
 from functools import reduce
 from logging import Logger
 from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import DefaultDict
 from typing import Dict
 from typing import Iterator
 from typing import List
 from typing import Mapping
@@ -18,28 +19,71 @@
 from typing import Sequence
 from typing import TextIO
 from typing import TypeVar
 from typing import Union
 
 import orjson
 from humps import main as humps
+from pydantic import BaseModel
+from pydantic import ValidationError
 
 from dipdup.exceptions import FrameworkException
+from dipdup.exceptions import InvalidDataError
 from dipdup.exceptions import ProjectImportError
 
+ObjectT = TypeVar('ObjectT', bound=BaseModel)
+
+_logger = logging.getLogger(__name__)
+
+
+if TYPE_CHECKING:
+    from jinja2 import Template
+
+
+def load_template(*path: str) -> 'Template':
+    """Load template from path relative to dipdup package"""
+    from jinja2 import Template
+
+    full_path = Path(__file__).parent.joinpath(*path)
+    return Template(full_path.read_text())
+
+
+def touch(path: Path) -> None:
+    """Create empty file, ignore if already exists"""
+    if not path.parent.exists():
+        _logger.info('Creating directory `%s`', path.parent)
+        path.parent.mkdir(parents=True, exist_ok=True)
+
+    if not path.is_file():
+        _logger.info('Creating file `%s`', path)
+        path.touch()
+
+
+def write(path: Path, content: Union[str, bytes], overwrite: bool = False) -> bool:
+    """Write content to file, create directory tree if necessary"""
+    if not path.parent.exists():
+        _logger.info('Creating directory `%s`', path.parent)
+        path.parent.mkdir(parents=True, exist_ok=True)
+
+    if path.exists() and not overwrite:
+        return False
+
+    _logger.info('Writing into file `%s`', path)
+    if isinstance(content, str):
+        content = content.encode()
+    path.write_bytes(content)
+    return True
+
 
 def import_submodules(package: str) -> Dict[str, types.ModuleType]:
     """Recursively import all submodules of a package"""
     module = importlib.import_module(package)
     results = {}
     for subpackage in pkgutil.walk_packages(module.__path__):
         name = subpackage.name
-        # NOTE: Special case; `<package>.types.<package>` causes infinite recursion
-        if '.' in name:
-            continue
         is_pkg = subpackage.ispkg
         full_name = package + '.' + name
         results[full_name] = importlib.import_module(full_name)
         if is_pkg:
             results.update(import_submodules(full_name))
     return results
 
@@ -135,26 +179,56 @@
     for path in paths:
         if ext and path.suffix != ext:
             continue
         if not path.exists():
             continue
         if not path.stat().st_size:
             continue
-        with open(path) as file:
+        with path.open() as file:
             yield file
 
 
 def import_from(module: str, obj: str) -> Any:
     """Import object from module, raise ProjectImportError on failure"""
     try:
         return getattr(importlib.import_module(module), obj)
     except (ImportError, AttributeError) as e:
         raise ProjectImportError(module, obj) from e
 
 
-def json_dumps_decimals(obj: Any) -> str:
-    def _default(obj: Any) -> Any:
-        if isinstance(obj, Decimal):
-            return str(obj)
-        raise TypeError
+def parse_object(
+    type_: type[ObjectT],
+    data: Mapping[str, Any] | Sequence[Any],
+    plain: bool = False,
+) -> ObjectT:
+    try:
+        if plain is False:
+            return type_.parse_obj(data)
+
+        model_keys = tuple(field.alias for field in type_.__fields__.values())
+        return type_(**dict(zip(model_keys, data)))
+
+    except ValidationError as e:
+        raise InvalidDataError(f'Failed to parse: {e.errors()}', type_, data) from e
 
-    return orjson.dumps(obj, default=_default).decode()
+
+def _default_for_decimals(obj: Any) -> Any:
+    if isinstance(obj, Decimal):
+        return str(obj)
+    raise TypeError
+
+
+def json_dumps_plain(obj: Any | str) -> str:
+    """Smarter json.dumps"""
+    return orjson.dumps(
+        obj,
+        default=_default_for_decimals,
+    ).decode()
+
+
+def json_dumps(obj: Any | str, option: int | None = orjson.OPT_INDENT_2) -> bytes:
+    """Smarter json.dumps"""
+    return orjson.dumps(
+        obj,
+        default=_default_for_decimals,
+        option=option,
+    )
```

### Comparing `dipdup-6.5.9/src/dipdup/utils/database.py` & `dipdup-7.0.0rc1/src/dipdup/database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 import asyncio
+import atexit
 import decimal
 import hashlib
 import importlib
 import logging
 from contextlib import asynccontextmanager
 from contextlib import suppress
 from pathlib import Path
 from types import ModuleType
 from typing import Any
 from typing import AsyncIterator
 from typing import Iterable
 from typing import Iterator
-from typing import Optional
-from typing import Set
-from typing import Type
+from typing import cast
 
+import asyncpg.exceptions  # type: ignore[import]
 import sqlparse  # type: ignore[import]
-from asyncpg import CannotConnectNowError  # type: ignore[import]
 from tortoise import Tortoise
 from tortoise.backends.asyncpg.client import AsyncpgDBClient
 from tortoise.backends.base.client import BaseDBAsyncClient
 from tortoise.backends.base.executor import EXECUTOR_CACHE
 from tortoise.backends.sqlite.client import SqliteClient
 from tortoise.connection import connections
 from tortoise.fields import DecimalField
-from tortoise.fields.relational import ForeignKeyFieldInstance
 from tortoise.models import Model as TortoiseModel
 from tortoise.utils import get_schema_sql
 
+from dipdup.exceptions import ConfigurationError
+from dipdup.exceptions import FrameworkException
 from dipdup.exceptions import InvalidModelsError
 from dipdup.utils import iter_files
 from dipdup.utils import pascal_to_snake
 
-_logger = logging.getLogger('dipdup.database')
-_truncate_schema_path = Path(__file__).parent.parent / 'sql' / 'truncate_schema.sql'
+_logger = logging.getLogger(__name__)
 
 DEFAULT_CONNECTION_NAME = 'default'
 HEAD_STATUS_TIMEOUT = 3 * 60
 
 
-def get_connection() -> BaseDBAsyncClient:
-    return connections.get(DEFAULT_CONNECTION_NAME)
+AsyncpgClient = AsyncpgDBClient
+SupportedClient = SqliteClient | AsyncpgClient
 
 
-def set_connection(conn: BaseDBAsyncClient) -> None:
+def get_connection() -> SupportedClient:
+    return cast(SupportedClient, connections.get(DEFAULT_CONNECTION_NAME))
+
+
+def set_connection(conn: SupportedClient) -> None:
     connections.set(DEFAULT_CONNECTION_NAME, conn)
 
 
 @asynccontextmanager
 async def tortoise_wrapper(
     url: str,
     models: str | None = None,
     timeout: int = 60,
     decimal_precision: int | None = None,
+    unsafe_sqlite: bool = False,
 ) -> AsyncIterator[None]:
     """Initialize Tortoise with internal and project models, close connections when done"""
     model_modules: dict[str, Iterable[str | ModuleType]] = {
         'int_models': ['dipdup.models'],
     }
     if models:
         if not models.endswith('.models'):
@@ -73,44 +77,57 @@
             try:
                 await Tortoise.init(
                     db_url=url,
                     modules=model_modules,
                 )
 
                 conn = get_connection()
-                await conn.execute_query('SELECT 1')
+                try:
+                    await conn.execute_query('SELECT 1')
+                except asyncpg.exceptions.InvalidPasswordError as e:
+                    raise ConfigurationError(f'{e.__class__.__name__}: {e}') from e
+
+                if unsafe_sqlite:
+                    _logger.warning('Unsafe SQLite mode enabled; database integrity is not guaranteed!')
+                    await conn.execute_script('PRAGMA foreign_keys = OFF')
+                    await conn.execute_script('PRAGMA synchronous = OFF')
+                    await conn.execute_script('PRAGMA journal_mode = OFF')
+
             # FIXME: Poor logging
-            except (OSError, CannotConnectNowError):
+            except (OSError, asyncpg.exceptions.CannotConnectNowError):
                 _logger.warning("Can't establish database connection, attempt %s/%s", attempt, timeout)
                 if attempt == timeout - 1:
                     raise
                 await asyncio.sleep(1)
             else:
                 break
         yield
     finally:
         await Tortoise.close_connections()
 
 
+from dipdup.models import CachedModel
+from dipdup.models import Model
+
+
 def is_model_class(obj: Any) -> bool:
     """Is subclass of tortoise.Model, but not the base class"""
-    from dipdup.models import Model
 
     if not isinstance(obj, type):
         return False
     if not issubclass(obj, TortoiseModel):
         return False
     if obj in (TortoiseModel, Model):
         return False
     if obj._meta.abstract:
         return False
     return True
 
 
-def iter_models(package: Optional[str]) -> Iterator[tuple[str, Type[TortoiseModel]]]:
+def iter_models(package: str | None) -> Iterator[tuple[str, type[TortoiseModel]]]:
     """Iterate over built-in and project's models"""
     modules = [
         ('int_models', importlib.import_module('dipdup.models')),
     ]
 
     if package:
         if not package.endswith('.models'):
@@ -125,145 +142,174 @@
                 continue
 
             attr_value = getattr(module, attr)
             if is_model_class(attr_value):
                 yield app, attr_value
 
 
-def get_schema_hash(conn: BaseDBAsyncClient) -> str:
+def get_schema_hash(conn: SupportedClient) -> str:
     """Get hash of the current schema"""
     schema_sql = get_schema_sql(conn, False)
-    # NOTE: Column order could differ in two generated schemas for the same models, drop commas and sort strings to eliminate this
+    # NOTE: Column order in generated CREATE TABLE expressions could differ, so drop commas and sort strings first.
     processed_schema_sql = '\n'.join(sorted(schema_sql.replace(',', '').split('\n'))).encode()
     return hashlib.sha256(processed_schema_sql).hexdigest()
 
 
-async def create_schema(conn: BaseDBAsyncClient, name: str) -> None:
-    if isinstance(conn, SqliteClient):
-        raise NotImplementedError
-
-    await conn.execute_script(f'CREATE SCHEMA IF NOT EXISTS {name}')
-    # NOTE: Recreate `truncate_schema` function on fresh schema
-    await conn.execute_script(_truncate_schema_path.read_text())
-
-
 async def execute_sql(
     conn: BaseDBAsyncClient,
     path: Path,
     *args: Any,
     **kwargs: Any,
 ) -> None:
+    """Execute SQL script(s) with formatting"""
     for file in iter_files(path, ext='.sql'):
         _logger.info('Executing script `%s`', file.name)
-        sql = file.read()
-        # NOTE: Generally it's a very bad idea to format SQL scripts with arbitrary arguments.
-        # NOTE: We trust package developers here.
-        sql = sql.format(*args, **kwargs)
+        # NOTE: Usually string-formating SQL scripts is a very bad idea. But for indexers it's totally fine.
+        sql = file.read().format(*args, **kwargs)
         for statement in sqlparse.split(sql):
             # NOTE: Ignore empty statements
             with suppress(AttributeError):
                 await conn.execute_script(statement)
 
 
 async def execute_sql_query(
-    conn: BaseDBAsyncClient,
+    conn: SupportedClient,
     path: Path,
     *values: Any,
 ) -> Any:
-    for file in iter_files(path, ext='.sql'):
-        _logger.info('Executing query `%s`', file.name)
-        sql = file.read()
-        return await conn.execute_query(sql, list(values))
+    """Execute SQL query with arguments"""
+    _logger.info('Executing query `%s`', path.name)
+    sql = path.read_text()
+    return await conn.execute_query(sql, list(values))
 
 
 async def generate_schema(
-    conn: BaseDBAsyncClient,
+    conn: SupportedClient,
     name: str,
 ) -> None:
-    if isinstance(conn, SqliteClient):
-        await Tortoise.generate_schemas()
-    elif isinstance(conn, AsyncpgDBClient):
-        await create_schema(conn, name)
-        await Tortoise.generate_schemas()
+    if isinstance(conn, AsyncpgClient):
+        await pg_create_schema(conn, name)
+
+    await Tortoise.generate_schemas()
 
+    if isinstance(conn, AsyncpgClient):
         # NOTE: Create a view for monitoring head status
-        sql_path = Path(__file__).parent.parent / 'sql' / 'dipdup_head_status.sql'
+        sql_path = Path(__file__).parent / 'sql' / 'dipdup_head_status.sql'
         # TODO: Configurable interval
         await execute_sql(conn, sql_path, HEAD_STATUS_TIMEOUT)
-    else:
-        raise NotImplementedError(f'`{conn.__class__.__name__}` is not supported')
 
 
-async def truncate_schema(conn: BaseDBAsyncClient, name: str) -> None:
-    if isinstance(conn, SqliteClient):
-        raise NotImplementedError
+async def _wipe_schema_postgres(
+    conn: AsyncpgClient,
+    schema_name: str,
+    immune_tables: set[str],
+) -> None:
+    immune_schema_name = f'{schema_name}_immune'
+
+    # NOTE: Create a truncate_schema function to trigger cascade deletion
+    sql_path = Path(__file__).parent / 'sql' / 'truncate_schema.sql'
+    await execute_sql(conn, sql_path, schema_name, immune_schema_name)
+
+    # NOTE: Move immune tables to a separate schema - it's free!
+    if immune_tables:
+        await pg_create_schema(conn, immune_schema_name)
+        for table in immune_tables:
+            await pg_move_table(conn, table, schema_name, immune_schema_name)
+
+    await conn.execute_script(f"SELECT truncate_schema('{schema_name}')")
+
+    if immune_tables:
+        for table in immune_tables:
+            await pg_move_table(conn, table, immune_schema_name, schema_name)
+        await pg_drop_schema(conn, immune_schema_name)
+
+
+async def _wipe_schema_sqlite(
+    conn: SqliteClient,
+    path: str,
+    immune_tables: set[str],
+) -> None:
+    if path == ':memory:':
+        raise FrameworkException('Attempted to wipe in-memory database; that makes no sense')
+
+    # NOTE: Dropping huge tables and deleting from them is slow and I/O heavy in SQLite. It's better to save the tables of interest
+    # elsewhere and drop the whole database. First, create a new database and attach it to the current connection:
+    immune_path, namespace = f'{path}.immune', 'immune'
+    await conn.execute_script(f'ATTACH DATABASE "{immune_path}" AS {namespace}')
+
+    # NOTE: Copy immune tables to the new database.
+    master_query = 'SELECT name, type FROM sqlite_master'
+    result = await conn.execute_query(master_query)
+    for name, type_ in result[1]:
+        if type_ != 'table' or name not in immune_tables:
+            continue
+
+        expr = f'CREATE TABLE {namespace}.{name} AS SELECT * FROM {name}'
+        _logger.info('Executing `%s`', expr)
+        await conn.execute_script(expr)
+
+    # NOTE: Now the weirdest part - swap the databases when the program exits and all connections are closed.
+    def _finish_wipe() -> None:
+        _logger.info('Restoring immune tables')
+        Path(immune_path).replace(path)
 
-    await conn.execute_script(_truncate_schema_path.read_text())
-    await conn.execute_script(f"SELECT truncate_schema('{name}')")
+    atexit.register(_finish_wipe)
 
 
 async def wipe_schema(
-    conn: BaseDBAsyncClient,
+    conn: SupportedClient,
     schema_name: str,
-    immune_tables: Set[str],
+    immune_tables: set[str],
 ) -> None:
     """Truncate schema preserving immune tables. Executes in a transaction"""
-    if isinstance(conn, SqliteClient):
-        raise NotImplementedError
+    async with conn._in_transaction() as conn:
+        if isinstance(conn, SqliteClient):
+            await _wipe_schema_sqlite(conn, schema_name, immune_tables)
+        elif isinstance(conn, AsyncpgClient):
+            await _wipe_schema_postgres(conn, schema_name, immune_tables)
+        else:
+            raise NotImplementedError
 
-    immune_schema_name = f'{schema_name}_immune'
 
-    async with conn._in_transaction() as conn:
-        if immune_tables:
-            await create_schema(conn, immune_schema_name)
-            for table in immune_tables:
-                await move_table(conn, table, schema_name, immune_schema_name)
-
-        await truncate_schema(conn, schema_name)
-
-        if immune_tables:
-            for table in immune_tables:
-                await move_table(conn, table, immune_schema_name, schema_name)
-            await drop_schema(conn, immune_schema_name)
-
-
-async def drop_schema(conn: BaseDBAsyncClient, name: str) -> None:
-    if isinstance(conn, SqliteClient):
-        raise NotImplementedError
+async def pg_create_schema(conn: AsyncpgClient, name: str) -> None:
+    """Create PostgreSQL schema if not exists"""
+    await conn.execute_script(f'CREATE SCHEMA IF NOT EXISTS {name}')
+
 
+async def pg_drop_schema(conn: AsyncpgClient, name: str) -> None:
     await conn.execute_script(f'DROP SCHEMA IF EXISTS {name}')
 
 
-async def move_table(conn: BaseDBAsyncClient, name: str, schema: str, new_schema: str) -> None:
+async def pg_move_table(conn: AsyncpgClient, name: str, schema: str, new_schema: str) -> None:
     """Move table from one schema to another"""
-    if isinstance(conn, SqliteClient):
-        raise NotImplementedError
-
     await conn.execute_script(f'ALTER TABLE {schema}.{name} SET SCHEMA {new_schema}')
 
 
 def prepare_models(package: str | None) -> None:
     """Prepare TortoiseORM models to use with DipDup.
     Generate missing table names, validate models, increase decimal precision if needed.
     """
     # NOTE: Circular imports
+    import dipdup.fields
     import dipdup.models
 
     # NOTE: Required for pytest-xdist. Models with the same name in different packages cause conflicts otherwise.
     EXECUTOR_CACHE.clear()
 
     db_tables: set[str] = set()
 
     for app, model in iter_models(package):
         # NOTE: Enforce our class for user models
         if app != 'int_models' and not issubclass(model, dipdup.models.Model):
             raise InvalidModelsError(
-                'Project models must be subclassed from `dipdup.models.Model`.'
-                '\n\n'
-                'Replace `from tortoise import Model` import with `from dipdup.models import Model`.',
+                (
+                    'Project models must be subclassed from `dipdup.models.Model`.'
+                    '\n\n'
+                    'Replace `from tortoise import Model` import with `from dipdup.models import Model`.'
+                ),
                 model,
             )
 
         # NOTE: Generate missing table names before Tortoise does
         if not model._meta.db_table:
             model._meta.db_table = pascal_to_snake(model.__name__)
 
@@ -280,40 +326,57 @@
         if table_name != pascal_to_snake(table_name):
             raise InvalidModelsError(
                 'Table name must be in snake_case.',
                 model,
             )
 
         for field in model._meta.fields_map.values():
+            # NOTE: Ensure that field is imported from dipdup.fields
+            if app != 'int_models' and not field.__module__.startswith('dipdup.fields'):
+                raise InvalidModelsError(
+                    'Model fields must be imported from `dipdup.fields`.',
+                    model,
+                    field.model_field_name,
+                )
+
             # NOTE: Enforce fields in snake_case
             field_name = field.model_field_name
             if field_name != pascal_to_snake(field_name):
                 raise InvalidModelsError(
                     'Model fields must be in snake_case.',
                     model,
                     field_name,
                 )
 
             # NOTE: Enforce unique field names to avoid GraphQL issues
             if field_name == table_name:
                 raise InvalidModelsError(
-                    'Model field names must differ from table name.',
+                    'Model field names must differ from the table name.',
                     model,
                     field_name,
                 )
 
             # NOTE: The same for backward relations
-            if isinstance(field, ForeignKeyFieldInstance) and field.related_name == table_name:
+            if isinstance(field, dipdup.fields.ForeignKeyField) and field.related_name == table_name:
                 raise InvalidModelsError(
-                    'Model field names must differ from table name.',
+                    'Model field names must differ from the table name.',
                     model,
                     f'related_name={field.related_name}',
                 )
 
 
+async def preload_cached_models(package: str | None) -> None:
+    from dipdup.performance import caches
+
+    for _, model in iter_models(package):
+        if issubclass(model, CachedModel):
+            caches.add_model(model)
+            await model.preload()
+
+
 def guess_decimal_precision(package: str | None) -> int:
     """Guess decimal precision from project models.
 
     Doesn't work for realy big numbers.
     """
     prec = 0
     for _, model in iter_models(package):
```

### Comparing `dipdup-6.5.9/src/dipdup/utils/sys.py` & `dipdup-7.0.0rc1/src/dipdup/sys.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,25 @@
 import signal
 import sys
 import warnings
 from pathlib import Path
 
 from dipdup import env
 
-# NOTE: Do not try to load config for these commands as they don't need it
-IGNORE_CONFIG_CMDS = {'new', 'install', 'uninstall', 'update'}
-# NOTE: Our signal handler conflicts with Click's one in prompt mode
-IGNORE_SIGINT_CMDS = {*IGNORE_CONFIG_CMDS, None, 'schema', 'wipe'}
-
 _is_shutting_down = False
 
 
 async def _shutdown() -> None:  # pragma: no cover
     global _is_shutting_down
     if _is_shutting_down:
         return
     _is_shutting_down = True
 
     # NOTE: Prevents BrokenPipeError when piping output to another process
-    sys.stderr.close()
+    # sys.stderr.close()
 
     tasks = filter(lambda t: t != asyncio.current_task(), asyncio.all_tasks())
     list(map(asyncio.Task.cancel, tasks))
     await asyncio.gather(*tasks, return_exceptions=True)
 
 
 def is_shutting_down() -> bool:
@@ -40,28 +35,29 @@
     handler.setFormatter(formatter)
     root.addHandler(handler)
 
     # NOTE: Nothing useful there
     logging.getLogger('tortoise').setLevel(logging.WARNING)
 
 
-def set_up_process(cmd: str | None) -> None:
+def set_up_process(signals: bool) -> None:
     """Set up interpreter process-wide state"""
     # NOTE: Skip for integration tests
     if env.TEST:
         return
 
     # NOTE: Register shutdown handler for non-interactive commands (avoiding conflicts with Click prompts)
-    if cmd not in IGNORE_SIGINT_CMDS:
+    if signals:
         loop = asyncio.get_running_loop()
         loop.add_signal_handler(
             signal.SIGINT,
             lambda: asyncio.ensure_future(_shutdown()),
         )
 
     # NOTE: Better discoverability of DipDup packages and configs
     sys.path.append(str(Path.cwd()))
     sys.path.append(str(Path.cwd() / 'src'))
+    sys.path.append(str(Path.cwd() / '..'))
 
     # NOTE: Format warnings as normal log messages
     logging.captureWarnings(True)
     warnings.formatwarning = lambda msg, *a, **kw: str(msg)
```

### Comparing `dipdup-6.5.9/src/dipdup/yaml.py` & `dipdup-7.0.0rc1/src/dipdup/yaml.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,34 +9,33 @@
 - Environment variables substitution (e.g. `${FOO}` -> `bar`)
 - Merging config from multiple files (currently, only first level deep)
 - Resolving aliases and references to remove `str` from union types
 """
 
 from __future__ import annotations
 
-import json
 import logging.config
 import re
 from copy import copy
 from io import StringIO
 from os import environ as env
 from pathlib import Path
 from typing import Any
 
-from pydantic.json import pydantic_encoder
 from ruamel.yaml import YAML
 
 from dipdup import __spec_version__
 from dipdup.exceptions import ConfigurationError
+from dipdup.utils import json_dumps
 
 # NOTE: ${VARIABLE:-default} | ${VARIABLE}
 ENV_VARIABLE_REGEX = r'\$\{(?P<var_name>[\w]+)(?:\:\-(?P<default_value>.*?))?\}'
 
 
-_logger = logging.getLogger('dipdup.yaml')
+_logger = logging.getLogger(__name__)
 
 
 def exclude_none(config_json: Any) -> Any:
     if isinstance(config_json, (list, tuple)):
         return [exclude_none(i) for i in config_json if i is not None]
     if isinstance(config_json, dict):
         return {k: exclude_none(v) for k, v in config_json.items() if v is not None}
@@ -44,39 +43,76 @@
 
 
 def filter_comments(line: str) -> bool:
     return '#' not in line or line.lstrip()[0] != '#'
 
 
 def read_config_yaml(path: Path) -> str:
-    _logger.debug('Loading config from %s', path)
+    _logger.debug('Discovering config `%s`', path)
+    if path.is_dir():
+        path /= 'dipdup.yaml'
+
+    yml_path = path.with_suffix('.yml')
+    yaml_path = path.with_suffix('.yaml')
+    if path.is_file():
+        pass
+    elif yml_path.is_file():
+        path = yml_path
+    elif yaml_path.is_file():
+        path = yaml_path
+    else:
+        raise ConfigurationError(f'Config file `{path}` is missing.')
+
+    _logger.debug('Loading config file `%s`', path)
     try:
-        with open(path) as file:
+        with path.open() as file:
             return ''.join(filter(filter_comments, file.readlines()))
     except OSError as e:
-        raise ConfigurationError(f'Config file `{path}` is missing or not readable.') from e
+        raise ConfigurationError(f'Config file `{path}` is not readable: {e}') from e
+
+
+def dump(value: Any) -> str:
+    yaml = YAML(typ='unsafe', pure=True)
+    yaml.default_flow_style = False
+    yaml.indent = 2
+
+    config_json = json_dumps(value)
+    config_yaml = exclude_none(yaml.load(config_json))
+    buffer = StringIO()
+    yaml.dump(config_yaml, buffer)
+    return buffer.getvalue()
 
 
 def substitute_env_variables(config_yaml: str) -> tuple[str, dict[str, str]]:
     _logger.debug('Substituting environment variables')
     environment: dict[str, str] = {}
 
     for match in re.finditer(ENV_VARIABLE_REGEX, config_yaml):
         variable, default_value = match.group('var_name'), match.group('default_value')
         value = env.get(variable, default_value)
         # NOTE: Don't fail on ''
         if value is None:
             raise ConfigurationError(f'Environment variable `{variable}` is not set')
         environment[variable] = value
         placeholder = match.group(0)
-        config_yaml = config_yaml.replace(placeholder, value or default_value)
+        config_yaml = config_yaml.replace(placeholder, value or default_value or '')
 
     return config_yaml, environment
 
 
+def get_default_env_variables(config_yaml: str) -> dict[str, str]:
+    environment: dict[str, str] = {}
+
+    for match in re.finditer(ENV_VARIABLE_REGEX, config_yaml):
+        variable, default_value = match.group('var_name'), match.group('default_value')
+        environment[variable] = default_value or ''
+
+    return environment
+
+
 def fix_dataclass_field_aliases(config: dict[str, Any]) -> None:
     for k, v in copy(config).items():
         if 'callack' in config and k == 'from':
             config['from_'] = config.pop('from')
         elif isinstance(v, dict):
             fix_dataclass_field_aliases(v)
         elif isinstance(v, list):
@@ -99,35 +135,32 @@
 
         for path in paths:
             path_yaml = read_config_yaml(path)
 
             if environment:
                 path_yaml, path_environment = substitute_env_variables(path_yaml)
                 config_environment.update(path_environment)
+            else:
+                config_environment |= get_default_env_variables(path_yaml)
 
             config.update(yaml.load(path_yaml))
 
-        config.validate_version()
-
-        # FIXME: Can't use `from_` field alias in dataclass; fixed in dipdup.yaml instead
-        # FIXME: See https://github.com/pydantic/pydantic/issues/4286
-        fix_dataclass_field_aliases(config)
+        config._post_load_hooks()
 
         return config, config_environment
 
     def dump(self) -> str:
-        yaml = YAML(typ='unsafe', pure=True)
-        yaml.default_flow_style = False
-        yaml.indent = 2
-
-        config_json = json.dumps(self, default=pydantic_encoder)
-        config_yaml = exclude_none(yaml.load(config_json))
-        buffer = StringIO()
-        yaml.dump(config_yaml, buffer)
-        return buffer.getvalue()
+        return dump(self)
 
     def validate_version(self) -> None:
         config_spec_version = self['spec_version']
         if config_spec_version != __spec_version__:
             raise ConfigurationError(
-                f'Incompatible spec version: expected {__spec_version__}, got {config_spec_version}. See https://docs.dipdup.io/config/spec_version'
+                f'Incompatible spec version: expected {__spec_version__}, got {config_spec_version}. See'
+                ' https://docs.dipdup.io/config/spec_version'
             )
+
+    def _post_load_hooks(self) -> None:
+        self.validate_version()
+        # FIXME: Can't use `from_` field alias in dataclass
+        # FIXME: See https://github.com/pydantic/pydantic/issues/4286 (fixed in upcoming v2)
+        fix_dataclass_field_aliases(self)
```

