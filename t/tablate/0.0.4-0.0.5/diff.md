# Comparing `tmp/tablate-0.0.4.tar.gz` & `tmp/tablate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablate-0.0.4.tar", last modified: Thu Jul 20 14:55:58 2023, max compression
+gzip compressed data, was "tablate-0.0.5.tar", last modified: Thu Jul 20 21:58:05 2023, max compression
```

## Comparing `tablate-0.0.4.tar` & `tablate-0.0.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.040969 tablate-0.0.4/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.4/LICENCE
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-20 14:55:58.040969 tablate-0.0.4/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22092 2023-07-17 17:27:17.000000 tablate-0.0.4/README.md
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      588 2023-07-20 14:55:50.000000 tablate-0.0.4/pyproject.toml
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-20 14:55:58.040969 tablate-0.0.4/setup.cfg
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.029969 tablate-0.0.4/tablate/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      117 2023-07-19 10:35:23.000000 tablate-0.0.4/tablate/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.030969 tablate-0.0.4/tablate/api/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    10056 2023-07-20 13:47:58.000000 tablate-0.0.4/tablate/api/Tablate.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.4/tablate/api/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.031969 tablate-0.0.4/tablate/characters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.4/tablate/characters/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.4/tablate/characters/corners.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.4/tablate/characters/line_h.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      108 2023-07-20 01:11:40.000000 tablate-0.0.4/tablate/characters/line_v.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2343 2023-07-19 23:07:53.000000 tablate-0.0.4/tablate/characters/matrix_cross.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.4/tablate/characters/matrix_side.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.031969 tablate-0.0.4/tablate/helpers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.4/tablate/helpers/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.031969 tablate-0.0.4/tablate/helpers/calcs/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.4/tablate/helpers/calcs/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1102 2023-07-19 21:31:48.000000 tablate-0.0.4/tablate/helpers/calcs/calc_column_percent.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2589 2023-07-19 01:22:54.000000 tablate-0.0.4/tablate/helpers/calcs/calc_column_widths.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-19 21:45:43.000000 tablate-0.0.4/tablate/helpers/calcs/get_row_colspan.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      150 2023-07-19 22:13:11.000000 tablate-0.0.4/tablate/helpers/calcs/random_string.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.032969 tablate-0.0.4/tablate/helpers/checkers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.4/tablate/helpers/checkers/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.4/tablate/helpers/checkers/is_last_element.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.032969 tablate-0.0.4/tablate/helpers/formatters/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.4/tablate/helpers/formatters/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.033969 tablate-0.0.4/tablate/helpers/formatters/console/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.4/tablate/helpers/formatters/console/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4579 2023-07-20 08:05:59.000000 tablate-0.0.4/tablate/helpers/formatters/console/cell_string.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      539 2023-07-20 09:59:11.000000 tablate-0.0.4/tablate/helpers/formatters/console/row_border.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3160 2023-07-20 09:59:11.000000 tablate-0.0.4/tablate/helpers/formatters/console/row_divider.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.033969 tablate-0.0.4/tablate/helpers/formatters/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.4/tablate/helpers/formatters/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.033969 tablate-0.0.4/tablate/helpers/formatters/html/element/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:52.000000 tablate-0.0.4/tablate/helpers/formatters/html/element/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:39.000000 tablate-0.0.4/tablate/helpers/formatters/html/element/frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:45.000000 tablate-0.0.4/tablate/helpers/formatters/html/element/row.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:34.000000 tablate-0.0.4/tablate/helpers/formatters/html/element/text.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.034969 tablate-0.0.4/tablate/helpers/formatters/html/style/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:43:30.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.034969 tablate-0.0.4/tablate/helpers/formatters/html/style/border/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:38.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/border/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:51.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/border/border_bottom.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:46:57.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/border/border_right.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      416 2023-07-19 23:18:14.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/border/border_style.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      211 2023-07-20 10:49:54.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/selector.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.035969 tablate-0.0.4/tablate/helpers/formatters/html/style/text/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:34.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/text/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       25 2023-07-20 06:17:45.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/text/alignment.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       25 2023-07-20 06:17:45.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/text/multiline.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:48:28.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/text/overflow.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:12:25.000000 tablate-0.0.4/tablate/helpers/formatters/html/style/text/padding.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.035969 tablate-0.0.4/tablate/helpers/renderers/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.4/tablate/helpers/renderers/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.036969 tablate-0.0.4/tablate/helpers/renderers/console/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.4/tablate/helpers/renderers/console/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.036969 tablate-0.0.4/tablate/helpers/renderers/console/frames/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:15:27.000000 tablate-0.0.4/tablate/helpers/renderers/console/frames/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2113 2023-07-20 09:59:11.000000 tablate-0.0.4/tablate/helpers/renderers/console/frames/render_console_columns.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2530 2023-07-20 09:59:11.000000 tablate-0.0.4/tablate/helpers/renderers/console/frames/render_console_frame_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3869 2023-07-20 09:59:11.000000 tablate-0.0.4/tablate/helpers/renderers/console/frames/render_string_frame_table.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1936 2023-07-20 09:59:11.000000 tablate-0.0.4/tablate/helpers/renderers/console/frames/render_string_frame_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      800 2023-07-20 14:55:25.000000 tablate-0.0.4/tablate/helpers/renderers/console/render_console_foot.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2320 2023-07-20 14:45:23.000000 tablate-0.0.4/tablate/helpers/renderers/console/render_console_frames.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      777 2023-07-20 14:55:25.000000 tablate-0.0.4/tablate/helpers/renderers/console/render_console_head.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.037969 tablate-0.0.4/tablate/helpers/renderers/html/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.4/tablate/helpers/renderers/html/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.038969 tablate-0.0.4/tablate/helpers/renderers/html/frames/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      277 2023-07-19 20:38:22.000000 tablate-0.0.4/tablate/helpers/renderers/html/frames/render_html_grid.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1375 2023-07-20 11:47:48.000000 tablate-0.0.4/tablate/helpers/renderers/html/frames/render_html_table_body.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1023 2023-07-20 11:47:48.000000 tablate-0.0.4/tablate/helpers/renderers/html/frames/render_html_table_head.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 08:50:17.000000 tablate-0.0.4/tablate/helpers/renderers/html/frames/render_html_text.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       51 2023-07-19 21:52:25.000000 tablate-0.0.4/tablate/helpers/renderers/html/render_html_foot.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      760 2023-07-20 10:18:01.000000 tablate-0.0.4/tablate/helpers/renderers/html/render_html_frames.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1157 2023-07-20 11:47:48.000000 tablate-0.0.4/tablate/helpers/renderers/html/render_html_head.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.038969 tablate-0.0.4/tablate/helpers/validators/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:45.000000 tablate-0.0.4/tablate/helpers/validators/__init__.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.039969 tablate-0.0.4/tablate/tests/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 00:45:20.000000 tablate-0.0.4/tablate/tests/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       14 2023-07-20 14:52:15.000000 tablate-0.0.4/tablate/tests/blah.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3528 2023-07-20 14:50:58.000000 tablate-0.0.4/tablate/tests/test_decs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8057 2023-07-20 00:01:38.000000 tablate-0.0.4/tablate/tests/test_defs.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       67 2023-07-19 10:35:23.000000 tablate-0.0.4/tablate/tests/test_html.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       65 2023-07-19 09:16:41.000000 tablate-0.0.4/tablate/tests/test_text.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.039969 tablate-0.0.4/tablate/type/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 07:43:04.000000 tablate-0.0.4/tablate/type/__init__.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2473 2023-07-20 09:49:58.000000 tablate-0.0.4/tablate/type/dict_frame.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1129 2023-07-20 07:45:25.000000 tablate-0.0.4/tablate/type/dict_input.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      538 2023-07-20 13:47:58.000000 tablate-0.0.4/tablate/type/dict_options.py
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      414 2023-07-20 10:49:54.000000 tablate-0.0.4/tablate/type/primitives.py
-drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 14:55:58.030969 tablate-0.0.4/tablate.egg-info/
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-20 14:55:58.000000 tablate-0.0.4/tablate.egg-info/PKG-INFO
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3173 2023-07-20 14:55:58.000000 tablate-0.0.4/tablate.egg-info/SOURCES.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-20 14:55:58.000000 tablate-0.0.4/tablate.egg-info/dependency_links.txt
--rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        8 2023-07-20 14:55:58.000000 tablate-0.0.4/tablate.egg-info/top_level.txt
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.972311 tablate-0.0.5/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1069 2023-07-13 22:13:22.000000 tablate-0.0.5/LICENCE
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-20 21:58:05.972311 tablate-0.0.5/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22092 2023-07-17 17:27:17.000000 tablate-0.0.5/README.md
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      588 2023-07-20 21:58:00.000000 tablate-0.0.5/pyproject.toml
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       38 2023-07-20 21:58:05.972311 tablate-0.0.5/setup.cfg
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.959311 tablate-0.0.5/tablate/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      117 2023-07-19 10:35:23.000000 tablate-0.0.5/tablate/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.961311 tablate-0.0.5/tablate/api/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    10270 2023-07-20 21:18:19.000000 tablate-0.0.5/tablate/api/Tablate.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 22:41:07.000000 tablate-0.0.5/tablate/api/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.962311 tablate-0.0.5/tablate/characters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.5/tablate/characters/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      378 2023-07-16 22:19:15.000000 tablate-0.0.5/tablate/characters/corners.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 22:19:15.000000 tablate-0.0.5/tablate/characters/line_h.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      108 2023-07-20 01:11:40.000000 tablate-0.0.5/tablate/characters/line_v.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2343 2023-07-19 23:07:53.000000 tablate-0.0.5/tablate/characters/matrix_cross.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      965 2023-07-16 22:19:15.000000 tablate-0.0.5/tablate/characters/matrix_side.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.962311 tablate-0.0.5/tablate/helpers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-16 01:14:04.000000 tablate-0.0.5/tablate/helpers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.963311 tablate-0.0.5/tablate/helpers/calcs/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:23.000000 tablate-0.0.5/tablate/helpers/calcs/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1102 2023-07-19 21:31:48.000000 tablate-0.0.5/tablate/helpers/calcs/calc_column_percent.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2589 2023-07-19 01:22:54.000000 tablate-0.0.5/tablate/helpers/calcs/calc_column_widths.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      587 2023-07-19 21:45:43.000000 tablate-0.0.5/tablate/helpers/calcs/get_row_colspan.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      150 2023-07-19 22:13:11.000000 tablate-0.0.5/tablate/helpers/calcs/random_string.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.963311 tablate-0.0.5/tablate/helpers/checkers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:34:30.000000 tablate-0.0.5/tablate/helpers/checkers/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       89 2023-07-16 05:52:57.000000 tablate-0.0.5/tablate/helpers/checkers/is_last_element.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.963311 tablate-0.0.5/tablate/helpers/formatters/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.5/tablate/helpers/formatters/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.964311 tablate-0.0.5/tablate/helpers/formatters/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:58:20.000000 tablate-0.0.5/tablate/helpers/formatters/console/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     4579 2023-07-20 08:05:59.000000 tablate-0.0.5/tablate/helpers/formatters/console/cell_string.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      539 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/formatters/console/row_border.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3160 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/formatters/console/row_divider.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.964311 tablate-0.0.5/tablate/helpers/formatters/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:38:58.000000 tablate-0.0.5/tablate/helpers/formatters/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.965311 tablate-0.0.5/tablate/helpers/formatters/html/element/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:52.000000 tablate-0.0.5/tablate/helpers/formatters/html/element/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:39.000000 tablate-0.0.5/tablate/helpers/formatters/html/element/frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:45.000000 tablate-0.0.5/tablate/helpers/formatters/html/element/row.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:42:34.000000 tablate-0.0.5/tablate/helpers/formatters/html/element/text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.965311 tablate-0.0.5/tablate/helpers/formatters/html/style/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:43:30.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.965311 tablate-0.0.5/tablate/helpers/formatters/html/style/border/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:38.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/border/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:51.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/border/border_bottom.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:46:57.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/border/border_right.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      416 2023-07-19 23:18:14.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/border/border_style.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      211 2023-07-20 10:49:54.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/selector.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.966311 tablate-0.0.5/tablate/helpers/formatters/html/style/text/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:45:34.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       25 2023-07-20 06:17:45.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/alignment.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       25 2023-07-20 06:17:45.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/multiline.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 11:48:28.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/overflow.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:12:25.000000 tablate-0.0.5/tablate/helpers/formatters/html/style/text/padding.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.966311 tablate-0.0.5/tablate/helpers/renderers/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:33.000000 tablate-0.0.5/tablate/helpers/renderers/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.967311 tablate-0.0.5/tablate/helpers/renderers/console/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:13.000000 tablate-0.0.5/tablate/helpers/renderers/console/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.968311 tablate-0.0.5/tablate/helpers/renderers/console/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 06:15:27.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2113 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/render_console_columns.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2530 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/render_console_frame_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3869 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/render_string_frame_table.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1936 2023-07-20 09:59:11.000000 tablate-0.0.5/tablate/helpers/renderers/console/frames/render_string_frame_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      800 2023-07-20 14:55:25.000000 tablate-0.0.5/tablate/helpers/renderers/console/render_console_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2320 2023-07-20 14:45:23.000000 tablate-0.0.5/tablate/helpers/renderers/console/render_console_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      777 2023-07-20 14:55:25.000000 tablate-0.0.5/tablate/helpers/renderers/console/render_console_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.969311 tablate-0.0.5/tablate/helpers/renderers/html/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 03:40:21.000000 tablate-0.0.5/tablate/helpers/renderers/html/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.970311 tablate-0.0.5/tablate/helpers/renderers/html/frames/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      277 2023-07-19 20:38:22.000000 tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_grid.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1375 2023-07-20 11:47:48.000000 tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_table_body.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1023 2023-07-20 11:47:48.000000 tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_table_head.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-19 08:50:17.000000 tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_text.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       51 2023-07-19 21:52:25.000000 tablate-0.0.5/tablate/helpers/renderers/html/render_html_foot.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      760 2023-07-20 10:18:01.000000 tablate-0.0.5/tablate/helpers/renderers/html/render_html_frames.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1157 2023-07-20 11:47:48.000000 tablate-0.0.5/tablate/helpers/renderers/html/render_html_head.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.970311 tablate-0.0.5/tablate/helpers/validators/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-18 22:51:45.000000 tablate-0.0.5/tablate/helpers/validators/__init__.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.971311 tablate-0.0.5/tablate/tests/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 00:45:20.000000 tablate-0.0.5/tablate/tests/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       14 2023-07-20 14:52:15.000000 tablate-0.0.5/tablate/tests/blah.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3528 2023-07-20 14:50:58.000000 tablate-0.0.5/tablate/tests/test_decs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     8057 2023-07-20 00:01:38.000000 tablate-0.0.5/tablate/tests/test_defs.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       67 2023-07-19 10:35:23.000000 tablate-0.0.5/tablate/tests/test_html.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)       66 2023-07-20 21:47:24.000000 tablate-0.0.5/tablate/tests/test_text.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.971311 tablate-0.0.5/tablate/type/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 07:43:04.000000 tablate-0.0.5/tablate/type/__init__.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     2473 2023-07-20 09:49:58.000000 tablate-0.0.5/tablate/type/dict_frame.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     1281 2023-07-20 21:47:24.000000 tablate-0.0.5/tablate/type/dict_input.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      538 2023-07-20 13:47:58.000000 tablate-0.0.5/tablate/type/dict_options.py
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)      414 2023-07-20 10:49:54.000000 tablate-0.0.5/tablate/type/primitives.py
+drwxr-xr-x   0 guydewinton  (1000) guydewinton  (1000)        0 2023-07-20 21:58:05.960311 tablate-0.0.5/tablate.egg-info/
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)    22606 2023-07-20 21:58:05.000000 tablate-0.0.5/tablate.egg-info/PKG-INFO
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)     3173 2023-07-20 21:58:05.000000 tablate-0.0.5/tablate.egg-info/SOURCES.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        1 2023-07-20 21:58:05.000000 tablate-0.0.5/tablate.egg-info/dependency_links.txt
+-rw-r--r--   0 guydewinton  (1000) guydewinton  (1000)        8 2023-07-20 21:58:05.000000 tablate-0.0.5/tablate.egg-info/top_level.txt
```

### Comparing `tablate-0.0.4/LICENCE` & `tablate-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/PKG-INFO` & `tablate-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablate
-Version: 0.0.4
+Version: 0.0.5
 Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablate-0.0.4/README.md` & `tablate-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/pyproject.toml` & `tablate-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tablate"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Guy de Winton", email="guy@codehippie.io" },
 ]
 description = "An ASCII plain text table renderer."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `tablate-0.0.4/tablate/api/Tablate.py` & `tablate-0.0.5/tablate/api/Tablate.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 
 class Tablate:
 
     # todo: maybe allow align/padding/frame_divider defaults in constructor??
     # todo: allow frame names (will make TextFrame iPython friendly) -- also constructor options `show_frame_names` & `frame_name_align`
     # todo: allow cell level definition of padding/v_line/trunc_value in `add_` constructor objects??? => a lot of fuss and complication for marginal use... v_lines might be useful...
 
+    # todo: text styles / colours
+
     def __init__(self,
                  border_style: Border = "thick",
-                 frame_padding: int = 1,
+                 frame_padding: int = 1, # todo: allow padding definition for all sides => int: all sides, string: css style ('0' or '0 0' or '0 0 0 0') // dict: {"top", "bottom", "left", "right"} // three input methods
                  frame_divider: BaseDivider = "thick",
                  frame_width: int = None,
                  html_px_size: int = 6,
                  html_text_size: int = 12,
                  html_frame_width: str = "100%",
                  html_css_injection: str = ""):
```

### Comparing `tablate-0.0.4/tablate/characters/matrix_cross.py` & `tablate-0.0.5/tablate/characters/matrix_cross.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/characters/matrix_side.py` & `tablate-0.0.5/tablate/characters/matrix_side.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/calcs/calc_column_percent.py` & `tablate-0.0.5/tablate/helpers/calcs/calc_column_percent.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/calcs/calc_column_widths.py` & `tablate-0.0.5/tablate/helpers/calcs/calc_column_widths.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/calcs/get_row_colspan.py` & `tablate-0.0.5/tablate/helpers/calcs/get_row_colspan.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/formatters/console/cell_string.py` & `tablate-0.0.5/tablate/helpers/formatters/console/cell_string.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/formatters/console/row_border.py` & `tablate-0.0.5/tablate/helpers/formatters/console/row_border.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/formatters/console/row_divider.py` & `tablate-0.0.5/tablate/helpers/formatters/console/row_divider.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/console/frames/render_console_columns.py` & `tablate-0.0.5/tablate/helpers/renderers/console/frames/render_console_columns.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/console/frames/render_console_frame_grid.py` & `tablate-0.0.5/tablate/helpers/renderers/console/frames/render_console_frame_grid.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/console/frames/render_string_frame_table.py` & `tablate-0.0.5/tablate/helpers/renderers/console/frames/render_string_frame_table.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/console/frames/render_string_frame_text.py` & `tablate-0.0.5/tablate/helpers/renderers/console/frames/render_string_frame_text.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/console/render_console_foot.py` & `tablate-0.0.5/tablate/helpers/renderers/console/render_console_foot.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/console/render_console_frames.py` & `tablate-0.0.5/tablate/helpers/renderers/console/render_console_frames.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/console/render_console_head.py` & `tablate-0.0.5/tablate/helpers/renderers/console/render_console_head.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/html/frames/render_html_table_body.py` & `tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_table_body.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/html/frames/render_html_table_head.py` & `tablate-0.0.5/tablate/helpers/renderers/html/frames/render_html_table_head.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/html/render_html_frames.py` & `tablate-0.0.5/tablate/helpers/renderers/html/render_html_frames.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/helpers/renderers/html/render_html_head.py` & `tablate-0.0.5/tablate/helpers/renderers/html/render_html_head.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/tests/test_decs.py` & `tablate-0.0.5/tablate/tests/test_decs.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/tests/test_defs.py` & `tablate-0.0.5/tablate/tests/test_defs.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/type/dict_frame.py` & `tablate-0.0.5/tablate/type/dict_frame.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate/type/dict_options.py` & `tablate-0.0.5/tablate/type/dict_options.py`

 * *Files identical despite different names*

### Comparing `tablate-0.0.4/tablate.egg-info/PKG-INFO` & `tablate-0.0.5/tablate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablate
-Version: 0.0.4
+Version: 0.0.5
 Summary: An ASCII plain text table renderer.
 Author-email: Guy de Winton <guy@codehippie.io>
 Project-URL: Homepage, https://gitlab.com/guydewinton/textframe
 Project-URL: Bug Tracker, https://gitlab.com/guydewinton/textframe/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tablate-0.0.4/tablate.egg-info/SOURCES.txt` & `tablate-0.0.5/tablate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

