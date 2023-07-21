# Comparing `tmp/taipy-gui-2.4.0.dev0.tar.gz` & `tmp/taipy-gui-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-gui-2.4.0.dev0.tar", last modified: Fri Jul 21 11:17:36 2023, max compression
+gzip compressed data, was "taipy-gui-3.0.0.dev0.tar", last modified: Fri Jun 23 10:28:46 2023, max compression
```

## Comparing `taipy-gui-2.4.0.dev0.tar` & `taipy-gui-3.0.0.dev0.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.392567 taipy-gui-2.4.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-21 11:17:36.392567 taipy-gui-2.4.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:17:36.392567 taipy-gui-2.4.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-21 11:12:41.000000 taipy-gui-2.4.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.356567 taipy-gui-2.4.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.360566 taipy-gui-2.4.0.dev0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.360566 taipy-gui-2.4.0.dev0/src/taipy/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/_gui_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/_gui_section.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.364567 taipy-gui-2.4.0.dev0/src/taipy/gui/data/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/array_dict_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/content_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/data_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.364567 taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/lttb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/minmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/rdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/scatter_decimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/numpy_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/pandas_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.364567 taipy-gui-2.4.0.dev0/src/taipy/gui/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/extension/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    92274 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/gui_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/partial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.364567 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.364567 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_html/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_html/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_html/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.364567 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/blocproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/postproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    41961 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.372567 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_locals_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_map_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_runtime_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_variable_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/chart_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/clientvarname.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/expr_var_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/filename.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/filter_locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/get_imported_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/get_module_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/getdatecolstrname.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/is_debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/isnotebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/table_col_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/utils/varnamefromcontent.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/version.json
--rw-r--r--   0 runner    (1001) docker     (123)    56267 2023-07-21 11:12:34.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/viselements.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.384567 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-21 11:16:37.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/227.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)   204350 2023-07-21 11:16:37.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/499.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)  3591394 2023-07-21 11:16:37.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-21 11:16:37.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.384567 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.384567 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/base/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/base/fontfaces.css
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/base/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.384567 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/blocks/layout.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.388567 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/button.css
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/date.css
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/expandable.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/image.css
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/input.css
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/navbar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/number.css
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/selector.css
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/slider.css
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/table.css
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/toggle.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.388567 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/elements/card.css
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/elements/container.css
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/elements/header.css
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/elements/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/stylekit.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.388567 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/utilities/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/utilities/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/utilities/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/utilities/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.392567 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/elements.css
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/shapes.css
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/typography.css
--rw-r--r--   0 runner    (1001) docker     (123)   218114 2023-07-21 11:14:07.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)  5259716 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-21 11:14:07.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui-dom.js
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)  1085537 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-21 11:16:37.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 11:17:28.000000 taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy.status.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:17:36.392567 taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-21 11:17:36.000000 taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-21 11:17:36.000000 taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:17:36.000000 taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:17:29.000000 taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-21 11:17:36.000000 taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 11:17:36.000000 taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.955158 taipy-gui-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-23 10:28:46.955158 taipy-gui-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:28:46.955158 taipy-gui-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-23 10:24:33.000000 taipy-gui-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.927158 taipy-gui-3.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.927158 taipy-gui-3.0.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.927158 taipy-gui-3.0.0.dev0/src/taipy/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_gui_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_gui_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/array_dict_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/content_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/lttb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/scatter_decimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/numpy_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16809 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/pandas_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/extension/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92173 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/gui_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/partial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.931158 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/blocproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/postproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41961 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.935158 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_locals_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_map_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_runtime_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_variable_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/chart_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/clientvarname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/expr_var_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/filter_locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/get_imported_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/get_module_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/getdatecolstrname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/is_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/isnotebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/table_col_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/utils/varnamefromcontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56267 2023-06-23 10:24:22.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/viselements.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.947158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/227.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)   204350 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/499.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3591394 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.947158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/fontfaces.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/blocks/layout.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/button.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/date.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/expandable.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/image.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/number.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/selector.css
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/toggle.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/card.css
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/container.css
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/header.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/stylekit.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.951158 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/elements.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/shapes.css
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/typography.css
+-rw-r--r--   0 runner    (1001) docker     (123)   218114 2023-06-23 10:25:50.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5259716 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-23 10:25:50.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-dom.js
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)  1085146 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-23 10:27:57.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-23 10:28:39.000000 taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy.status.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:46.955158 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:28:40.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 10:28:46.000000 taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/top_level.txt
```

### Comparing `taipy-gui-2.4.0.dev0/LICENSE` & `taipy-gui-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/PKG-INFO` & `taipy-gui-3.0.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-gui-2.4.0.dev0/README.md` & `taipy-gui-3.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/setup.py` & `taipy-gui-3.0.0.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,23 +29,23 @@
         version_string = f"{version_string}.{vext}"
 
 requirements = [
     "flask>=2.2,<2.3",
     "flask-cors>=3.0.10,<4.0",
     "flask-socketio>=5.3.0,<6.0",
     "markdown>=3.4.1,<4.0",
-    "pandas>=2.0.0,<3.0",
+    "pandas>=1.5.1,<2.0",
     "python-dotenv>=0.19,<0.21",
     "pytz>=2021.3,<2022.2",
     "tzlocal>=3.0,<5.0",
     "backports.zoneinfo>=0.2.1,<0.3;python_version<'3.9'",
     "gevent>=22.10.2,<23.0",
     "gevent-websocket>=0.10.1,<0.11",
     "kthread>=0.2.3,<0.3",
-    "taipy-config==2.4.0.dev0",
+    "taipy-config==3.0.0.dev0",
     "gitignore-parser>=0.1,<0.2",
     "simple-websocket>=0.9,<1.0",
     "twisted>=22.10",
 ]
 
 test_requirements = ["pytest>=3.8"]
```

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/_default_config.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/_default_config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/_gui_cli.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/_gui_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/_gui_section.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/_gui_section.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/_init.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/_page.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/_page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/config.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/array_dict_data_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/array_dict_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/content_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/content_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/data_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/data_format.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_format.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/data_scope.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/data_scope.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/lttb.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/lttb.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/minmax.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/minmax.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/rdp.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/rdp.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/decimator/scatter_decimator.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/decimator/scatter_decimator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/numpy_data_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/numpy_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/pandas_data_accessor.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/pandas_data_accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,21 +194,14 @@
         elif isinstance(value, list):
             ret_dict: t.Dict[str, str] = {}
             for i, v in enumerate(value):
                 ret_dict.update({f"{i}/{k}": v for k, v in v.dtypes.apply(lambda x: x.name).items()})
             return ret_dict
         return None
 
-    @staticmethod
-    def __add_index_col(value: pd.DataFrame, columns: t.List[str]):
-        if _PandasDataAccessor.__INDEX_COL not in value.columns:
-            value[_PandasDataAccessor.__INDEX_COL] = value.index
-        if _PandasDataAccessor.__INDEX_COL not in columns:
-            columns.append(_PandasDataAccessor.__INDEX_COL)
-
     def __get_data(  # noqa: C901
         self,
         gui: Gui,
         var_name: str,
         value: pd.DataFrame,
         payload: t.Dict[str, t.Any],
         data_format: _DataFormat,
@@ -234,15 +227,14 @@
                     vars.append(val)
                 val = f"@vars[{len(vars) - 1}]" if isinstance(val, (str, datetime)) else val
                 right = f".str.contains({val})" if action == "contains" else f" {action} {val}"
                 if query:
                     query += " and "
                 query += f"`{col}`{right}"
             try:
-                self.__add_index_col(value, columns)
                 value = value.query(query)
             except Exception as e:
                 _warn(f"Dataframe filtering: invalid query '{query}' on {value.head()}:\n{e}")
 
         if paged:
             aggregates = payload.get("aggregates")
             applies = payload.get("applies")
@@ -291,15 +283,18 @@
                     if value.columns.dtype.name == "int64":
                         order_by = int(order_by)
                     new_indexes = value[order_by].values.argsort(axis=0)
                     if payload.get("sort") == "desc":
                         # reverse order
                         new_indexes = new_indexes[::-1]
                     new_indexes = new_indexes[slice(start, end + 1)]
-                    self.__add_index_col(value, columns)
+                    if _PandasDataAccessor.__INDEX_COL not in value.columns:
+                        value[_PandasDataAccessor.__INDEX_COL] = value.index
+                    if _PandasDataAccessor.__INDEX_COL not in columns:
+                        columns.append(_PandasDataAccessor.__INDEX_COL)
                 except Exception:
                     _warn(f"Cannot sort {var_name} on columns {order_by}.")
                     new_indexes = slice(start, end + 1)  # type: ignore
             else:
                 new_indexes = slice(start, end + 1)  # type: ignore
             value = self.__build_transferred_cols(
                 gui, columns, value.iloc[new_indexes], styles=payload.get("styles"), tooltips=payload.get("tooltips")
```

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/data/utils.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/data/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/extension/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/extension/library.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/extension/library.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/gui.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,19 +273,25 @@
                 If this argument is set, this `Gui` instance will use the value of this argument
                 as the underlying server. If omitted or set to None, this `Gui` will create its
                 own Flask application instance and use it to serve the pages.
         """
         # store suspected local containing frame
         self.__frame = t.cast(FrameType, t.cast(FrameType, inspect.currentframe()).f_back)
         self.__default_module_name = _get_module_name_from_frame(self.__frame)
-        self._set_css_file(css_file)
 
         # Preserve server config for server initialization
         self._path_mapping = path_mapping
         self._flask = flask
+        if css_file is None:
+            script_file = pathlib.Path(self.__frame.f_code.co_filename or ".").resolve()
+            if script_file.with_suffix(".css").exists():
+                css_file = f"{script_file.stem}.css"
+            elif script_file.is_dir() and (script_file / "taipy.css").exists():
+                css_file = "taipy.css"
+        self.__css_file = css_file
 
         self._config = _Config()
         self.__content_accessor = None
         self._accessors = _DataAccessors()
         self.__state: t.Optional[State] = None
         self.__bindings = _Bindings(self)
         self.__locals_context = _LocalsContext()
@@ -1690,23 +1696,14 @@
 
     def _set_frame(self, frame: FrameType):
         if not isinstance(frame, FrameType):  # pragma: no cover
             raise RuntimeError("frame must be a FrameType where Gui can collect the local variables.")
         self.__frame = frame
         self.__default_module_name = _get_module_name_from_frame(self.__frame)
 
-    def _set_css_file(self, css_file: t.Optional[str] = None):
-        if css_file is None:
-            script_file = pathlib.Path(self.__frame.f_code.co_filename or ".").resolve()
-            if script_file.with_suffix(".css").exists():
-                css_file = f"{script_file.stem}.css"
-            elif script_file.is_dir() and (script_file / "taipy.css").exists():
-                css_file = "taipy.css"
-        self.__css_file = css_file
-
     def _set_state(self, state: State):
         if isinstance(state, State):
             self.__state = state
 
     def __get_client_config(self) -> t.Dict[str, t.Any]:
         config = {
             "timeZone": self._config.get_time_zone(),
```

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/gui_actions.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/gui_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,19 +139,19 @@
     a path at run-time that, when queried, will deliver some user-defined content defined in the
     *on_user_content* callback (see the description of the `Gui^` class for more information).
 
     Arguments:
         state (State^): The current user state as received in any callback.
         path: An optional additional path to the URL.
         params: An optional dictionary sent to the *on_user_content* callback.<br/>
-            These arguments are added as query parameters to the generated URL and converted into
-            strings.
+           These arguments are added as query parameters to the generated URL and converted into
+           strings.
 
     Returns:
-        An URL that, when queried, triggers the *on_user_content* callback.
+        An URL that, when queried, triggers the `on_user_content()^` callback.
     """
     if state and isinstance(state._gui, Gui):
         return state._gui._get_user_content_url(path, params)
     _warn("'get_user_content_url()' must be called in the context of a callback.")
     return None
```

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/icon.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/icon.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/page.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/partial.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/partial.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_html/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_html/factory.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_html/parser.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_html/parser.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/blocproc.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/blocproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/control.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/control.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/factory.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/postproc.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/postproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/_markdown/preproc.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/_markdown/preproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/builder.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/factory.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/json.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/json.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/renderers/utils.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/renderers/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/server.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/server.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/state.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/state.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/types.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/types.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/__init__.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_adapter.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_attributes.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_attributes.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_bindings.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_bindings.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_evaluator.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_evaluator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_locals_context.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_locals_context.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_map_dict.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_map_dict.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_runtime_manager.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_runtime_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/_variable_directory.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/_variable_directory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/boolean.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/boolean.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/chart_config_builder.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/chart_config_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/clientvarname.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/clientvarname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/datatype.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/date.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/date.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/expr_var_name.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/expr_var_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/filename.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/filename.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/filter_locals.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/filter_locals.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/get_imported_var.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/get_imported_var.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/get_module_name.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/get_module_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/getdatecolstrname.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/getdatecolstrname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/html.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/html.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/is_debugging.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/is_debugging.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/isnotebook.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/isnotebook.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/proxy.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,38 +22,38 @@
 
 from .singleton import _Singleton
 
 if t.TYPE_CHECKING:
     from ..gui import Gui
 
 
-def _modifiedHandleResponseEnd(self):
+def modifiedHandleResponseEnd(self):
     if self._finished:
         return
     self._finished = True
     with contextlib.suppress(Exception):
         self.father.finish()
     self.transport.loseConnection()
 
 
-setattr(ProxyClient, "handleResponseEnd", _modifiedHandleResponseEnd)
+setattr(ProxyClient, "handleResponseEnd", modifiedHandleResponseEnd)
 
 
-class _TaipyReverseProxyResource(Resource):
+class TaipyReverseProxyResource(Resource):
     proxyClientFactoryClass = ProxyClientFactory
 
     def __init__(self, host, path, gui: "Gui", reactor=reactor):
         Resource.__init__(self)
         self.host = host
         self.path = path
         self.reactor = reactor
         self._gui = gui
 
     def getChild(self, path, request):
-        return _TaipyReverseProxyResource(
+        return TaipyReverseProxyResource(
             self.host,
             self.path + b"/" + urlquote(path, safe=b"").encode("utf-8"),
             self._gui,
             self.reactor,
         )
 
     def _get_port(self):
@@ -83,15 +83,15 @@
         self._gui = gui
         self._is_running = False
 
     def run(self):
         if self._is_running:
             return
         self._is_running = True
-        site = Site(_TaipyReverseProxyResource(self._gui._get_config("host", "127.0.0.1"), b"", self._gui))
+        site = Site(TaipyReverseProxyResource(self._gui._get_config("host", "127.0.0.1"), b"", self._gui))
         reactor.listenTCP(self._listening_port, site)
         Thread(target=reactor.run, args=(False,)).start()
 
     def stop(self):
         if not self._is_running:
             return
         self._is_running = False
```

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/singleton.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/table_col_builder.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/table_col_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/types.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/types.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/utils/varnamefromcontent.py` & `taipy-gui-3.0.0.dev0/src/taipy/gui/utils/varnamefromcontent.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/viselements.json` & `taipy-gui-3.0.0.dev0/src/taipy/gui/viselements.json`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/227.taipy-gui.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/227.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/499.taipy-gui.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/499.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/favicon.ico` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/favicon.ico`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/favicon.png` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/favicon.png`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/index.html` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/index.html`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/base/base.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/base.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/base/fontfaces.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/fontfaces.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/base/typography.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/base/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/blocks/layout.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/blocks/layout.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/button.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/button.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/chart.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/chart.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/date.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/date.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/expandable.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/expandable.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/image.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/image.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/input.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/input.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/navbar.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/navbar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/number.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/number.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/selector.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/selector.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/slider.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/slider.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/table.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/table.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/controls/toggle.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/controls/toggle.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/elements/card.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/card.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/elements/container.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/container.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/elements/header.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/header.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/elements/sidebar.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/elements/sidebar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/stylekit.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/stylekit.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/utilities/colors.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/utilities/misc.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/utilities/spacing.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/utilities/typography.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/utilities/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/colors.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/elements.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/elements.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/misc.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/shapes.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/shapes.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/spacing.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/stylekit/variables/typography.css` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/stylekit/variables/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui-deps-manifest.json` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps-manifest.json`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui-dom.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui-dom.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui.d.ts` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.d.ts`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui.js` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -35171,24 +35171,24 @@
                     propagate: o = !0,
                     defaultValue: s = "",
                     onAction: l,
                     onChange: c,
                     multiline: u = !1,
                     linesShown: d = 5
                 } = e, [p, h] = (0, n.useState)(s), f = qd(), m = (0, n.useRef)(-1), [g] = (0, n.useState)((() => l ? (e => {
-                    const t = (e ? e.split(";").map((e => e.trim().toLowerCase())).filter((e => BS.some((t => t.toLowerCase() === e)))) : []).map((e => BS.find((t => t.toLowerCase() == e))));
+                    const t = e ? e.split(";").filter((e => BS.includes(e.trim()))).map((e => e.trim())) : [];
                     return t.length > 0 ? t : [BS[0]]
                 })(e.actionKeys) : [])), v = Yd(), b = "number" == typeof e.changeDelay && e.changeDelay >= 0 ? e.changeDelay : 300, y = Gd(e.libClassName, e.dynamicClassName, e.className), x = zd(e.active, e.defaultActive, !0), w = zd(e.hoverText, e.defaultHoverText, void 0), k = (0, n.useCallback)((e => {
                     const t = e.target.value;
                     h(t), b ? (m.current > 0 && clearTimeout(m.current), m.current = window.setTimeout((() => {
                         m.current = -1, f(Ss(a, t, v, c, o))
                     }), b)) : f(Ss(a, t, v, c, o))
                 }), [a, f, o, c, b, v]), S = (0, n.useCallback)((e => {
                     var t;
-                    if (l && !e.shiftKey && !e.ctrlKey && !e.altKey && g.includes(e.key)) {
+                    if (l && g.includes(e.key)) {
                         const n = null === (t = e.currentTarget.querySelector("input")) || void 0 === t ? void 0 : t.value;
                         b && m.current > 0 && (clearTimeout(m.current), m.current = -1, f(Ss(a, n, v, c, o))), f(Ts(i, v, l, e.key, a, n)), e.preventDefault()
                     }
                 }), [g, a, l, i, f, c, b, o, v]);
                 return (0, n.useEffect)((() => {
                     void 0 !== e.value && h(e.value)
                 }), [e.value]), (0, t.jsx)(qr, Object.assign({
@@ -43537,28 +43537,26 @@
                             }))
                         }))]
                     }))
                 };
             var WR = e => {
                 const {
                     onValidate: r,
-                    appliedFilters: i,
+                    appliedFilters: i = [],
                     columns: a,
                     colsOrder: o,
                     className: s = ""
                 } = e, [l, c] = (0, n.useState)(!1), u = (0, n.useRef)(null), [d, p] = (0, n.useState)([]), h = (0, n.useCallback)((() => c((e => !e))), []), f = (0, n.useCallback)(((e, t, n) => {
                     p((r => e > -1 ? n ? (r.splice(e, 1), [...r]) : r.map(((n, r) => r == e ? t : n)) : n ? r : [...r, t]))
                 }), []), m = (0, n.useCallback)((() => {
                     r([...d]), h()
                 }), [r, d, h]), g = (0, n.useCallback)((() => {
                     r([]), h()
                 }), [r, h]);
-                return (0, n.useEffect)((() => {
-                    a && i && p(i.filter((e => Object.values(a).some((t => t.dfid === e.col)))))
-                }), [a, i]), (0, t.jsxs)(t.Fragment, {
+                return (0, t.jsxs)(t.Fragment, {
                     children: [(0, t.jsx)(qr, Object.assign({
                         title: "Filter list"
                     }, {
                         children: (0, t.jsx)(Jr, Object.assign({
                             onClick: h,
                             size: "small",
                             ref: u,
@@ -43596,19 +43594,19 @@
                                 })]
                             })), (0, t.jsxs)(Ep, Object.assign({
                                 sx: LR
                             }, {
                                 children: [(0, t.jsx)(oe, Object.assign({
                                     endIcon: (0, t.jsx)($P.Z, {}),
                                     onClick: g,
-                                    disabled: 0 == d.length,
+                                    disabled: 0 == i.length,
                                     variant: "outlined",
                                     color: "inherit"
                                 }, {
-                                    children: `Reset list (remove applied filter${d.length>1?"s":""})`
+                                    children: `Reset list (remove applied filter${i.length>1?"s":""})`
                                 })), (0, t.jsx)(oe, Object.assign({
                                     endIcon: (0, t.jsx)(TO.Z, {}),
                                     onClick: m,
                                     disabled: 0 == d.length,
                                     variant: "outlined"
                                 }, {
                                     children: `Apply ${d.length} filter${d.length>1?"s":""}`
@@ -43742,39 +43740,38 @@
                     j.current && Array.from(j.current.cells).forEach(((e, t) => {
                         W[$[t]].widthHint = e.offsetWidth
                     }))
                 }), [W, $]);
                 const K = (0, n.useCallback)(((e, t) => (w.current.promises[e] && w.current.promises[e].reject(), new Promise(((n, a) => {
                         const o = M.length ? $.reduce(((e, t, n) => M.includes(W[t].dfid) ? e + "-" + n : e), "-agg") : "",
                             s = $.map((e => W[e].dfid)).filter((e => e != nO)),
-                            l = E.filter((e => Object.values(W).some((t => t.dfid === e.col)))),
-                            c = `Infinite-${s.join()}-${k}-${C}${o}${l.map((e=>`${e.col}${e.action}${e.value}`))}`;
+                            l = `Infinite-${s.join()}-${k}-${C}${o}`;
                         w.current = {
-                            key: c,
+                            key: l,
                             promises: Object.assign(Object.assign({}, w.current.promises), {
                                 [e]: {
                                     resolve: n,
                                     reject: a
                                 }
                             })
                         };
-                        const u = M.length ? $.reduce(((e, t) => (W[t].apply && (e[W[t].dfid] = W[t].apply), e)), {}) : void 0;
+                        const c = M.length ? $.reduce(((e, t) => (W[t].apply && (e[W[t].dfid] = W[t].apply), e)), {}) : void 0;
                         x(((e, t, n, r, i, a, o, s, l, c, u, d, p, h, f) => Ps(e, t, n, r, i, {
                             infinite: !0,
                             start: a,
                             end: o,
                             orderby: s,
                             sort: l,
                             aggregates: c,
                             applies: u,
                             styles: d,
                             tooltips: p,
                             handlenan: h,
                             filters: f
-                        }))(i, r, N, s, c, e, t, k, C, M, u, U, H, q, l))
+                        }))(i, r, N, s, l, e, t, k, C, M, c, U, H, q, E))
                     })))), [M, U, H, i, k, C, r, $, W, q, E, x, N]),
                     X = (0, n.useCallback)((() => x(Ts(i, N, {
                         action: h,
                         index: O
                     }))), [O, x, i, h, N]),
                     Q = (0, n.useCallback)((e => e < g.length && !!g[e]), [g]),
                     J = (0, n.useCallback)(((e, t, n, r) => x(Ts(i, N, {
@@ -44382,31 +44379,30 @@
                     Wd(D, r, L, u), (0, n.useEffect)((() => {
                         c.length && (c[0] < x || c[0] > x + k) && (Z(!0), w(k * Math.floor(c[0] / k)))
                     }), [c, x, k]), (0, n.useEffect)((() => {
                         e.data && void 0 !== e.data[N.current] && (y(e.data[N.current]), Z(!1))
                     }), [e.data]), (0, n.useEffect)((() => {
                         const t = s ? -1 : x + k - 1,
                             n = M.length ? U.reduce(((e, t, n) => M.includes(H[t].dfid) ? e + "-" + n : e), "-agg") : "",
-                            a = U.map((e => H[e].dfid)).filter((e => e != nO)),
-                            o = A.filter((e => Object.values(H).some((t => t.dfid === e.col))));
-                        if (N.current = `${x}-${t}-${a.join()}-${E}-${C}${n}${o.map((e=>`${e.col}${e.action}${e.value}`))}`, F || !e.data || void 0 === e.data[N.current]) {
+                            a = U.map((e => H[e].dfid)).filter((e => e != nO));
+                        if (N.current = `${x}-${t}-${a.join()}-${E}-${C}${n}${A.map((e=>`${e.col}${e.action}${e.value}`))}`, F || !e.data || void 0 === e.data[N.current]) {
                             Z(!0);
                             const e = M.length ? U.reduce(((e, t) => (H[t].apply && (e[H[t].dfid] = H[t].apply), e)), {}) : void 0;
                             D(((e, t, n, r, i, a, o, s, l, c, u, d, p, h, f) => Ps(e, t, n, r, i, {
                                 start: a,
                                 end: o,
                                 orderby: s,
                                 sort: l,
                                 aggregates: c,
                                 applies: u,
                                 styles: d,
                                 tooltips: p,
                                 handlenan: h,
                                 filters: f
-                            }))(i, r, L, a, N.current, x, t, E, C, M, e, q, Y, G, o))
+                            }))(i, r, L, a, N.current, x, t, E, C, M, e, q, Y, G, A))
                         } else y(e.data[N.current]), Z(!1)
                     }), [F, x, M, U, H, s, k, C, E, i, r, G, A, D, L]);
                     const X = (0, n.useCallback)((e => {
                             const t = e.currentTarget.getAttribute("data-dfid");
                             t && (T(E === t && "asc" === C ? "desc" : "asc"), P(t))
                         }), [E, C]),
                         Q = (0, n.useCallback)(((e, t) => {
@@ -47902,16 +47898,15 @@
                                                                     path: "*",
                                                                     element: (0, t.jsx)(GN, {})
                                                                 }, "NotFound")]
                                                             }))
                                                         }) : null
                                                     }))
                                                 })), e.ackList.length ? (0, t.jsx)(Ep, Object.assign({
-                                                    sx: QN,
-                                                    className: "taipy-busy"
+                                                    sx: QN
                                                 }, {
                                                     children: (0, t.jsx)(oD, {
                                                         size: "1em",
                                                         disableShrink: !0
                                                     })
                                                 })) : null]
                                             })), (0, t.jsxs)(Md, Object.assign({
```

### Comparing `taipy-gui-2.4.0.dev0/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt` & `taipy-gui-3.0.0.dev0/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/PKG-INFO` & `taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/SOURCES.txt` & `taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.4.0.dev0/src/taipy_gui.egg-info/requires.txt` & `taipy-gui-3.0.0.dev0/src/taipy_gui.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 flask<2.3,>=2.2
 flask-cors<4.0,>=3.0.10
 flask-socketio<6.0,>=5.3.0
 markdown<4.0,>=3.4.1
-pandas<3.0,>=2.0.0
+pandas<2.0,>=1.5.1
 python-dotenv<0.21,>=0.19
 pytz<2022.2,>=2021.3
 tzlocal<5.0,>=3.0
 gevent<23.0,>=22.10.2
 gevent-websocket<0.11,>=0.10.1
 kthread<0.3,>=0.2.3
-taipy-config==2.4.0.dev0
+taipy-config==3.0.0.dev0
 gitignore-parser<0.2,>=0.1
 simple-websocket<1.0,>=0.9
 twisted>=22.10
 
 [:python_version < "3.9"]
 backports.zoneinfo<0.3,>=0.2.1
```

