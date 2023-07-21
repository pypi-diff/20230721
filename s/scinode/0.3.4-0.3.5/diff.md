# Comparing `tmp/scinode-0.3.4.tar.gz` & `tmp/scinode-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scinode-0.3.4.tar", last modified: Tue Jul 18 15:29:40 2023, max compression
+gzip compressed data, was "dist/scinode-0.3.5.tar", last modified: Fri Jul 21 15:20:52 2023, max compression
```

## Comparing `scinode-0.3.4.tar` & `scinode-0.3.5.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.649232 scinode-0.3.4/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2022-12-06 13:50:07.000000 scinode-0.3.4/LICENSE
--rw-rw-r--   0 xing      (1000) xing      (1000)      444 2023-05-02 12:47:10.000000 scinode-0.3.4/MANIFEST.in
--rw-rw-r--   0 xing      (1000) xing      (1000)     1843 2023-07-18 15:29:40.645233 scinode-0.3.4/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     1509 2023-06-16 06:56:57.000000 scinode-0.3.4/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.613232 scinode-0.3.4/scinode/
--rw-rw-r--   0 xing      (1000) xing      (1000)      240 2023-06-19 22:26:26.000000 scinode-0.3.4/scinode/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.617232 scinode-0.3.4/scinode/app/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3661 2023-06-23 03:21:15.000000 scinode-0.3.4/scinode/app/app.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.617232 scinode-0.3.4/scinode/app/blueprints/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.617232 scinode-0.3.4/scinode/app/blueprints/component/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-06-23 03:20:16.000000 scinode-0.3.4/scinode/app/blueprints/component/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6676 2023-06-23 03:20:19.000000 scinode-0.3.4/scinode/app/blueprints/component/component.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.617232 scinode-0.3.4/scinode/app/blueprints/component/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     7092 2023-06-23 03:20:25.000000 scinode-0.3.4/scinode/app/blueprints/component/templates/component_editor.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      594 2023-06-23 03:20:27.000000 scinode-0.3.4/scinode/app/blueprints/component/templates/component_exporter.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      359 2023-06-23 03:20:28.000000 scinode-0.3.4/scinode/app/blueprints/component/templates/component_importer.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1613 2023-06-23 03:20:30.000000 scinode-0.3.4/scinode/app/blueprints/component/templates/component_table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1474 2023-06-23 03:20:23.000000 scinode-0.3.4/scinode/app/blueprints/component/utils.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.617232 scinode-0.3.4/scinode/app/blueprints/config/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/config/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2644 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/config/config.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.617232 scinode-0.3.4/scinode/app/blueprints/config/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     4699 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/app/blueprints/config/templates/config.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      739 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/config/templates/daemon_logfile.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.617232 scinode-0.3.4/scinode/app/blueprints/data/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/data/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2371 2023-06-23 12:59:21.000000 scinode-0.3.4/scinode/app/blueprints/data/data.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.617232 scinode-0.3.4/scinode/app/blueprints/data/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)      800 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/data/templates/data_table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1265 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/data/templates/data_viewer.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.617232 scinode-0.3.4/scinode/app/blueprints/node/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/node/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3607 2023-07-04 16:50:55.000000 scinode-0.3.4/scinode/app/blueprints/node/node.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.621232 scinode-0.3.4/scinode/app/blueprints/node/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1717 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/node/templates/node_table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2715 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/node/templates/node_viewer.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.621232 scinode-0.3.4/scinode/app/blueprints/nodetree/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7694 2023-07-04 16:50:55.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/nodetree.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.621232 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     4081 2023-06-22 16:37:56.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/nodetree_editor.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      605 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/nodetree_exporter.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      359 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/nodetree_importer.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2079 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/nodetree_table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2930 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/nodetree_viewer.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      249 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/tab-description.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     6594 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/tab-graph-sidebar.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1545 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/tab-graph.html
--rw-rw-r--   0 xing      (1000) xing      (1000)      789 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/tab-table.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1036 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/templates/tab.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     1807 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/app/blueprints/nodetree/utils.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.621232 scinode-0.3.4/scinode/app/blueprints/scheduler/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/scheduler/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      738 2023-06-23 12:59:21.000000 scinode-0.3.4/scinode/app/blueprints/scheduler/scheduler.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.621232 scinode-0.3.4/scinode/app/blueprints/scheduler/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/scheduler/templates/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.621232 scinode-0.3.4/scinode/app/blueprints/template/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/template/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2361 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/template/template.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.621232 scinode-0.3.4/scinode/app/blueprints/template/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1757 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/blueprints/template/templates/template_table.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.621232 scinode-0.3.4/scinode/app/cli/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/cli/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.621232 scinode-0.3.4/scinode/app/cli/commands/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/cli/commands/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1451 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/cli/commands/plugin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1971 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/app/cli/commands/web.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8290 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/app/db.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      428 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/app/init_data.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.625233 scinode-0.3.4/scinode/app/static/
--rw-rw-r--   0 xing      (1000) xing      (1000)      345 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/static/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.625233 scinode-0.3.4/scinode/app/static/__pycache__/
--rw-rw-r--   0 xing      (1000) xing      (1000)      555 2023-05-05 04:32:32.000000 scinode-0.3.4/scinode/app/static/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 xing      (1000) xing      (1000)    14636 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/static/component_editor.js
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.625233 scinode-0.3.4/scinode/app/static/components/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/static/components/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.625233 scinode-0.3.4/scinode/app/static/components/__pycache__/
--rw-rw-r--   0 xing      (1000) xing      (1000)      170 2023-05-01 07:20:25.000000 scinode-0.3.4/scinode/app/static/components/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 xing      (1000) xing      (1000)    24254 2023-06-23 12:59:21.000000 scinode-0.3.4/scinode/app/static/components/app_components.js
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.625233 scinode-0.3.4/scinode/app/static/controls/
--rw-rw-r--   0 xing      (1000) xing      (1000)    21168 2023-06-23 12:59:21.000000 scinode-0.3.4/scinode/app/static/controls/app_controls.js
--rw-rw-r--   0 xing      (1000) xing      (1000)      950 2023-06-23 12:59:21.000000 scinode-0.3.4/scinode/app/static/init_editor.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     5620 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/static/json_components.js
--rw-rw-r--   0 xing      (1000) xing      (1000)    22329 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/static/logo.png
--rw-rw-r--   0 xing      (1000) xing      (1000)    10849 2023-06-23 12:59:21.000000 scinode-0.3.4/scinode/app/static/nodetree_editor.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     1572 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/static/nodetree_node_table.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     7589 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/static/scinode_components.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     2639 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/app/static/scinode_editor.js
--rw-rw-r--   0 xing      (1000) xing      (1000)      759 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/static/sidebar.js
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.625233 scinode-0.3.4/scinode/app/static/sockets/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1276 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/static/sockets/app_sockets.js
--rw-rw-r--   0 xing      (1000) xing      (1000)     3501 2023-06-23 12:59:21.000000 scinode-0.3.4/scinode/app/static/styles.css
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.625233 scinode-0.3.4/scinode/app/templates/
--rw-rw-r--   0 xing      (1000) xing      (1000)     3713 2023-06-23 03:20:54.000000 scinode-0.3.4/scinode/app/templates/base.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2371 2023-06-23 03:20:52.000000 scinode-0.3.4/scinode/app/templates/base_editor.html
--rw-rw-r--   0 xing      (1000) xing      (1000)     2065 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/templates/index.html
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.625233 scinode-0.3.4/scinode/app/utils/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1020 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/app/utils/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     7820 2023-07-04 16:50:55.000000 scinode-0.3.4/scinode/app/utils/rete_adapter.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.629233 scinode-0.3.4/scinode/cli/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.4/scinode/cli/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.629233 scinode-0.3.4/scinode/cli/commands/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.4/scinode/cli/commands/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2011 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/cli/commands/computer.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1756 2023-04-17 08:55:44.000000 scinode-0.3.4/scinode/cli/commands/data.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      665 2023-04-18 11:52:21.000000 scinode-0.3.4/scinode/cli/commands/mq.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    12475 2023-06-08 03:15:13.000000 scinode-0.3.4/scinode/cli/commands/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8471 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/cli/commands/nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3319 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/cli/commands/profile.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3497 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/cli/commands/scheduler.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1249 2023-06-21 11:00:22.000000 scinode-0.3.4/scinode/cli/commands/shell.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8666 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/cli/commands/worker.py
--rwxrwxr-x   0 xing      (1000) xing      (1000)     4570 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/cli/main.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.629233 scinode-0.3.4/scinode/common/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/common/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1034 2023-06-30 06:08:15.000000 scinode-0.3.4/scinode/common/log.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.629233 scinode-0.3.4/scinode/config/
--rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/config/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2584 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/config/base_config.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      611 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/config/computer.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1882 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/config/profile.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.633232 scinode-0.3.4/scinode/core/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-03-20 09:18:35.000000 scinode-0.3.4/scinode/core/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    10793 2023-06-19 08:05:52.000000 scinode-0.3.4/scinode/core/collection.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1733 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/core/executor.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3570 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/core/link.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    26023 2023-07-18 09:41:39.000000 scinode-0.3.4/scinode/core/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    16705 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/core/nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3412 2023-06-15 06:06:55.000000 scinode-0.3.4/scinode/core/property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4392 2023-07-04 16:50:55.000000 scinode-0.3.4/scinode/core/socket.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.633232 scinode-0.3.4/scinode/daemon/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.4/scinode/daemon/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4635 2023-04-21 13:20:34.000000 scinode-0.3.4/scinode/daemon/daemon.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1675 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/daemon/scheduler.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      440 2023-04-28 02:27:11.000000 scinode-0.3.4/scinode/daemon/scheduler_config.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5426 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/daemon/worker.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2819 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/daemon/worker_config.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.633232 scinode-0.3.4/scinode/database/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.4/scinode/database/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      530 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/database/client.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2081 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/database/data.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1514 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/database/db.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3652 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/database/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8140 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/database/nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.4/scinode/database/utils.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4250 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/database/worker.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.637232 scinode-0.3.4/scinode/engine/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/engine/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.637232 scinode-0.3.4/scinode/engine/celery/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-03-01 08:01:27.000000 scinode-0.3.4/scinode/engine/celery/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      154 2023-03-01 08:01:27.000000 scinode-0.3.4/scinode/engine/celery/app.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      708 2023-03-01 08:01:27.000000 scinode-0.3.4/scinode/engine/celery/base.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      296 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/engine/celery/celery_config.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6674 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/engine/celery/tasks.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2250 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/engine/celery/worker.py
--rw-rw-r--   0 xing      (1000) xing      (1000)       32 2023-04-21 13:20:34.000000 scinode-0.3.4/scinode/engine/config.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    30817 2023-06-19 22:26:26.000000 scinode-0.3.4/scinode/engine/local_run.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4218 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/engine/mq.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11266 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/engine/node_engine.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    30817 2023-06-19 09:08:54.000000 scinode-0.3.4/scinode/engine/nodetree_engine.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11981 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/engine/nodetree_launch.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3688 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/engine/scheduler.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1958 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/engine/send_to_queue.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6494 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/engine/worker.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.637232 scinode-0.3.4/scinode/executors/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.4/scinode/executors/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1140 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/executors/bash_executor.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4047 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/executors/built_in.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.641233 scinode-0.3.4/scinode/executors/controls/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.4/scinode/executors/controls/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1646 2023-06-21 11:00:22.000000 scinode-0.3.4/scinode/executors/controls/for_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1692 2023-06-21 11:00:22.000000 scinode-0.3.4/scinode/executors/controls/if_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4573 2023-06-21 11:00:22.000000 scinode-0.3.4/scinode/executors/controls/scatter_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1398 2023-06-21 11:00:22.000000 scinode-0.3.4/scinode/executors/controls/switch_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1819 2023-06-21 11:00:22.000000 scinode-0.3.4/scinode/executors/controls/update_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1397 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/executors/folder_manager.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3291 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/executors/hpc_scheduler.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     4131 2023-06-23 12:59:21.000000 scinode-0.3.4/scinode/executors/python.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.641233 scinode-0.3.4/scinode/executors/ssh/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/executors/ssh/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     6614 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/executors/ssh/ssh_client.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5305 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/executors/ssh/ssh_executor.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5087 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/executors/ssh/ssh_python_executor.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1363 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/executors/ssh/test_ssh_executor.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3542 2023-07-17 11:40:00.000000 scinode-0.3.4/scinode/executors/test.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      133 2023-06-08 03:15:13.000000 scinode-0.3.4/scinode/executors/utils.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.641233 scinode-0.3.4/scinode/nodes/
--rw-rw-r--   0 xing      (1000) xing      (1000)      122 2022-12-23 08:17:58.000000 scinode-0.3.4/scinode/nodes/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      912 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/nodes/bash_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5623 2023-02-14 21:05:04.000000 scinode-0.3.4/scinode/nodes/build_node_from_database.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      986 2023-06-19 08:05:52.000000 scinode-0.3.4/scinode/nodes/built_in.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5076 2023-06-19 08:05:52.000000 scinode-0.3.4/scinode/nodes/control.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1289 2023-02-14 20:38:16.000000 scinode-0.3.4/scinode/nodes/node_from_database.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    23404 2023-06-21 11:00:22.000000 scinode-0.3.4/scinode/nodes/numpy_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    14377 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/nodes/python_builtin.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     9202 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/nodes/test.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3234 2023-06-16 06:56:57.000000 scinode-0.3.4/scinode/nodes/test_node_group.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      773 2023-06-16 06:56:57.000000 scinode-0.3.4/scinode/nodes/utils.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.645233 scinode-0.3.4/scinode/orm/
--rw-rw-r--   0 xing      (1000) xing      (1000)     5674 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/orm/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      687 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/orm/data.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8770 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/orm/db_node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    12720 2023-06-19 22:26:26.000000 scinode-0.3.4/scinode/orm/db_nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1654 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/orm/db_property.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2852 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/orm/db_socket.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     5294 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/orm/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2932 2023-06-25 08:59:23.000000 scinode-0.3.4/scinode/orm/nodetree.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.645233 scinode-0.3.4/scinode/properties/
--rw-rw-r--   0 xing      (1000) xing      (1000)      140 2022-12-23 08:17:58.000000 scinode-0.3.4/scinode/properties/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    11952 2023-07-04 16:50:55.000000 scinode-0.3.4/scinode/properties/built_in.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.645233 scinode-0.3.4/scinode/serialization/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-02-10 18:56:33.000000 scinode-0.3.4/scinode/serialization/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1595 2023-03-20 09:18:35.000000 scinode-0.3.4/scinode/serialization/built_in.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.645233 scinode-0.3.4/scinode/sockets/
--rw-rw-r--   0 xing      (1000) xing      (1000)      128 2022-12-23 08:17:58.000000 scinode-0.3.4/scinode/sockets/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3343 2023-06-19 08:05:52.000000 scinode-0.3.4/scinode/sockets/built_in.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.645233 scinode-0.3.4/scinode/utils/
--rw-rw-r--   0 xing      (1000) xing      (1000)     2116 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/utils/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      935 2023-04-21 13:20:34.000000 scinode-0.3.4/scinode/utils/daemon.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2413 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/utils/db.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8816 2023-07-17 12:00:23.000000 scinode-0.3.4/scinode/utils/decorator.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1089 2023-04-28 02:27:11.000000 scinode-0.3.4/scinode/utils/emoji.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      565 2023-04-21 13:20:34.000000 scinode-0.3.4/scinode/utils/formater.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    18292 2023-07-17 11:40:05.000000 scinode-0.3.4/scinode/utils/node.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     8018 2023-06-15 06:21:11.000000 scinode-0.3.4/scinode/utils/nodetree.py
--rw-rw-r--   0 xing      (1000) xing      (1000)    12630 2023-06-16 06:56:57.000000 scinode-0.3.4/scinode/utils/nt_analysis.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      977 2023-05-02 12:47:10.000000 scinode-0.3.4/scinode/utils/process.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-06-19 08:05:52.000000 scinode-0.3.4/scinode/version.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-18 15:29:40.613232 scinode-0.3.4/scinode.egg-info/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1843 2023-07-18 15:29:40.000000 scinode-0.3.4/scinode.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     6567 2023-07-18 15:29:40.000000 scinode-0.3.4/scinode.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2023-07-18 15:29:40.000000 scinode-0.3.4/scinode.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)     1071 2023-07-18 15:29:40.000000 scinode-0.3.4/scinode.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      188 2023-07-18 15:29:40.000000 scinode-0.3.4/scinode.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        8 2023-07-18 15:29:40.000000 scinode-0.3.4/scinode.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2023-07-18 15:29:40.649232 scinode-0.3.4/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     2857 2023-07-18 15:29:38.000000 scinode-0.3.4/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.814226 scinode-0.3.5/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1064 2022-12-06 13:50:07.000000 scinode-0.3.5/LICENSE
+-rw-rw-r--   0 xing      (1000) xing      (1000)      444 2023-05-02 12:47:10.000000 scinode-0.3.5/MANIFEST.in
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1843 2023-07-21 15:20:52.814226 scinode-0.3.5/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1509 2023-06-16 06:56:57.000000 scinode-0.3.5/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.778226 scinode-0.3.5/scinode/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      240 2023-06-19 22:26:26.000000 scinode-0.3.5/scinode/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode/app/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3661 2023-06-23 03:21:15.000000 scinode-0.3.5/scinode/app/app.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode/app/blueprints/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode/app/blueprints/component/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-06-23 03:20:16.000000 scinode-0.3.5/scinode/app/blueprints/component/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6676 2023-06-23 03:20:19.000000 scinode-0.3.5/scinode/app/blueprints/component/component.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode/app/blueprints/component/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7092 2023-06-23 03:20:25.000000 scinode-0.3.5/scinode/app/blueprints/component/templates/component_editor.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      594 2023-06-23 03:20:27.000000 scinode-0.3.5/scinode/app/blueprints/component/templates/component_exporter.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      359 2023-06-23 03:20:28.000000 scinode-0.3.5/scinode/app/blueprints/component/templates/component_importer.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1613 2023-06-23 03:20:30.000000 scinode-0.3.5/scinode/app/blueprints/component/templates/component_table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1474 2023-06-23 03:20:23.000000 scinode-0.3.5/scinode/app/blueprints/component/utils.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode/app/blueprints/config/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/config/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2644 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/config/config.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode/app/blueprints/config/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4699 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/app/blueprints/config/templates/config.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      739 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/config/templates/daemon_logfile.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode/app/blueprints/data/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/data/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2371 2023-06-23 12:59:21.000000 scinode-0.3.5/scinode/app/blueprints/data/data.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode/app/blueprints/data/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      800 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/data/templates/data_table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1265 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/data/templates/data_viewer.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode/app/blueprints/node/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/node/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3607 2023-07-04 16:50:55.000000 scinode-0.3.5/scinode/app/blueprints/node/node.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.786226 scinode-0.3.5/scinode/app/blueprints/node/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1717 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/node/templates/node_table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2715 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/node/templates/node_viewer.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.786226 scinode-0.3.5/scinode/app/blueprints/nodetree/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7694 2023-07-04 16:50:55.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/nodetree.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.786226 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4081 2023-06-22 16:37:56.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/nodetree_editor.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      605 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/nodetree_exporter.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      359 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/nodetree_importer.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2079 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/nodetree_table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2930 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/nodetree_viewer.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      249 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/tab-description.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6594 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/tab-graph-sidebar.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1545 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/tab-graph.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)      789 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/tab-table.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1036 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/templates/tab.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1807 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/app/blueprints/nodetree/utils.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.786226 scinode-0.3.5/scinode/app/blueprints/scheduler/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/scheduler/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      738 2023-06-23 12:59:21.000000 scinode-0.3.5/scinode/app/blueprints/scheduler/scheduler.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.786226 scinode-0.3.5/scinode/app/blueprints/scheduler/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/scheduler/templates/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.786226 scinode-0.3.5/scinode/app/blueprints/template/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/template/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2361 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/template/template.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.786226 scinode-0.3.5/scinode/app/blueprints/template/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1757 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/blueprints/template/templates/template_table.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.786226 scinode-0.3.5/scinode/app/cli/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/cli/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.786226 scinode-0.3.5/scinode/app/cli/commands/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/cli/commands/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1451 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/cli/commands/plugin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1971 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/app/cli/commands/web.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8290 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/app/db.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      428 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/app/init_data.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.790226 scinode-0.3.5/scinode/app/static/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      345 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/static/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.790226 scinode-0.3.5/scinode/app/static/__pycache__/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      555 2023-05-05 04:32:32.000000 scinode-0.3.5/scinode/app/static/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 xing      (1000) xing      (1000)    14636 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/static/component_editor.js
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.790226 scinode-0.3.5/scinode/app/static/components/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/static/components/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.790226 scinode-0.3.5/scinode/app/static/components/__pycache__/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      170 2023-05-01 07:20:25.000000 scinode-0.3.5/scinode/app/static/components/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 xing      (1000) xing      (1000)    24254 2023-06-23 12:59:21.000000 scinode-0.3.5/scinode/app/static/components/app_components.js
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.790226 scinode-0.3.5/scinode/app/static/controls/
+-rw-rw-r--   0 xing      (1000) xing      (1000)    21168 2023-06-23 12:59:21.000000 scinode-0.3.5/scinode/app/static/controls/app_controls.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)      950 2023-06-23 12:59:21.000000 scinode-0.3.5/scinode/app/static/init_editor.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5620 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/static/json_components.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)    22329 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/static/logo.png
+-rw-rw-r--   0 xing      (1000) xing      (1000)    10849 2023-06-23 12:59:21.000000 scinode-0.3.5/scinode/app/static/nodetree_editor.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1572 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/static/nodetree_node_table.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7589 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/static/scinode_components.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2639 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/app/static/scinode_editor.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)      759 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/static/sidebar.js
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.790226 scinode-0.3.5/scinode/app/static/sockets/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1276 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/static/sockets/app_sockets.js
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3501 2023-06-23 12:59:21.000000 scinode-0.3.5/scinode/app/static/styles.css
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.790226 scinode-0.3.5/scinode/app/templates/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3713 2023-06-23 03:20:54.000000 scinode-0.3.5/scinode/app/templates/base.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2371 2023-06-23 03:20:52.000000 scinode-0.3.5/scinode/app/templates/base_editor.html
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2065 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/templates/index.html
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.790226 scinode-0.3.5/scinode/app/utils/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1020 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/app/utils/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     7820 2023-07-04 16:50:55.000000 scinode-0.3.5/scinode/app/utils/rete_adapter.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.790226 scinode-0.3.5/scinode/cli/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.5/scinode/cli/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.794226 scinode-0.3.5/scinode/cli/commands/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.5/scinode/cli/commands/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2011 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/cli/commands/computer.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1756 2023-04-17 08:55:44.000000 scinode-0.3.5/scinode/cli/commands/data.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      665 2023-04-18 11:52:21.000000 scinode-0.3.5/scinode/cli/commands/mq.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    12475 2023-06-08 03:15:13.000000 scinode-0.3.5/scinode/cli/commands/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8471 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/cli/commands/nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3319 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/cli/commands/profile.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3497 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/cli/commands/scheduler.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1249 2023-06-21 11:00:22.000000 scinode-0.3.5/scinode/cli/commands/shell.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8666 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/cli/commands/worker.py
+-rwxrwxr-x   0 xing      (1000) xing      (1000)     4570 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/cli/main.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.794226 scinode-0.3.5/scinode/common/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/common/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1034 2023-06-30 06:08:15.000000 scinode-0.3.5/scinode/common/log.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.794226 scinode-0.3.5/scinode/config/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      616 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/config/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2584 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/config/base_config.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      611 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/config/computer.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1882 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/config/profile.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.798226 scinode-0.3.5/scinode/core/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-03-20 09:18:35.000000 scinode-0.3.5/scinode/core/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11331 2023-07-21 13:16:20.000000 scinode-0.3.5/scinode/core/collection.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1733 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/core/executor.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3570 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/core/link.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    26023 2023-07-18 09:41:39.000000 scinode-0.3.5/scinode/core/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    16705 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/core/nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3412 2023-06-15 06:06:55.000000 scinode-0.3.5/scinode/core/property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4392 2023-07-04 16:50:55.000000 scinode-0.3.5/scinode/core/socket.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.798226 scinode-0.3.5/scinode/daemon/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.5/scinode/daemon/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4635 2023-04-21 13:20:34.000000 scinode-0.3.5/scinode/daemon/daemon.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1675 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/daemon/scheduler.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      440 2023-04-28 02:27:11.000000 scinode-0.3.5/scinode/daemon/scheduler_config.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5426 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/daemon/worker.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2819 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/daemon/worker_config.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.798226 scinode-0.3.5/scinode/database/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.5/scinode/database/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      530 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/database/client.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2081 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/database/data.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1514 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/database/db.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3652 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/database/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8140 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/database/nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.5/scinode/database/utils.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4250 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/database/worker.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.802226 scinode-0.3.5/scinode/engine/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/engine/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.802226 scinode-0.3.5/scinode/engine/celery/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-03-01 08:01:27.000000 scinode-0.3.5/scinode/engine/celery/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      154 2023-03-01 08:01:27.000000 scinode-0.3.5/scinode/engine/celery/app.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      708 2023-03-01 08:01:27.000000 scinode-0.3.5/scinode/engine/celery/base.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      296 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/engine/celery/celery_config.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6674 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/engine/celery/tasks.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2250 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/engine/celery/worker.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)       32 2023-04-21 13:20:34.000000 scinode-0.3.5/scinode/engine/config.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    30817 2023-06-19 22:26:26.000000 scinode-0.3.5/scinode/engine/local_run.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4218 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/engine/mq.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11266 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/engine/node_engine.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    30817 2023-06-19 09:08:54.000000 scinode-0.3.5/scinode/engine/nodetree_engine.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11981 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/engine/nodetree_launch.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3688 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/engine/scheduler.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1958 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/engine/send_to_queue.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6494 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/engine/worker.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.802226 scinode-0.3.5/scinode/executors/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.5/scinode/executors/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1140 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/executors/bash_executor.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4047 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/executors/built_in.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.806226 scinode-0.3.5/scinode/executors/controls/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2022-12-06 13:50:07.000000 scinode-0.3.5/scinode/executors/controls/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1646 2023-06-21 11:00:22.000000 scinode-0.3.5/scinode/executors/controls/for_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1692 2023-06-21 11:00:22.000000 scinode-0.3.5/scinode/executors/controls/if_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4573 2023-06-21 11:00:22.000000 scinode-0.3.5/scinode/executors/controls/scatter_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1398 2023-06-21 11:00:22.000000 scinode-0.3.5/scinode/executors/controls/switch_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1819 2023-06-21 11:00:22.000000 scinode-0.3.5/scinode/executors/controls/update_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1397 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/executors/folder_manager.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3291 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/executors/hpc_scheduler.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     4131 2023-06-23 12:59:21.000000 scinode-0.3.5/scinode/executors/python.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.806226 scinode-0.3.5/scinode/executors/ssh/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/executors/ssh/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6614 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/executors/ssh/ssh_client.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5305 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/executors/ssh/ssh_executor.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5087 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/executors/ssh/ssh_python_executor.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1363 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/executors/ssh/test_ssh_executor.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3329 2023-07-21 13:32:06.000000 scinode-0.3.5/scinode/executors/test.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      133 2023-06-08 03:15:13.000000 scinode-0.3.5/scinode/executors/utils.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.806226 scinode-0.3.5/scinode/nodes/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      122 2022-12-23 08:17:58.000000 scinode-0.3.5/scinode/nodes/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      912 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/nodes/bash_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5623 2023-02-14 21:05:04.000000 scinode-0.3.5/scinode/nodes/build_node_from_database.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      986 2023-06-19 08:05:52.000000 scinode-0.3.5/scinode/nodes/built_in.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5076 2023-06-19 08:05:52.000000 scinode-0.3.5/scinode/nodes/control.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1289 2023-02-14 20:38:16.000000 scinode-0.3.5/scinode/nodes/node_from_database.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    23404 2023-06-21 11:00:22.000000 scinode-0.3.5/scinode/nodes/numpy_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    14377 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/nodes/python_builtin.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     9202 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/nodes/test.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3234 2023-06-16 06:56:57.000000 scinode-0.3.5/scinode/nodes/test_node_group.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      773 2023-06-16 06:56:57.000000 scinode-0.3.5/scinode/nodes/utils.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.810226 scinode-0.3.5/scinode/orm/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5674 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/orm/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      687 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/orm/data.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8770 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/orm/db_node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    12720 2023-06-19 22:26:26.000000 scinode-0.3.5/scinode/orm/db_nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1654 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/orm/db_property.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2852 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/orm/db_socket.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     5294 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/orm/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2932 2023-06-25 08:59:23.000000 scinode-0.3.5/scinode/orm/nodetree.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.810226 scinode-0.3.5/scinode/properties/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      140 2022-12-23 08:17:58.000000 scinode-0.3.5/scinode/properties/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    11952 2023-07-04 16:50:55.000000 scinode-0.3.5/scinode/properties/built_in.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.810226 scinode-0.3.5/scinode/serialization/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2023-02-10 18:56:33.000000 scinode-0.3.5/scinode/serialization/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1595 2023-03-20 09:18:35.000000 scinode-0.3.5/scinode/serialization/built_in.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.810226 scinode-0.3.5/scinode/sockets/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      128 2022-12-23 08:17:58.000000 scinode-0.3.5/scinode/sockets/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3343 2023-06-19 08:05:52.000000 scinode-0.3.5/scinode/sockets/built_in.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.814226 scinode-0.3.5/scinode/utils/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2116 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/utils/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      935 2023-04-21 13:20:34.000000 scinode-0.3.5/scinode/utils/daemon.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2413 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/utils/db.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     9054 2023-07-21 13:16:20.000000 scinode-0.3.5/scinode/utils/decorator.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1089 2023-04-28 02:27:11.000000 scinode-0.3.5/scinode/utils/emoji.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      565 2023-04-21 13:20:34.000000 scinode-0.3.5/scinode/utils/formater.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    18292 2023-07-17 11:40:05.000000 scinode-0.3.5/scinode/utils/node.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8018 2023-06-15 06:21:11.000000 scinode-0.3.5/scinode/utils/nodetree.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)    12630 2023-06-16 06:56:57.000000 scinode-0.3.5/scinode/utils/nt_analysis.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      977 2023-05-02 12:47:10.000000 scinode-0.3.5/scinode/utils/process.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      103 2023-06-19 08:05:52.000000 scinode-0.3.5/scinode/version.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2023-07-21 15:20:52.782226 scinode-0.3.5/scinode.egg-info/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1843 2023-07-21 15:20:52.000000 scinode-0.3.5/scinode.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     6567 2023-07-21 15:20:52.000000 scinode-0.3.5/scinode.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2023-07-21 15:20:52.000000 scinode-0.3.5/scinode.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1071 2023-07-21 15:20:52.000000 scinode-0.3.5/scinode.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      188 2023-07-21 15:20:52.000000 scinode-0.3.5/scinode.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        8 2023-07-21 15:20:52.000000 scinode-0.3.5/scinode.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2023-07-21 15:20:52.814226 scinode-0.3.5/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2857 2023-07-21 15:20:50.000000 scinode-0.3.5/setup.py
```

### Comparing `scinode-0.3.4/LICENSE` & `scinode-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/PKG-INFO` & `scinode-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinode
-Version: 0.3.4
+Version: 0.3.5
 Summary: Design computational workflow using nodes.
 Home-page: https://github.com/scinode/scinode
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scinode-0.3.4/README.md` & `scinode-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/app.py` & `scinode-0.3.5/scinode/app/app.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/component/component.py` & `scinode-0.3.5/scinode/app/blueprints/component/component.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/component/templates/component_editor.html` & `scinode-0.3.5/scinode/app/blueprints/component/templates/component_editor.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/component/templates/component_exporter.html` & `scinode-0.3.5/scinode/app/blueprints/component/templates/component_exporter.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/component/templates/component_table.html` & `scinode-0.3.5/scinode/app/blueprints/component/templates/component_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/component/utils.py` & `scinode-0.3.5/scinode/app/blueprints/component/utils.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/config/config.py` & `scinode-0.3.5/scinode/app/blueprints/config/config.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/config/templates/config.html` & `scinode-0.3.5/scinode/app/blueprints/config/templates/config.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/config/templates/daemon_logfile.html` & `scinode-0.3.5/scinode/app/blueprints/config/templates/daemon_logfile.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/data/data.py` & `scinode-0.3.5/scinode/app/blueprints/data/data.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/data/templates/data_table.html` & `scinode-0.3.5/scinode/app/blueprints/data/templates/data_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/data/templates/data_viewer.html` & `scinode-0.3.5/scinode/app/blueprints/data/templates/data_viewer.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/node/node.py` & `scinode-0.3.5/scinode/app/blueprints/node/node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/node/templates/node_table.html` & `scinode-0.3.5/scinode/app/blueprints/node/templates/node_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/node/templates/node_viewer.html` & `scinode-0.3.5/scinode/app/blueprints/node/templates/node_viewer.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/nodetree.py` & `scinode-0.3.5/scinode/app/blueprints/nodetree/nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/templates/nodetree_editor.html` & `scinode-0.3.5/scinode/app/blueprints/nodetree/templates/nodetree_editor.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/templates/nodetree_exporter.html` & `scinode-0.3.5/scinode/app/blueprints/nodetree/templates/nodetree_exporter.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/templates/nodetree_table.html` & `scinode-0.3.5/scinode/app/blueprints/nodetree/templates/nodetree_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/templates/nodetree_viewer.html` & `scinode-0.3.5/scinode/app/blueprints/nodetree/templates/nodetree_viewer.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/templates/tab-graph-sidebar.html` & `scinode-0.3.5/scinode/app/blueprints/nodetree/templates/tab-graph-sidebar.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/templates/tab-graph.html` & `scinode-0.3.5/scinode/app/blueprints/nodetree/templates/tab-graph.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/templates/tab-table.html` & `scinode-0.3.5/scinode/app/blueprints/nodetree/templates/tab-table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/templates/tab.html` & `scinode-0.3.5/scinode/app/blueprints/nodetree/templates/tab.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/nodetree/utils.py` & `scinode-0.3.5/scinode/app/blueprints/nodetree/utils.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/scheduler/scheduler.py` & `scinode-0.3.5/scinode/app/blueprints/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/template/template.py` & `scinode-0.3.5/scinode/app/blueprints/template/template.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/blueprints/template/templates/template_table.html` & `scinode-0.3.5/scinode/app/blueprints/template/templates/template_table.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/cli/commands/plugin.py` & `scinode-0.3.5/scinode/app/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/cli/commands/web.py` & `scinode-0.3.5/scinode/app/cli/commands/web.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/db.py` & `scinode-0.3.5/scinode/app/db.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/__pycache__/__init__.cpython-310.pyc` & `scinode-0.3.5/scinode/app/static/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/component_editor.js` & `scinode-0.3.5/scinode/app/static/component_editor.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/components/app_components.js` & `scinode-0.3.5/scinode/app/static/components/app_components.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/controls/app_controls.js` & `scinode-0.3.5/scinode/app/static/controls/app_controls.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/init_editor.js` & `scinode-0.3.5/scinode/app/static/init_editor.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/json_components.js` & `scinode-0.3.5/scinode/app/static/json_components.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/logo.png` & `scinode-0.3.5/scinode/app/static/logo.png`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/nodetree_editor.js` & `scinode-0.3.5/scinode/app/static/nodetree_editor.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/nodetree_node_table.js` & `scinode-0.3.5/scinode/app/static/nodetree_node_table.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/scinode_components.js` & `scinode-0.3.5/scinode/app/static/scinode_components.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/scinode_editor.js` & `scinode-0.3.5/scinode/app/static/scinode_editor.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/sidebar.js` & `scinode-0.3.5/scinode/app/static/sidebar.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/sockets/app_sockets.js` & `scinode-0.3.5/scinode/app/static/sockets/app_sockets.js`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/static/styles.css` & `scinode-0.3.5/scinode/app/static/styles.css`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/templates/base.html` & `scinode-0.3.5/scinode/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/templates/base_editor.html` & `scinode-0.3.5/scinode/app/templates/base_editor.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/templates/index.html` & `scinode-0.3.5/scinode/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/utils/__init__.py` & `scinode-0.3.5/scinode/app/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/app/utils/rete_adapter.py` & `scinode-0.3.5/scinode/app/utils/rete_adapter.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/commands/computer.py` & `scinode-0.3.5/scinode/cli/commands/computer.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/commands/data.py` & `scinode-0.3.5/scinode/cli/commands/data.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/commands/mq.py` & `scinode-0.3.5/scinode/cli/commands/mq.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/commands/node.py` & `scinode-0.3.5/scinode/cli/commands/node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/commands/nodetree.py` & `scinode-0.3.5/scinode/cli/commands/nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/commands/profile.py` & `scinode-0.3.5/scinode/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/commands/scheduler.py` & `scinode-0.3.5/scinode/cli/commands/scheduler.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/commands/shell.py` & `scinode-0.3.5/scinode/cli/commands/shell.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/commands/worker.py` & `scinode-0.3.5/scinode/cli/commands/worker.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/cli/main.py` & `scinode-0.3.5/scinode/cli/main.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/common/log.py` & `scinode-0.3.5/scinode/common/log.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/config/__init__.py` & `scinode-0.3.5/scinode/config/__init__.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/config/base_config.py` & `scinode-0.3.5/scinode/config/base_config.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/config/computer.py` & `scinode-0.3.5/scinode/config/computer.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/config/profile.py` & `scinode-0.3.5/scinode/config/profile.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/core/collection.py` & `scinode-0.3.5/scinode/core/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,15 +152,16 @@
         func (_type_): _description_
     """
 
     def wrapper_func(*args, **kwargs):
         import difflib
 
         identifier = args[1]
-        if identifier not in args[0].pool:
+        # print("identifier: ", identifier)
+        if isinstance(identifier, str) and identifier not in args[0].pool:
             items = difflib.get_close_matches(identifier, args[0].pool)
             if len(items) == 0:
                 msg = "Identifier: {} is not defined.".format(identifier)
             else:
                 msg = "Identifier: {} is not defined. Do you mean {}".format(
                     identifier, ", ".join(items)
                 )
@@ -205,17 +206,27 @@
         from scinode.nodes import node_pool
 
         self.pool = node_pool
         super().__init__(parent)
 
     @decorator_check_identifier_name
     def new(self, identifier, name=None, uuid=None, **kwargs):
+        from scinode.core.node import Node
 
-        ItemClass = self.pool[identifier]
         inner_id = self.get_inner_id()
+        if isinstance(identifier, str):
+            ItemClass = self.pool[identifier]
+        elif isinstance(identifier, type) and issubclass(identifier, Node):
+            ItemClass = identifier
+        elif isinstance(getattr(identifier, "node", None), type) and issubclass(
+            identifier.node, Node
+        ):
+            ItemClass = identifier.node
+        else:
+            raise Exception(f"Identifier {identifier} is not a node or node name.")
         # logger.debug("New node, inner_id: {}, name: {}".format(inner_id, name))
         item = ItemClass(inner_id, name=name, uuid=uuid)
         self.append(item)
         item.set(kwargs)
         return item
 
     def copy(self, parent=None):
```

### Comparing `scinode-0.3.4/scinode/core/executor.py` & `scinode-0.3.5/scinode/core/executor.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/core/link.py` & `scinode-0.3.5/scinode/core/link.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/core/node.py` & `scinode-0.3.5/scinode/core/node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/core/nodetree.py` & `scinode-0.3.5/scinode/core/nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/core/property.py` & `scinode-0.3.5/scinode/core/property.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/core/socket.py` & `scinode-0.3.5/scinode/core/socket.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/daemon/daemon.py` & `scinode-0.3.5/scinode/daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/daemon/scheduler.py` & `scinode-0.3.5/scinode/daemon/scheduler.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/daemon/worker.py` & `scinode-0.3.5/scinode/daemon/worker.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/daemon/worker_config.py` & `scinode-0.3.5/scinode/daemon/worker_config.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/database/client.py` & `scinode-0.3.5/scinode/database/client.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/database/data.py` & `scinode-0.3.5/scinode/database/data.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/database/db.py` & `scinode-0.3.5/scinode/database/db.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/database/node.py` & `scinode-0.3.5/scinode/database/node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/database/nodetree.py` & `scinode-0.3.5/scinode/database/nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/database/worker.py` & `scinode-0.3.5/scinode/database/worker.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/celery/base.py` & `scinode-0.3.5/scinode/engine/celery/base.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/celery/tasks.py` & `scinode-0.3.5/scinode/engine/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/celery/worker.py` & `scinode-0.3.5/scinode/engine/celery/worker.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/local_run.py` & `scinode-0.3.5/scinode/engine/local_run.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/mq.py` & `scinode-0.3.5/scinode/engine/mq.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/node_engine.py` & `scinode-0.3.5/scinode/engine/node_engine.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/nodetree_engine.py` & `scinode-0.3.5/scinode/engine/nodetree_engine.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/nodetree_launch.py` & `scinode-0.3.5/scinode/engine/nodetree_launch.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/scheduler.py` & `scinode-0.3.5/scinode/engine/scheduler.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/send_to_queue.py` & `scinode-0.3.5/scinode/engine/send_to_queue.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/engine/worker.py` & `scinode-0.3.5/scinode/engine/worker.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/bash_executor.py` & `scinode-0.3.5/scinode/executors/bash_executor.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/built_in.py` & `scinode-0.3.5/scinode/executors/built_in.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/controls/for_node.py` & `scinode-0.3.5/scinode/executors/controls/for_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/controls/if_node.py` & `scinode-0.3.5/scinode/executors/controls/if_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/controls/scatter_node.py` & `scinode-0.3.5/scinode/executors/controls/scatter_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/controls/switch_node.py` & `scinode-0.3.5/scinode/executors/controls/switch_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/controls/update_node.py` & `scinode-0.3.5/scinode/executors/controls/update_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/folder_manager.py` & `scinode-0.3.5/scinode/executors/folder_manager.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/hpc_scheduler.py` & `scinode-0.3.5/scinode/executors/hpc_scheduler.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/python.py` & `scinode-0.3.5/scinode/executors/python.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/ssh/ssh_client.py` & `scinode-0.3.5/scinode/executors/ssh/ssh_client.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/ssh/ssh_executor.py` & `scinode-0.3.5/scinode/executors/ssh/ssh_executor.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/ssh/ssh_python_executor.py` & `scinode-0.3.5/scinode/executors/ssh/ssh_python_executor.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/ssh/test_ssh_executor.py` & `scinode-0.3.5/scinode/executors/ssh/test_ssh_executor.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/executors/test.py` & `scinode-0.3.5/scinode/executors/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,16 +110,14 @@
 
 
 def person(name, age):
     return Person(name, age)
 
 
 @node(
-    identifier="NodeTreeIfInExecutor",
-    inputs=[["General", "x"]],
     outputs=[["General", "result"]],
 )
 def test_nodetree_if_in_executor(x):
     """Test run nodetree in an executor."""
     from scinode import NodeTree
 
     nt = NodeTree(name="nodetree_in_executor")
@@ -129,16 +127,14 @@
         op1 = nt.nodes.new("Operator", operator="-", x=x, y=1)
     nt.launch()
     nt.wait()
     return op1.results[0]["value"]
 
 
 @node(
-    identifier="NodeTreeForInExecutor",
-    inputs=[["General", "x"]],
     outputs=[["General", "result"]],
 )
 def test_nodetree_for_in_executor(x):
     """Test run nodetree in an executor."""
     from scinode import NodeTree
 
     nt = NodeTree(name="nodetree_in_executor")
@@ -146,16 +142,14 @@
     nt.launch()
     nt.wait()
     y = [op.results[0]["value"] for op in ops]
     return y
 
 
 @node(
-    identifier="NodeTreeForInExecutor2",
-    inputs=[["General", "x"]],
     outputs=[["General", "result"]],
 )
 def test_nodetree_for_in_executor_2(x):
     """Test run nodetree in an executor."""
     from scinode import NodeTree
 
     nt = NodeTree(name="nodetree_in_executor")
```

### Comparing `scinode-0.3.4/scinode/nodes/bash_node.py` & `scinode-0.3.5/scinode/nodes/bash_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/nodes/build_node_from_database.py` & `scinode-0.3.5/scinode/nodes/build_node_from_database.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/nodes/built_in.py` & `scinode-0.3.5/scinode/nodes/built_in.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/nodes/control.py` & `scinode-0.3.5/scinode/nodes/control.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/nodes/node_from_database.py` & `scinode-0.3.5/scinode/nodes/node_from_database.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/nodes/numpy_node.py` & `scinode-0.3.5/scinode/nodes/numpy_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/nodes/python_builtin.py` & `scinode-0.3.5/scinode/nodes/python_builtin.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/nodes/test.py` & `scinode-0.3.5/scinode/nodes/test.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/nodes/test_node_group.py` & `scinode-0.3.5/scinode/nodes/test_node_group.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/nodes/utils.py` & `scinode-0.3.5/scinode/nodes/utils.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/orm/__init__.py` & `scinode-0.3.5/scinode/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/orm/data.py` & `scinode-0.3.5/scinode/orm/data.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/orm/db_node.py` & `scinode-0.3.5/scinode/orm/db_node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/orm/db_nodetree.py` & `scinode-0.3.5/scinode/orm/db_nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/orm/db_property.py` & `scinode-0.3.5/scinode/orm/db_property.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/orm/db_socket.py` & `scinode-0.3.5/scinode/orm/db_socket.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/orm/node.py` & `scinode-0.3.5/scinode/orm/node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/orm/nodetree.py` & `scinode-0.3.5/scinode/orm/nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/properties/built_in.py` & `scinode-0.3.5/scinode/properties/built_in.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/serialization/built_in.py` & `scinode-0.3.5/scinode/serialization/built_in.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/sockets/built_in.py` & `scinode-0.3.5/scinode/sockets/built_in.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/utils/__init__.py` & `scinode-0.3.5/scinode/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/utils/daemon.py` & `scinode-0.3.5/scinode/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/utils/db.py` & `scinode-0.3.5/scinode/utils/db.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/utils/decorator.py` & `scinode-0.3.5/scinode/utils/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,21 +197,21 @@
     except Exception as e:
         return None
     return node
 
 
 # decorator with arguments indentifier, args, kwargs, properties, inputs, outputs, executor
 def decorator_node(
-    identifier,
+    identifier=None,
     node_type="Normal",
     properties=None,
     inputs=None,
     outputs=None,
     catalog="Others",
-    type = "function",
+    executor_type="function",
 ):
     """Generate a decorator that register a function as a SciNode node.
 
     Attributes:
         indentifier (str): node identifier
         catalog (str): node catalog
         args (list): node args
@@ -223,34 +223,40 @@
     properties = properties or []
     inputs = inputs or []
     outputs = outputs or []
 
     def decorator(func):
         import cloudpickle as pickle
 
+        nonlocal identifier
+
+        if identifier is None:
+            identifier = func.__name__
+
         # use cloudpickle to serialize function
         executor = {
             "executor": pickle.dumps(func),
-            "type": type,
+            "type": executor_type,
             "is_pickle": True,
         }
         #
         # Get the args and kwargs of the function
         args, kwargs, _inputs = generate_input_sockets(func, inputs, properties)
-        node = register_node(
-            identifier,
-            node_type,
-            args,
-            kwargs,
-            properties,
-            _inputs,
-            outputs,
-            executor,
-            catalog=catalog,
-        )
+        ndata = {
+            "identifier": identifier,
+            "node_type": node_type,
+            "args": args,
+            "kwargs": kwargs,
+            "properties": properties,
+            "inputs": _inputs,
+            "outputs": outputs,
+            "executor": executor,
+            "catalog": catalog,
+        }
+        node = create_node(ndata)
         func.identifier = identifier
         func.node = node
         return func
 
     return decorator
```

### Comparing `scinode-0.3.4/scinode/utils/emoji.py` & `scinode-0.3.5/scinode/utils/emoji.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/utils/formater.py` & `scinode-0.3.5/scinode/utils/formater.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/utils/node.py` & `scinode-0.3.5/scinode/utils/node.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/utils/nodetree.py` & `scinode-0.3.5/scinode/utils/nodetree.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/utils/nt_analysis.py` & `scinode-0.3.5/scinode/utils/nt_analysis.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode/utils/process.py` & `scinode-0.3.5/scinode/utils/process.py`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode.egg-info/PKG-INFO` & `scinode-0.3.5/scinode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinode
-Version: 0.3.4
+Version: 0.3.5
 Summary: Design computational workflow using nodes.
 Home-page: https://github.com/scinode/scinode
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `scinode-0.3.4/scinode.egg-info/SOURCES.txt` & `scinode-0.3.5/scinode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/scinode.egg-info/entry_points.txt` & `scinode-0.3.5/scinode.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `scinode-0.3.4/setup.py` & `scinode-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="scinode",
-    version="0.3.4",
+    version="0.3.5",
     description="Design computational workflow using nodes.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/scinode/scinode",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
```

